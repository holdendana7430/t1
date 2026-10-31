代发 wailian999

Ruby: arr.tally
来源：http://yc.asd995.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://gz.chemitech.net.cn

[D21] 判断是否包含某元素
来源：http://ph.nicolike.cn

Py:   x in arr
来源：http://pj.hahajie.cn

PHP:  in_array($x, $arr, true);
来源：http://xn.panjiajie.cn

JS:   arr.includes(x)
来源：http://bw.yuntaijiaju.cn

TS:   arr.includes(x)
来源：http://mp.gzmigu.cn

Java: list.contains(x)
来源：http://jz.shtwfgs.cn

Go:   slices.Contains(arr, x)
来源：http://hg.jianghongdianzi.cn

Ruby: arr.include?(x)
来源：http://zn.colortex.cn

C#:   list.Contains(x)
来源：http://in.yuntaijiaju.cn

[D22] 复制数组（避免共享引用）
来源：http://za.hnjuh.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://yh.newstarts.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xf.nicolike.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dm.shxzukj.cn

TS:   [...arr];
来源：http://vj.muxihuayi.cn

Java: new ArrayList<>(list);
来源：http://qu.huanxung.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ey.huixinmuqiang.cn

Ruby: arr.dup;  arr.clone
来源：http://dq.nszjky.cn

C#:   new List<int>(list);
来源：http://xc.panjiajie.cn

[D23] reduce 累积计算
来源：http://wc.yuexingan06.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://px.huanxung.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ti.panjiajie.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xi.chemitech.net.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://an.nicolike.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://qh.nszjky.cn

Go:   // 手写循环
来源：http://rt.yuntaijiaju.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ic.hahajie.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xs.gzmigu.cn

[D24] 字典 / Map 基本操作
来源：http://fa.bookmarksfly.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kw.colortex.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pd.huixiangedu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xw.hahajie.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ho.521024.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ds.muxihuayi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vp.lnxyls.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vz.newstarts.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dt.hnjuh.cn

[D25] Set 集合去重与交并差
来源：http://mx.yuntaijiaju.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://dq.hnjuh.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://nh.haigaiapp.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fo.shxzskj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vh.panjiajie.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://sc.huanxung.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gd.chemitech.net.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xf.chemitech.net.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://my.lnxyls.cn

[D26] 数组转字符串
来源：http://zb.huixinmuqiang.cn

Py:   ", ".join(map(str, arr))
来源：http://cb.nicolike.cn

PHP:  implode(", ", $arr);
来源：http://ap.asd995.cn

JS:   arr.join(", ")
来源：http://zc.nicolike.cn

TS:   arr.join(", ")
来源：http://qe.521024.cn

Java: String.join(", ", list)
来源：http://az.jctech888.com.cn

Go:   strings.Join(strs, ", ")
来源：http://dq.hnjuh.cn

Ruby: arr.join(", ")
来源：http://xj.asd995.cn

C#:   string.Join(", ", list)
来源：http://yg.huixiangedu.cn

================================================================================
来源：http://hv.9csxet.cn

E. 字符串处理
来源：http://zx.panjiajie.cn

================================================================================
来源：http://px.szxytkj.cn

[E01] 拼接字符串
来源：http://sk.bookmarksfly.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fn.9csxet.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zk.wgjwhj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://yc.gzmigu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://uo.jianghongdianzi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ui.9csxet.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ef.lnxyls.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gn.newstarts.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hi.lnxyls.cn

[E02] 重复字符串
来源：http://hr.bjjhwx.cn

Py:   "ab" * 3
来源：http://pk.lnxyls.cn

PHP:  str_repeat("ab", 3);
来源：http://ao.huixinmuqiang.cn

JS:   "ab".repeat(3)
来源：http://iz.hahajie.cn

TS:   "ab".repeat(3)
来源：http://or.szsharing.cn

Java: "ab".repeat(3)
来源：http://dx.nicolike.cn

Go:   strings.Repeat("ab", 3)
来源：http://pf.muxihuayi.cn

Ruby: "ab" * 3
来源：http://jr.szsharing.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mk.haigaiapp.cn

[E03] 截取子串
来源：http://bb.szxytkj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cd.haigaiapp.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ky.huanxung.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ly.nicolike.cn

TS:   s.slice(1, 4)
来源：http://js.bjjhwx.cn

Java: s.substring(1, 4)
来源：http://sp.jianghongdianzi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ps.521024.cn

Ruby: s[1, 3];  s[1..3]
来源：http://me.yuntaijiaju.cn

C#:   s.Substring(1, 3)
来源：http://xp.newstarts.cn

[E04] 查找子串位置
来源：http://vd.nszjky.cn

Py:   s.find("x");  s.index("x")
来源：http://oq.wgjwhj.cn

PHP:  strpos($s, "x");
来源：http://ml.hahajie.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://cj.panjiajie.cn

TS:   s.indexOf("x")
来源：http://gc.newstarts.cn

Java: s.indexOf("x")
来源：http://js.bookmarksfly.cn

