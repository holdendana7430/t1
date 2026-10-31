代发 wailian999

Ruby: arr.tally
来源：http://xx.jctech888.com.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ov.chemitech.net.cn

[D21] 判断是否包含某元素
来源：http://uu.panjiajie.cn

Py:   x in arr
来源：http://ws.huixinmuqiang.cn

PHP:  in_array($x, $arr, true);
来源：http://bn.jctech888.com.cn

JS:   arr.includes(x)
来源：http://lm.chemitech.net.cn

TS:   arr.includes(x)
来源：http://pa.shxzskj.cn

Java: list.contains(x)
来源：http://vh.shxzukj.cn

Go:   slices.Contains(arr, x)
来源：http://wb.asd995.cn

Ruby: arr.include?(x)
来源：http://kl.hnjuh.cn

C#:   list.Contains(x)
来源：http://ni.asd995.cn

[D22] 复制数组（避免共享引用）
来源：http://ar.nszjky.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ln.shxzukj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kc.shtwfgs.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://sg.9csxet.cn

TS:   [...arr];
来源：http://hw.nszjky.cn

Java: new ArrayList<>(list);
来源：http://km.shtwfgs.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ag.huanxung.cn

Ruby: arr.dup;  arr.clone
来源：http://yp.shtwfgs.cn

C#:   new List<int>(list);
来源：http://co.gzmigu.cn

[D23] reduce 累积计算
来源：http://xc.shtwfgs.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yt.hahajie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wh.panjiajie.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hq.lnxyls.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://va.nszjky.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ft.shxzukj.cn

Go:   // 手写循环
来源：http://sk.hnjuh.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zm.panjiajie.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tz.huanxung.cn

[D24] 字典 / Map 基本操作
来源：http://uj.huixinmuqiang.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://lj.huanxung.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://lp.521024.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ks.nicolike.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zf.bookmarksfly.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://iz.521024.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bp.szsharing.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://td.bjjhwx.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lh.jianghongdianzi.cn

[D25] Set 集合去重与交并差
来源：http://il.huixinmuqiang.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wn.jctech888.com.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rq.gzmigu.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wz.asd995.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zm.bjjhwx.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dd.9csxet.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wt.jianghongdianzi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zq.huixiangedu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qg.huanxung.cn

[D26] 数组转字符串
来源：http://nq.nszjky.cn

Py:   ", ".join(map(str, arr))
来源：http://tv.chemitech.net.cn

PHP:  implode(", ", $arr);
来源：http://cv.bjjhwx.cn

JS:   arr.join(", ")
来源：http://vg.hahajie.cn

TS:   arr.join(", ")
来源：http://xw.hnjuh.cn

Java: String.join(", ", list)
来源：http://kb.bjjhwx.cn

Go:   strings.Join(strs, ", ")
来源：http://wx.hahajie.cn

Ruby: arr.join(", ")
来源：http://nq.huixiangedu.cn

C#:   string.Join(", ", list)
来源：http://cb.asd995.cn

================================================================================
来源：http://sp.colortex.cn

E. 字符串处理
来源：http://qn.shxzukj.cn

================================================================================
来源：http://hj.yuntaijiaju.cn

[E01] 拼接字符串
来源：http://yv.newstarts.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ql.huanxung.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://eq.521024.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ba.bjjhwx.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mt.shxzukj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://yg.yuntaijiaju.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jo.shtwfgs.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gl.shxzukj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bk.shtwfgs.cn

[E02] 重复字符串
来源：http://bv.szxytkj.cn

Py:   "ab" * 3
来源：http://ao.asd995.cn

PHP:  str_repeat("ab", 3);
来源：http://qb.nicolike.cn

JS:   "ab".repeat(3)
来源：http://ne.bjjhwx.cn

TS:   "ab".repeat(3)
来源：http://ji.nicolike.cn

Java: "ab".repeat(3)
来源：http://ib.bjjhwx.cn

Go:   strings.Repeat("ab", 3)
来源：http://xa.huixinmuqiang.cn

Ruby: "ab" * 3
来源：http://fp.wgjwhj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://po.huixinmuqiang.cn

[E03] 截取子串
来源：http://qc.yuexingan06.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qc.chemitech.net.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tz.nicolike.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wh.jianghongdianzi.cn

TS:   s.slice(1, 4)
来源：http://eg.lnxyls.cn

Java: s.substring(1, 4)
来源：http://hp.colortex.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gl.nicolike.cn

Ruby: s[1, 3];  s[1..3]
来源：http://xv.yuntaijiaju.cn

C#:   s.Substring(1, 3)
来源：http://bc.nicolike.cn

[E04] 查找子串位置
来源：http://zx.shtwfgs.cn

Py:   s.find("x");  s.index("x")
来源：http://qw.shxzskj.cn

PHP:  strpos($s, "x");
来源：http://sy.panjiajie.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fj.jianghongdianzi.cn

TS:   s.indexOf("x")
来源：http://ue.chemitech.net.cn

Java: s.indexOf("x")
来源：http://mf.bjjhwx.cn

