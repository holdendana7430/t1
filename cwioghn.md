代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ms.huixiangedu.cn

[D20] 统计每个元素出现次数
来源：http://hz.huanxung.cn

Py:   Counter(arr)
来源：http://mr.szxytkj.cn

PHP:  array_count_values($arr);
来源：http://ht.yuexingan06.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fy.yuntaijiaju.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dw.huixiangedu.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://pu.colortex.cn

Go:   // 手写 map[T]int
来源：http://yc.huixiangedu.cn

Ruby: arr.tally
来源：http://ca.521024.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kt.newstarts.cn

[D21] 判断是否包含某元素
来源：http://ux.521024.cn

Py:   x in arr
来源：http://jr.newstarts.cn

PHP:  in_array($x, $arr, true);
来源：http://na.bjjhwx.cn

JS:   arr.includes(x)
来源：http://tf.jianghongdianzi.cn

TS:   arr.includes(x)
来源：http://kx.szsharing.cn

Java: list.contains(x)
来源：http://qj.521024.cn

Go:   slices.Contains(arr, x)
来源：http://qr.lnxyls.cn

Ruby: arr.include?(x)
来源：http://oc.jianghongdianzi.cn

C#:   list.Contains(x)
来源：http://jt.muxihuayi.cn

[D22] 复制数组（避免共享引用）
来源：http://dx.hahajie.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fe.newstarts.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://pj.yuntaijiaju.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ml.panjiajie.cn

TS:   [...arr];
来源：http://wo.shtwfgs.cn

Java: new ArrayList<>(list);
来源：http://cx.huixiangedu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://gt.chemitech.net.cn

Ruby: arr.dup;  arr.clone
来源：http://os.yuntaijiaju.cn

C#:   new List<int>(list);
来源：http://ul.asd995.cn

[D23] reduce 累积计算
来源：http://gb.wgjwhj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://nn.shtwfgs.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wj.jianghongdianzi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sj.szsharing.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://le.chemitech.net.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://my.huixiangedu.cn

Go:   // 手写循环
来源：http://my.9csxet.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lh.panjiajie.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wk.yuntaijiaju.cn

[D24] 字典 / Map 基本操作
来源：http://oc.nicolike.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pc.jianghongdianzi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jx.szsharing.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ab.szxytkj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rz.yuexingan06.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://dx.newstarts.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wu.chemitech.net.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ok.hahajie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://br.hahajie.cn

[D25] Set 集合去重与交并差
来源：http://ko.hahajie.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ts.szsharing.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://yl.hahajie.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://oo.shtwfgs.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dj.huixinmuqiang.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dd.shxzukj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hf.shxzukj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ap.colortex.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://yd.nicolike.cn

[D26] 数组转字符串
来源：http://nx.bookmarksfly.cn

Py:   ", ".join(map(str, arr))
来源：http://pz.nicolike.cn

PHP:  implode(", ", $arr);
来源：http://gb.jctech888.com.cn

JS:   arr.join(", ")
来源：http://en.asd995.cn

TS:   arr.join(", ")
来源：http://qb.yuexingan06.cn

Java: String.join(", ", list)
来源：http://wx.shtwfgs.cn

Go:   strings.Join(strs, ", ")
来源：http://gl.shxzukj.cn

Ruby: arr.join(", ")
来源：http://vv.521024.cn

C#:   string.Join(", ", list)
来源：http://mr.haigaiapp.cn

================================================================================
来源：http://hi.colortex.cn

E. 字符串处理
来源：http://gx.nszjky.cn

================================================================================
来源：http://hu.asd995.cn

[E01] 拼接字符串
来源：http://am.szxytkj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://sw.gzmigu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://gw.521024.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qz.szxytkj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://od.jianghongdianzi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://jw.huixiangedu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pq.szsharing.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://le.nicolike.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zk.bjjhwx.cn

[E02] 重复字符串
来源：http://ab.newstarts.cn

Py:   "ab" * 3
来源：http://si.hahajie.cn

PHP:  str_repeat("ab", 3);
来源：http://qz.shxzukj.cn

JS:   "ab".repeat(3)
来源：http://lv.yuntaijiaju.cn

TS:   "ab".repeat(3)
来源：http://dp.colortex.cn

Java: "ab".repeat(3)
来源：http://ye.hnjuh.cn

Go:   strings.Repeat("ab", 3)
来源：http://wy.newstarts.cn

Ruby: "ab" * 3
来源：http://le.newstarts.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ig.nszjky.cn

[E03] 截取子串
来源：http://jl.yuntaijiaju.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ct.nicolike.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nm.huanxung.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://py.asd995.cn

TS:   s.slice(1, 4)
来源：http://sg.lnxyls.cn

Java: s.substring(1, 4)
来源：http://ii.jianghongdianzi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://yy.asd995.cn

Ruby: s[1, 3];  s[1..3]
来源：http://zq.nicolike.cn

C#:   s.Substring(1, 3)
来源：http://hy.huanxung.cn

