代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://yz.hahajie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://oe.bjjhwx.cn

Go:   // 手写 map[string][]T
来源：http://il.huixiangedu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://lo.huixiangedu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lc.9csxet.cn

[D20] 统计每个元素出现次数
来源：http://wx.yuntaijiaju.cn

Py:   Counter(arr)
来源：http://wx.yuexingan06.cn

PHP:  array_count_values($arr);
来源：http://xh.hnjuh.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://to.muxihuayi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dg.yuntaijiaju.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ss.lnxyls.cn

Go:   // 手写 map[T]int
来源：http://gb.huixiangedu.cn

Ruby: arr.tally
来源：http://xl.yuexingan06.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dx.huixiangedu.cn

[D21] 判断是否包含某元素
来源：http://sp.hahajie.cn

Py:   x in arr
来源：http://tx.huixinmuqiang.cn

PHP:  in_array($x, $arr, true);
来源：http://oh.521024.cn

JS:   arr.includes(x)
来源：http://wo.asd995.cn

TS:   arr.includes(x)
来源：http://jl.hnjuh.cn

Java: list.contains(x)
来源：http://np.muxihuayi.cn

Go:   slices.Contains(arr, x)
来源：http://fs.chemitech.net.cn

Ruby: arr.include?(x)
来源：http://sx.jctech888.com.cn

C#:   list.Contains(x)
来源：http://lf.jctech888.com.cn

[D22] 复制数组（避免共享引用）
来源：http://qe.shxzskj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://iv.nicolike.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wk.newstarts.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rc.hnjuh.cn

TS:   [...arr];
来源：http://vd.nszjky.cn

Java: new ArrayList<>(list);
来源：http://gs.jianghongdianzi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://vq.panjiajie.cn

Ruby: arr.dup;  arr.clone
来源：http://wo.shtwfgs.cn

C#:   new List<int>(list);
来源：http://wo.hnjuh.cn

[D23] reduce 累积计算
来源：http://dz.yuexingan06.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vu.shxzskj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qj.chemitech.net.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ac.9csxet.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cm.bjjhwx.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://il.nszjky.cn

Go:   // 手写循环
来源：http://xi.yuntaijiaju.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://sz.bookmarksfly.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zk.nicolike.cn

[D24] 字典 / Map 基本操作
来源：http://du.asd995.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wi.shtwfgs.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://de.shtwfgs.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gj.gzmigu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ya.huixiangedu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vb.panjiajie.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qi.huixiangedu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mb.huixinmuqiang.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://al.bjjhwx.cn

[D25] Set 集合去重与交并差
来源：http://op.nszjky.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ep.wgjwhj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zs.jctech888.com.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ag.huixinmuqiang.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://om.szxytkj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://lk.yuntaijiaju.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ov.huixiangedu.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vm.lnxyls.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://yr.nszjky.cn

[D26] 数组转字符串
来源：http://gb.jctech888.com.cn

Py:   ", ".join(map(str, arr))
来源：http://nl.hnjuh.cn

PHP:  implode(", ", $arr);
来源：http://pp.bookmarksfly.cn

JS:   arr.join(", ")
来源：http://nc.jctech888.com.cn

TS:   arr.join(", ")
来源：http://eo.szxytkj.cn

Java: String.join(", ", list)
来源：http://pj.panjiajie.cn

Go:   strings.Join(strs, ", ")
来源：http://dt.haigaiapp.cn

Ruby: arr.join(", ")
来源：http://gl.shxzskj.cn

C#:   string.Join(", ", list)
来源：http://rm.jianghongdianzi.cn

================================================================================
来源：http://bh.huanxung.cn

E. 字符串处理
来源：http://ul.colortex.cn

================================================================================
来源：http://ho.lnxyls.cn

[E01] 拼接字符串
来源：http://yx.nicolike.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lq.gzmigu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mp.nszjky.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://cu.huixinmuqiang.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://it.wgjwhj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vx.nicolike.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fc.jianghongdianzi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lu.521024.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ub.yuntaijiaju.cn

[E02] 重复字符串
来源：http://gj.lnxyls.cn

Py:   "ab" * 3
来源：http://hq.bjjhwx.cn

PHP:  str_repeat("ab", 3);
来源：http://tn.asd995.cn

JS:   "ab".repeat(3)
来源：http://ml.lnxyls.cn

TS:   "ab".repeat(3)
来源：http://kj.shxzukj.cn

Java: "ab".repeat(3)
来源：http://ts.nszjky.cn

Go:   strings.Repeat("ab", 3)
来源：http://xs.colortex.cn

Ruby: "ab" * 3
来源：http://qe.szsharing.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ft.huixinmuqiang.cn

[E03] 截取子串
来源：http://zy.huixinmuqiang.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://da.wgjwhj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qz.hnjuh.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://is.hahajie.cn

TS:   s.slice(1, 4)
来源：http://qk.hahajie.cn

Java: s.substring(1, 4)
来源：http://pk.9csxet.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://uo.shxzukj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://qx.colortex.cn

