代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cr.huanxung.cn

[D20] 统计每个元素出现次数
来源：http://wx.muxihuayi.cn

Py:   Counter(arr)
来源：http://ei.muxihuayi.cn

PHP:  array_count_values($arr);
来源：http://bz.jianghongdianzi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qw.colortex.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ca.huanxung.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://lg.szsharing.cn

Go:   // 手写 map[T]int
来源：http://be.521024.cn

Ruby: arr.tally
来源：http://qi.9csxet.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://gx.shxzskj.cn

[D21] 判断是否包含某元素
来源：http://rw.haigaiapp.cn

Py:   x in arr
来源：http://xs.asd995.cn

PHP:  in_array($x, $arr, true);
来源：http://zb.szsharing.cn

JS:   arr.includes(x)
来源：http://pc.panjiajie.cn

TS:   arr.includes(x)
来源：http://xw.szsharing.cn

Java: list.contains(x)
来源：http://xc.gzmigu.cn

Go:   slices.Contains(arr, x)
来源：http://xz.bookmarksfly.cn

Ruby: arr.include?(x)
来源：http://nh.shxzukj.cn

C#:   list.Contains(x)
来源：http://qn.jianghongdianzi.cn

[D22] 复制数组（避免共享引用）
来源：http://ey.nicolike.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ig.jctech888.com.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://en.muxihuayi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ys.szxytkj.cn

TS:   [...arr];
来源：http://ed.bookmarksfly.cn

Java: new ArrayList<>(list);
来源：http://vj.bjjhwx.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ak.colortex.cn

Ruby: arr.dup;  arr.clone
来源：http://uf.huanxung.cn

C#:   new List<int>(list);
来源：http://md.jianghongdianzi.cn

[D23] reduce 累积计算
来源：http://ul.szxytkj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hn.521024.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://po.jctech888.com.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ao.colortex.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lv.bookmarksfly.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://yk.9csxet.cn

Go:   // 手写循环
来源：http://za.521024.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://de.yuexingan06.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tf.lnxyls.cn

[D24] 字典 / Map 基本操作
来源：http://mz.chemitech.net.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pe.szxytkj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ee.shxzukj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://he.panjiajie.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hu.shxzskj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ui.jctech888.com.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jt.nszjky.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fb.asd995.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wc.yuexingan06.cn

[D25] Set 集合去重与交并差
来源：http://ch.wgjwhj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://om.asd995.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vn.nicolike.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://pk.shtwfgs.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fg.szsharing.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://io.gzmigu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ss.colortex.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ud.bjjhwx.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fa.haigaiapp.cn

[D26] 数组转字符串
来源：http://jz.szsharing.cn

Py:   ", ".join(map(str, arr))
来源：http://cl.hnjuh.cn

PHP:  implode(", ", $arr);
来源：http://ev.panjiajie.cn

JS:   arr.join(", ")
来源：http://dn.nicolike.cn

TS:   arr.join(", ")
来源：http://nu.yuntaijiaju.cn

Java: String.join(", ", list)
来源：http://do.huanxung.cn

Go:   strings.Join(strs, ", ")
来源：http://po.szsharing.cn

Ruby: arr.join(", ")
来源：http://et.nicolike.cn

C#:   string.Join(", ", list)
来源：http://zv.szsharing.cn

================================================================================
来源：http://vz.yuexingan06.cn

E. 字符串处理
来源：http://rx.nszjky.cn

================================================================================
来源：http://uz.jctech888.com.cn

[E01] 拼接字符串
来源：http://pt.yuexingan06.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hy.huanxung.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ss.bookmarksfly.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xg.colortex.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vu.jianghongdianzi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://jv.nszjky.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rl.nszjky.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gf.521024.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nt.hnjuh.cn

[E02] 重复字符串
来源：http://fk.hnjuh.cn

Py:   "ab" * 3
来源：http://by.huixinmuqiang.cn

PHP:  str_repeat("ab", 3);
来源：http://wq.asd995.cn

JS:   "ab".repeat(3)
来源：http://ho.panjiajie.cn

TS:   "ab".repeat(3)
来源：http://nt.gzmigu.cn

Java: "ab".repeat(3)
来源：http://in.haigaiapp.cn

Go:   strings.Repeat("ab", 3)
来源：http://vv.shtwfgs.cn

Ruby: "ab" * 3
来源：http://ro.newstarts.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ro.hnjuh.cn

[E03] 截取子串
来源：http://jc.bjjhwx.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ho.bjjhwx.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ml.asd995.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://us.newstarts.cn

TS:   s.slice(1, 4)
来源：http://oa.nszjky.cn

Java: s.substring(1, 4)
来源：http://yr.gzmigu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ze.shxzskj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://hc.shtwfgs.cn

C#:   s.Substring(1, 3)
来源：http://tg.huanxung.cn

[E04] 查找子串位置
来源：http://fm.yuntaijiaju.cn

Py:   s.find("x");  s.index("x")
来源：http://ot.shxzskj.cn

