代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ei.wgjwhj.cn

[D20] 统计每个元素出现次数
来源：http://yf.asd995.cn

Py:   Counter(arr)
来源：http://xv.haigaiapp.cn

PHP:  array_count_values($arr);
来源：http://ju.hahajie.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sh.nicolike.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dh.yuexingan06.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vr.wgjwhj.cn

Go:   // 手写 map[T]int
来源：http://nx.lnxyls.cn

Ruby: arr.tally
来源：http://on.colortex.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ab.wgjwhj.cn

[D21] 判断是否包含某元素
来源：http://yp.bookmarksfly.cn

Py:   x in arr
来源：http://bg.jianghongdianzi.cn

PHP:  in_array($x, $arr, true);
来源：http://js.jianghongdianzi.cn

JS:   arr.includes(x)
来源：http://zl.gzmigu.cn

TS:   arr.includes(x)
来源：http://tb.chemitech.net.cn

Java: list.contains(x)
来源：http://on.chemitech.net.cn

Go:   slices.Contains(arr, x)
来源：http://eg.shtwfgs.cn

Ruby: arr.include?(x)
来源：http://ys.newstarts.cn

C#:   list.Contains(x)
来源：http://rb.shxzskj.cn

[D22] 复制数组（避免共享引用）
来源：http://gm.gzmigu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://yv.chemitech.net.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qd.muxihuayi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lv.shtwfgs.cn

TS:   [...arr];
来源：http://qd.yuntaijiaju.cn

Java: new ArrayList<>(list);
来源：http://at.yuexingan06.cn

Go:   copied := append([]int(nil), arr...)
来源：http://tr.colortex.cn

Ruby: arr.dup;  arr.clone
来源：http://wy.9csxet.cn

C#:   new List<int>(list);
来源：http://xw.bookmarksfly.cn

[D23] reduce 累积计算
来源：http://ln.jctech888.com.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://oi.huanxung.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pf.yuntaijiaju.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kn.yuexingan06.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yw.jctech888.com.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://kv.yuexingan06.cn

Go:   // 手写循环
来源：http://ad.asd995.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lv.newstarts.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ba.huixinmuqiang.cn

[D24] 字典 / Map 基本操作
来源：http://ej.chemitech.net.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://dl.shxzskj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ei.9csxet.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jj.521024.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bi.huixiangedu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qh.yuexingan06.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://uw.haigaiapp.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gw.shxzskj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fm.9csxet.cn

[D25] Set 集合去重与交并差
来源：http://tt.asd995.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hr.bjjhwx.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vu.nicolike.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://nj.lnxyls.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kp.yuexingan06.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hl.yuexingan06.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ig.huixiangedu.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bn.huixiangedu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://pc.haigaiapp.cn

[D26] 数组转字符串
来源：http://vy.shxzskj.cn

Py:   ", ".join(map(str, arr))
来源：http://kp.szsharing.cn

PHP:  implode(", ", $arr);
来源：http://fv.yuntaijiaju.cn

JS:   arr.join(", ")
来源：http://ne.asd995.cn

TS:   arr.join(", ")
来源：http://mg.jianghongdianzi.cn

Java: String.join(", ", list)
来源：http://xz.chemitech.net.cn

Go:   strings.Join(strs, ", ")
来源：http://aa.yuntaijiaju.cn

Ruby: arr.join(", ")
来源：http://fx.szsharing.cn

C#:   string.Join(", ", list)
来源：http://cf.haigaiapp.cn

================================================================================
来源：http://pn.szsharing.cn

E. 字符串处理
来源：http://dg.shxzukj.cn

================================================================================
来源：http://gz.yuexingan06.cn

[E01] 拼接字符串
来源：http://gf.huanxung.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://or.gzmigu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://no.colortex.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zb.shtwfgs.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://md.nicolike.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qn.nszjky.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ax.9csxet.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://yy.bookmarksfly.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rp.521024.cn

[E02] 重复字符串
来源：http://rb.nicolike.cn

Py:   "ab" * 3
来源：http://nl.lnxyls.cn

PHP:  str_repeat("ab", 3);
来源：http://ok.huixiangedu.cn

JS:   "ab".repeat(3)
来源：http://tt.bjjhwx.cn

TS:   "ab".repeat(3)
来源：http://rw.jctech888.com.cn

Java: "ab".repeat(3)
来源：http://cr.yuntaijiaju.cn

Go:   strings.Repeat("ab", 3)
来源：http://ze.szxytkj.cn

Ruby: "ab" * 3
来源：http://sc.yuexingan06.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://yw.shtwfgs.cn

[E03] 截取子串
来源：http://or.shxzukj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://id.gzmigu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://un.szxytkj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://pk.newstarts.cn

TS:   s.slice(1, 4)
来源：http://cw.nicolike.cn

Java: s.substring(1, 4)
来源：http://bq.huanxung.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://eg.huanxung.cn

Ruby: s[1, 3];  s[1..3]
来源：http://mi.haigaiapp.cn

