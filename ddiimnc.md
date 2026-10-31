代发 wailian999

Ruby: arr.tally
来源：http://nc.panjiajie.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://bk.nszjky.cn

[D21] 判断是否包含某元素
来源：http://gq.hnjuh.cn

Py:   x in arr
来源：http://xp.bjjhwx.cn

PHP:  in_array($x, $arr, true);
来源：http://di.bookmarksfly.cn

JS:   arr.includes(x)
来源：http://zu.nicolike.cn

TS:   arr.includes(x)
来源：http://ux.yuexingan06.cn

Java: list.contains(x)
来源：http://dy.szsharing.cn

Go:   slices.Contains(arr, x)
来源：http://zx.bookmarksfly.cn

Ruby: arr.include?(x)
来源：http://mx.huanxung.cn

C#:   list.Contains(x)
来源：http://ke.huanxung.cn

[D22] 复制数组（避免共享引用）
来源：http://ti.shtwfgs.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jm.wgjwhj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xb.shxzukj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zf.chemitech.net.cn

TS:   [...arr];
来源：http://kw.haigaiapp.cn

Java: new ArrayList<>(list);
来源：http://em.shxzukj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://dz.huixinmuqiang.cn

Ruby: arr.dup;  arr.clone
来源：http://wv.hnjuh.cn

C#:   new List<int>(list);
来源：http://rx.shtwfgs.cn

[D23] reduce 累积计算
来源：http://rp.muxihuayi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zx.lnxyls.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ct.yuntaijiaju.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wu.bookmarksfly.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wu.haigaiapp.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ve.bjjhwx.cn

Go:   // 手写循环
来源：http://by.huixinmuqiang.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vf.wgjwhj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://uk.521024.cn

[D24] 字典 / Map 基本操作
来源：http://ju.shxzukj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gq.panjiajie.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ci.huixiangedu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gh.lnxyls.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qh.jctech888.com.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jm.9csxet.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vi.wgjwhj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ox.huixiangedu.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jx.9csxet.cn

[D25] Set 集合去重与交并差
来源：http://xb.bookmarksfly.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://oa.gzmigu.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jp.shxzskj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://kl.hahajie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xh.hnjuh.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ph.yuntaijiaju.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://dr.shxzskj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mc.521024.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://we.bookmarksfly.cn

[D26] 数组转字符串
来源：http://ic.huixiangedu.cn

Py:   ", ".join(map(str, arr))
来源：http://nv.lnxyls.cn

PHP:  implode(", ", $arr);
来源：http://tn.nszjky.cn

JS:   arr.join(", ")
来源：http://be.huixiangedu.cn

TS:   arr.join(", ")
来源：http://fi.nicolike.cn

Java: String.join(", ", list)
来源：http://ze.nicolike.cn

Go:   strings.Join(strs, ", ")
来源：http://ki.colortex.cn

Ruby: arr.join(", ")
来源：http://zp.huanxung.cn

C#:   string.Join(", ", list)
来源：http://rp.nicolike.cn

================================================================================
来源：http://mk.bjjhwx.cn

E. 字符串处理
来源：http://jv.yuexingan06.cn

================================================================================
来源：http://bo.9csxet.cn

[E01] 拼接字符串
来源：http://uq.bookmarksfly.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xe.nszjky.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://sr.nszjky.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ys.yuntaijiaju.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ht.szsharing.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://cl.shxzskj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hx.lnxyls.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jw.nicolike.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://am.gzmigu.cn

[E02] 重复字符串
来源：http://od.hnjuh.cn

Py:   "ab" * 3
来源：http://lr.hnjuh.cn

PHP:  str_repeat("ab", 3);
来源：http://lr.nicolike.cn

JS:   "ab".repeat(3)
来源：http://oh.521024.cn

TS:   "ab".repeat(3)
来源：http://tm.9csxet.cn

Java: "ab".repeat(3)
来源：http://oi.yuntaijiaju.cn

Go:   strings.Repeat("ab", 3)
来源：http://og.chemitech.net.cn

Ruby: "ab" * 3
来源：http://ew.newstarts.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://iu.jianghongdianzi.cn

[E03] 截取子串
来源：http://ze.shxzukj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nv.yuntaijiaju.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qk.asd995.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zn.huixiangedu.cn

TS:   s.slice(1, 4)
来源：http://qp.huanxung.cn

Java: s.substring(1, 4)
来源：http://gu.nicolike.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://oy.szsharing.cn

Ruby: s[1, 3];  s[1..3]
来源：http://yo.jctech888.com.cn

C#:   s.Substring(1, 3)
来源：http://ha.bookmarksfly.cn

[E04] 查找子串位置
来源：http://md.muxihuayi.cn

Py:   s.find("x");  s.index("x")
来源：http://gc.wgjwhj.cn

PHP:  strpos($s, "x");
来源：http://rf.huanxung.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://st.huixinmuqiang.cn

TS:   s.indexOf("x")
来源：http://ni.bookmarksfly.cn

