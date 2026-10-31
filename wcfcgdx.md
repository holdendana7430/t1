代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://is.huanxung.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zt.521024.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://tm.chemitech.net.cn

TS:   [...arr];
来源：http://nt.521024.cn

Java: new ArrayList<>(list);
来源：http://at.lnxyls.cn

Go:   copied := append([]int(nil), arr...)
来源：http://gr.shxzskj.cn

Ruby: arr.dup;  arr.clone
来源：http://yr.hahajie.cn

C#:   new List<int>(list);
来源：http://fh.shxzskj.cn

[D23] reduce 累积计算
来源：http://rt.szsharing.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://nf.wgjwhj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://uv.shxzskj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nx.szsharing.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zo.nicolike.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://gu.bjjhwx.cn

Go:   // 手写循环
来源：http://cp.szxytkj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://rn.wgjwhj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://aj.asd995.cn

[D24] 字典 / Map 基本操作
来源：http://ry.hnjuh.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hc.shxzukj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://le.hahajie.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://se.szsharing.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zf.szxytkj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fr.panjiajie.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bb.panjiajie.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zp.muxihuayi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lx.gzmigu.cn

[D25] Set 集合去重与交并差
来源：http://nq.shxzukj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://il.shxzskj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vg.panjiajie.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://cl.szsharing.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://so.lnxyls.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ao.szxytkj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ui.521024.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vj.huixiangedu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ip.huixinmuqiang.cn

[D26] 数组转字符串
来源：http://gs.9csxet.cn

Py:   ", ".join(map(str, arr))
来源：http://kb.chemitech.net.cn

PHP:  implode(", ", $arr);
来源：http://nn.hnjuh.cn

JS:   arr.join(", ")
来源：http://gb.521024.cn

TS:   arr.join(", ")
来源：http://mn.panjiajie.cn

Java: String.join(", ", list)
来源：http://yk.newstarts.cn

Go:   strings.Join(strs, ", ")
来源：http://ze.shxzukj.cn

Ruby: arr.join(", ")
来源：http://uk.huixiangedu.cn

C#:   string.Join(", ", list)
来源：http://fp.chemitech.net.cn

================================================================================
来源：http://bd.szsharing.cn

E. 字符串处理
来源：http://dp.szsharing.cn

================================================================================
来源：http://gs.haigaiapp.cn

[E01] 拼接字符串
来源：http://jr.jianghongdianzi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xz.muxihuayi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://yo.huixinmuqiang.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://rl.haigaiapp.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vb.colortex.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://va.jianghongdianzi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://oy.shtwfgs.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://sw.szxytkj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fb.chemitech.net.cn

[E02] 重复字符串
来源：http://rj.huixiangedu.cn

Py:   "ab" * 3
来源：http://fo.gzmigu.cn

PHP:  str_repeat("ab", 3);
来源：http://wh.jianghongdianzi.cn

JS:   "ab".repeat(3)
来源：http://tg.yuntaijiaju.cn

TS:   "ab".repeat(3)
来源：http://vi.colortex.cn

Java: "ab".repeat(3)
来源：http://ia.szsharing.cn

Go:   strings.Repeat("ab", 3)
来源：http://it.huixinmuqiang.cn

Ruby: "ab" * 3
来源：http://iu.chemitech.net.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dk.nszjky.cn

[E03] 截取子串
来源：http://re.chemitech.net.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cf.huixinmuqiang.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bc.szsharing.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wv.panjiajie.cn

TS:   s.slice(1, 4)
来源：http://vw.szxytkj.cn

Java: s.substring(1, 4)
来源：http://kq.shxzskj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qa.hahajie.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ih.hnjuh.cn

C#:   s.Substring(1, 3)
来源：http://fo.shxzskj.cn

[E04] 查找子串位置
来源：http://ta.9csxet.cn

Py:   s.find("x");  s.index("x")
来源：http://lj.muxihuayi.cn

PHP:  strpos($s, "x");
来源：http://qx.jctech888.com.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gr.bookmarksfly.cn

TS:   s.indexOf("x")
来源：http://rt.nicolike.cn

Java: s.indexOf("x")
来源：http://jt.wgjwhj.cn

Go:   strings.Index(s, "x")
来源：http://wl.colortex.cn

Ruby: s.index("x")
来源：http://zo.9csxet.cn

C#:   s.IndexOf("x")
来源：http://cq.wgjwhj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://zq.jctech888.com.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ka.yuexingan06.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://av.9csxet.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sy.bookmarksfly.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://cs.shxzskj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uj.jctech888.com.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://da.wgjwhj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://bj.asd995.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mg.huixinmuqiang.cn

[E06] 替换子串
来源：http://ul.hnjuh.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bx.gzmigu.cn

PHP:  str_replace("a", "b", $s);
来源：http://rk.9csxet.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fp.yuexingan06.cn

TS:   s.replaceAll("a", "b")
来源：http://jb.shxzukj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://he.wgjwhj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://lj.jctech888.com.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ck.colortex.cn

