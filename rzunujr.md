代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://nm.9csxet.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dg.bjjhwx.cn

Go:   // 手写 map[string][]T
来源：http://em.jianghongdianzi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ur.huixinmuqiang.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://au.jctech888.com.cn

[D20] 统计每个元素出现次数
来源：http://iq.huixinmuqiang.cn

Py:   Counter(arr)
来源：http://iw.shxzukj.cn

PHP:  array_count_values($arr);
来源：http://hr.nszjky.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ut.nicolike.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gb.panjiajie.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://kv.huixinmuqiang.cn

Go:   // 手写 map[T]int
来源：http://df.bjjhwx.cn

Ruby: arr.tally
来源：http://xi.hahajie.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ch.huanxung.cn

[D21] 判断是否包含某元素
来源：http://nj.nszjky.cn

Py:   x in arr
来源：http://nv.huixinmuqiang.cn

PHP:  in_array($x, $arr, true);
来源：http://ac.yuntaijiaju.cn

JS:   arr.includes(x)
来源：http://fg.yuntaijiaju.cn

TS:   arr.includes(x)
来源：http://kf.jctech888.com.cn

Java: list.contains(x)
来源：http://de.szxytkj.cn

Go:   slices.Contains(arr, x)
来源：http://fv.hnjuh.cn

Ruby: arr.include?(x)
来源：http://vs.jianghongdianzi.cn

C#:   list.Contains(x)
来源：http://ba.bjjhwx.cn

[D22] 复制数组（避免共享引用）
来源：http://ja.haigaiapp.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gz.9csxet.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cn.shxzskj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://co.521024.cn

TS:   [...arr];
来源：http://pq.haigaiapp.cn

Java: new ArrayList<>(list);
来源：http://wv.bjjhwx.cn

Go:   copied := append([]int(nil), arr...)
来源：http://am.9csxet.cn

Ruby: arr.dup;  arr.clone
来源：http://bv.bjjhwx.cn

C#:   new List<int>(list);
来源：http://eq.yuexingan06.cn

[D23] reduce 累积计算
来源：http://gp.nszjky.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jz.521024.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://nm.huixiangedu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fq.jctech888.com.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ma.panjiajie.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://tp.nicolike.cn

Go:   // 手写循环
来源：http://rk.jctech888.com.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ul.muxihuayi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wr.521024.cn

[D24] 字典 / Map 基本操作
来源：http://rf.yuexingan06.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pc.9csxet.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://st.colortex.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rk.muxihuayi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://sv.muxihuayi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jk.wgjwhj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fg.yuexingan06.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cx.panjiajie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ev.colortex.cn

[D25] Set 集合去重与交并差
来源：http://ww.huixinmuqiang.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://cz.szsharing.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fa.szxytkj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rs.yuntaijiaju.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ss.nszjky.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ci.shtwfgs.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://yp.lnxyls.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://yg.shxzukj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ci.shtwfgs.cn

[D26] 数组转字符串
来源：http://xx.shtwfgs.cn

Py:   ", ".join(map(str, arr))
来源：http://dh.chemitech.net.cn

PHP:  implode(", ", $arr);
来源：http://pc.shxzukj.cn

JS:   arr.join(", ")
来源：http://ri.lnxyls.cn

TS:   arr.join(", ")
来源：http://ck.wgjwhj.cn

Java: String.join(", ", list)
来源：http://hi.szxytkj.cn

Go:   strings.Join(strs, ", ")
来源：http://yh.yuntaijiaju.cn

Ruby: arr.join(", ")
来源：http://oq.nszjky.cn

C#:   string.Join(", ", list)
来源：http://fl.colortex.cn

================================================================================
来源：http://rw.asd995.cn

E. 字符串处理
来源：http://ys.shtwfgs.cn

================================================================================
来源：http://zk.bjjhwx.cn

[E01] 拼接字符串
来源：http://ln.chemitech.net.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gp.muxihuayi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://uo.shxzukj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://df.haigaiapp.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ik.hahajie.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://av.bjjhwx.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ob.shxzukj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ik.jianghongdianzi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vy.panjiajie.cn

[E02] 重复字符串
来源：http://wm.nszjky.cn

Py:   "ab" * 3
来源：http://ok.chemitech.net.cn

PHP:  str_repeat("ab", 3);
来源：http://df.gzmigu.cn

JS:   "ab".repeat(3)
来源：http://hu.jianghongdianzi.cn

TS:   "ab".repeat(3)
来源：http://yf.yuexingan06.cn

Java: "ab".repeat(3)
来源：http://mk.shtwfgs.cn

Go:   strings.Repeat("ab", 3)
来源：http://ag.gzmigu.cn

Ruby: "ab" * 3
来源：http://ny.huixiangedu.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://oo.haigaiapp.cn

[E03] 截取子串
来源：http://rz.panjiajie.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rv.gzmigu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://rf.shtwfgs.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wz.yuexingan06.cn

TS:   s.slice(1, 4)
来源：http://jw.nicolike.cn

Java: s.substring(1, 4)
来源：http://bz.haigaiapp.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://he.chemitech.net.cn