Go:   strings.Index(s, "x")
来源：http://pg.wgjwhj.cn

Ruby: s.index("x")
来源：http://en.bjjhwx.cn

C#:   s.IndexOf("x")
来源：http://gh.bookmarksfly.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://uz.jianghongdianzi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://vb.521024.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://sm.yuntaijiaju.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wd.hnjuh.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://un.shtwfgs.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xm.szxytkj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mx.huixinmuqiang.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vg.muxihuayi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://cs.nicolike.cn

[E06] 替换子串
来源：http://hr.521024.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://iz.huixiangedu.cn

PHP:  str_replace("a", "b", $s);
来源：http://uj.asd995.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hn.panjiajie.cn

TS:   s.replaceAll("a", "b")
来源：http://ar.haigaiapp.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vp.gzmigu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jc.lnxyls.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jv.lnxyls.cn

C#:   s.Replace("a", "b")
来源：http://qb.nicolike.cn

[E07] 按分隔符拆分
来源：http://su.asd995.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://an.9csxet.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qe.yuntaijiaju.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ku.bookmarksfly.cn

TS:   s.split(",")
来源：http://xg.shxzukj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://es.huixinmuqiang.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://cs.jctech888.com.cn

Ruby: s.split(",");  s.split
来源：http://nm.yuexingan06.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fo.shxzskj.cn

[E08] 数组按分隔符合并
来源：http://zb.nicolike.cn

Py:   ",".join(items)
来源：http://ck.shxzukj.cn

PHP:  implode(",", $items);
来源：http://wa.muxihuayi.cn

JS:   items.join(",")
来源：http://bt.asd995.cn

TS:   items.join(",")
来源：http://en.9csxet.cn

Java: String.join(",", items)
来源：http://nv.nszjky.cn

Go:   strings.Join(items, ",")
来源：http://zw.yuntaijiaju.cn

Ruby: items.join(",")
来源：http://ml.huixiangedu.cn

C#:   string.Join(",", items)
来源：http://il.shxzskj.cn

[E09] 去除所有空白字符
来源：http://mr.huixinmuqiang.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://au.gzmigu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://yl.wgjwhj.cn

JS:   s.replace(/\s+/g, "")
来源：http://zu.colortex.cn

TS:   s.replace(/\s+/g, "")
来源：http://it.wgjwhj.cn

Java: s.replaceAll("\\s+", "")
来源：http://ft.wgjwhj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://tu.hnjuh.cn

Ruby: s.gsub(/\s+/, "")
来源：http://uu.panjiajie.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rf.shxzskj.cn

[E10] 左侧补零 / 定长填充
来源：http://un.asd995.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ge.huixinmuqiang.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://kn.shtwfgs.cn

JS:   "7".padStart(3, "0")
来源：http://il.huixiangedu.cn

TS:   "7".padStart(3, "0")
来源：http://uu.bookmarksfly.cn

Java: String.format("%03d", 7)
来源：http://ik.newstarts.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://hf.asd995.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://oj.szsharing.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kr.hahajie.cn

[E11] 反转字符串
来源：http://ba.jctech888.com.cn

Py:   s[::-1]
来源：http://vx.gzmigu.cn

PHP:  strrev($s);
来源：http://yy.hahajie.cn

JS:   [...s].reverse().join("")
来源：http://ku.shxzukj.cn

TS:   [...s].reverse().join("")
来源：http://ry.hahajie.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://pi.colortex.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ry.chemitech.net.cn

Ruby: s.reverse
来源：http://cd.521024.cn

C#:   new string(s.Reverse().ToArray())
来源：http://fb.szsharing.cn

[E12] 统计某字符出现次数
来源：http://zo.bjjhwx.cn

Py:   s.count("a")
来源：http://li.521024.cn

PHP:  substr_count($s, "a");
来源：http://xr.shxzskj.cn

JS:   s.split("a").length - 1
来源：http://ga.huixiangedu.cn

TS:   s.split("a").length - 1
来源：http://rr.wgjwhj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://sm.hnjuh.cn

Go:   strings.Count(s, "a")
来源：http://wl.gzmigu.cn

Ruby: s.count("a")
来源：http://nt.szxytkj.cn

C#:   s.Count(c => c == 'a')
来源：http://ok.chemitech.net.cn

[E13] 逐字符遍历
来源：http://tz.colortex.cn

Py:   for ch in s: print(ch)
来源：http://pc.haigaiapp.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://lp.521024.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://hf.bookmarksfly.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://lz.huixinmuqiang.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://dc.yuntaijiaju.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://oz.lnxyls.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://kb.shxzukj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://nu.hahajie.cn

[E14] URL 编码与 Base64
来源：http://bf.shxzskj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vd.szxytkj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ux.nicolike.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://lz.9csxet.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qe.muxihuayi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ek.nszjky.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ua.wgjwhj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ud.nszjky.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mt.shxzskj.cn