PHP:  strpos($s, "x");
来源：http://lp.lnxyls.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://cx.newstarts.cn

TS:   s.indexOf("x")
来源：http://ey.9csxet.cn

Java: s.indexOf("x")
来源：http://ih.yuexingan06.cn

Go:   strings.Index(s, "x")
来源：http://vb.521024.cn

Ruby: s.index("x")
来源：http://ku.wgjwhj.cn

C#:   s.IndexOf("x")
来源：http://lk.yuexingan06.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://mk.colortex.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://et.jctech888.com.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bc.szxytkj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zn.521024.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ug.szxytkj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://at.hahajie.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kp.shxzskj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qh.jianghongdianzi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kl.lnxyls.cn

[E06] 替换子串
来源：http://qe.521024.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ex.9csxet.cn

PHP:  str_replace("a", "b", $s);
来源：http://ma.yuexingan06.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ey.huixinmuqiang.cn

TS:   s.replaceAll("a", "b")
来源：http://lt.shxzskj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pk.newstarts.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://dx.wgjwhj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nv.asd995.cn

C#:   s.Replace("a", "b")
来源：http://wy.gzmigu.cn

[E07] 按分隔符拆分
来源：http://kv.newstarts.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://kp.haigaiapp.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qg.bookmarksfly.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://kq.shtwfgs.cn

TS:   s.split(",")
来源：http://ye.lnxyls.cn

Java: s.split(",");  s.split("\\s+")
来源：http://kn.newstarts.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xr.huanxung.cn

Ruby: s.split(",");  s.split
来源：http://xn.jctech888.com.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rc.lnxyls.cn

[E08] 数组按分隔符合并
来源：http://du.lnxyls.cn

Py:   ",".join(items)
来源：http://zi.huanxung.cn

PHP:  implode(",", $items);
来源：http://ru.shxzukj.cn

JS:   items.join(",")
来源：http://nc.szsharing.cn

TS:   items.join(",")
来源：http://ur.shtwfgs.cn

Java: String.join(",", items)
来源：http://wh.bookmarksfly.cn

Go:   strings.Join(items, ",")
来源：http://xl.yuexingan06.cn

Ruby: items.join(",")
来源：http://rf.haigaiapp.cn

C#:   string.Join(",", items)
来源：http://td.huanxung.cn

[E09] 去除所有空白字符
来源：http://pt.9csxet.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ob.521024.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ug.muxihuayi.cn

JS:   s.replace(/\s+/g, "")
来源：http://dm.bookmarksfly.cn

TS:   s.replace(/\s+/g, "")
来源：http://an.panjiajie.cn

Java: s.replaceAll("\\s+", "")
来源：http://zn.panjiajie.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://bg.chemitech.net.cn

Ruby: s.gsub(/\s+/, "")
来源：http://pu.panjiajie.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ri.9csxet.cn

[E10] 左侧补零 / 定长填充
来源：http://tq.gzmigu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tm.panjiajie.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jo.nicolike.cn

JS:   "7".padStart(3, "0")
来源：http://ka.colortex.cn

TS:   "7".padStart(3, "0")
来源：http://ay.nszjky.cn

Java: String.format("%03d", 7)
来源：http://dt.hnjuh.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://jl.wgjwhj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qd.muxihuayi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wg.nszjky.cn

[E11] 反转字符串
来源：http://kb.asd995.cn

Py:   s[::-1]
来源：http://ml.shxzskj.cn

PHP:  strrev($s);
来源：http://nj.nszjky.cn

JS:   [...s].reverse().join("")
来源：http://dr.521024.cn

TS:   [...s].reverse().join("")
来源：http://iy.shxzskj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ij.jctech888.com.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ax.shtwfgs.cn

Ruby: s.reverse
来源：http://wq.huanxung.cn

C#:   new string(s.Reverse().ToArray())
来源：http://dg.asd995.cn

[E12] 统计某字符出现次数
来源：http://lp.shxzskj.cn

Py:   s.count("a")
来源：http://as.9csxet.cn

PHP:  substr_count($s, "a");
来源：http://xm.hahajie.cn

JS:   s.split("a").length - 1
来源：http://wh.9csxet.cn

TS:   s.split("a").length - 1
来源：http://lw.haigaiapp.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wn.szxytkj.cn

Go:   strings.Count(s, "a")
来源：http://bc.wgjwhj.cn

Ruby: s.count("a")
来源：http://kj.huixiangedu.cn

C#:   s.Count(c => c == 'a')
来源：http://cl.huixiangedu.cn

[E13] 逐字符遍历
来源：http://wh.haigaiapp.cn

Py:   for ch in s: print(ch)
来源：http://ud.muxihuayi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gi.asd995.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://fx.huanxung.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://pa.nicolike.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xh.bookmarksfly.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xi.huixiangedu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://na.huanxung.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cj.wgjwhj.cn

