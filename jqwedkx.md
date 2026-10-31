代发 wailian999

Ruby: arr.tally
来源：http://yi.lnxyls.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tt.9csxet.cn

[D21] 判断是否包含某元素
来源：http://oy.huanxung.cn

Py:   x in arr
来源：http://ie.colortex.cn

PHP:  in_array($x, $arr, true);
来源：http://rt.nicolike.cn

JS:   arr.includes(x)
来源：http://qf.521024.cn

TS:   arr.includes(x)
来源：http://cq.yuntaijiaju.cn

Java: list.contains(x)
来源：http://ab.asd995.cn

Go:   slices.Contains(arr, x)
来源：http://lb.521024.cn

Ruby: arr.include?(x)
来源：http://ex.521024.cn

C#:   list.Contains(x)
来源：http://cn.wgjwhj.cn

[D22] 复制数组（避免共享引用）
来源：http://px.521024.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nf.huixinmuqiang.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://yb.wgjwhj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://le.bookmarksfly.cn

TS:   [...arr];
来源：http://gz.jctech888.com.cn

Java: new ArrayList<>(list);
来源：http://gy.nszjky.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ka.panjiajie.cn

Ruby: arr.dup;  arr.clone
来源：http://wj.huixinmuqiang.cn

C#:   new List<int>(list);
来源：http://kb.yuntaijiaju.cn

[D23] reduce 累积计算
来源：http://bn.jianghongdianzi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rb.hahajie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zq.bookmarksfly.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cb.9csxet.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zl.shxzskj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://tk.colortex.cn

Go:   // 手写循环
来源：http://ge.huixinmuqiang.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://uj.muxihuayi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://sd.521024.cn

[D24] 字典 / Map 基本操作
来源：http://ip.panjiajie.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://oi.bookmarksfly.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://st.asd995.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ja.521024.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nj.colortex.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qv.lnxyls.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rr.gzmigu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lj.hnjuh.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qm.huixiangedu.cn

[D25] Set 集合去重与交并差
来源：http://tz.lnxyls.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://oi.muxihuayi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fx.nszjky.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xt.521024.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xj.shxzukj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://df.gzmigu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://fd.hnjuh.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gi.huanxung.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://eq.haigaiapp.cn

[D26] 数组转字符串
来源：http://sq.panjiajie.cn

Py:   ", ".join(map(str, arr))
来源：http://gk.huixinmuqiang.cn

PHP:  implode(", ", $arr);
来源：http://wa.huixinmuqiang.cn

JS:   arr.join(", ")
来源：http://nj.haigaiapp.cn

TS:   arr.join(", ")
来源：http://kh.jianghongdianzi.cn

Java: String.join(", ", list)
来源：http://rr.szxytkj.cn

Go:   strings.Join(strs, ", ")
来源：http://xf.hahajie.cn

Ruby: arr.join(", ")
来源：http://mv.chemitech.net.cn

C#:   string.Join(", ", list)
来源：http://aa.bookmarksfly.cn

================================================================================
来源：http://wu.szsharing.cn

E. 字符串处理
来源：http://xr.bjjhwx.cn

================================================================================
来源：http://cc.9csxet.cn

[E01] 拼接字符串
来源：http://th.jctech888.com.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mq.newstarts.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://bh.hahajie.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fe.wgjwhj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rf.gzmigu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qs.shtwfgs.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wb.lnxyls.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ki.bjjhwx.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xt.huixiangedu.cn

[E02] 重复字符串
来源：http://uj.haigaiapp.cn

Py:   "ab" * 3
来源：http://cc.huixinmuqiang.cn

PHP:  str_repeat("ab", 3);
来源：http://sg.nszjky.cn

JS:   "ab".repeat(3)
来源：http://ox.szsharing.cn

TS:   "ab".repeat(3)
来源：http://hx.shxzukj.cn

Java: "ab".repeat(3)
来源：http://uk.jctech888.com.cn

Go:   strings.Repeat("ab", 3)
来源：http://yx.lnxyls.cn

Ruby: "ab" * 3
来源：http://tt.hnjuh.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://nw.shxzskj.cn

[E03] 截取子串
来源：http://xf.shxzukj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yv.panjiajie.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vh.asd995.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wn.gzmigu.cn

TS:   s.slice(1, 4)
来源：http://ai.nicolike.cn

Java: s.substring(1, 4)
来源：http://fs.shxzskj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ki.szxytkj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://xy.lnxyls.cn

C#:   s.Substring(1, 3)
来源：http://mo.colortex.cn

[E04] 查找子串位置
来源：http://xb.shtwfgs.cn

Py:   s.find("x");  s.index("x")
来源：http://ls.wgjwhj.cn

PHP:  strpos($s, "x");
来源：http://nn.hnjuh.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://lf.huanxung.cn

TS:   s.indexOf("x")
来源：http://dl.huixinmuqiang.cn

Java: s.indexOf("x")
来源：http://jv.bjjhwx.cn

