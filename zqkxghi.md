代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hd.wgjwhj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://iq.shxzukj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rs.colortex.cn

Go:   // 手写 map[T]int
来源：http://oz.colortex.cn

Ruby: arr.tally
来源：http://cd.shxzukj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://eq.yuntaijiaju.cn

[D21] 判断是否包含某元素
来源：http://kx.wgjwhj.cn

Py:   x in arr
来源：http://td.bjjhwx.cn

PHP:  in_array($x, $arr, true);
来源：http://ue.lnxyls.cn

JS:   arr.includes(x)
来源：http://yx.bjjhwx.cn

TS:   arr.includes(x)
来源：http://gt.newstarts.cn

Java: list.contains(x)
来源：http://dl.huanxung.cn

Go:   slices.Contains(arr, x)
来源：http://qw.hahajie.cn

Ruby: arr.include?(x)
来源：http://tx.panjiajie.cn

C#:   list.Contains(x)
来源：http://jp.bookmarksfly.cn

[D22] 复制数组（避免共享引用）
来源：http://uz.shtwfgs.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://sq.bookmarksfly.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rp.huanxung.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wy.nicolike.cn

TS:   [...arr];
来源：http://fi.bjjhwx.cn

Java: new ArrayList<>(list);
来源：http://hh.szxytkj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://is.hnjuh.cn

Ruby: arr.dup;  arr.clone
来源：http://yi.colortex.cn

C#:   new List<int>(list);
来源：http://de.muxihuayi.cn

[D23] reduce 累积计算
来源：http://yl.asd995.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ee.hahajie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qz.colortex.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bq.bjjhwx.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ax.nszjky.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://qf.521024.cn

Go:   // 手写循环
来源：http://vl.szxytkj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ax.colortex.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://em.gzmigu.cn

[D24] 字典 / Map 基本操作
来源：http://ha.colortex.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jt.nicolike.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gt.shxzukj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://au.nicolike.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zn.colortex.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://eu.chemitech.net.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://nk.lnxyls.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lj.wgjwhj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rx.shxzukj.cn

[D25] Set 集合去重与交并差
来源：http://cr.hnjuh.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ni.jctech888.com.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fn.9csxet.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://lm.huixiangedu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qr.shxzskj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zh.colortex.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://id.haigaiapp.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ka.shxzukj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bn.shtwfgs.cn

[D26] 数组转字符串
来源：http://wg.hahajie.cn

Py:   ", ".join(map(str, arr))
来源：http://iv.yuexingan06.cn

PHP:  implode(", ", $arr);
来源：http://jf.bookmarksfly.cn

JS:   arr.join(", ")
来源：http://mz.huixiangedu.cn

TS:   arr.join(", ")
来源：http://jl.panjiajie.cn

Java: String.join(", ", list)
来源：http://ng.huixinmuqiang.cn

Go:   strings.Join(strs, ", ")
来源：http://xh.lnxyls.cn

Ruby: arr.join(", ")
来源：http://cx.haigaiapp.cn

C#:   string.Join(", ", list)
来源：http://by.shtwfgs.cn

================================================================================
来源：http://gq.nszjky.cn

E. 字符串处理
来源：http://ok.shtwfgs.cn

================================================================================
来源：http://rq.jctech888.com.cn

[E01] 拼接字符串
来源：http://ze.haigaiapp.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://br.chemitech.net.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://kd.panjiajie.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jz.gzmigu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vo.panjiajie.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://jv.szxytkj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://kw.hnjuh.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://uc.wgjwhj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vo.bjjhwx.cn

[E02] 重复字符串
来源：http://wq.shxzskj.cn

Py:   "ab" * 3
来源：http://nr.huixinmuqiang.cn

PHP:  str_repeat("ab", 3);
来源：http://dq.shtwfgs.cn

JS:   "ab".repeat(3)
来源：http://jt.bookmarksfly.cn

TS:   "ab".repeat(3)
来源：http://zj.newstarts.cn

Java: "ab".repeat(3)
来源：http://no.chemitech.net.cn

Go:   strings.Repeat("ab", 3)
来源：http://pc.szxytkj.cn

Ruby: "ab" * 3
来源：http://fw.huixiangedu.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lk.huanxung.cn

[E03] 截取子串
来源：http://en.shxzskj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rc.9csxet.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wy.jctech888.com.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vh.muxihuayi.cn

TS:   s.slice(1, 4)
来源：http://fa.asd995.cn

Java: s.substring(1, 4)
来源：http://jf.haigaiapp.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ci.huixiangedu.cn

Ruby: s[1, 3];  s[1..3]
来源：http://qa.9csxet.cn

C#:   s.Substring(1, 3)
来源：http://np.yuexingan06.cn

[E04] 查找子串位置
来源：http://iw.lnxyls.cn

Py:   s.find("x");  s.index("x")
来源：http://lo.szxytkj.cn