C#:   s.Replace("a", "b")
来源：http://rv.521024.cn

[E07] 按分隔符拆分
来源：http://bl.szxytkj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hj.szsharing.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ct.shxzskj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://hp.szsharing.cn

TS:   s.split(",")
来源：http://kr.bjjhwx.cn

Java: s.split(",");  s.split("\\s+")
来源：http://wm.newstarts.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bg.wgjwhj.cn

Ruby: s.split(",");  s.split
来源：http://wz.haigaiapp.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ce.szsharing.cn

[E08] 数组按分隔符合并
来源：http://sw.shxzukj.cn

Py:   ",".join(items)
来源：http://xs.hahajie.cn

PHP:  implode(",", $items);
来源：http://nh.chemitech.net.cn

JS:   items.join(",")
来源：http://ux.muxihuayi.cn

TS:   items.join(",")
来源：http://jw.shxzukj.cn

Java: String.join(",", items)
来源：http://ln.hnjuh.cn

Go:   strings.Join(items, ",")
来源：http://rp.nicolike.cn

Ruby: items.join(",")
来源：http://fp.521024.cn

C#:   string.Join(",", items)
来源：http://le.9csxet.cn

[E09] 去除所有空白字符
来源：http://qa.colortex.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pf.shxzskj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://oo.szxytkj.cn

JS:   s.replace(/\s+/g, "")
来源：http://wr.jianghongdianzi.cn

TS:   s.replace(/\s+/g, "")
来源：http://hs.colortex.cn

Java: s.replaceAll("\\s+", "")
来源：http://rt.szxytkj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://vz.nicolike.cn

Ruby: s.gsub(/\s+/, "")
来源：http://gt.szxytkj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://px.jianghongdianzi.cn

[E10] 左侧补零 / 定长填充
来源：http://fd.asd995.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bh.nicolike.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fl.yuntaijiaju.cn

JS:   "7".padStart(3, "0")
来源：http://th.shtwfgs.cn

TS:   "7".padStart(3, "0")
来源：http://fj.hnjuh.cn

Java: String.format("%03d", 7)
来源：http://qv.bjjhwx.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://vb.panjiajie.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qt.lnxyls.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://tr.shxzskj.cn

[E11] 反转字符串
来源：http://sg.wgjwhj.cn

Py:   s[::-1]
来源：http://ak.bjjhwx.cn

PHP:  strrev($s);
来源：http://uv.lnxyls.cn

JS:   [...s].reverse().join("")
来源：http://wp.szxytkj.cn

TS:   [...s].reverse().join("")
来源：http://og.gzmigu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ps.newstarts.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://lr.muxihuayi.cn

Ruby: s.reverse
来源：http://lm.nszjky.cn

C#:   new string(s.Reverse().ToArray())
来源：http://vo.asd995.cn

[E12] 统计某字符出现次数
来源：http://gj.nicolike.cn

Py:   s.count("a")
来源：http://rk.asd995.cn

PHP:  substr_count($s, "a");
来源：http://vr.lnxyls.cn

JS:   s.split("a").length - 1
来源：http://wo.9csxet.cn

TS:   s.split("a").length - 1
来源：http://gn.nszjky.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://se.panjiajie.cn

Go:   strings.Count(s, "a")
来源：http://ao.chemitech.net.cn

Ruby: s.count("a")
来源：http://qc.9csxet.cn

C#:   s.Count(c => c == 'a')
来源：http://iv.yuexingan06.cn

[E13] 逐字符遍历
来源：http://zh.bjjhwx.cn

Py:   for ch in s: print(ch)
来源：http://pg.shxzskj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://cr.huixiangedu.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://df.lnxyls.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://yf.yuntaijiaju.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ne.haigaiapp.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://je.colortex.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://uu.huixiangedu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fw.huanxung.cn

[E14] URL 编码与 Base64
来源：http://gj.bookmarksfly.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://uq.nicolike.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ca.nicolike.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rg.yuexingan06.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hu.hahajie.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ry.shtwfgs.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gh.jctech888.com.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wn.hnjuh.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rh.muxihuayi.cn

[E15] HTML 转义 / 反转义
来源：http://wo.huixinmuqiang.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://wv.jctech888.com.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://sh.newstarts.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gd.shxzskj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://nx.gzmigu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kf.huixiangedu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://am.nszjky.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://yi.shxzukj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vy.jctech888.com.cn

[E16] 数字千分位
来源：http://pg.nicolike.cn

Py:   f"{1234567:,}"
来源：http://xm.shxzukj.cn

PHP:  number_format(1234567);
来源：http://xq.huixinmuqiang.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://dm.colortex.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://gy.haigaiapp.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jf.haigaiapp.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yj.9csxet.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://al.newstarts.cn

C#:   1234567.ToString("N0")
来源：http://xu.nszjky.cn

[E17] 首字母大写
来源：http://lj.panjiajie.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cl.panjiajie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://xm.hnjuh.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wu.bjjhwx.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xs.shxzskj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vz.hnjuh.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lg.nicolike.cn