[E04] 查找子串位置
来源：http://qn.521024.cn

Py:   s.find("x");  s.index("x")
来源：http://ea.yuntaijiaju.cn

PHP:  strpos($s, "x");
来源：http://da.huixinmuqiang.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://lh.shxzukj.cn

TS:   s.indexOf("x")
来源：http://wo.wgjwhj.cn

Java: s.indexOf("x")
来源：http://jd.newstarts.cn

Go:   strings.Index(s, "x")
来源：http://ok.asd995.cn

Ruby: s.index("x")
来源：http://sn.lnxyls.cn

C#:   s.IndexOf("x")
来源：http://qk.nszjky.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://vo.huanxung.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://so.shtwfgs.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://le.szxytkj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://or.chemitech.net.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://xe.chemitech.net.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yq.huixiangedu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fl.hnjuh.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://eh.hahajie.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://no.huixinmuqiang.cn

[E06] 替换子串
来源：http://ql.szsharing.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://th.nszjky.cn

PHP:  str_replace("a", "b", $s);
来源：http://lm.shxzskj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://eq.wgjwhj.cn

TS:   s.replaceAll("a", "b")
来源：http://lf.szxytkj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://st.newstarts.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bp.521024.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://pv.bjjhwx.cn

C#:   s.Replace("a", "b")
来源：http://yp.wgjwhj.cn

[E07] 按分隔符拆分
来源：http://at.9csxet.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rv.huixinmuqiang.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rq.jianghongdianzi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://iw.wgjwhj.cn

TS:   s.split(",")
来源：http://at.nicolike.cn

Java: s.split(",");  s.split("\\s+")
来源：http://nv.shtwfgs.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vk.hnjuh.cn

Ruby: s.split(",");  s.split
来源：http://gv.jctech888.com.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ri.chemitech.net.cn

[E08] 数组按分隔符合并
来源：http://an.jianghongdianzi.cn

Py:   ",".join(items)
来源：http://iq.bjjhwx.cn

PHP:  implode(",", $items);
来源：http://iz.hnjuh.cn

JS:   items.join(",")
来源：http://mr.panjiajie.cn

TS:   items.join(",")
来源：http://nj.huixiangedu.cn

Java: String.join(",", items)
来源：http://lt.9csxet.cn

Go:   strings.Join(items, ",")
来源：http://ku.hahajie.cn

Ruby: items.join(",")
来源：http://aq.gzmigu.cn

C#:   string.Join(",", items)
来源：http://bn.huixiangedu.cn

[E09] 去除所有空白字符
来源：http://ks.jianghongdianzi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ha.shtwfgs.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mz.huanxung.cn

JS:   s.replace(/\s+/g, "")
来源：http://xs.hnjuh.cn

TS:   s.replace(/\s+/g, "")
来源：http://rn.wgjwhj.cn

Java: s.replaceAll("\\s+", "")
来源：http://sb.lnxyls.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://mq.gzmigu.cn

Ruby: s.gsub(/\s+/, "")
来源：http://be.wgjwhj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qy.shtwfgs.cn

[E10] 左侧补零 / 定长填充
来源：http://ok.colortex.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vf.jctech888.com.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fg.huixiangedu.cn

JS:   "7".padStart(3, "0")
来源：http://or.colortex.cn

TS:   "7".padStart(3, "0")
来源：http://ge.huanxung.cn

Java: String.format("%03d", 7)
来源：http://ae.hnjuh.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://hs.szxytkj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ov.wgjwhj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://tb.shxzskj.cn

[E11] 反转字符串
来源：http://nb.jianghongdianzi.cn

Py:   s[::-1]
来源：http://sg.shxzukj.cn

PHP:  strrev($s);
来源：http://ej.yuexingan06.cn

JS:   [...s].reverse().join("")
来源：http://zw.chemitech.net.cn

TS:   [...s].reverse().join("")
来源：http://ou.chemitech.net.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://vu.shxzskj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://go.shxzskj.cn

Ruby: s.reverse
来源：http://sv.gzmigu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://qy.shxzskj.cn

[E12] 统计某字符出现次数
来源：http://fn.hahajie.cn

Py:   s.count("a")
来源：http://vh.521024.cn

PHP:  substr_count($s, "a");
来源：http://td.bookmarksfly.cn

JS:   s.split("a").length - 1
来源：http://or.huixiangedu.cn

TS:   s.split("a").length - 1
来源：http://vq.shxzukj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jd.huanxung.cn

Go:   strings.Count(s, "a")
来源：http://pt.shtwfgs.cn

Ruby: s.count("a")
来源：http://uo.haigaiapp.cn

C#:   s.Count(c => c == 'a')
来源：http://bx.huixinmuqiang.cn

[E13] 逐字符遍历
来源：http://yo.jianghongdianzi.cn

Py:   for ch in s: print(ch)
来源：http://qv.jianghongdianzi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wv.hnjuh.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://dz.muxihuayi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://vk.bookmarksfly.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wg.hahajie.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://px.hnjuh.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ce.shtwfgs.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gs.jctech888.com.cn