C#:   s.Substring(1, 3)
来源：http://be.hahajie.cn

[E04] 查找子串位置
来源：http://lb.shxzukj.cn

Py:   s.find("x");  s.index("x")
来源：http://gk.huixinmuqiang.cn

PHP:  strpos($s, "x");
来源：http://ub.haigaiapp.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kc.huixiangedu.cn

TS:   s.indexOf("x")
来源：http://wx.bookmarksfly.cn

Java: s.indexOf("x")
来源：http://kx.colortex.cn

Go:   strings.Index(s, "x")
来源：http://we.huixinmuqiang.cn

Ruby: s.index("x")
来源：http://tz.chemitech.net.cn

C#:   s.IndexOf("x")
来源：http://kx.nicolike.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://er.nicolike.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xl.shtwfgs.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fj.huixinmuqiang.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qq.gzmigu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://sw.shtwfgs.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gp.colortex.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kd.panjiajie.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jp.9csxet.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://md.hnjuh.cn

[E06] 替换子串
来源：http://sk.colortex.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rz.chemitech.net.cn

PHP:  str_replace("a", "b", $s);
来源：http://ti.gzmigu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://de.521024.cn

TS:   s.replaceAll("a", "b")
来源：http://so.wgjwhj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ke.nszjky.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://sp.521024.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://iv.muxihuayi.cn

C#:   s.Replace("a", "b")
来源：http://lp.hahajie.cn

[E07] 按分隔符拆分
来源：http://nc.lnxyls.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jw.lnxyls.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wl.hnjuh.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://la.huanxung.cn

TS:   s.split(",")
来源：http://gn.colortex.cn

Java: s.split(",");  s.split("\\s+")
来源：http://sc.shxzukj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rh.bjjhwx.cn

Ruby: s.split(",");  s.split
来源：http://bv.szsharing.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rl.yuntaijiaju.cn

[E08] 数组按分隔符合并
来源：http://xw.haigaiapp.cn

Py:   ",".join(items)
来源：http://ue.szsharing.cn

PHP:  implode(",", $items);
来源：http://nx.521024.cn

JS:   items.join(",")
来源：http://dv.hahajie.cn

TS:   items.join(",")
来源：http://gu.nszjky.cn

Java: String.join(",", items)
来源：http://yw.jctech888.com.cn

Go:   strings.Join(items, ",")
来源：http://xv.shtwfgs.cn

Ruby: items.join(",")
来源：http://sq.huixiangedu.cn

C#:   string.Join(",", items)
来源：http://ke.nszjky.cn

[E09] 去除所有空白字符
来源：http://sr.jctech888.com.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://oa.haigaiapp.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mc.nszjky.cn

JS:   s.replace(/\s+/g, "")
来源：http://jo.haigaiapp.cn

TS:   s.replace(/\s+/g, "")
来源：http://zo.colortex.cn

Java: s.replaceAll("\\s+", "")
来源：http://kh.colortex.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://bc.shxzukj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://nw.yuexingan06.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://sc.asd995.cn

[E10] 左侧补零 / 定长填充
来源：http://ew.bookmarksfly.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tq.newstarts.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xo.shxzukj.cn

JS:   "7".padStart(3, "0")
来源：http://rz.shxzukj.cn

TS:   "7".padStart(3, "0")
来源：http://yc.asd995.cn

Java: String.format("%03d", 7)
来源：http://kj.9csxet.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://kz.shxzskj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://iq.panjiajie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://sz.colortex.cn

[E11] 反转字符串
来源：http://bt.szxytkj.cn

Py:   s[::-1]
来源：http://er.bookmarksfly.cn

PHP:  strrev($s);
来源：http://pn.nszjky.cn

JS:   [...s].reverse().join("")
来源：http://be.521024.cn

TS:   [...s].reverse().join("")
来源：http://by.nicolike.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ef.huixiangedu.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://tn.muxihuayi.cn

Ruby: s.reverse
来源：http://ot.chemitech.net.cn

C#:   new string(s.Reverse().ToArray())
来源：http://mk.shtwfgs.cn

[E12] 统计某字符出现次数
来源：http://ds.hahajie.cn

Py:   s.count("a")
来源：http://vo.newstarts.cn

PHP:  substr_count($s, "a");
来源：http://ay.521024.cn

JS:   s.split("a").length - 1
来源：http://dr.yuntaijiaju.cn

TS:   s.split("a").length - 1
来源：http://qv.hahajie.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://az.521024.cn

Go:   strings.Count(s, "a")
来源：http://vq.yuexingan06.cn

Ruby: s.count("a")
来源：http://he.bjjhwx.cn

C#:   s.Count(c => c == 'a')
来源：http://nb.haigaiapp.cn

[E13] 逐字符遍历
来源：http://ep.huanxung.cn

Py:   for ch in s: print(ch)
来源：http://dr.asd995.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://nb.jianghongdianzi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ow.szsharing.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://fp.muxihuayi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://sa.lnxyls.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://lu.haigaiapp.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://mh.colortex.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ex.jctech888.com.cn

