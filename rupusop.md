代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://js.chemitech.net.cn

Ruby: arr.include?(x)
来源：http://kk.hnjuh.cn

C#:   list.Contains(x)
来源：http://tm.panjiajie.cn

[D22] 复制数组（避免共享引用）
来源：http://ko.muxihuayi.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zn.newstarts.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ap.asd995.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rk.asd995.cn

TS:   [...arr];
来源：http://dz.wgjwhj.cn

Java: new ArrayList<>(list);
来源：http://pr.hnjuh.cn

Go:   copied := append([]int(nil), arr...)
来源：http://zk.9csxet.cn

Ruby: arr.dup;  arr.clone
来源：http://wz.asd995.cn

C#:   new List<int>(list);
来源：http://df.yuntaijiaju.cn

[D23] reduce 累积计算
来源：http://an.muxihuayi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://dt.szxytkj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gl.521024.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ck.shxzukj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ll.huixinmuqiang.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://pp.panjiajie.cn

Go:   // 手写循环
来源：http://rb.bjjhwx.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qn.muxihuayi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://vx.asd995.cn

[D24] 字典 / Map 基本操作
来源：http://oe.colortex.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pq.yuexingan06.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://nd.shtwfgs.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fo.bookmarksfly.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://na.hnjuh.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://uh.hnjuh.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ey.bookmarksfly.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gn.shxzukj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ay.shxzukj.cn

[D25] Set 集合去重与交并差
来源：http://as.haigaiapp.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tq.nicolike.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://yf.hnjuh.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://nr.shxzukj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bv.huixinmuqiang.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://fw.shxzukj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://dr.lnxyls.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ip.huixinmuqiang.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vg.muxihuayi.cn

[D26] 数组转字符串
来源：http://zc.521024.cn

Py:   ", ".join(map(str, arr))
来源：http://qn.shxzskj.cn

PHP:  implode(", ", $arr);
来源：http://ol.9csxet.cn

JS:   arr.join(", ")
来源：http://zz.huixiangedu.cn

TS:   arr.join(", ")
来源：http://jh.bjjhwx.cn

Java: String.join(", ", list)
来源：http://kp.muxihuayi.cn

Go:   strings.Join(strs, ", ")
来源：http://op.huanxung.cn

Ruby: arr.join(", ")
来源：http://ky.asd995.cn

C#:   string.Join(", ", list)
来源：http://ci.9csxet.cn

================================================================================
来源：http://lo.hnjuh.cn

E. 字符串处理
来源：http://ly.shtwfgs.cn

================================================================================
来源：http://oq.9csxet.cn

[E01] 拼接字符串
来源：http://ha.shxzukj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fh.haigaiapp.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://px.haigaiapp.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gj.jctech888.com.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hl.lnxyls.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://jf.shxzukj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://cj.521024.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://nc.szxytkj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ek.9csxet.cn

[E02] 重复字符串
来源：http://lb.colortex.cn

Py:   "ab" * 3
来源：http://wc.huixiangedu.cn

PHP:  str_repeat("ab", 3);
来源：http://fm.huixinmuqiang.cn

JS:   "ab".repeat(3)
来源：http://rk.yuexingan06.cn

TS:   "ab".repeat(3)
来源：http://gq.gzmigu.cn

Java: "ab".repeat(3)
来源：http://km.muxihuayi.cn

Go:   strings.Repeat("ab", 3)
来源：http://ds.shxzukj.cn

Ruby: "ab" * 3
来源：http://ut.huixinmuqiang.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://iq.shtwfgs.cn

[E03] 截取子串
来源：http://ar.chemitech.net.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cf.colortex.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fr.nszjky.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ky.nicolike.cn

TS:   s.slice(1, 4)
来源：http://cz.bookmarksfly.cn

Java: s.substring(1, 4)
来源：http://lm.hahajie.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jj.jctech888.com.cn

Ruby: s[1, 3];  s[1..3]
来源：http://es.lnxyls.cn

C#:   s.Substring(1, 3)
来源：http://gi.hahajie.cn

[E04] 查找子串位置
来源：http://wc.jctech888.com.cn

Py:   s.find("x");  s.index("x")
来源：http://lr.shxzukj.cn

PHP:  strpos($s, "x");
来源：http://wl.gzmigu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mi.huixinmuqiang.cn

TS:   s.indexOf("x")
来源：http://st.bookmarksfly.cn

Java: s.indexOf("x")
来源：http://vg.panjiajie.cn

Go:   strings.Index(s, "x")
来源：http://oh.jianghongdianzi.cn

Ruby: s.index("x")
来源：http://xo.szsharing.cn

C#:   s.IndexOf("x")
来源：http://cd.yuexingan06.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://eu.huanxung.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zi.szxytkj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vw.wgjwhj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lz.huixiangedu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://cc.lnxyls.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cq.jianghongdianzi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pv.nicolike.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lf.nicolike.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://be.hnjuh.cn

[E06] 替换子串
来源：http://hy.newstarts.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ox.panjiajie.cn

