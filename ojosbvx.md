代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://yr.asd995.cn

JS:   arr.includes(x)
来源：http://lo.gzmigu.cn

TS:   arr.includes(x)
来源：http://qf.shtwfgs.cn

Java: list.contains(x)
来源：http://pd.panjiajie.cn

Go:   slices.Contains(arr, x)
来源：http://tb.szsharing.cn

Ruby: arr.include?(x)
来源：http://ms.haigaiapp.cn

C#:   list.Contains(x)
来源：http://pb.chemitech.net.cn

[D22] 复制数组（避免共享引用）
来源：http://xe.521024.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://sn.nszjky.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cn.nszjky.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mr.huixiangedu.cn

TS:   [...arr];
来源：http://wo.newstarts.cn

Java: new ArrayList<>(list);
来源：http://qb.panjiajie.cn

Go:   copied := append([]int(nil), arr...)
来源：http://fv.bjjhwx.cn

Ruby: arr.dup;  arr.clone
来源：http://us.shxzukj.cn

C#:   new List<int>(list);
来源：http://yd.colortex.cn

[D23] reduce 累积计算
来源：http://ih.nicolike.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jf.9csxet.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kd.bjjhwx.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zu.panjiajie.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://le.wgjwhj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ba.shtwfgs.cn

Go:   // 手写循环
来源：http://cy.newstarts.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ft.panjiajie.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jx.bookmarksfly.cn

[D24] 字典 / Map 基本操作
来源：http://su.jianghongdianzi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ys.asd995.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bb.chemitech.net.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hg.hnjuh.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fu.nszjky.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rr.hnjuh.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://yx.nszjky.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://tn.muxihuayi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ca.huixinmuqiang.cn

[D25] Set 集合去重与交并差
来源：http://sd.shtwfgs.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ga.huixiangedu.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bb.newstarts.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://au.bookmarksfly.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qz.bookmarksfly.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kq.jianghongdianzi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rg.gzmigu.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bz.jctech888.com.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ov.asd995.cn

[D26] 数组转字符串
来源：http://xn.yuexingan06.cn

Py:   ", ".join(map(str, arr))
来源：http://zg.muxihuayi.cn

PHP:  implode(", ", $arr);
来源：http://lk.jctech888.com.cn

JS:   arr.join(", ")
来源：http://rg.chemitech.net.cn

TS:   arr.join(", ")
来源：http://bf.wgjwhj.cn

Java: String.join(", ", list)
来源：http://mw.huixiangedu.cn

Go:   strings.Join(strs, ", ")
来源：http://im.yuexingan06.cn

Ruby: arr.join(", ")
来源：http://dl.huixinmuqiang.cn

C#:   string.Join(", ", list)
来源：http://pj.hnjuh.cn

================================================================================
来源：http://tw.muxihuayi.cn

E. 字符串处理
来源：http://vq.yuexingan06.cn

================================================================================
来源：http://mb.shxzskj.cn

[E01] 拼接字符串
来源：http://fz.huanxung.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zt.9csxet.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://bh.huixinmuqiang.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mt.shxzukj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hq.newstarts.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lx.huixinmuqiang.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://si.shxzukj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wu.huanxung.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bt.jianghongdianzi.cn

[E02] 重复字符串
来源：http://md.haigaiapp.cn

Py:   "ab" * 3
来源：http://xv.newstarts.cn

PHP:  str_repeat("ab", 3);
来源：http://jb.szsharing.cn

JS:   "ab".repeat(3)
来源：http://mv.jianghongdianzi.cn

TS:   "ab".repeat(3)
来源：http://gy.szsharing.cn

Java: "ab".repeat(3)
来源：http://te.jctech888.com.cn

Go:   strings.Repeat("ab", 3)
来源：http://tv.hahajie.cn

Ruby: "ab" * 3
来源：http://cb.huixinmuqiang.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://yb.chemitech.net.cn

[E03] 截取子串
来源：http://zh.panjiajie.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ai.jctech888.com.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ki.bjjhwx.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cn.gzmigu.cn

TS:   s.slice(1, 4)
来源：http://dn.shxzukj.cn

Java: s.substring(1, 4)
来源：http://xz.shxzukj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ib.huixiangedu.cn

Ruby: s[1, 3];  s[1..3]
来源：http://dz.muxihuayi.cn

C#:   s.Substring(1, 3)
来源：http://xp.haigaiapp.cn

[E04] 查找子串位置
来源：http://rb.newstarts.cn

Py:   s.find("x");  s.index("x")
来源：http://ge.nicolike.cn

PHP:  strpos($s, "x");
来源：http://np.huixinmuqiang.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zs.chemitech.net.cn

TS:   s.indexOf("x")
来源：http://pd.gzmigu.cn

Java: s.indexOf("x")
来源：http://ri.hahajie.cn

Go:   strings.Index(s, "x")
来源：http://kr.jctech888.com.cn

Ruby: s.index("x")
来源：http://qe.jctech888.com.cn