Ruby: s.capitalize
来源：http://ag.yuexingan06.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fd.newstarts.cn

[E18] 模板占位符替换
来源：http://fl.wgjwhj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://uo.shxzukj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://el.panjiajie.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://tz.shtwfgs.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://dg.shxzukj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qh.chemitech.net.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lt.newstarts.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ix.chemitech.net.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ft.bookmarksfly.cn

[E19] 多行文本按行拆分
来源：http://bo.wgjwhj.cn

Py:   s.splitlines()
来源：http://ao.521024.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://bv.shxzukj.cn

JS:   s.split(/\r?\n/)
来源：http://ay.asd995.cn

TS:   s.split(/\r?\n/)
来源：http://zs.szxytkj.cn

Java: s.lines().toList()
来源：http://hu.yuntaijiaju.cn

Go:   strings.Split(s, "\n")
来源：http://qn.gzmigu.cn

Ruby: s.lines
来源：http://qz.chemitech.net.cn

C#:   s.Split('\n')
来源：http://rv.jctech888.com.cn

[E20] 判断字符串是否为空
来源：http://vl.haigaiapp.cn

Py:   if not s:
来源：http://kj.yuntaijiaju.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://uq.huanxung.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lk.yuexingan06.cn

TS:   if (s === "") {}
来源：http://ic.huanxung.cn

Java: if (s.isEmpty()) {}
来源：http://zk.asd995.cn

Go:   if s == "" {}
来源：http://pc.huixinmuqiang.cn

Ruby: if s.empty?
来源：http://hw.9csxet.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wn.szxytkj.cn

[E21] 超长截断加省略号
来源：http://bz.wgjwhj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://jo.huanxung.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://et.bjjhwx.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zf.shxzskj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jf.shxzskj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ih.chemitech.net.cn

Go:   // 按 rune 判断长度后截断
来源：http://yr.haigaiapp.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://kh.jctech888.com.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mb.shxzskj.cn

[E22] 字节长度与字符长度
来源：http://wy.bookmarksfly.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jc.521024.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://be.hahajie.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mt.lnxyls.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wz.jctech888.com.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ga.haigaiapp.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ex.haigaiapp.cn

Ruby: s.bytesize;  s.length
来源：http://km.521024.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://iu.hnjuh.cn

================================================================================
来源：http://if.asd995.cn

F. 文件与目录
来源：http://dn.hahajie.cn

================================================================================
来源：http://uw.szxytkj.cn

[F01] 读取整个文件
来源：http://kj.huixiangedu.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rh.yuexingan06.cn

PHP:  file_get_contents("a.txt");
来源：http://ma.jctech888.com.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jb.hahajie.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://cs.jianghongdianzi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://kc.szsharing.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dn.hahajie.cn

Ruby: File.read("a.txt")
来源：http://gg.hnjuh.cn

C#:   File.ReadAllText("a.txt");
来源：http://cr.huanxung.cn

[F02] 逐行读取文件
来源：http://et.asd995.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://uv.shxzskj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://nk.jianghongdianzi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hk.shxzskj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ay.jianghongdianzi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bm.hnjuh.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ne.wgjwhj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ev.shxzskj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://yb.szxytkj.cn

[F03] 写入文件（覆盖）
来源：http://jj.huanxung.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://yk.chemitech.net.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://qy.yuntaijiaju.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yo.newstarts.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ae.gzmigu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ko.muxihuayi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://iv.szxytkj.cn

Ruby: File.write("a.txt", "hi")
来源：http://ji.jctech888.com.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ew.hahajie.cn

[F04] 追加写入文件
来源：http://zk.bookmarksfly.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://nj.gzmigu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://au.huixiangedu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ka.haigaiapp.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ew.wgjwhj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fq.szxytkj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ha.muxihuayi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://uy.shtwfgs.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dl.huixinmuqiang.cn

[F05] 判断文件或目录是否存在
来源：http://vn.muxihuayi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ux.colortex.cn

PHP:  file_exists("a.txt");
来源：http://cu.bookmarksfly.cn

JS:   fs.existsSync("a.txt")
来源：http://fm.nicolike.cn

TS:   fs.existsSync("a.txt")
来源：http://sg.asd995.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://bg.yuexingan06.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://uy.wgjwhj.cn

Ruby: File.exist?("a.txt")
来源：http://gx.colortex.cn

C#:   File.Exists("a.txt")
来源：http://dn.jianghongdianzi.cn

[F06] 删除文件
来源：http://ho.521024.cn

Py:   os.remove("a.txt")
来源：http://dj.colortex.cn

PHP:  unlink("a.txt");
来源：http://ti.nszjky.cn

JS:   fs.unlinkSync("a.txt")
来源：http://yy.521024.cn

TS:   fs.unlinkSync("a.txt")
来源：http://aa.lnxyls.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ct.colortex.cn

Go:   os.Remove("a.txt")
来源：http://ly.shxzukj.cn


<!-- 参考信息 -->