PHP:  str_replace("a", "b", $s);
来源：http://oi.shtwfgs.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pl.muxihuayi.cn

TS:   s.replaceAll("a", "b")
来源：http://yd.huanxung.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fv.bookmarksfly.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wu.panjiajie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vh.asd995.cn

C#:   s.Replace("a", "b")
来源：http://yb.huixiangedu.cn

[E07] 按分隔符拆分
来源：http://ke.jianghongdianzi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ck.colortex.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mv.yuexingan06.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://qv.bookmarksfly.cn

TS:   s.split(",")
来源：http://pb.gzmigu.cn

Java: s.split(",");  s.split("\\s+")
来源：http://mm.muxihuayi.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pt.shxzskj.cn

Ruby: s.split(",");  s.split
来源：http://rl.shxzukj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lj.shtwfgs.cn

[E08] 数组按分隔符合并
来源：http://zs.szxytkj.cn

Py:   ",".join(items)
来源：http://pq.haigaiapp.cn

PHP:  implode(",", $items);
来源：http://ic.bookmarksfly.cn

JS:   items.join(",")
来源：http://fx.huixinmuqiang.cn

TS:   items.join(",")
来源：http://vw.521024.cn

Java: String.join(",", items)
来源：http://eg.521024.cn

Go:   strings.Join(items, ",")
来源：http://mc.huixinmuqiang.cn

Ruby: items.join(",")
来源：http://wx.shxzukj.cn

C#:   string.Join(",", items)
来源：http://nb.lnxyls.cn

[E09] 去除所有空白字符
来源：http://fx.muxihuayi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ml.9csxet.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ug.bookmarksfly.cn

JS:   s.replace(/\s+/g, "")
来源：http://ct.shxzukj.cn

TS:   s.replace(/\s+/g, "")
来源：http://xv.lnxyls.cn

Java: s.replaceAll("\\s+", "")
来源：http://jv.nicolike.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://wu.nszjky.cn

Ruby: s.gsub(/\s+/, "")
来源：http://xj.shxzukj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ha.yuexingan06.cn

[E10] 左侧补零 / 定长填充
来源：http://vd.wgjwhj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ev.bjjhwx.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://yf.bookmarksfly.cn

JS:   "7".padStart(3, "0")
来源：http://kx.shtwfgs.cn

TS:   "7".padStart(3, "0")
来源：http://sf.bjjhwx.cn

Java: String.format("%03d", 7)
来源：http://ib.szxytkj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://uw.newstarts.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ee.huanxung.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hv.muxihuayi.cn

[E11] 反转字符串
来源：http://bj.huanxung.cn

Py:   s[::-1]
来源：http://fw.lnxyls.cn

PHP:  strrev($s);
来源：http://hi.shxzskj.cn

JS:   [...s].reverse().join("")
来源：http://tx.shxzukj.cn

TS:   [...s].reverse().join("")
来源：http://xi.hnjuh.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://gg.lnxyls.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://zr.huanxung.cn

Ruby: s.reverse
来源：http://up.wgjwhj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://kf.yuexingan06.cn

[E12] 统计某字符出现次数
来源：http://ai.jianghongdianzi.cn

Py:   s.count("a")
来源：http://gw.521024.cn

PHP:  substr_count($s, "a");
来源：http://ak.nszjky.cn

JS:   s.split("a").length - 1
来源：http://lx.521024.cn

TS:   s.split("a").length - 1
来源：http://bi.hahajie.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xz.521024.cn

Go:   strings.Count(s, "a")
来源：http://zg.colortex.cn

Ruby: s.count("a")
来源：http://dh.colortex.cn

C#:   s.Count(c => c == 'a')
来源：http://ud.bjjhwx.cn

[E13] 逐字符遍历
来源：http://zx.asd995.cn

Py:   for ch in s: print(ch)
来源：http://fu.colortex.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://nn.huanxung.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://tm.shtwfgs.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://wj.newstarts.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ni.521024.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gf.newstarts.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://sv.nicolike.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hh.colortex.cn

[E14] URL 编码与 Base64
来源：http://ob.panjiajie.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hk.yuntaijiaju.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://lx.chemitech.net.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kh.huanxung.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vo.shxzukj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://dk.bjjhwx.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fm.nicolike.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kw.bjjhwx.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bd.yuntaijiaju.cn

[E15] HTML 转义 / 反转义
来源：http://or.wgjwhj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://zs.huixinmuqiang.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zg.huanxung.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xz.yuexingan06.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ic.muxihuayi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zh.haigaiapp.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://pz.colortex.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xd.jctech888.com.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lk.shxzukj.cn

[E16] 数字千分位
来源：http://wn.panjiajie.cn

Py:   f"{1234567:,}"
来源：http://bt.panjiajie.cn

PHP:  number_format(1234567);
来源：http://tj.newstarts.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://sa.chemitech.net.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://zx.szxytkj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vg.haigaiapp.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://dy.lnxyls.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mq.chemitech.net.cn