C#:   s.Substring(1, 3)
来源：http://tv.colortex.cn

[E04] 查找子串位置
来源：http://as.shxzskj.cn

Py:   s.find("x");  s.index("x")
来源：http://jt.huixiangedu.cn

PHP:  strpos($s, "x");
来源：http://oo.chemitech.net.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gz.hnjuh.cn

TS:   s.indexOf("x")
来源：http://oe.bjjhwx.cn

Java: s.indexOf("x")
来源：http://qr.521024.cn

Go:   strings.Index(s, "x")
来源：http://vd.szxytkj.cn

Ruby: s.index("x")
来源：http://aj.muxihuayi.cn

C#:   s.IndexOf("x")
来源：http://lw.nicolike.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ai.huanxung.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://uc.nicolike.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://sf.521024.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sb.hahajie.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://cj.asd995.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xv.yuntaijiaju.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lb.asd995.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fe.panjiajie.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ek.gzmigu.cn

[E06] 替换子串
来源：http://wc.newstarts.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ai.9csxet.cn

PHP:  str_replace("a", "b", $s);
来源：http://iq.jianghongdianzi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qj.haigaiapp.cn

TS:   s.replaceAll("a", "b")
来源：http://ez.muxihuayi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ab.jctech888.com.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://nd.nicolike.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lh.bjjhwx.cn

C#:   s.Replace("a", "b")
来源：http://le.chemitech.net.cn

[E07] 按分隔符拆分
来源：http://ez.huixiangedu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bg.hahajie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dy.shxzukj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://be.gzmigu.cn

TS:   s.split(",")
来源：http://rj.colortex.cn

Java: s.split(",");  s.split("\\s+")
来源：http://hb.jianghongdianzi.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wy.nszjky.cn

Ruby: s.split(",");  s.split
来源：http://xu.haigaiapp.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://nu.huanxung.cn

[E08] 数组按分隔符合并
来源：http://nd.szsharing.cn

Py:   ",".join(items)
来源：http://mm.shtwfgs.cn

PHP:  implode(",", $items);
来源：http://yt.jianghongdianzi.cn

JS:   items.join(",")
来源：http://vp.yuexingan06.cn

TS:   items.join(",")
来源：http://cv.colortex.cn

Java: String.join(",", items)
来源：http://at.colortex.cn

Go:   strings.Join(items, ",")
来源：http://ew.jianghongdianzi.cn

Ruby: items.join(",")
来源：http://eq.yuntaijiaju.cn

C#:   string.Join(",", items)
来源：http://rc.gzmigu.cn

[E09] 去除所有空白字符
来源：http://dr.shxzskj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wp.szsharing.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jn.chemitech.net.cn

JS:   s.replace(/\s+/g, "")
来源：http://qx.chemitech.net.cn

TS:   s.replace(/\s+/g, "")
来源：http://bz.hahajie.cn

Java: s.replaceAll("\\s+", "")
来源：http://ah.bjjhwx.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://gy.huixinmuqiang.cn

Ruby: s.gsub(/\s+/, "")
来源：http://yc.bjjhwx.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://li.hahajie.cn

[E10] 左侧补零 / 定长填充
来源：http://yb.wgjwhj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qw.huanxung.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://lj.hahajie.cn

JS:   "7".padStart(3, "0")
来源：http://lj.shxzskj.cn

TS:   "7".padStart(3, "0")
来源：http://de.huanxung.cn

Java: String.format("%03d", 7)
来源：http://sd.shxzukj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://wd.hahajie.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://yx.panjiajie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kr.jctech888.com.cn

[E11] 反转字符串
来源：http://jb.colortex.cn

Py:   s[::-1]
来源：http://mf.hahajie.cn

PHP:  strrev($s);
来源：http://yf.bookmarksfly.cn

JS:   [...s].reverse().join("")
来源：http://rn.9csxet.cn

TS:   [...s].reverse().join("")
来源：http://cy.colortex.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://xu.shxzukj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://gf.huanxung.cn

Ruby: s.reverse
来源：http://dc.jctech888.com.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ft.hnjuh.cn

[E12] 统计某字符出现次数
来源：http://hq.shtwfgs.cn

Py:   s.count("a")
来源：http://xw.muxihuayi.cn

PHP:  substr_count($s, "a");
来源：http://lx.panjiajie.cn

JS:   s.split("a").length - 1
来源：http://rs.gzmigu.cn

TS:   s.split("a").length - 1
来源：http://fg.gzmigu.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://bv.bookmarksfly.cn

Go:   strings.Count(s, "a")
来源：http://fp.huanxung.cn

Ruby: s.count("a")
来源：http://fl.jianghongdianzi.cn

C#:   s.Count(c => c == 'a')
来源：http://ef.shtwfgs.cn

[E13] 逐字符遍历
来源：http://dp.newstarts.cn

Py:   for ch in s: print(ch)
来源：http://qu.huixinmuqiang.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://eb.chemitech.net.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://tx.muxihuayi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://vk.huixinmuqiang.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rd.jctech888.com.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://lq.shxzskj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ql.shxzskj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://sa.szsharing.cn