Ruby: s[1, 3];  s[1..3]
来源：http://au.nszjky.cn

C#:   s.Substring(1, 3)
来源：http://hv.muxihuayi.cn

[E04] 查找子串位置
来源：http://zl.haigaiapp.cn

Py:   s.find("x");  s.index("x")
来源：http://gh.bookmarksfly.cn

PHP:  strpos($s, "x");
来源：http://nf.jianghongdianzi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mq.jianghongdianzi.cn

TS:   s.indexOf("x")
来源：http://sr.huanxung.cn

Java: s.indexOf("x")
来源：http://ar.muxihuayi.cn

Go:   strings.Index(s, "x")
来源：http://eg.521024.cn

Ruby: s.index("x")
来源：http://ho.hnjuh.cn

C#:   s.IndexOf("x")
来源：http://jd.bjjhwx.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://fx.colortex.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xp.chemitech.net.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jk.haigaiapp.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dz.521024.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://bd.szsharing.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sh.szsharing.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://de.szsharing.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ps.yuntaijiaju.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xb.huixinmuqiang.cn

[E06] 替换子串
来源：http://mf.bookmarksfly.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rf.jianghongdianzi.cn

PHP:  str_replace("a", "b", $s);
来源：http://su.lnxyls.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cg.shxzukj.cn

TS:   s.replaceAll("a", "b")
来源：http://lh.colortex.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kd.yuexingan06.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ph.szsharing.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zl.bookmarksfly.cn

C#:   s.Replace("a", "b")
来源：http://yz.nicolike.cn

[E07] 按分隔符拆分
来源：http://ki.hahajie.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rb.asd995.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zk.nszjky.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://cp.yuntaijiaju.cn

TS:   s.split(",")
来源：http://bu.huanxung.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ms.huanxung.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mj.muxihuayi.cn

Ruby: s.split(",");  s.split
来源：http://pf.bookmarksfly.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://en.huixinmuqiang.cn

[E08] 数组按分隔符合并
来源：http://pf.hahajie.cn

Py:   ",".join(items)
来源：http://zf.jianghongdianzi.cn

PHP:  implode(",", $items);
来源：http://os.bjjhwx.cn

JS:   items.join(",")
来源：http://rk.colortex.cn

TS:   items.join(",")
来源：http://wq.yuntaijiaju.cn

Java: String.join(",", items)
来源：http://hf.9csxet.cn

Go:   strings.Join(items, ",")
来源：http://fa.jianghongdianzi.cn

Ruby: items.join(",")
来源：http://yz.bookmarksfly.cn

C#:   string.Join(",", items)
来源：http://sb.colortex.cn

[E09] 去除所有空白字符
来源：http://um.muxihuayi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://he.shtwfgs.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lo.asd995.cn

JS:   s.replace(/\s+/g, "")
来源：http://gj.hahajie.cn

TS:   s.replace(/\s+/g, "")
来源：http://ft.bjjhwx.cn

Java: s.replaceAll("\\s+", "")
来源：http://ht.shxzukj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://fe.chemitech.net.cn

Ruby: s.gsub(/\s+/, "")
来源：http://eh.9csxet.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kn.bookmarksfly.cn

[E10] 左侧补零 / 定长填充
来源：http://bq.521024.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vc.yuntaijiaju.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ul.yuntaijiaju.cn

JS:   "7".padStart(3, "0")
来源：http://oi.jianghongdianzi.cn

TS:   "7".padStart(3, "0")
来源：http://gq.colortex.cn

Java: String.format("%03d", 7)
来源：http://rs.szxytkj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://pj.asd995.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ba.muxihuayi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ik.jianghongdianzi.cn

[E11] 反转字符串
来源：http://xn.shxzskj.cn

Py:   s[::-1]
来源：http://fu.wgjwhj.cn

PHP:  strrev($s);
来源：http://gp.haigaiapp.cn

JS:   [...s].reverse().join("")
来源：http://dc.szsharing.cn

TS:   [...s].reverse().join("")
来源：http://gd.lnxyls.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://gf.shxzskj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://du.newstarts.cn

Ruby: s.reverse
来源：http://yt.nicolike.cn

C#:   new string(s.Reverse().ToArray())
来源：http://dv.gzmigu.cn

[E12] 统计某字符出现次数
来源：http://tc.newstarts.cn

Py:   s.count("a")
来源：http://jp.huanxung.cn

PHP:  substr_count($s, "a");
来源：http://xe.colortex.cn

JS:   s.split("a").length - 1
来源：http://az.nszjky.cn

TS:   s.split("a").length - 1
来源：http://ih.muxihuayi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://se.9csxet.cn

Go:   strings.Count(s, "a")
来源：http://ie.huixinmuqiang.cn

Ruby: s.count("a")
来源：http://cg.colortex.cn

C#:   s.Count(c => c == 'a')
来源：http://qz.yuexingan06.cn

[E13] 逐字符遍历
来源：http://li.haigaiapp.cn

