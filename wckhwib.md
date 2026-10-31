代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rz.yuntaijiaju.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sb.hahajie.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://kl.shtwfgs.cn

Go:   // 手写 map[T]int
来源：http://qp.haigaiapp.cn

Ruby: arr.tally
来源：http://tz.asd995.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://om.shtwfgs.cn

[D21] 判断是否包含某元素
来源：http://tq.gzmigu.cn

Py:   x in arr
来源：http://uf.9csxet.cn

PHP:  in_array($x, $arr, true);
来源：http://ts.jctech888.com.cn

JS:   arr.includes(x)
来源：http://zq.nicolike.cn

TS:   arr.includes(x)
来源：http://mn.gzmigu.cn

Java: list.contains(x)
来源：http://ui.yuexingan06.cn

Go:   slices.Contains(arr, x)
来源：http://il.newstarts.cn

Ruby: arr.include?(x)
来源：http://vn.hnjuh.cn

C#:   list.Contains(x)
来源：http://uv.chemitech.net.cn

[D22] 复制数组（避免共享引用）
来源：http://ue.nicolike.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gj.muxihuayi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://sl.huixinmuqiang.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vz.nszjky.cn

TS:   [...arr];
来源：http://vp.521024.cn

Java: new ArrayList<>(list);
来源：http://vb.9csxet.cn

Go:   copied := append([]int(nil), arr...)
来源：http://jn.muxihuayi.cn

Ruby: arr.dup;  arr.clone
来源：http://pe.wgjwhj.cn

C#:   new List<int>(list);
来源：http://hz.bjjhwx.cn

[D23] reduce 累积计算
来源：http://dt.panjiajie.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ug.bookmarksfly.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tr.gzmigu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uu.wgjwhj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zp.shxzukj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://hs.yuexingan06.cn

Go:   // 手写循环
来源：http://hs.newstarts.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://tg.asd995.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://yg.yuntaijiaju.cn

[D24] 字典 / Map 基本操作
来源：http://ck.shxzskj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gc.shxzskj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://nc.shtwfgs.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hy.jianghongdianzi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ku.jianghongdianzi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jk.hnjuh.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hv.bookmarksfly.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://dj.bjjhwx.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://yc.lnxyls.cn

[D25] Set 集合去重与交并差
来源：http://jv.yuexingan06.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wx.nszjky.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ho.szsharing.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://tr.colortex.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vi.colortex.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://pa.huanxung.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rp.wgjwhj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ca.wgjwhj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://he.huanxung.cn

[D26] 数组转字符串
来源：http://bo.9csxet.cn

Py:   ", ".join(map(str, arr))
来源：http://fo.bjjhwx.cn

PHP:  implode(", ", $arr);
来源：http://bp.chemitech.net.cn

JS:   arr.join(", ")
来源：http://ak.shxzukj.cn

TS:   arr.join(", ")
来源：http://um.bookmarksfly.cn

Java: String.join(", ", list)
来源：http://qf.jianghongdianzi.cn

Go:   strings.Join(strs, ", ")
来源：http://gh.huanxung.cn

Ruby: arr.join(", ")
来源：http://fw.szsharing.cn

C#:   string.Join(", ", list)
来源：http://qr.yuexingan06.cn

================================================================================
来源：http://we.shxzskj.cn

E. 字符串处理
来源：http://jm.yuntaijiaju.cn

================================================================================
来源：http://al.hahajie.cn

[E01] 拼接字符串
来源：http://vd.bookmarksfly.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vn.asd995.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vf.huanxung.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dg.szsharing.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ei.lnxyls.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lc.nicolike.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://sr.bjjhwx.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://on.szxytkj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qa.nicolike.cn

[E02] 重复字符串
来源：http://ip.bjjhwx.cn

Py:   "ab" * 3
来源：http://ty.jianghongdianzi.cn

PHP:  str_repeat("ab", 3);
来源：http://aj.bookmarksfly.cn

JS:   "ab".repeat(3)
来源：http://zx.gzmigu.cn

TS:   "ab".repeat(3)
来源：http://ay.bjjhwx.cn

Java: "ab".repeat(3)
来源：http://rs.shxzskj.cn

Go:   strings.Repeat("ab", 3)
来源：http://bf.shxzskj.cn

Ruby: "ab" * 3
来源：http://tz.muxihuayi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jd.lnxyls.cn

[E03] 截取子串
来源：http://jv.haigaiapp.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hh.asd995.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ln.huixiangedu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://np.nszjky.cn

TS:   s.slice(1, 4)
来源：http://cl.yuexingan06.cn

Java: s.substring(1, 4)
来源：http://jn.9csxet.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qi.chemitech.net.cn

Ruby: s[1, 3];  s[1..3]
来源：http://mn.jianghongdianzi.cn

C#:   s.Substring(1, 3)
来源：http://xt.521024.cn

[E04] 查找子串位置
来源：http://mi.yuexingan06.cn

Py:   s.find("x");  s.index("x")
来源：http://hl.jctech888.com.cn