Go:   strings.Index(s, "x")
来源：http://mg.szsharing.cn

Ruby: s.index("x")
来源：http://ue.huixiangedu.cn

C#:   s.IndexOf("x")
来源：http://eq.hnjuh.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://wo.szsharing.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gv.panjiajie.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://cf.nszjky.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://eh.shxzskj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ny.szsharing.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://np.jctech888.com.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://np.asd995.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rb.lnxyls.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mo.jianghongdianzi.cn

[E06] 替换子串
来源：http://ny.szsharing.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://oh.newstarts.cn

PHP:  str_replace("a", "b", $s);
来源：http://oa.panjiajie.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ht.colortex.cn

TS:   s.replaceAll("a", "b")
来源：http://qs.shtwfgs.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ws.szsharing.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://dd.huanxung.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hr.szxytkj.cn

C#:   s.Replace("a", "b")
来源：http://ks.521024.cn

[E07] 按分隔符拆分
来源：http://na.huixinmuqiang.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://tf.hahajie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://lz.jianghongdianzi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ms.shxzskj.cn

TS:   s.split(",")
来源：http://eq.bookmarksfly.cn

Java: s.split(",");  s.split("\\s+")
来源：http://xw.huixinmuqiang.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pk.hahajie.cn

Ruby: s.split(",");  s.split
来源：http://ku.yuntaijiaju.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ss.huixiangedu.cn

[E08] 数组按分隔符合并
来源：http://xp.szxytkj.cn

Py:   ",".join(items)
来源：http://bf.haigaiapp.cn

PHP:  implode(",", $items);
来源：http://zd.jianghongdianzi.cn

JS:   items.join(",")
来源：http://vd.hnjuh.cn

TS:   items.join(",")
来源：http://jf.panjiajie.cn

Java: String.join(",", items)
来源：http://kp.colortex.cn

Go:   strings.Join(items, ",")
来源：http://hu.yuntaijiaju.cn

Ruby: items.join(",")
来源：http://fz.bookmarksfly.cn

C#:   string.Join(",", items)
来源：http://ur.hnjuh.cn

[E09] 去除所有空白字符
来源：http://yd.panjiajie.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jh.521024.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zu.colortex.cn

JS:   s.replace(/\s+/g, "")
来源：http://hh.chemitech.net.cn

TS:   s.replace(/\s+/g, "")
来源：http://px.chemitech.net.cn

Java: s.replaceAll("\\s+", "")
来源：http://zj.haigaiapp.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://wm.wgjwhj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://sl.asd995.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://aq.wgjwhj.cn

[E10] 左侧补零 / 定长填充
来源：http://hm.huixiangedu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ze.yuntaijiaju.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qa.yuexingan06.cn

JS:   "7".padStart(3, "0")
来源：http://sl.colortex.cn

TS:   "7".padStart(3, "0")
来源：http://pd.jctech888.com.cn

Java: String.format("%03d", 7)
来源：http://cz.bjjhwx.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://as.shtwfgs.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ot.nszjky.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jb.muxihuayi.cn

[E11] 反转字符串
来源：http://hh.jctech888.com.cn

Py:   s[::-1]
来源：http://ys.bjjhwx.cn

PHP:  strrev($s);
来源：http://ms.nszjky.cn

JS:   [...s].reverse().join("")
来源：http://fl.huixinmuqiang.cn

TS:   [...s].reverse().join("")
来源：http://el.9csxet.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://dh.hnjuh.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://zf.hahajie.cn

Ruby: s.reverse
来源：http://xk.newstarts.cn

C#:   new string(s.Reverse().ToArray())
来源：http://bj.haigaiapp.cn

[E12] 统计某字符出现次数
来源：http://jy.colortex.cn

Py:   s.count("a")
来源：http://ya.huixinmuqiang.cn

PHP:  substr_count($s, "a");
来源：http://gp.wgjwhj.cn

JS:   s.split("a").length - 1
来源：http://by.jianghongdianzi.cn

TS:   s.split("a").length - 1
来源：http://xa.9csxet.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gc.newstarts.cn

Go:   strings.Count(s, "a")
来源：http://xw.yuexingan06.cn

Ruby: s.count("a")
来源：http://up.hnjuh.cn

C#:   s.Count(c => c == 'a')
来源：http://zq.nicolike.cn

[E13] 逐字符遍历
来源：http://mk.chemitech.net.cn

Py:   for ch in s: print(ch)
来源：http://tl.huixinmuqiang.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ps.jianghongdianzi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://lv.nszjky.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://es.asd995.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ww.gzmigu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tg.huixinmuqiang.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://yj.chemitech.net.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://yk.hnjuh.cn

[E14] URL 编码与 Base64
来源：http://jf.colortex.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pe.bjjhwx.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://cw.shxzukj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://av.asd995.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gk.asd995.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qu.huanxung.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qo.shxzukj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://su.chemitech.net.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wv.muxihuayi.cn