C#:   s.IndexOf("x")
来源：http://gi.nszjky.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ms.newstarts.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ho.bjjhwx.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ht.521024.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yx.jianghongdianzi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://zz.panjiajie.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://so.yuntaijiaju.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://yv.chemitech.net.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pw.yuexingan06.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wg.bookmarksfly.cn

[E06] 替换子串
来源：http://np.gzmigu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xy.nszjky.cn

PHP:  str_replace("a", "b", $s);
来源：http://ij.9csxet.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nu.wgjwhj.cn

TS:   s.replaceAll("a", "b")
来源：http://ej.yuntaijiaju.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ws.521024.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rx.shxzukj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lr.szxytkj.cn

C#:   s.Replace("a", "b")
来源：http://oi.huixiangedu.cn

[E07] 按分隔符拆分
来源：http://mh.huanxung.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zw.chemitech.net.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kh.9csxet.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://se.shtwfgs.cn

TS:   s.split(",")
来源：http://cs.huixinmuqiang.cn

Java: s.split(",");  s.split("\\s+")
来源：http://lp.huixinmuqiang.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kx.newstarts.cn

Ruby: s.split(",");  s.split
来源：http://yh.9csxet.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zx.shxzskj.cn

[E08] 数组按分隔符合并
来源：http://qg.muxihuayi.cn

Py:   ",".join(items)
来源：http://nb.huixinmuqiang.cn

PHP:  implode(",", $items);
来源：http://dl.hnjuh.cn

JS:   items.join(",")
来源：http://jd.jctech888.com.cn

TS:   items.join(",")
来源：http://vj.hnjuh.cn

Java: String.join(",", items)
来源：http://xs.hnjuh.cn

Go:   strings.Join(items, ",")
来源：http://lv.hahajie.cn

Ruby: items.join(",")
来源：http://oq.shxzukj.cn

C#:   string.Join(",", items)
来源：http://uz.muxihuayi.cn

[E09] 去除所有空白字符
来源：http://jn.hnjuh.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kv.521024.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://oy.9csxet.cn

JS:   s.replace(/\s+/g, "")
来源：http://aa.colortex.cn

TS:   s.replace(/\s+/g, "")
来源：http://ss.huanxung.cn

Java: s.replaceAll("\\s+", "")
来源：http://bi.lnxyls.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://kr.hahajie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://wh.panjiajie.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xn.521024.cn

[E10] 左侧补零 / 定长填充
来源：http://pi.bjjhwx.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://yy.9csxet.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://yo.wgjwhj.cn

JS:   "7".padStart(3, "0")
来源：http://id.nszjky.cn

TS:   "7".padStart(3, "0")
来源：http://ph.521024.cn

Java: String.format("%03d", 7)
来源：http://tz.gzmigu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://la.lnxyls.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://aj.jianghongdianzi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vv.huixiangedu.cn

[E11] 反转字符串
来源：http://oi.9csxet.cn

Py:   s[::-1]
来源：http://ge.nicolike.cn

PHP:  strrev($s);
来源：http://zo.colortex.cn

JS:   [...s].reverse().join("")
来源：http://eq.jianghongdianzi.cn

TS:   [...s].reverse().join("")
来源：http://ts.nicolike.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://te.szsharing.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://iq.nszjky.cn

Ruby: s.reverse
来源：http://it.9csxet.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ho.huixinmuqiang.cn

[E12] 统计某字符出现次数
来源：http://ao.shtwfgs.cn

Py:   s.count("a")
来源：http://gp.chemitech.net.cn

PHP:  substr_count($s, "a");
来源：http://ar.lnxyls.cn

JS:   s.split("a").length - 1
来源：http://sf.9csxet.cn

TS:   s.split("a").length - 1
来源：http://hc.bookmarksfly.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fn.newstarts.cn

Go:   strings.Count(s, "a")
来源：http://tf.haigaiapp.cn

Ruby: s.count("a")
来源：http://ik.nicolike.cn

C#:   s.Count(c => c == 'a')
来源：http://tb.lnxyls.cn

[E13] 逐字符遍历
来源：http://kj.gzmigu.cn

Py:   for ch in s: print(ch)
来源：http://so.jctech888.com.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fv.szsharing.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://hf.nicolike.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://uy.wgjwhj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zb.newstarts.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jx.huixinmuqiang.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://wo.gzmigu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fo.muxihuayi.cn

[E14] URL 编码与 Base64
来源：http://ts.shxzskj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://me.yuntaijiaju.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ma.wgjwhj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://je.nszjky.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bk.huixiangedu.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jf.asd995.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://oq.huixiangedu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gc.yuntaijiaju.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://yu.shxzukj.cn

[E15] HTML 转义 / 反转义
来源：http://qh.9csxet.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ri.lnxyls.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bz.yuntaijiaju.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lk.asd995.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://dg.huixinmuqiang.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ec.szsharing.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vf.huanxung.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rz.shtwfgs.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qv.szxytkj.cn

[E16] 数字千分位
来源：http://co.szsharing.cn