Java: s.indexOf("x")
来源：http://dx.lnxyls.cn

Go:   strings.Index(s, "x")
来源：http://ki.haigaiapp.cn

Ruby: s.index("x")
来源：http://ts.yuexingan06.cn

C#:   s.IndexOf("x")
来源：http://eg.wgjwhj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ub.asd995.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jz.wgjwhj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qj.hahajie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ym.wgjwhj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://gd.shxzskj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wv.huixiangedu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ld.wgjwhj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://dp.muxihuayi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ff.huixiangedu.cn

[E06] 替换子串
来源：http://ae.huixiangedu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://sr.jianghongdianzi.cn

PHP:  str_replace("a", "b", $s);
来源：http://pk.bookmarksfly.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://el.nicolike.cn

TS:   s.replaceAll("a", "b")
来源：http://ug.bookmarksfly.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kl.jctech888.com.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xw.szxytkj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://sh.nszjky.cn

C#:   s.Replace("a", "b")
来源：http://kw.asd995.cn

[E07] 按分隔符拆分
来源：http://zb.haigaiapp.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pi.yuntaijiaju.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qa.hnjuh.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://gv.jctech888.com.cn

TS:   s.split(",")
来源：http://xa.jctech888.com.cn

Java: s.split(",");  s.split("\\s+")
来源：http://na.nszjky.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ch.nicolike.cn

Ruby: s.split(",");  s.split
来源：http://dc.gzmigu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rk.asd995.cn

[E08] 数组按分隔符合并
来源：http://ok.huixinmuqiang.cn

Py:   ",".join(items)
来源：http://lc.nicolike.cn

PHP:  implode(",", $items);
来源：http://vs.bookmarksfly.cn

JS:   items.join(",")
来源：http://lu.yuntaijiaju.cn

TS:   items.join(",")
来源：http://ua.lnxyls.cn

Java: String.join(",", items)
来源：http://pl.wgjwhj.cn

Go:   strings.Join(items, ",")
来源：http://qz.521024.cn

Ruby: items.join(",")
来源：http://xd.szxytkj.cn

C#:   string.Join(",", items)
来源：http://gv.huixinmuqiang.cn

[E09] 去除所有空白字符
来源：http://vx.yuexingan06.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://js.colortex.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://cy.szxytkj.cn

JS:   s.replace(/\s+/g, "")
来源：http://yl.hnjuh.cn

TS:   s.replace(/\s+/g, "")
来源：http://qh.huanxung.cn

Java: s.replaceAll("\\s+", "")
来源：http://nz.jctech888.com.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://aw.wgjwhj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ff.shxzukj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://we.jctech888.com.cn

[E10] 左侧补零 / 定长填充
来源：http://lu.colortex.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ld.asd995.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ad.jianghongdianzi.cn

JS:   "7".padStart(3, "0")
来源：http://zk.hahajie.cn

TS:   "7".padStart(3, "0")
来源：http://tf.hnjuh.cn

Java: String.format("%03d", 7)
来源：http://wp.huanxung.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://fc.lnxyls.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://gx.jianghongdianzi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vs.huanxung.cn

[E11] 反转字符串
来源：http://qr.shtwfgs.cn

Py:   s[::-1]
来源：http://xi.9csxet.cn

PHP:  strrev($s);
来源：http://wr.521024.cn

JS:   [...s].reverse().join("")
来源：http://js.bjjhwx.cn

TS:   [...s].reverse().join("")
来源：http://db.jianghongdianzi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://qf.lnxyls.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://cb.haigaiapp.cn

Ruby: s.reverse
来源：http://hn.jianghongdianzi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://hd.nszjky.cn

[E12] 统计某字符出现次数
来源：http://rn.jctech888.com.cn

Py:   s.count("a")
来源：http://yf.nszjky.cn

PHP:  substr_count($s, "a");
来源：http://sx.chemitech.net.cn

JS:   s.split("a").length - 1
来源：http://fj.lnxyls.cn

TS:   s.split("a").length - 1
来源：http://tp.newstarts.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://eq.yuexingan06.cn

Go:   strings.Count(s, "a")
来源：http://fg.jianghongdianzi.cn

Ruby: s.count("a")
来源：http://cy.muxihuayi.cn

C#:   s.Count(c => c == 'a')
来源：http://tu.hahajie.cn

[E13] 逐字符遍历
来源：http://iz.shxzskj.cn

Py:   for ch in s: print(ch)
来源：http://do.huixiangedu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://yt.haigaiapp.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://yn.hnjuh.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://dv.shxzskj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qd.chemitech.net.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mi.bjjhwx.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ls.wgjwhj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://uo.jianghongdianzi.cn

[E14] URL 编码与 Base64
来源：http://fa.shxzukj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zg.shxzukj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://or.bjjhwx.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dh.hahajie.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pu.asd995.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://um.szsharing.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ri.asd995.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://il.jctech888.com.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nj.huixiangedu.cn