[E15] HTML 转义 / 反转义
来源：http://bn.colortex.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://yu.szxytkj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wc.panjiajie.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mq.newstarts.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://kj.chemitech.net.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://yv.panjiajie.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xq.panjiajie.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pc.szxytkj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cv.nicolike.cn

[E16] 数字千分位
来源：http://kx.panjiajie.cn

Py:   f"{1234567:,}"
来源：http://df.jianghongdianzi.cn

PHP:  number_format(1234567);
来源：http://ux.bjjhwx.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://rd.lnxyls.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://xq.yuntaijiaju.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ka.shtwfgs.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ss.hnjuh.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nq.hnjuh.cn

C#:   1234567.ToString("N0")
来源：http://by.521024.cn

[E17] 首字母大写
来源：http://jy.jctech888.com.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bw.haigaiapp.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://vv.9csxet.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tz.bookmarksfly.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fw.colortex.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://yh.yuntaijiaju.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://nj.521024.cn

Ruby: s.capitalize
来源：http://ub.colortex.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mn.lnxyls.cn

[E18] 模板占位符替换
来源：http://fx.muxihuayi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ej.hnjuh.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ec.huanxung.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://xh.panjiajie.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://sv.shxzskj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://an.huanxung.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kj.wgjwhj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://me.huanxung.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jl.bjjhwx.cn

[E19] 多行文本按行拆分
来源：http://fd.colortex.cn

Py:   s.splitlines()
来源：http://nh.asd995.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gp.521024.cn

JS:   s.split(/\r?\n/)
来源：http://rs.9csxet.cn

TS:   s.split(/\r?\n/)
来源：http://cw.panjiajie.cn

Java: s.lines().toList()
来源：http://uh.szxytkj.cn

Go:   strings.Split(s, "\n")
来源：http://am.jianghongdianzi.cn

Ruby: s.lines
来源：http://vh.shtwfgs.cn

C#:   s.Split('\n')
来源：http://xy.nszjky.cn

[E20] 判断字符串是否为空
来源：http://da.nszjky.cn

Py:   if not s:
来源：http://ti.muxihuayi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yb.colortex.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ax.wgjwhj.cn

TS:   if (s === "") {}
来源：http://fx.haigaiapp.cn

Java: if (s.isEmpty()) {}
来源：http://rk.colortex.cn

Go:   if s == "" {}
来源：http://fy.huanxung.cn

Ruby: if s.empty?
来源：http://sf.9csxet.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.newstarts.cn

[E21] 超长截断加省略号
来源：http://dl.bjjhwx.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://pn.huanxung.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://eo.521024.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dr.wgjwhj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://of.hahajie.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qh.muxihuayi.cn

Go:   // 按 rune 判断长度后截断
来源：http://ud.panjiajie.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://or.nszjky.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tz.szxytkj.cn

[E22] 字节长度与字符长度
来源：http://cg.nszjky.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vl.shtwfgs.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vv.huixinmuqiang.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://yh.yuntaijiaju.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qo.szsharing.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rw.jianghongdianzi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mx.newstarts.cn

Ruby: s.bytesize;  s.length
来源：http://ie.521024.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://pm.chemitech.net.cn

================================================================================
来源：http://mm.panjiajie.cn

F. 文件与目录
来源：http://cp.jianghongdianzi.cn

================================================================================
来源：http://ro.szxytkj.cn

[F01] 读取整个文件
来源：http://iy.yuntaijiaju.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ma.hnjuh.cn

PHP:  file_get_contents("a.txt");
来源：http://rm.jianghongdianzi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fh.shxzukj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://tg.haigaiapp.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ov.huanxung.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://uv.nicolike.cn

Ruby: File.read("a.txt")
来源：http://cf.wgjwhj.cn

C#:   File.ReadAllText("a.txt");
来源：http://cy.521024.cn

[F02] 逐行读取文件
来源：http://fo.szxytkj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gj.521024.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://tx.huanxung.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ya.asd995.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ej.bjjhwx.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://tj.chemitech.net.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xd.wgjwhj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gs.jianghongdianzi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xo.9csxet.cn

[F03] 写入文件（覆盖）
来源：http://vu.lnxyls.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ie.bjjhwx.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://pq.gzmigu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wr.nicolike.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://by.gzmigu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://pu.hahajie.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://op.huixiangedu.cn

Ruby: File.write("a.txt", "hi")
来源：http://no.huixinmuqiang.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ij.nszjky.cn

[F04] 追加写入文件
来源：http://tc.shxzskj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://sp.nszjky.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qn.colortex.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yz.hnjuh.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pi.jianghongdianzi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ux.muxihuayi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mx.hahajie.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dt.gzmigu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://oj.huixinmuqiang.cn

[F05] 判断文件或目录是否存在
来源：http://pc.9csxet.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://re.bjjhwx.cn

PHP:  file_exists("a.txt");
来源：http://gd.jctech888.com.cn

JS:   fs.existsSync("a.txt")
来源：http://do.huanxung.cn


<!-- 参考信息 -->