PHP:  strpos($s, "x");
来源：http://kx.wgjwhj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ni.bookmarksfly.cn

TS:   s.indexOf("x")
来源：http://yc.muxihuayi.cn

Java: s.indexOf("x")
来源：http://qp.huixiangedu.cn

Go:   strings.Index(s, "x")
来源：http://jh.asd995.cn

Ruby: s.index("x")
来源：http://aj.huanxung.cn

C#:   s.IndexOf("x")
来源：http://rw.panjiajie.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://bx.asd995.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mv.lnxyls.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://dl.szxytkj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ym.gzmigu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://rz.shtwfgs.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jp.chemitech.net.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zu.muxihuayi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mt.shxzukj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jj.gzmigu.cn

[E06] 替换子串
来源：http://ke.hahajie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ly.muxihuayi.cn

PHP:  str_replace("a", "b", $s);
来源：http://zx.muxihuayi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nr.nszjky.cn

TS:   s.replaceAll("a", "b")
来源：http://pj.huixinmuqiang.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nn.chemitech.net.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ks.panjiajie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ey.panjiajie.cn

C#:   s.Replace("a", "b")
来源：http://da.9csxet.cn

[E07] 按分隔符拆分
来源：http://zh.yuexingan06.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://no.colortex.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mm.hnjuh.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://yu.muxihuayi.cn

TS:   s.split(",")
来源：http://sh.bjjhwx.cn

Java: s.split(",");  s.split("\\s+")
来源：http://bj.yuntaijiaju.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hx.jctech888.com.cn

Ruby: s.split(",");  s.split
来源：http://ub.huanxung.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yb.szsharing.cn

[E08] 数组按分隔符合并
来源：http://fz.yuntaijiaju.cn

Py:   ",".join(items)
来源：http://bn.newstarts.cn

PHP:  implode(",", $items);
来源：http://ig.huixinmuqiang.cn

JS:   items.join(",")
来源：http://lb.521024.cn

TS:   items.join(",")
来源：http://xx.shxzskj.cn

Java: String.join(",", items)
来源：http://ac.hnjuh.cn

Go:   strings.Join(items, ",")
来源：http://ck.nicolike.cn

Ruby: items.join(",")
来源：http://wr.shxzskj.cn

C#:   string.Join(",", items)
来源：http://nb.yuexingan06.cn

[E09] 去除所有空白字符
来源：http://uj.bjjhwx.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xb.shxzskj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://kw.yuexingan06.cn

JS:   s.replace(/\s+/g, "")
来源：http://vi.muxihuayi.cn

TS:   s.replace(/\s+/g, "")
来源：http://xx.newstarts.cn

Java: s.replaceAll("\\s+", "")
来源：http://ge.szxytkj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://pd.yuexingan06.cn

Ruby: s.gsub(/\s+/, "")
来源：http://xs.nicolike.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bh.shxzskj.cn

[E10] 左侧补零 / 定长填充
来源：http://as.nszjky.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://rh.jianghongdianzi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ko.yuexingan06.cn

JS:   "7".padStart(3, "0")
来源：http://ka.yuexingan06.cn

TS:   "7".padStart(3, "0")
来源：http://ny.jctech888.com.cn

Java: String.format("%03d", 7)
来源：http://wl.chemitech.net.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://bd.huixinmuqiang.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://dl.nszjky.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://uj.nszjky.cn

[E11] 反转字符串
来源：http://hr.hnjuh.cn

Py:   s[::-1]
来源：http://sl.shxzukj.cn

PHP:  strrev($s);
来源：http://hz.colortex.cn

JS:   [...s].reverse().join("")
来源：http://tg.nicolike.cn

TS:   [...s].reverse().join("")
来源：http://lp.szsharing.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://wt.huanxung.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ru.bjjhwx.cn

Ruby: s.reverse
来源：http://me.panjiajie.cn

C#:   new string(s.Reverse().ToArray())
来源：http://kb.521024.cn

[E12] 统计某字符出现次数
来源：http://id.colortex.cn

Py:   s.count("a")
来源：http://ic.hahajie.cn

PHP:  substr_count($s, "a");
来源：http://cg.hahajie.cn

JS:   s.split("a").length - 1
来源：http://tp.hnjuh.cn

TS:   s.split("a").length - 1
来源：http://xf.bookmarksfly.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://pb.huanxung.cn

Go:   strings.Count(s, "a")
来源：http://af.bookmarksfly.cn

Ruby: s.count("a")
来源：http://ln.bookmarksfly.cn

C#:   s.Count(c => c == 'a')
来源：http://xf.nicolike.cn

[E13] 逐字符遍历
来源：http://my.huanxung.cn

Py:   for ch in s: print(ch)
来源：http://ro.wgjwhj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vs.newstarts.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://jn.lnxyls.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://zo.muxihuayi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://dy.nszjky.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xj.bjjhwx.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://bq.yuexingan06.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://yz.yuntaijiaju.cn