[E15] HTML 转义 / 反转义
来源：http://cr.bjjhwx.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://gz.bookmarksfly.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://cj.bookmarksfly.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hg.lnxyls.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ti.haigaiapp.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://el.huanxung.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fo.huanxung.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nk.hnjuh.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://yp.huixiangedu.cn

[E16] 数字千分位
来源：http://uv.huanxung.cn

Py:   f"{1234567:,}"
来源：http://xr.panjiajie.cn

PHP:  number_format(1234567);
来源：http://gm.jianghongdianzi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://lr.shxzukj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://lh.shtwfgs.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ef.szsharing.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hn.jianghongdianzi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zn.yuntaijiaju.cn

C#:   1234567.ToString("N0")
来源：http://ff.szsharing.cn

[E17] 首字母大写
来源：http://vn.chemitech.net.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://uy.jianghongdianzi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://yi.chemitech.net.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hd.gzmigu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fk.muxihuayi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fu.9csxet.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://we.huixinmuqiang.cn

Ruby: s.capitalize
来源：http://aj.asd995.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jw.hnjuh.cn

[E18] 模板占位符替换
来源：http://qz.huixiangedu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mr.huixinmuqiang.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://of.newstarts.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://bl.521024.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://bz.szsharing.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://te.jianghongdianzi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://rn.panjiajie.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ya.muxihuayi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://el.jctech888.com.cn

[E19] 多行文本按行拆分
来源：http://gj.nicolike.cn

Py:   s.splitlines()
来源：http://ho.yuntaijiaju.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://fr.jctech888.com.cn

JS:   s.split(/\r?\n/)
来源：http://ke.bjjhwx.cn

TS:   s.split(/\r?\n/)
来源：http://vg.huixiangedu.cn

Java: s.lines().toList()
来源：http://hk.szsharing.cn

Go:   strings.Split(s, "\n")
来源：http://xi.chemitech.net.cn

Ruby: s.lines
来源：http://jf.wgjwhj.cn

C#:   s.Split('\n')
来源：http://bq.szxytkj.cn

[E20] 判断字符串是否为空
来源：http://qh.bjjhwx.cn

Py:   if not s:
来源：http://ev.yuexingan06.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ka.hahajie.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tm.521024.cn

TS:   if (s === "") {}
来源：http://pu.lnxyls.cn

Java: if (s.isEmpty()) {}
来源：http://vz.szxytkj.cn

Go:   if s == "" {}
来源：http://wb.nszjky.cn

Ruby: if s.empty?
来源：http://cs.nszjky.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.lnxyls.cn

[E21] 超长截断加省略号
来源：http://jp.hahajie.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ag.yuntaijiaju.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://tc.jctech888.com.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xb.gzmigu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vx.hahajie.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ac.panjiajie.cn

Go:   // 按 rune 判断长度后截断
来源：http://li.521024.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cv.hnjuh.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hh.gzmigu.cn

[E22] 字节长度与字符长度
来源：http://ik.wgjwhj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ws.bookmarksfly.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pd.szxytkj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ax.hnjuh.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rd.newstarts.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://uu.huixinmuqiang.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tk.wgjwhj.cn

Ruby: s.bytesize;  s.length
来源：http://iz.colortex.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cl.chemitech.net.cn

================================================================================
来源：http://xd.hnjuh.cn

F. 文件与目录
来源：http://bw.wgjwhj.cn

================================================================================
来源：http://lw.nszjky.cn

[F01] 读取整个文件
来源：http://qo.haigaiapp.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://bu.colortex.cn

PHP:  file_get_contents("a.txt");
来源：http://rm.lnxyls.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ry.yuexingan06.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://tr.panjiajie.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://bg.newstarts.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://oa.haigaiapp.cn

Ruby: File.read("a.txt")
来源：http://ze.wgjwhj.cn

C#:   File.ReadAllText("a.txt");
来源：http://qz.gzmigu.cn

[F02] 逐行读取文件
来源：http://qj.bookmarksfly.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xh.nszjky.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://nk.hahajie.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uy.521024.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kt.nszjky.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://sc.yuntaijiaju.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hr.huixinmuqiang.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zh.lnxyls.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://aq.huixiangedu.cn

[F03] 写入文件（覆盖）
来源：http://na.hnjuh.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cs.panjiajie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://mo.nszjky.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gw.yuntaijiaju.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://az.chemitech.net.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ru.9csxet.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hf.lnxyls.cn

Ruby: File.write("a.txt", "hi")
来源：http://qg.huixiangedu.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://es.haigaiapp.cn

[F04] 追加写入文件
来源：http://tl.jianghongdianzi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://oi.shxzskj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://en.hahajie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sz.panjiajie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ni.521024.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ab.colortex.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bz.bjjhwx.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fx.gzmigu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jo.shxzskj.cn

[F05] 判断文件或目录是否存在
来源：http://vg.bookmarksfly.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ad.lnxyls.cn

PHP:  file_exists("a.txt");
来源：http://sn.shtwfgs.cn

JS:   fs.existsSync("a.txt")
来源：http://qx.szxytkj.cn


<!-- 参考信息 -->