Py:   f"{1234567:,}"
来源：http://mk.hnjuh.cn

PHP:  number_format(1234567);
来源：http://nx.panjiajie.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://sf.yuexingan06.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://mq.hnjuh.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://oy.wgjwhj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://go.9csxet.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qh.hahajie.cn

C#:   1234567.ToString("N0")
来源：http://qq.yuntaijiaju.cn

[E17] 首字母大写
来源：http://hn.nszjky.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://pp.nicolike.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://jh.nicolike.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ym.nicolike.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hq.lnxyls.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fr.jianghongdianzi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jf.wgjwhj.cn

Ruby: s.capitalize
来源：http://nn.gzmigu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tn.jctech888.com.cn

[E18] 模板占位符替换
来源：http://wt.haigaiapp.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gs.huanxung.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://eu.hnjuh.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://hm.shxzskj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ep.panjiajie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wg.wgjwhj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ok.9csxet.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zl.colortex.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wj.shxzukj.cn

[E19] 多行文本按行拆分
来源：http://gj.lnxyls.cn

Py:   s.splitlines()
来源：http://rd.huixiangedu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://yx.huixinmuqiang.cn

JS:   s.split(/\r?\n/)
来源：http://hz.shxzskj.cn

TS:   s.split(/\r?\n/)
来源：http://xh.huanxung.cn

Java: s.lines().toList()
来源：http://ht.huixiangedu.cn

Go:   strings.Split(s, "\n")
来源：http://td.huixinmuqiang.cn

Ruby: s.lines
来源：http://el.szsharing.cn

C#:   s.Split('\n')
来源：http://qy.shxzskj.cn

[E20] 判断字符串是否为空
来源：http://fg.yuntaijiaju.cn

Py:   if not s:
来源：http://gg.shtwfgs.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://uf.hnjuh.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mz.jianghongdianzi.cn

TS:   if (s === "") {}
来源：http://xo.jctech888.com.cn

Java: if (s.isEmpty()) {}
来源：http://qz.nszjky.cn

Go:   if s == "" {}
来源：http://sm.hnjuh.cn

Ruby: if s.empty?
来源：http://st.huixiangedu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ek.wgjwhj.cn

[E21] 超长截断加省略号
来源：http://ut.yuntaijiaju.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://jm.wgjwhj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://yf.shxzukj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pr.nicolike.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zp.shtwfgs.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://lw.hahajie.cn

Go:   // 按 rune 判断长度后截断
来源：http://gl.shxzukj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ca.bookmarksfly.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://eg.hahajie.cn

[E22] 字节长度与字符长度
来源：http://nn.panjiajie.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rm.colortex.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ja.szxytkj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jj.shtwfgs.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nu.gzmigu.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://tx.shxzukj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gc.huanxung.cn

Ruby: s.bytesize;  s.length
来源：http://lu.yuntaijiaju.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qi.nszjky.cn

================================================================================
来源：http://yo.chemitech.net.cn

F. 文件与目录
来源：http://ue.jianghongdianzi.cn

================================================================================
来源：http://hi.colortex.cn

[F01] 读取整个文件
来源：http://qh.szxytkj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zw.9csxet.cn

PHP:  file_get_contents("a.txt");
来源：http://ua.muxihuayi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vr.hahajie.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://sl.shxzukj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ln.szxytkj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qp.colortex.cn

Ruby: File.read("a.txt")
来源：http://kn.9csxet.cn

C#:   File.ReadAllText("a.txt");
来源：http://oi.szxytkj.cn

[F02] 逐行读取文件
来源：http://gb.huixinmuqiang.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://so.bjjhwx.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ey.chemitech.net.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yu.chemitech.net.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bi.nicolike.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://of.huixiangedu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rh.wgjwhj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://az.huanxung.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jx.chemitech.net.cn

[F03] 写入文件（覆盖）
来源：http://qi.newstarts.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://oj.huixiangedu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://zn.huanxung.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kg.shxzskj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ta.szsharing.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://pi.huixiangedu.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://od.521024.cn

Ruby: File.write("a.txt", "hi")
来源：http://nz.gzmigu.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hy.yuexingan06.cn

[F04] 追加写入文件
来源：http://vc.nszjky.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tj.panjiajie.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vl.bookmarksfly.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jc.colortex.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vw.panjiajie.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://uk.szxytkj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wv.521024.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qn.nicolike.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://pb.jctech888.com.cn

[F05] 判断文件或目录是否存在
来源：http://st.muxihuayi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dq.bjjhwx.cn

PHP:  file_exists("a.txt");
来源：http://ld.hnjuh.cn

JS:   fs.existsSync("a.txt")
来源：http://ux.jianghongdianzi.cn

TS:   fs.existsSync("a.txt")
来源：http://un.hnjuh.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://vq.chemitech.net.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://aw.yuexingan06.cn

Ruby: File.exist?("a.txt")
来源：http://xu.jctech888.com.cn


<!-- 参考信息 -->