[E14] URL 编码与 Base64
来源：http://fn.shxzukj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vs.newstarts.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://te.chemitech.net.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vs.shtwfgs.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nh.haigaiapp.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qe.wgjwhj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hq.wgjwhj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fg.yuntaijiaju.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vs.hnjuh.cn

[E15] HTML 转义 / 反转义
来源：http://pt.szxytkj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ah.521024.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wj.huixinmuqiang.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xg.szxytkj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://dt.shxzukj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mx.bjjhwx.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jx.yuntaijiaju.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bo.wgjwhj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://sf.gzmigu.cn

[E16] 数字千分位
来源：http://dh.nicolike.cn

Py:   f"{1234567:,}"
来源：http://ja.chemitech.net.cn

PHP:  number_format(1234567);
来源：http://ox.szxytkj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://te.jctech888.com.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://aj.nszjky.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qr.nicolike.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://de.9csxet.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dj.521024.cn

C#:   1234567.ToString("N0")
来源：http://pl.9csxet.cn

[E17] 首字母大写
来源：http://sx.hahajie.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ri.521024.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://sn.shxzskj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pq.szxytkj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tr.yuntaijiaju.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dg.yuntaijiaju.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vu.gzmigu.cn

Ruby: s.capitalize
来源：http://vl.yuexingan06.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://bk.huanxung.cn

[E18] 模板占位符替换
来源：http://oq.hnjuh.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ym.hahajie.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://cu.jianghongdianzi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://rz.newstarts.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://rz.huanxung.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://bw.huanxung.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://sv.colortex.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ex.shxzskj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://fb.asd995.cn

[E19] 多行文本按行拆分
来源：http://eu.newstarts.cn

Py:   s.splitlines()
来源：http://ae.huixinmuqiang.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zh.bjjhwx.cn

JS:   s.split(/\r?\n/)
来源：http://hk.bookmarksfly.cn

TS:   s.split(/\r?\n/)
来源：http://im.nicolike.cn

Java: s.lines().toList()
来源：http://mx.huixinmuqiang.cn

Go:   strings.Split(s, "\n")
来源：http://nu.huixinmuqiang.cn

Ruby: s.lines
来源：http://ne.jctech888.com.cn

C#:   s.Split('\n')
来源：http://au.jctech888.com.cn

[E20] 判断字符串是否为空
来源：http://em.szsharing.cn

Py:   if not s:
来源：http://eg.panjiajie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zy.asd995.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ng.nszjky.cn

TS:   if (s === "") {}
来源：http://re.muxihuayi.cn

Java: if (s.isEmpty()) {}
来源：http://mq.shtwfgs.cn

Go:   if s == "" {}
来源：http://az.huanxung.cn

Ruby: if s.empty?
来源：http://io.gzmigu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://im.lnxyls.cn

[E21] 超长截断加省略号
来源：http://mr.521024.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://jq.shtwfgs.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://dn.bjjhwx.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wn.nszjky.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://aj.wgjwhj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rg.shxzukj.cn

Go:   // 按 rune 判断长度后截断
来源：http://nu.yuexingan06.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://sw.asd995.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://cx.yuntaijiaju.cn

[E22] 字节长度与字符长度
来源：http://im.chemitech.net.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://de.haigaiapp.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xz.chemitech.net.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ud.shxzukj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://he.muxihuayi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rc.hahajie.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wb.bookmarksfly.cn

Ruby: s.bytesize;  s.length
来源：http://fd.gzmigu.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://el.9csxet.cn

================================================================================
来源：http://sn.521024.cn

F. 文件与目录
来源：http://dh.bookmarksfly.cn

================================================================================
来源：http://vg.haigaiapp.cn

[F01] 读取整个文件
来源：http://la.asd995.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://oq.chemitech.net.cn

PHP:  file_get_contents("a.txt");
来源：http://na.521024.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vi.haigaiapp.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://dd.chemitech.net.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://gr.nszjky.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://cn.haigaiapp.cn

Ruby: File.read("a.txt")
来源：http://xd.nszjky.cn

C#:   File.ReadAllText("a.txt");
来源：http://ce.colortex.cn

[F02] 逐行读取文件
来源：http://ae.shxzskj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://zy.muxihuayi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ib.9csxet.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tl.panjiajie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hi.shtwfgs.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jj.9csxet.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vy.shxzskj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://uq.shtwfgs.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ma.huixinmuqiang.cn

[F03] 写入文件（覆盖）
来源：http://je.hahajie.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bh.bookmarksfly.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://vk.hahajie.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yc.muxihuayi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kw.szsharing.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gp.shxzukj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://js.521024.cn

Ruby: File.write("a.txt", "hi")
来源：http://zi.shtwfgs.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://gm.hnjuh.cn

[F04] 追加写入文件
来源：http://tx.newstarts.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rr.9csxet.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jm.nicolike.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xi.szsharing.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ex.lnxyls.cn


<!-- 参考信息 -->