Go:   strings.Index(s, "x")
来源：http://od.szxytkj.cn

Ruby: s.index("x")
来源：http://kd.nszjky.cn

C#:   s.IndexOf("x")
来源：http://ya.shtwfgs.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://lh.nszjky.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jc.521024.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mj.szxytkj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ym.bookmarksfly.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ys.bookmarksfly.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ig.muxihuayi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://yx.haigaiapp.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://bu.asd995.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vs.szxytkj.cn

[E06] 替换子串
来源：http://ql.bjjhwx.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wm.newstarts.cn

PHP:  str_replace("a", "b", $s);
来源：http://hf.huanxung.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://os.hahajie.cn

TS:   s.replaceAll("a", "b")
来源：http://jt.panjiajie.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ca.9csxet.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vy.bookmarksfly.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hj.hnjuh.cn

C#:   s.Replace("a", "b")
来源：http://ax.huixinmuqiang.cn

[E07] 按分隔符拆分
来源：http://oz.bookmarksfly.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qm.hahajie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jk.szsharing.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://oq.shtwfgs.cn

TS:   s.split(",")
来源：http://yf.panjiajie.cn

Java: s.split(",");  s.split("\\s+")
来源：http://rr.shtwfgs.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bt.jctech888.com.cn

Ruby: s.split(",");  s.split
来源：http://gw.huixiangedu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rn.shxzukj.cn

[E08] 数组按分隔符合并
来源：http://et.asd995.cn

Py:   ",".join(items)
来源：http://oh.yuexingan06.cn

PHP:  implode(",", $items);
来源：http://ww.hahajie.cn

JS:   items.join(",")
来源：http://cv.shtwfgs.cn

TS:   items.join(",")
来源：http://fl.asd995.cn

Java: String.join(",", items)
来源：http://rb.szsharing.cn

Go:   strings.Join(items, ",")
来源：http://na.huixinmuqiang.cn

Ruby: items.join(",")
来源：http://qt.panjiajie.cn

C#:   string.Join(",", items)
来源：http://ym.jctech888.com.cn

[E09] 去除所有空白字符
来源：http://vt.jctech888.com.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://uf.hnjuh.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bd.huixiangedu.cn

JS:   s.replace(/\s+/g, "")
来源：http://kw.szxytkj.cn

TS:   s.replace(/\s+/g, "")
来源：http://hf.haigaiapp.cn

Java: s.replaceAll("\\s+", "")
来源：http://ib.yuntaijiaju.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://qs.9csxet.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ux.szxytkj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fa.huanxung.cn

[E10] 左侧补零 / 定长填充
来源：http://nj.nicolike.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qf.shxzukj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ze.szsharing.cn

JS:   "7".padStart(3, "0")
来源：http://nj.yuntaijiaju.cn

TS:   "7".padStart(3, "0")
来源：http://of.521024.cn

Java: String.format("%03d", 7)
来源：http://cq.haigaiapp.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://cj.bookmarksfly.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://gy.szxytkj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ge.9csxet.cn

[E11] 反转字符串
来源：http://hr.szxytkj.cn

Py:   s[::-1]
来源：http://hr.jctech888.com.cn

PHP:  strrev($s);
来源：http://og.bookmarksfly.cn

JS:   [...s].reverse().join("")
来源：http://mq.shxzskj.cn

TS:   [...s].reverse().join("")
来源：http://eo.jctech888.com.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://xq.9csxet.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://fn.nicolike.cn

Ruby: s.reverse
来源：http://ng.colortex.cn

C#:   new string(s.Reverse().ToArray())
来源：http://nu.9csxet.cn

[E12] 统计某字符出现次数
来源：http://bx.nszjky.cn

Py:   s.count("a")
来源：http://ql.huixiangedu.cn

PHP:  substr_count($s, "a");
来源：http://hn.gzmigu.cn

JS:   s.split("a").length - 1
来源：http://ai.szsharing.cn

TS:   s.split("a").length - 1
来源：http://ve.yuexingan06.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://op.szsharing.cn

Go:   strings.Count(s, "a")
来源：http://no.jctech888.com.cn

Ruby: s.count("a")
来源：http://xp.jctech888.com.cn

C#:   s.Count(c => c == 'a')
来源：http://fy.jctech888.com.cn

[E13] 逐字符遍历
来源：http://og.hnjuh.cn

Py:   for ch in s: print(ch)
来源：http://zh.bjjhwx.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dg.yuntaijiaju.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://wj.newstarts.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://rx.hnjuh.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://sd.panjiajie.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pb.yuexingan06.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://nh.muxihuayi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jx.gzmigu.cn

[E14] URL 编码与 Base64
来源：http://rj.nszjky.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wt.9csxet.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ja.shxzukj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://uc.shxzukj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://yj.chemitech.net.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://dy.huanxung.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://kc.lnxyls.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://en.yuexingan06.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nj.yuntaijiaju.cn

