代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yf.hnjuh.cn

Go:   // 手写双层循环
来源：http://zk.hahajie.cn

Ruby: nested.flatten
来源：http://bj.jianghongdianzi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ok.jctech888.com.cn

[D19] 按字段分组
来源：http://fk.bjjhwx.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wo.jianghongdianzi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ov.jianghongdianzi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ta.9csxet.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://xj.hahajie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ld.yuexingan06.cn

Go:   // 手写 map[string][]T
来源：http://kz.jctech888.com.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ti.hnjuh.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ep.jianghongdianzi.cn

[D20] 统计每个元素出现次数
来源：http://mz.shxzskj.cn

Py:   Counter(arr)
来源：http://gx.muxihuayi.cn

PHP:  array_count_values($arr);
来源：http://dy.hnjuh.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kv.hnjuh.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fm.nszjky.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wk.nicolike.cn

Go:   // 手写 map[T]int
来源：http://ge.jianghongdianzi.cn

Ruby: arr.tally
来源：http://gj.yuexingan06.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tw.haigaiapp.cn

[D21] 判断是否包含某元素
来源：http://ep.panjiajie.cn

Py:   x in arr
来源：http://yy.521024.cn

PHP:  in_array($x, $arr, true);
来源：http://rc.shxzukj.cn

JS:   arr.includes(x)
来源：http://xn.9csxet.cn

TS:   arr.includes(x)
来源：http://zd.haigaiapp.cn

Java: list.contains(x)
来源：http://cl.shxzukj.cn

Go:   slices.Contains(arr, x)
来源：http://qz.gzmigu.cn

Ruby: arr.include?(x)
来源：http://yl.huanxung.cn

C#:   list.Contains(x)
来源：http://nc.huixiangedu.cn

[D22] 复制数组（避免共享引用）
来源：http://kk.yuntaijiaju.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wm.newstarts.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://st.lnxyls.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hu.shtwfgs.cn

TS:   [...arr];
来源：http://jy.huixinmuqiang.cn

Java: new ArrayList<>(list);
来源：http://sl.hahajie.cn

Go:   copied := append([]int(nil), arr...)
来源：http://mb.yuexingan06.cn

Ruby: arr.dup;  arr.clone
来源：http://lx.chemitech.net.cn

C#:   new List<int>(list);
来源：http://hm.9csxet.cn

[D23] reduce 累积计算
来源：http://sr.panjiajie.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bo.shxzukj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://aw.gzmigu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ko.haigaiapp.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fd.hahajie.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://bb.lnxyls.cn

Go:   // 手写循环
来源：http://fa.lnxyls.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pg.haigaiapp.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nr.huanxung.cn

[D24] 字典 / Map 基本操作
来源：http://ne.huanxung.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://cv.szxytkj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hq.wgjwhj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vo.huanxung.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mv.yuntaijiaju.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gp.shxzskj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://cs.shxzukj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vi.szxytkj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ky.muxihuayi.cn

[D25] Set 集合去重与交并差
来源：http://mj.newstarts.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rs.chemitech.net.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ir.szsharing.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mr.yuexingan06.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rz.yuexingan06.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mx.lnxyls.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ir.chemitech.net.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ll.gzmigu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ng.panjiajie.cn

[D26] 数组转字符串
来源：http://hz.bookmarksfly.cn

Py:   ", ".join(map(str, arr))
来源：http://ut.asd995.cn

PHP:  implode(", ", $arr);
来源：http://lt.bjjhwx.cn

JS:   arr.join(", ")
来源：http://nu.newstarts.cn

TS:   arr.join(", ")
来源：http://ki.shxzukj.cn

Java: String.join(", ", list)
来源：http://db.panjiajie.cn

Go:   strings.Join(strs, ", ")
来源：http://rl.bookmarksfly.cn

Ruby: arr.join(", ")
来源：http://nk.9csxet.cn

C#:   string.Join(", ", list)
来源：http://so.szxytkj.cn

================================================================================
来源：http://jr.colortex.cn

E. 字符串处理
来源：http://bs.szsharing.cn

================================================================================
来源：http://ro.jianghongdianzi.cn

[E01] 拼接字符串
来源：http://qp.nicolike.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://dg.szsharing.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qy.jianghongdianzi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://uq.szxytkj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://of.panjiajie.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xx.huixiangedu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zo.hnjuh.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mj.bookmarksfly.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rq.lnxyls.cn

[E02] 重复字符串
来源：http://yn.colortex.cn

Py:   "ab" * 3
来源：http://ul.hnjuh.cn

PHP:  str_repeat("ab", 3);
来源：http://ho.bookmarksfly.cn

JS:   "ab".repeat(3)
来源：http://kn.hnjuh.cn

TS:   "ab".repeat(3)
来源：http://nn.521024.cn

Java: "ab".repeat(3)
来源：http://yk.jianghongdianzi.cn

Go:   strings.Repeat("ab", 3)
来源：http://nk.colortex.cn

Ruby: "ab" * 3
来源：http://ed.nszjky.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rt.yuexingan06.cn