PHP:  strpos($s, "x");
来源：http://xq.huanxung.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://pm.huanxung.cn

TS:   s.indexOf("x")
来源：http://km.shtwfgs.cn

Java: s.indexOf("x")
来源：http://fw.nszjky.cn

Go:   strings.Index(s, "x")
来源：http://ku.huixiangedu.cn

Ruby: s.index("x")
来源：http://gr.huixinmuqiang.cn

C#:   s.IndexOf("x")
来源：http://mx.chemitech.net.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://tp.shxzskj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ht.hahajie.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fn.shtwfgs.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ct.gzmigu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://kc.szxytkj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qj.bookmarksfly.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ej.lnxyls.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://al.hahajie.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ot.lnxyls.cn

[E06] 替换子串
来源：http://yq.bookmarksfly.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fw.asd995.cn

PHP:  str_replace("a", "b", $s);
来源：http://xx.szxytkj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kq.9csxet.cn

TS:   s.replaceAll("a", "b")
来源：http://ar.shtwfgs.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sb.521024.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rw.newstarts.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://uw.huanxung.cn

C#:   s.Replace("a", "b")
来源：http://gl.jctech888.com.cn

[E07] 按分隔符拆分
来源：http://ks.bookmarksfly.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lh.shxzskj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://cy.colortex.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ov.hnjuh.cn

TS:   s.split(",")
来源：http://jy.jianghongdianzi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ya.yuntaijiaju.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tn.521024.cn

Ruby: s.split(",");  s.split
来源：http://tm.jianghongdianzi.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fe.huixiangedu.cn

[E08] 数组按分隔符合并
来源：http://us.colortex.cn

Py:   ",".join(items)
来源：http://so.panjiajie.cn

PHP:  implode(",", $items);
来源：http://ji.panjiajie.cn

JS:   items.join(",")
来源：http://az.huixinmuqiang.cn

TS:   items.join(",")
来源：http://vz.chemitech.net.cn

Java: String.join(",", items)
来源：http://iq.muxihuayi.cn

Go:   strings.Join(items, ",")
来源：http://mb.yuexingan06.cn

Ruby: items.join(",")
来源：http://xp.nszjky.cn

C#:   string.Join(",", items)
来源：http://ip.huanxung.cn

[E09] 去除所有空白字符
来源：http://rr.gzmigu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zq.colortex.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qj.haigaiapp.cn

JS:   s.replace(/\s+/g, "")
来源：http://lq.bjjhwx.cn

TS:   s.replace(/\s+/g, "")
来源：http://cg.newstarts.cn

Java: s.replaceAll("\\s+", "")
来源：http://mj.yuntaijiaju.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://we.bookmarksfly.cn

Ruby: s.gsub(/\s+/, "")
来源：http://dg.huixiangedu.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://na.huixiangedu.cn

[E10] 左侧补零 / 定长填充
来源：http://mk.asd995.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ly.newstarts.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ez.asd995.cn

JS:   "7".padStart(3, "0")
来源：http://cl.hahajie.cn

TS:   "7".padStart(3, "0")
来源：http://ql.szsharing.cn

Java: String.format("%03d", 7)
来源：http://wm.szxytkj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://yt.shtwfgs.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hg.521024.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rz.wgjwhj.cn

[E11] 反转字符串
来源：http://mj.newstarts.cn

Py:   s[::-1]
来源：http://cy.bookmarksfly.cn

PHP:  strrev($s);
来源：http://wu.chemitech.net.cn

JS:   [...s].reverse().join("")
来源：http://xz.panjiajie.cn

TS:   [...s].reverse().join("")
来源：http://gz.chemitech.net.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ts.bjjhwx.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://is.bjjhwx.cn

Ruby: s.reverse
来源：http://ro.hnjuh.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ze.9csxet.cn

[E12] 统计某字符出现次数
来源：http://es.newstarts.cn

Py:   s.count("a")
来源：http://dd.yuntaijiaju.cn

PHP:  substr_count($s, "a");
来源：http://uw.huixiangedu.cn

JS:   s.split("a").length - 1
来源：http://qb.chemitech.net.cn

TS:   s.split("a").length - 1
来源：http://pf.chemitech.net.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qt.bookmarksfly.cn

Go:   strings.Count(s, "a")
来源：http://af.yuntaijiaju.cn

Ruby: s.count("a")
来源：http://ot.lnxyls.cn

C#:   s.Count(c => c == 'a')
来源：http://hr.shxzskj.cn

[E13] 逐字符遍历
来源：http://mb.huixinmuqiang.cn

Py:   for ch in s: print(ch)
来源：http://jo.wgjwhj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ar.shxzukj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://wr.panjiajie.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://rm.muxihuayi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://aw.newstarts.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://cn.9csxet.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://tz.panjiajie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qz.wgjwhj.cn

[E14] URL 编码与 Base64
来源：http://pl.yuntaijiaju.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://js.shxzskj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://td.huanxung.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dp.jctech888.com.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://lk.panjiajie.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hn.szsharing.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fs.muxihuayi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://sl.shxzukj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bz.muxihuayi.cn