Py:   for ch in s: print(ch)
来源：http://nq.szsharing.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gf.jianghongdianzi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://kr.szxytkj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://eo.jianghongdianzi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://yc.nicolike.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fs.chemitech.net.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://tc.muxihuayi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://or.huixiangedu.cn

[E14] URL 编码与 Base64
来源：http://in.jctech888.com.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://es.nicolike.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://kg.yuntaijiaju.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://eb.jianghongdianzi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://sp.jctech888.com.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kv.colortex.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://il.hnjuh.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qd.wgjwhj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hd.szxytkj.cn

[E15] HTML 转义 / 反转义
来源：http://jr.yuexingan06.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://xz.panjiajie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jr.521024.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fl.jctech888.com.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://km.shtwfgs.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fy.muxihuayi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gm.jctech888.com.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://na.wgjwhj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://yi.jctech888.com.cn

[E16] 数字千分位
来源：http://zb.yuntaijiaju.cn

Py:   f"{1234567:,}"
来源：http://nh.521024.cn

PHP:  number_format(1234567);
来源：http://od.bookmarksfly.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://gh.yuntaijiaju.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://hc.521024.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lu.szsharing.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://dm.gzmigu.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tq.9csxet.cn

C#:   1234567.ToString("N0")
来源：http://fr.lnxyls.cn

[E17] 首字母大写
来源：http://oe.newstarts.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zh.nicolike.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://wj.shtwfgs.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mb.asd995.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qt.huanxung.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qj.asd995.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xh.bjjhwx.cn

Ruby: s.capitalize
来源：http://ev.gzmigu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nq.szxytkj.cn

[E18] 模板占位符替换
来源：http://md.panjiajie.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fk.jctech888.com.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://oq.huanxung.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://qm.bjjhwx.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://db.shxzukj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xq.wgjwhj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://uw.colortex.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://sh.jctech888.com.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wd.9csxet.cn

[E19] 多行文本按行拆分
来源：http://nb.nicolike.cn

Py:   s.splitlines()
来源：http://ki.shtwfgs.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kj.colortex.cn

JS:   s.split(/\r?\n/)
来源：http://hn.yuexingan06.cn

TS:   s.split(/\r?\n/)
来源：http://dj.huixinmuqiang.cn

Java: s.lines().toList()
来源：http://ke.szsharing.cn

Go:   strings.Split(s, "\n")
来源：http://ks.chemitech.net.cn

Ruby: s.lines
来源：http://xv.asd995.cn

C#:   s.Split('\n')
来源：http://on.nicolike.cn

[E20] 判断字符串是否为空
来源：http://ro.panjiajie.cn

Py:   if not s:
来源：http://gl.wgjwhj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://nn.haigaiapp.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://oy.hahajie.cn

TS:   if (s === "") {}
来源：http://dc.lnxyls.cn

Java: if (s.isEmpty()) {}
来源：http://qt.bjjhwx.cn

Go:   if s == "" {}
来源：http://pd.hnjuh.cn

Ruby: if s.empty?
来源：http://gw.jctech888.com.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bq.yuntaijiaju.cn

[E21] 超长截断加省略号
来源：http://nq.jianghongdianzi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://yi.muxihuayi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lt.yuntaijiaju.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://li.huixinmuqiang.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jh.521024.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hj.hahajie.cn

Go:   // 按 rune 判断长度后截断
来源：http://vh.shxzskj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vw.szsharing.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kg.bookmarksfly.cn

[E22] 字节长度与字符长度
来源：http://ot.huanxung.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zv.yuntaijiaju.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ho.gzmigu.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ai.521024.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://sk.colortex.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://nu.huixinmuqiang.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://sx.jctech888.com.cn

Ruby: s.bytesize;  s.length
来源：http://jr.newstarts.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://or.jctech888.com.cn

================================================================================
来源：http://ce.jctech888.com.cn

F. 文件与目录
来源：http://xt.yuexingan06.cn

================================================================================
来源：http://iz.szsharing.cn

[F01] 读取整个文件
来源：http://ll.asd995.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://al.nicolike.cn

PHP:  file_get_contents("a.txt");
来源：http://st.asd995.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://it.szxytkj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ub.newstarts.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://lk.colortex.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kb.hahajie.cn

Ruby: File.read("a.txt")
来源：http://pi.panjiajie.cn

C#:   File.ReadAllText("a.txt");
来源：http://vm.muxihuayi.cn

[F02] 逐行读取文件
来源：http://pn.hnjuh.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lg.huixiangedu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kt.wgjwhj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fu.asd995.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yk.newstarts.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fk.shxzskj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mo.shxzukj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kk.bjjhwx.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gu.nszjky.cn

[F03] 写入文件（覆盖）
来源：http://ib.huanxung.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ma.wgjwhj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://hs.huanxung.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ts.bjjhwx.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bx.panjiajie.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xw.szsharing.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wz.panjiajie.cn

Ruby: File.write("a.txt", "hi")
来源：http://ql.wgjwhj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lh.bookmarksfly.cn

[F04] 追加写入文件
来源：http://jl.bookmarksfly.cn


<!-- 参考信息 -->