C#:   1234567.ToString("N0")
来源：http://ut.gzmigu.cn

[E17] 首字母大写
来源：http://xf.newstarts.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fa.shxzukj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://yz.asd995.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kn.newstarts.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vv.yuexingan06.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xe.nszjky.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://di.hnjuh.cn

Ruby: s.capitalize
来源：http://jw.haigaiapp.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://sh.9csxet.cn

[E18] 模板占位符替换
来源：http://dx.shxzskj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ky.chemitech.net.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jp.shxzukj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://pi.shxzukj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://hh.jianghongdianzi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qc.muxihuayi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hw.haigaiapp.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://tn.yuntaijiaju.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://oi.huixinmuqiang.cn

[E19] 多行文本按行拆分
来源：http://vr.nicolike.cn

Py:   s.splitlines()
来源：http://ul.hahajie.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://lp.yuntaijiaju.cn

JS:   s.split(/\r?\n/)
来源：http://ed.panjiajie.cn

TS:   s.split(/\r?\n/)
来源：http://vj.newstarts.cn

Java: s.lines().toList()
来源：http://ky.shxzukj.cn

Go:   strings.Split(s, "\n")
来源：http://fk.jianghongdianzi.cn

Ruby: s.lines
来源：http://zy.huanxung.cn

C#:   s.Split('\n')
来源：http://ek.newstarts.cn

[E20] 判断字符串是否为空
来源：http://un.newstarts.cn

Py:   if not s:
来源：http://qg.gzmigu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://de.nszjky.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ob.huanxung.cn

TS:   if (s === "") {}
来源：http://da.chemitech.net.cn

Java: if (s.isEmpty()) {}
来源：http://gl.colortex.cn

Go:   if s == "" {}
来源：http://zu.huixiangedu.cn

Ruby: if s.empty?
来源：http://fa.huanxung.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://si.wgjwhj.cn

[E21] 超长截断加省略号
来源：http://qt.newstarts.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://aq.9csxet.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xu.colortex.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yv.hahajie.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mk.521024.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dq.shxzskj.cn

Go:   // 按 rune 判断长度后截断
来源：http://yi.bookmarksfly.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://du.wgjwhj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tl.yuntaijiaju.cn

[E22] 字节长度与字符长度
来源：http://qc.jctech888.com.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ib.huixiangedu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bd.hahajie.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://je.colortex.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hr.chemitech.net.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://uj.newstarts.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ov.colortex.cn

Ruby: s.bytesize;  s.length
来源：http://hm.chemitech.net.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://rt.colortex.cn

================================================================================
来源：http://eq.bjjhwx.cn

F. 文件与目录
来源：http://hd.nicolike.cn

================================================================================
来源：http://in.yuntaijiaju.cn

[F01] 读取整个文件
来源：http://xz.hahajie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://sy.jianghongdianzi.cn

PHP:  file_get_contents("a.txt");
来源：http://qz.9csxet.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://pd.shxzukj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://cs.9csxet.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://en.bjjhwx.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://lz.huixiangedu.cn

Ruby: File.read("a.txt")
来源：http://fj.nszjky.cn

C#:   File.ReadAllText("a.txt");
来源：http://gh.huixinmuqiang.cn

[F02] 逐行读取文件
来源：http://bz.asd995.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jc.haigaiapp.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hm.asd995.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mc.panjiajie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zw.hnjuh.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://na.chemitech.net.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gs.nszjky.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vi.lnxyls.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zp.asd995.cn

[F03] 写入文件（覆盖）
来源：http://yx.hnjuh.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jr.gzmigu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://mu.haigaiapp.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ce.shtwfgs.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rm.hnjuh.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fe.nicolike.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://yp.shxzukj.cn

Ruby: File.write("a.txt", "hi")
来源：http://zm.shtwfgs.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://af.haigaiapp.cn

[F04] 追加写入文件
来源：http://br.shtwfgs.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ir.huixinmuqiang.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://eg.shxzukj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kl.521024.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lf.521024.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://cu.colortex.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kx.jctech888.com.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vm.nszjky.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://nf.newstarts.cn

[F05] 判断文件或目录是否存在
来源：http://ir.nszjky.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dc.yuexingan06.cn

PHP:  file_exists("a.txt");
来源：http://yp.wgjwhj.cn

JS:   fs.existsSync("a.txt")
来源：http://zh.bjjhwx.cn

TS:   fs.existsSync("a.txt")
来源：http://vl.muxihuayi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://oi.gzmigu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ul.huanxung.cn

Ruby: File.exist?("a.txt")
来源：http://sr.huixinmuqiang.cn

C#:   File.Exists("a.txt")
来源：http://kh.jianghongdianzi.cn

[F06] 删除文件
来源：http://ru.shxzukj.cn

Py:   os.remove("a.txt")
来源：http://ma.newstarts.cn

PHP:  unlink("a.txt");
来源：http://el.hahajie.cn


<!-- 参考信息 -->