[E03] 截取子串
来源：http://oe.bookmarksfly.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://br.9csxet.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vq.nicolike.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://to.bookmarksfly.cn

TS:   s.slice(1, 4)
来源：http://wg.nicolike.cn

Java: s.substring(1, 4)
来源：http://wa.szsharing.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://de.shtwfgs.cn

Ruby: s[1, 3];  s[1..3]
来源：http://kh.huixiangedu.cn

C#:   s.Substring(1, 3)
来源：http://ce.9csxet.cn

[E04] 查找子串位置
来源：http://qs.shxzukj.cn

Py:   s.find("x");  s.index("x")
来源：http://gk.szsharing.cn

PHP:  strpos($s, "x");
来源：http://ln.shxzukj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://pf.colortex.cn

TS:   s.indexOf("x")
来源：http://md.hahajie.cn

Java: s.indexOf("x")
来源：http://jo.jctech888.com.cn

Go:   strings.Index(s, "x")
来源：http://er.lnxyls.cn

Ruby: s.index("x")
来源：http://pv.szxytkj.cn

C#:   s.IndexOf("x")
来源：http://uw.newstarts.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://xd.haigaiapp.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://pi.bookmarksfly.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kr.shtwfgs.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qd.yuntaijiaju.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://lt.hnjuh.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qk.huixinmuqiang.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jn.huixinmuqiang.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fk.huixiangedu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://at.gzmigu.cn

[E06] 替换子串
来源：http://xa.haigaiapp.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://im.huanxung.cn

PHP:  str_replace("a", "b", $s);
来源：http://wy.nicolike.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nm.yuexingan06.cn

TS:   s.replaceAll("a", "b")
来源：http://up.jianghongdianzi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://eo.hahajie.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://cb.hahajie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://sh.wgjwhj.cn

C#:   s.Replace("a", "b")
来源：http://ub.hnjuh.cn

[E07] 按分隔符拆分
来源：http://tg.muxihuayi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://re.huixinmuqiang.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vz.bookmarksfly.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://wn.lnxyls.cn

TS:   s.split(",")
来源：http://xw.panjiajie.cn

Java: s.split(",");  s.split("\\s+")
来源：http://no.panjiajie.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jd.haigaiapp.cn

Ruby: s.split(",");  s.split
来源：http://ws.shxzskj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://um.nszjky.cn

[E08] 数组按分隔符合并
来源：http://gl.panjiajie.cn

Py:   ",".join(items)
来源：http://fm.gzmigu.cn

PHP:  implode(",", $items);
来源：http://uw.lnxyls.cn

JS:   items.join(",")
来源：http://rp.szsharing.cn

TS:   items.join(",")
来源：http://ua.huixinmuqiang.cn

Java: String.join(",", items)
来源：http://bi.huixinmuqiang.cn

Go:   strings.Join(items, ",")
来源：http://jj.szxytkj.cn

Ruby: items.join(",")
来源：http://gl.bjjhwx.cn

C#:   string.Join(",", items)
来源：http://hf.nicolike.cn

[E09] 去除所有空白字符
来源：http://kl.chemitech.net.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ai.nszjky.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://yp.521024.cn

JS:   s.replace(/\s+/g, "")
来源：http://yc.wgjwhj.cn

TS:   s.replace(/\s+/g, "")
来源：http://fk.shxzukj.cn

Java: s.replaceAll("\\s+", "")
来源：http://gg.wgjwhj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://au.newstarts.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ju.hnjuh.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://iv.panjiajie.cn

[E10] 左侧补零 / 定长填充
来源：http://vj.hahajie.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hx.shxzukj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tp.gzmigu.cn

JS:   "7".padStart(3, "0")
来源：http://rh.nicolike.cn

TS:   "7".padStart(3, "0")
来源：http://vk.nszjky.cn

Java: String.format("%03d", 7)
来源：http://hq.gzmigu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://jk.szsharing.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://gi.9csxet.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kf.yuntaijiaju.cn

[E11] 反转字符串
来源：http://ti.shtwfgs.cn

Py:   s[::-1]
来源：http://op.newstarts.cn

PHP:  strrev($s);
来源：http://rh.szsharing.cn

JS:   [...s].reverse().join("")
来源：http://yp.jianghongdianzi.cn

TS:   [...s].reverse().join("")
来源：http://fk.panjiajie.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://xu.muxihuayi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://qg.9csxet.cn

Ruby: s.reverse
来源：http://ny.szxytkj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://sq.yuexingan06.cn

[E12] 统计某字符出现次数
来源：http://pn.huanxung.cn

Py:   s.count("a")
来源：http://fx.muxihuayi.cn

PHP:  substr_count($s, "a");
来源：http://ak.szxytkj.cn

JS:   s.split("a").length - 1
来源：http://xf.wgjwhj.cn

TS:   s.split("a").length - 1
来源：http://wx.jianghongdianzi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://na.nszjky.cn

Go:   strings.Count(s, "a")
来源：http://hd.9csxet.cn