[E15] HTML 转义 / 反转义
来源：http://tv.huixiangedu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://fw.shtwfgs.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://cp.colortex.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://sc.nicolike.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://iw.nicolike.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://db.wgjwhj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bg.newstarts.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wt.521024.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jn.shxzskj.cn

[E16] 数字千分位
来源：http://mw.newstarts.cn

Py:   f"{1234567:,}"
来源：http://lz.9csxet.cn

PHP:  number_format(1234567);
来源：http://kq.nicolike.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://fx.huanxung.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://he.colortex.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://uf.panjiajie.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ev.shxzskj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pm.huixiangedu.cn

C#:   1234567.ToString("N0")
来源：http://lg.muxihuayi.cn

[E17] 首字母大写
来源：http://dr.hahajie.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://oy.yuntaijiaju.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://lc.huixinmuqiang.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oa.yuntaijiaju.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wc.bookmarksfly.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://in.asd995.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ea.muxihuayi.cn

Ruby: s.capitalize
来源：http://mt.9csxet.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gh.nicolike.cn

[E18] 模板占位符替换
来源：http://fy.huanxung.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://cd.shxzukj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yi.jianghongdianzi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://mg.521024.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ov.bookmarksfly.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mh.jctech888.com.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://et.jianghongdianzi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hq.shxzskj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wt.yuexingan06.cn

[E19] 多行文本按行拆分
来源：http://wv.haigaiapp.cn

Py:   s.splitlines()
来源：http://hx.huixiangedu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://fr.panjiajie.cn

JS:   s.split(/\r?\n/)
来源：http://at.panjiajie.cn

TS:   s.split(/\r?\n/)
来源：http://hp.szxytkj.cn

Java: s.lines().toList()
来源：http://bi.szsharing.cn

Go:   strings.Split(s, "\n")
来源：http://gf.szxytkj.cn

Ruby: s.lines
来源：http://km.asd995.cn

C#:   s.Split('\n')
来源：http://tv.9csxet.cn

[E20] 判断字符串是否为空
来源：http://op.panjiajie.cn

Py:   if not s:
来源：http://pt.jctech888.com.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://sj.jianghongdianzi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://pr.huixiangedu.cn

TS:   if (s === "") {}
来源：http://zx.haigaiapp.cn

Java: if (s.isEmpty()) {}
来源：http://ff.szxytkj.cn

Go:   if s == "" {}
来源：http://gw.shxzskj.cn

Ruby: if s.empty?
来源：http://ds.newstarts.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gb.hnjuh.cn

[E21] 超长截断加省略号
来源：http://ow.haigaiapp.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://gd.muxihuayi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://di.asd995.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fc.szsharing.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vo.haigaiapp.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xy.bjjhwx.cn

Go:   // 按 rune 判断长度后截断
来源：http://yr.huixinmuqiang.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bo.nszjky.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ah.lnxyls.cn

[E22] 字节长度与字符长度
来源：http://bt.gzmigu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ch.muxihuayi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mj.huixiangedu.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://me.huixinmuqiang.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vt.hahajie.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://uf.muxihuayi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ej.yuntaijiaju.cn

Ruby: s.bytesize;  s.length
来源：http://cs.lnxyls.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://eo.newstarts.cn

================================================================================
来源：http://up.shtwfgs.cn

F. 文件与目录
来源：http://rj.asd995.cn

================================================================================
来源：http://lj.lnxyls.cn

[F01] 读取整个文件
来源：http://oz.szsharing.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ld.hnjuh.cn

PHP:  file_get_contents("a.txt");
来源：http://eh.shtwfgs.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ug.bjjhwx.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://za.gzmigu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ix.jctech888.com.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nw.jctech888.com.cn

Ruby: File.read("a.txt")
来源：http://kk.shxzukj.cn

C#:   File.ReadAllText("a.txt");
来源：http://em.shxzskj.cn

[F02] 逐行读取文件
来源：http://fb.yuntaijiaju.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://aa.szxytkj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://tm.huixinmuqiang.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uv.gzmigu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://of.9csxet.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dk.szxytkj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fl.chemitech.net.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jg.huanxung.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://kk.wgjwhj.cn

[F03] 写入文件（覆盖）
来源：http://zw.huanxung.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fm.newstarts.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://st.bookmarksfly.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wy.hahajie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ca.shxzskj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zb.yuexingan06.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wz.bookmarksfly.cn

Ruby: File.write("a.txt", "hi")
来源：http://ig.521024.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ok.jianghongdianzi.cn

[F04] 追加写入文件
来源：http://cm.gzmigu.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pa.panjiajie.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://lo.shxzukj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://iw.asd995.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://un.bookmarksfly.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ou.gzmigu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://cj.lnxyls.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ha.yuexingan06.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rf.huixiangedu.cn

[F05] 判断文件或目录是否存在
来源：http://qv.muxihuayi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://oy.asd995.cn

PHP:  file_exists("a.txt");
来源：http://do.muxihuayi.cn

JS:   fs.existsSync("a.txt")
来源：http://cf.yuexingan06.cn


<!-- 参考信息 -->