[E14] URL 编码与 Base64
来源：http://ke.shxzukj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xx.shxzskj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://dn.bookmarksfly.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ur.newstarts.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://cg.shtwfgs.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wp.colortex.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mk.bookmarksfly.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gw.hnjuh.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://iu.muxihuayi.cn

[E15] HTML 转义 / 反转义
来源：http://wm.bjjhwx.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://vr.huixiangedu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hv.szxytkj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zu.wgjwhj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://tk.hahajie.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qo.nicolike.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ov.lnxyls.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zm.asd995.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ym.lnxyls.cn

[E16] 数字千分位
来源：http://wf.yuntaijiaju.cn

Py:   f"{1234567:,}"
来源：http://ew.szsharing.cn

PHP:  number_format(1234567);
来源：http://vl.nszjky.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ae.chemitech.net.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://kr.muxihuayi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ho.gzmigu.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fj.bookmarksfly.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://yq.lnxyls.cn

C#:   1234567.ToString("N0")
来源：http://fn.yuexingan06.cn

[E17] 首字母大写
来源：http://sj.szsharing.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gd.jctech888.com.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ju.asd995.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gw.newstarts.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jo.colortex.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zy.bookmarksfly.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vr.lnxyls.cn

Ruby: s.capitalize
来源：http://pv.jctech888.com.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gt.shtwfgs.cn

[E18] 模板占位符替换
来源：http://oc.panjiajie.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://sq.nicolike.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://sv.jctech888.com.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://og.521024.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://lt.huixinmuqiang.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pb.521024.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://yh.asd995.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://au.szsharing.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hk.colortex.cn

[E19] 多行文本按行拆分
来源：http://rs.newstarts.cn

Py:   s.splitlines()
来源：http://rt.chemitech.net.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://tp.huixiangedu.cn

JS:   s.split(/\r?\n/)
来源：http://hi.newstarts.cn

TS:   s.split(/\r?\n/)
来源：http://ag.shxzukj.cn

Java: s.lines().toList()
来源：http://br.muxihuayi.cn

Go:   strings.Split(s, "\n")
来源：http://tk.yuexingan06.cn

Ruby: s.lines
来源：http://oq.bookmarksfly.cn

C#:   s.Split('\n')
来源：http://kh.asd995.cn

[E20] 判断字符串是否为空
来源：http://rm.huixinmuqiang.cn

Py:   if not s:
来源：http://ff.chemitech.net.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://pu.jctech888.com.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yg.chemitech.net.cn

TS:   if (s === "") {}
来源：http://cb.yuntaijiaju.cn

Java: if (s.isEmpty()) {}
来源：http://ll.chemitech.net.cn

Go:   if s == "" {}
来源：http://wr.panjiajie.cn

Ruby: if s.empty?
来源：http://my.yuntaijiaju.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://eu.gzmigu.cn

[E21] 超长截断加省略号
来源：http://tz.bookmarksfly.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://gy.bjjhwx.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://na.9csxet.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uh.9csxet.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mf.haigaiapp.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ik.shtwfgs.cn

Go:   // 按 rune 判断长度后截断
来源：http://fi.nszjky.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bz.hahajie.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://aa.gzmigu.cn

[E22] 字节长度与字符长度
来源：http://rs.shtwfgs.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hp.bookmarksfly.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ay.bookmarksfly.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ri.shxzukj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://si.hnjuh.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wj.jctech888.com.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jg.muxihuayi.cn

Ruby: s.bytesize;  s.length
来源：http://ls.jctech888.com.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xk.muxihuayi.cn

================================================================================
来源：http://wr.colortex.cn

F. 文件与目录
来源：http://su.shtwfgs.cn

================================================================================
来源：http://iy.9csxet.cn

[F01] 读取整个文件
来源：http://vh.521024.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ci.huixinmuqiang.cn

PHP:  file_get_contents("a.txt");
来源：http://zx.shxzukj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://nf.bookmarksfly.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qa.shxzukj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://lh.szxytkj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nk.9csxet.cn

Ruby: File.read("a.txt")
来源：http://zl.hahajie.cn

C#:   File.ReadAllText("a.txt");
来源：http://js.gzmigu.cn

[F02] 逐行读取文件
来源：http://yt.lnxyls.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://zk.wgjwhj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://tz.shtwfgs.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fr.huixiangedu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rt.asd995.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://at.szxytkj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://og.szxytkj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ld.hahajie.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ul.newstarts.cn

[F03] 写入文件（覆盖）
来源：http://vv.panjiajie.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ld.9csxet.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://wx.huixiangedu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gz.colortex.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tw.hnjuh.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://cp.jctech888.com.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zu.gzmigu.cn

Ruby: File.write("a.txt", "hi")
来源：http://jh.bookmarksfly.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zg.newstarts.cn

[F04] 追加写入文件
来源：http://yd.haigaiapp.cn


<!-- 参考信息 -->