[E14] URL 编码与 Base64
来源：http://xt.bookmarksfly.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kp.panjiajie.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://cn.hahajie.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://lo.lnxyls.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://kp.hahajie.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://da.shxzskj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xg.jctech888.com.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gd.lnxyls.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bg.haigaiapp.cn

[E15] HTML 转义 / 反转义
来源：http://mi.newstarts.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://zl.jctech888.com.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://yo.haigaiapp.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qb.jianghongdianzi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://tf.shxzukj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://im.bjjhwx.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fp.chemitech.net.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://yc.huixinmuqiang.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://xl.huanxung.cn

[E16] 数字千分位
来源：http://ep.yuntaijiaju.cn

Py:   f"{1234567:,}"
来源：http://dv.haigaiapp.cn

PHP:  number_format(1234567);
来源：http://nc.szxytkj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://yx.muxihuayi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://dg.hahajie.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ex.shtwfgs.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ca.asd995.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qy.yuntaijiaju.cn

C#:   1234567.ToString("N0")
来源：http://xq.panjiajie.cn

[E17] 首字母大写
来源：http://kw.521024.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fv.shtwfgs.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://nr.bookmarksfly.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fq.haigaiapp.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gw.shxzukj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qx.muxihuayi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hu.newstarts.cn

Ruby: s.capitalize
来源：http://lj.jctech888.com.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ij.shxzukj.cn

[E18] 模板占位符替换
来源：http://bh.asd995.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ut.yuntaijiaju.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mo.gzmigu.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://sp.muxihuayi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://vc.jctech888.com.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ao.huixinmuqiang.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ip.jctech888.com.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://pj.9csxet.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rm.huixiangedu.cn

[E19] 多行文本按行拆分
来源：http://dd.shxzskj.cn

Py:   s.splitlines()
来源：http://jv.shxzukj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://fh.nicolike.cn

JS:   s.split(/\r?\n/)
来源：http://wb.wgjwhj.cn

TS:   s.split(/\r?\n/)
来源：http://fp.jctech888.com.cn

Java: s.lines().toList()
来源：http://cp.szxytkj.cn

Go:   strings.Split(s, "\n")
来源：http://kl.yuexingan06.cn

Ruby: s.lines
来源：http://ev.jianghongdianzi.cn

C#:   s.Split('\n')
来源：http://ye.hahajie.cn

[E20] 判断字符串是否为空
来源：http://bh.521024.cn

Py:   if not s:
来源：http://ha.wgjwhj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://fm.lnxyls.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://iq.huixinmuqiang.cn

TS:   if (s === "") {}
来源：http://ey.haigaiapp.cn

Java: if (s.isEmpty()) {}
来源：http://uw.huanxung.cn

Go:   if s == "" {}
来源：http://tj.chemitech.net.cn

Ruby: if s.empty?
来源：http://qy.hahajie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wx.shtwfgs.cn

[E21] 超长截断加省略号
来源：http://fw.huixiangedu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://dt.wgjwhj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://cr.chemitech.net.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://br.nszjky.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lw.colortex.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ym.chemitech.net.cn

Go:   // 按 rune 判断长度后截断
来源：http://tp.colortex.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vb.wgjwhj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://br.nicolike.cn

[E22] 字节长度与字符长度
来源：http://nj.yuexingan06.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://lj.nicolike.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xr.yuntaijiaju.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vb.wgjwhj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qf.shxzukj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xl.shxzskj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xc.wgjwhj.cn

Ruby: s.bytesize;  s.length
来源：http://tc.colortex.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jz.jctech888.com.cn

================================================================================
来源：http://cn.asd995.cn

F. 文件与目录
来源：http://pa.nicolike.cn

================================================================================
来源：http://fw.shxzskj.cn

[F01] 读取整个文件
来源：http://nm.jianghongdianzi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hq.shxzukj.cn

PHP:  file_get_contents("a.txt");
来源：http://qg.bookmarksfly.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vw.panjiajie.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://kd.9csxet.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://is.szxytkj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zg.lnxyls.cn

Ruby: File.read("a.txt")
来源：http://vj.haigaiapp.cn

C#:   File.ReadAllText("a.txt");
来源：http://hc.gzmigu.cn

[F02] 逐行读取文件
来源：http://fj.shxzukj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://cu.jianghongdianzi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ak.bookmarksfly.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://iw.shxzskj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://eh.yuexingan06.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pr.bjjhwx.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wr.521024.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jg.szsharing.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xe.yuexingan06.cn

[F03] 写入文件（覆盖）
来源：http://xt.haigaiapp.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cu.bjjhwx.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ix.szsharing.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://te.jianghongdianzi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nr.huanxung.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wg.shtwfgs.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ky.nszjky.cn

Ruby: File.write("a.txt", "hi")
来源：http://jc.huixinmuqiang.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zo.wgjwhj.cn

[F04] 追加写入文件
来源：http://pe.bjjhwx.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ns.huanxung.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ql.panjiajie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rv.szxytkj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ta.haigaiapp.cn


<!-- 参考信息 -->