[E15] HTML 转义 / 反转义
来源：http://ab.gzmigu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://mo.newstarts.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vd.nszjky.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rz.bjjhwx.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://nh.wgjwhj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bg.szxytkj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ya.szxytkj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://yd.panjiajie.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://sj.nicolike.cn

[E16] 数字千分位
来源：http://df.colortex.cn

Py:   f"{1234567:,}"
来源：http://au.newstarts.cn

PHP:  number_format(1234567);
来源：http://dm.haigaiapp.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://bv.wgjwhj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://jl.szsharing.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://pr.bookmarksfly.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://uy.haigaiapp.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zh.szsharing.cn

C#:   1234567.ToString("N0")
来源：http://gc.haigaiapp.cn

[E17] 首字母大写
来源：http://on.bjjhwx.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ih.huanxung.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://kx.chemitech.net.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oz.colortex.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xt.szxytkj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://lx.yuexingan06.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mh.jianghongdianzi.cn

Ruby: s.capitalize
来源：http://ck.shxzukj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ax.hahajie.cn

[E18] 模板占位符替换
来源：http://jl.nszjky.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kg.muxihuayi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://uy.huanxung.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://dk.bookmarksfly.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://mb.lnxyls.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ke.colortex.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fh.nszjky.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fs.colortex.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://cx.shxzskj.cn

[E19] 多行文本按行拆分
来源：http://zz.yuntaijiaju.cn

Py:   s.splitlines()
来源：http://sa.wgjwhj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ay.haigaiapp.cn

JS:   s.split(/\r?\n/)
来源：http://rt.szsharing.cn

TS:   s.split(/\r?\n/)
来源：http://dz.szxytkj.cn

Java: s.lines().toList()
来源：http://uy.haigaiapp.cn

Go:   strings.Split(s, "\n")
来源：http://op.asd995.cn

Ruby: s.lines
来源：http://yk.szxytkj.cn

C#:   s.Split('\n')
来源：http://ja.hnjuh.cn

[E20] 判断字符串是否为空
来源：http://rr.muxihuayi.cn

Py:   if not s:
来源：http://cn.shtwfgs.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vy.nszjky.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hp.yuntaijiaju.cn

TS:   if (s === "") {}
来源：http://ym.yuntaijiaju.cn

Java: if (s.isEmpty()) {}
来源：http://bh.szxytkj.cn

Go:   if s == "" {}
来源：http://pw.bjjhwx.cn

Ruby: if s.empty?
来源：http://gy.huixiangedu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bi.haigaiapp.cn

[E21] 超长截断加省略号
来源：http://fd.jianghongdianzi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rf.huixiangedu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xa.szsharing.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ht.jianghongdianzi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xo.huixinmuqiang.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ag.bjjhwx.cn

Go:   // 按 rune 判断长度后截断
来源：http://uy.yuexingan06.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tq.asd995.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ca.bookmarksfly.cn

[E22] 字节长度与字符长度
来源：http://ud.panjiajie.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://nn.bookmarksfly.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cf.hahajie.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://an.panjiajie.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://om.nszjky.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://my.wgjwhj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hm.huixinmuqiang.cn

Ruby: s.bytesize;  s.length
来源：http://dm.9csxet.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dd.lnxyls.cn

================================================================================
来源：http://ul.haigaiapp.cn

F. 文件与目录
来源：http://kf.shxzskj.cn

================================================================================
来源：http://si.asd995.cn

[F01] 读取整个文件
来源：http://pm.huixiangedu.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xz.huixiangedu.cn

PHP:  file_get_contents("a.txt");
来源：http://ne.nicolike.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qv.huixinmuqiang.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ba.9csxet.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://up.yuexingan06.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hv.hahajie.cn

Ruby: File.read("a.txt")
来源：http://un.shxzukj.cn

C#:   File.ReadAllText("a.txt");
来源：http://tf.shxzskj.cn

[F02] 逐行读取文件
来源：http://bz.szsharing.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://yc.gzmigu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cl.szxytkj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ka.panjiajie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zf.huixiangedu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://cx.nicolike.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xk.shxzukj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://cs.gzmigu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mk.huixiangedu.cn

[F03] 写入文件（覆盖）
来源：http://fb.huixinmuqiang.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://yx.hahajie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://mm.521024.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ro.521024.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ah.shxzskj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://cw.colortex.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://af.szxytkj.cn

Ruby: File.write("a.txt", "hi")
来源：http://yb.jianghongdianzi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tg.jianghongdianzi.cn

[F04] 追加写入文件
来源：http://ss.szxytkj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ip.huixinmuqiang.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ja.gzmigu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qb.9csxet.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://md.shxzskj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mi.bjjhwx.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hm.jctech888.com.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://oe.yuexingan06.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gy.hnjuh.cn

[F05] 判断文件或目录是否存在
来源：http://yz.asd995.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fr.szxytkj.cn

PHP:  file_exists("a.txt");
来源：http://sc.haigaiapp.cn

JS:   fs.existsSync("a.txt")
来源：http://xv.colortex.cn


<!-- 参考信息 -->