[E15] HTML 转义 / 反转义
来源：http://wl.shxzskj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://bn.wgjwhj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://sd.shtwfgs.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ea.yuntaijiaju.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ua.szxytkj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vv.shtwfgs.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mz.gzmigu.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ms.bjjhwx.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://po.521024.cn

[E16] 数字千分位
来源：http://jl.gzmigu.cn

Py:   f"{1234567:,}"
来源：http://qc.newstarts.cn

PHP:  number_format(1234567);
来源：http://ar.hahajie.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://gq.shxzskj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://be.nszjky.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tz.shxzskj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wv.haigaiapp.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://lq.shxzskj.cn

C#:   1234567.ToString("N0")
来源：http://kv.huixiangedu.cn

[E17] 首字母大写
来源：http://zh.szsharing.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xq.shxzskj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://kp.colortex.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sy.szxytkj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nu.bookmarksfly.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hg.huixinmuqiang.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://si.gzmigu.cn

Ruby: s.capitalize
来源：http://fp.jianghongdianzi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://al.jianghongdianzi.cn

[E18] 模板占位符替换
来源：http://wu.nszjky.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://pt.hnjuh.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://io.yuexingan06.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://xk.szxytkj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://sn.hahajie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vx.shtwfgs.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bm.haigaiapp.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://yw.nicolike.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yo.yuexingan06.cn

[E19] 多行文本按行拆分
来源：http://ip.huixiangedu.cn

Py:   s.splitlines()
来源：http://vw.521024.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zv.9csxet.cn

JS:   s.split(/\r?\n/)
来源：http://vb.jianghongdianzi.cn

TS:   s.split(/\r?\n/)
来源：http://ze.gzmigu.cn

Java: s.lines().toList()
来源：http://xk.nicolike.cn

Go:   strings.Split(s, "\n")
来源：http://zc.shxzukj.cn

Ruby: s.lines
来源：http://fh.szxytkj.cn

C#:   s.Split('\n')
来源：http://ux.9csxet.cn

[E20] 判断字符串是否为空
来源：http://ni.newstarts.cn

Py:   if not s:
来源：http://ge.wgjwhj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://no.newstarts.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rl.muxihuayi.cn

TS:   if (s === "") {}
来源：http://fj.haigaiapp.cn

Java: if (s.isEmpty()) {}
来源：http://gx.521024.cn

Go:   if s == "" {}
来源：http://pp.szxytkj.cn

Ruby: if s.empty?
来源：http://oq.shxzskj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ew.bookmarksfly.cn

[E21] 超长截断加省略号
来源：http://ry.nszjky.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ii.asd995.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://by.newstarts.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zl.panjiajie.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://oy.szsharing.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jo.bookmarksfly.cn

Go:   // 按 rune 判断长度后截断
来源：http://bn.asd995.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fg.nszjky.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jg.gzmigu.cn

[E22] 字节长度与字符长度
来源：http://bw.muxihuayi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xl.hnjuh.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uz.huixinmuqiang.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wq.bookmarksfly.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wt.asd995.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rm.bjjhwx.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gx.chemitech.net.cn

Ruby: s.bytesize;  s.length
来源：http://lj.newstarts.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mq.bookmarksfly.cn

================================================================================
来源：http://ab.nszjky.cn

F. 文件与目录
来源：http://tp.asd995.cn

================================================================================
来源：http://ij.huanxung.cn

[F01] 读取整个文件
来源：http://yz.nszjky.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dt.yuexingan06.cn

PHP:  file_get_contents("a.txt");
来源：http://xj.huixiangedu.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dh.yuexingan06.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xe.muxihuayi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://rc.shtwfgs.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vo.bjjhwx.cn

Ruby: File.read("a.txt")
来源：http://ta.shtwfgs.cn

C#:   File.ReadAllText("a.txt");
来源：http://dx.jianghongdianzi.cn

[F02] 逐行读取文件
来源：http://jt.huixiangedu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bq.gzmigu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ll.shxzukj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hq.bookmarksfly.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bg.shxzukj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pm.jianghongdianzi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pp.yuntaijiaju.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zq.colortex.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dq.haigaiapp.cn

[F03] 写入文件（覆盖）
来源：http://nu.haigaiapp.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gf.lnxyls.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://pf.asd995.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tl.nszjky.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pm.chemitech.net.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ce.chemitech.net.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ue.gzmigu.cn

Ruby: File.write("a.txt", "hi")
来源：http://wh.hnjuh.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zh.nicolike.cn

[F04] 追加写入文件
来源：http://fy.newstarts.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ma.nszjky.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hv.yuntaijiaju.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yo.colortex.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mf.gzmigu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qa.panjiajie.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hg.lnxyls.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hq.szsharing.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://pb.521024.cn


<!-- 参考信息 -->