[E14] URL 编码与 Base64
来源：http://rv.huanxung.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://id.yuntaijiaju.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://cm.chemitech.net.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://cg.jctech888.com.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://cg.newstarts.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kr.jianghongdianzi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ng.yuntaijiaju.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bj.shxzukj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wi.wgjwhj.cn

[E15] HTML 转义 / 反转义
来源：http://mh.muxihuayi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://px.asd995.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dc.wgjwhj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fp.szxytkj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ab.huixiangedu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://er.szsharing.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bq.haigaiapp.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pf.gzmigu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ux.yuntaijiaju.cn

[E16] 数字千分位
来源：http://vx.colortex.cn

Py:   f"{1234567:,}"
来源：http://kg.chemitech.net.cn

PHP:  number_format(1234567);
来源：http://xz.nszjky.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://hc.hnjuh.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://zh.gzmigu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://pt.shxzskj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://pz.jianghongdianzi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://oq.hahajie.cn

C#:   1234567.ToString("N0")
来源：http://yu.gzmigu.cn

[E17] 首字母大写
来源：http://om.bjjhwx.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://lv.jianghongdianzi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://es.huanxung.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vw.huixiangedu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fx.yuntaijiaju.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vn.bookmarksfly.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ov.bookmarksfly.cn

Ruby: s.capitalize
来源：http://xo.shxzukj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wj.9csxet.cn

[E18] 模板占位符替换
来源：http://va.shtwfgs.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qu.newstarts.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bg.chemitech.net.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://jn.shtwfgs.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://nu.lnxyls.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kj.jctech888.com.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zy.panjiajie.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dw.9csxet.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://uq.bjjhwx.cn

[E19] 多行文本按行拆分
来源：http://ts.muxihuayi.cn

Py:   s.splitlines()
来源：http://bn.wgjwhj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://py.haigaiapp.cn

JS:   s.split(/\r?\n/)
来源：http://qa.chemitech.net.cn

TS:   s.split(/\r?\n/)
来源：http://qp.shtwfgs.cn

Java: s.lines().toList()
来源：http://zj.szsharing.cn

Go:   strings.Split(s, "\n")
来源：http://jj.szsharing.cn

Ruby: s.lines
来源：http://pz.newstarts.cn

C#:   s.Split('\n')
来源：http://wl.huixiangedu.cn

[E20] 判断字符串是否为空
来源：http://js.shxzskj.cn

Py:   if not s:
来源：http://uw.huixiangedu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://iw.muxihuayi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gb.huanxung.cn

TS:   if (s === "") {}
来源：http://fb.lnxyls.cn

Java: if (s.isEmpty()) {}
来源：http://mh.shxzskj.cn

Go:   if s == "" {}
来源：http://sy.521024.cn

Ruby: if s.empty?
来源：http://qe.521024.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://sr.haigaiapp.cn

[E21] 超长截断加省略号
来源：http://jn.yuexingan06.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://fh.jianghongdianzi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://yu.wgjwhj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zz.asd995.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wf.yuexingan06.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://lj.chemitech.net.cn

Go:   // 按 rune 判断长度后截断
来源：http://ob.muxihuayi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ht.shxzukj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://om.huixiangedu.cn

[E22] 字节长度与字符长度
来源：http://ha.bjjhwx.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xb.hnjuh.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lj.huanxung.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://cz.bookmarksfly.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rl.shxzskj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bn.jctech888.com.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://az.szxytkj.cn

Ruby: s.bytesize;  s.length
来源：http://la.yuexingan06.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://tl.asd995.cn

================================================================================
来源：http://ml.muxihuayi.cn

F. 文件与目录
来源：http://or.hnjuh.cn

================================================================================
来源：http://dx.hahajie.cn

[F01] 读取整个文件
来源：http://vf.yuntaijiaju.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xj.shxzskj.cn

PHP:  file_get_contents("a.txt");
来源：http://ry.shxzskj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://df.yuntaijiaju.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wm.szsharing.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://dr.asd995.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://al.huanxung.cn

Ruby: File.read("a.txt")
来源：http://su.asd995.cn

C#:   File.ReadAllText("a.txt");
来源：http://iq.szsharing.cn

[F02] 逐行读取文件
来源：http://hm.muxihuayi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://cc.gzmigu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://in.panjiajie.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rn.panjiajie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tg.nszjky.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ls.hahajie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://aq.newstarts.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bj.huanxung.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://cq.jianghongdianzi.cn

[F03] 写入文件（覆盖）
来源：http://gl.shtwfgs.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ae.hnjuh.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://yb.szxytkj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pg.hahajie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wb.521024.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ul.wgjwhj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://pm.huanxung.cn

Ruby: File.write("a.txt", "hi")
来源：http://ce.shxzukj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://no.521024.cn

[F04] 追加写入文件
来源：http://ht.bookmarksfly.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://cx.szxytkj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yz.szxytkj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ze.muxihuayi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ps.huixinmuqiang.cn


<!-- 参考信息 -->