Ruby: s.count("a")
来源：http://do.jctech888.com.cn

C#:   s.Count(c => c == 'a')
来源：http://hx.szsharing.cn

[E13] 逐字符遍历
来源：http://ud.yuexingan06.cn

Py:   for ch in s: print(ch)
来源：http://yn.hnjuh.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zm.shxzukj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://na.haigaiapp.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ni.szxytkj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ex.jctech888.com.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nh.muxihuayi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://lt.bjjhwx.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wx.asd995.cn

[E14] URL 编码与 Base64
来源：http://io.nicolike.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://oa.lnxyls.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://sx.yuexingan06.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qh.newstarts.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ft.bookmarksfly.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bo.haigaiapp.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://aj.bjjhwx.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://pa.shxzukj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ps.szsharing.cn

[E15] HTML 转义 / 反转义
来源：http://jj.nszjky.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://mn.szxytkj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wx.521024.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wl.hnjuh.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://xp.huanxung.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://lv.chemitech.net.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wd.shxzukj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hp.jctech888.com.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://is.shxzskj.cn

[E16] 数字千分位
来源：http://op.panjiajie.cn

Py:   f"{1234567:,}"
来源：http://yn.bjjhwx.cn

PHP:  number_format(1234567);
来源：http://fy.huixinmuqiang.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://gv.szxytkj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://qu.hahajie.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ja.hahajie.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yg.hnjuh.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://va.jctech888.com.cn

C#:   1234567.ToString("N0")
来源：http://qn.9csxet.cn

[E17] 首字母大写
来源：http://dl.asd995.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bd.newstarts.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://aj.szxytkj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://eq.jctech888.com.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bn.yuntaijiaju.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xu.newstarts.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wn.colortex.cn

Ruby: s.capitalize
来源：http://ho.hnjuh.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ao.gzmigu.cn

[E18] 模板占位符替换
来源：http://px.panjiajie.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://dj.huixinmuqiang.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ny.huanxung.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ey.huixinmuqiang.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://zn.szxytkj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://iw.szsharing.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fs.9csxet.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://om.haigaiapp.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qe.huixiangedu.cn

[E19] 多行文本按行拆分
来源：http://de.hnjuh.cn

Py:   s.splitlines()
来源：http://dy.huanxung.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ow.wgjwhj.cn

JS:   s.split(/\r?\n/)
来源：http://gk.newstarts.cn

TS:   s.split(/\r?\n/)
来源：http://hg.huixinmuqiang.cn

Java: s.lines().toList()
来源：http://ri.asd995.cn

Go:   strings.Split(s, "\n")
来源：http://hh.huixiangedu.cn

Ruby: s.lines
来源：http://jg.shxzukj.cn

C#:   s.Split('\n')
来源：http://at.shxzukj.cn

[E20] 判断字符串是否为空
来源：http://tg.521024.cn

Py:   if not s:
来源：http://wr.jctech888.com.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vx.bjjhwx.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gl.shxzskj.cn

TS:   if (s === "") {}
来源：http://nw.shxzskj.cn

Java: if (s.isEmpty()) {}
来源：http://lw.haigaiapp.cn

Go:   if s == "" {}
来源：http://ss.hahajie.cn

Ruby: if s.empty?
来源：http://ve.hahajie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bd.asd995.cn

[E21] 超长截断加省略号
来源：http://lt.chemitech.net.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wh.shxzukj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qi.shxzskj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mn.jctech888.com.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qz.colortex.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ww.shxzskj.cn

Go:   // 按 rune 判断长度后截断
来源：http://kb.lnxyls.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://el.shxzskj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wx.colortex.cn

[E22] 字节长度与字符长度
来源：http://fm.gzmigu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ia.huixiangedu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ib.hnjuh.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mi.yuexingan06.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pq.jctech888.com.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xn.szsharing.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://sm.hahajie.cn

Ruby: s.bytesize;  s.length
来源：http://pb.panjiajie.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wc.lnxyls.cn

================================================================================
来源：http://wf.521024.cn

F. 文件与目录
来源：http://og.yuntaijiaju.cn

================================================================================
来源：http://mz.asd995.cn

[F01] 读取整个文件
来源：http://mj.bookmarksfly.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ca.wgjwhj.cn

PHP:  file_get_contents("a.txt");
来源：http://pl.shxzskj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ev.huanxung.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://uh.nszjky.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ab.shtwfgs.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ai.haigaiapp.cn

Ruby: File.read("a.txt")
来源：http://ah.9csxet.cn

C#:   File.ReadAllText("a.txt");
来源：http://xs.lnxyls.cn

[F02] 逐行读取文件
来源：http://lu.9csxet.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qc.jctech888.com.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://br.panjiajie.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cs.haigaiapp.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xg.nicolike.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ka.shxzskj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://he.szxytkj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://oa.wgjwhj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rg.521024.cn

[F03] 写入文件（覆盖）
来源：http://rj.szsharing.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://nx.chemitech.net.cn


<!-- 参考信息 -->