[E14] URL 编码与 Base64
来源：http://kd.hnjuh.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xg.newstarts.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://cv.yuntaijiaju.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qv.panjiajie.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hw.huixiangedu.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ed.asd995.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jz.gzmigu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vx.521024.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gg.yuntaijiaju.cn

[E15] HTML 转义 / 反转义
来源：http://sr.yuntaijiaju.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ax.panjiajie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ni.yuntaijiaju.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xq.haigaiapp.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://en.shtwfgs.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ul.yuntaijiaju.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zk.nicolike.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fv.panjiajie.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lx.shtwfgs.cn

[E16] 数字千分位
来源：http://fd.wgjwhj.cn

Py:   f"{1234567:,}"
来源：http://ao.yuntaijiaju.cn

PHP:  number_format(1234567);
来源：http://lz.shxzskj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://mz.lnxyls.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ah.jianghongdianzi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ur.hnjuh.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mu.shtwfgs.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ng.huixinmuqiang.cn

C#:   1234567.ToString("N0")
来源：http://pi.nicolike.cn

[E17] 首字母大写
来源：http://ue.521024.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://je.huixinmuqiang.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://zh.muxihuayi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wo.hnjuh.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ih.shxzskj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://go.huanxung.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ju.shxzskj.cn

Ruby: s.capitalize
来源：http://is.chemitech.net.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://yr.bookmarksfly.cn

[E18] 模板占位符替换
来源：http://bd.9csxet.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ce.gzmigu.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://oj.jctech888.com.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://od.chemitech.net.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://pb.panjiajie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://un.szsharing.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ii.521024.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://bg.chemitech.net.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://pl.jianghongdianzi.cn

[E19] 多行文本按行拆分
来源：http://rk.wgjwhj.cn

Py:   s.splitlines()
来源：http://gk.szsharing.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xu.shtwfgs.cn

JS:   s.split(/\r?\n/)
来源：http://pv.yuexingan06.cn

TS:   s.split(/\r?\n/)
来源：http://hz.haigaiapp.cn

Java: s.lines().toList()
来源：http://bl.muxihuayi.cn

Go:   strings.Split(s, "\n")
来源：http://ub.hahajie.cn

Ruby: s.lines
来源：http://cc.nicolike.cn

C#:   s.Split('\n')
来源：http://wn.shtwfgs.cn

[E20] 判断字符串是否为空
来源：http://dz.hahajie.cn

Py:   if not s:
来源：http://qn.wgjwhj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vp.521024.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vf.huixinmuqiang.cn

TS:   if (s === "") {}
来源：http://ec.hahajie.cn

Java: if (s.isEmpty()) {}
来源：http://io.bookmarksfly.cn

Go:   if s == "" {}
来源：http://il.hahajie.cn

Ruby: if s.empty?
来源：http://ov.hnjuh.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qb.colortex.cn

[E21] 超长截断加省略号
来源：http://ww.huixiangedu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://uh.jctech888.com.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jv.szxytkj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yk.lnxyls.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nn.jctech888.com.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ih.huixinmuqiang.cn

Go:   // 按 rune 判断长度后截断
来源：http://rc.shxzukj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cj.yuntaijiaju.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ev.huanxung.cn

[E22] 字节长度与字符长度
来源：http://ej.colortex.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://lz.huixiangedu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ra.haigaiapp.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://kf.jianghongdianzi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vx.huixiangedu.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://tn.shtwfgs.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hm.panjiajie.cn

Ruby: s.bytesize;  s.length
来源：http://ou.szsharing.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://iw.jctech888.com.cn

================================================================================
来源：http://jm.yuntaijiaju.cn

F. 文件与目录
来源：http://sq.hahajie.cn

================================================================================
来源：http://pt.lnxyls.cn

[F01] 读取整个文件
来源：http://sx.szsharing.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dg.nicolike.cn

PHP:  file_get_contents("a.txt");
来源：http://pz.szxytkj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://er.szsharing.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://em.hnjuh.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://cu.wgjwhj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://iv.haigaiapp.cn

Ruby: File.read("a.txt")
来源：http://ry.hahajie.cn

C#:   File.ReadAllText("a.txt");
来源：http://os.huanxung.cn

[F02] 逐行读取文件
来源：http://lc.colortex.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ii.shtwfgs.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ka.asd995.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kg.lnxyls.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wz.521024.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://oh.colortex.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kb.bookmarksfly.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fn.shxzukj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fz.521024.cn

[F03] 写入文件（覆盖）
来源：http://bc.hnjuh.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://sf.521024.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://gz.lnxyls.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yg.shxzukj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fs.yuexingan06.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://og.bjjhwx.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zx.nicolike.cn

Ruby: File.write("a.txt", "hi")
来源：http://xu.hnjuh.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ee.szsharing.cn

[F04] 追加写入文件
来源：http://hq.jianghongdianzi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lx.jianghongdianzi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zz.shxzskj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mr.huanxung.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dt.huixinmuqiang.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://es.yuexingan06.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://km.muxihuayi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lp.szxytkj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kl.newstarts.cn


<!-- 参考信息 -->