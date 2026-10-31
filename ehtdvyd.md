代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://ww.huanxung.cn

JS:   arr.includes(x)
来源：http://sw.jianghongdianzi.cn

TS:   arr.includes(x)
来源：http://vc.asd995.cn

Java: list.contains(x)
来源：http://oe.yuexingan06.cn

Go:   slices.Contains(arr, x)
来源：http://wm.bookmarksfly.cn

Ruby: arr.include?(x)
来源：http://ot.wgjwhj.cn

C#:   list.Contains(x)
来源：http://iw.newstarts.cn

[D22] 复制数组（避免共享引用）
来源：http://id.szxytkj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ke.nicolike.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rq.shxzukj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qw.panjiajie.cn

TS:   [...arr];
来源：http://ub.gzmigu.cn

Java: new ArrayList<>(list);
来源：http://cf.newstarts.cn

Go:   copied := append([]int(nil), arr...)
来源：http://rl.muxihuayi.cn

Ruby: arr.dup;  arr.clone
来源：http://is.yuexingan06.cn

C#:   new List<int>(list);
来源：http://hp.panjiajie.cn

[D23] reduce 累积计算
来源：http://dh.huixiangedu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bx.bookmarksfly.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vb.huixiangedu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gk.9csxet.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ak.gzmigu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://af.nicolike.cn

Go:   // 手写循环
来源：http://tl.521024.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vf.colortex.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://us.asd995.cn

[D24] 字典 / Map 基本操作
来源：http://pc.wgjwhj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hi.gzmigu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://sj.huixinmuqiang.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://pi.9csxet.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://np.nicolike.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://kx.bjjhwx.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://eu.szsharing.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qe.shxzskj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pb.wgjwhj.cn

[D25] Set 集合去重与交并差
来源：http://ea.gzmigu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ph.shtwfgs.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tv.bjjhwx.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bp.nicolike.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://lc.hahajie.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://li.lnxyls.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wm.huanxung.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://px.gzmigu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://yj.szsharing.cn

[D26] 数组转字符串
来源：http://oo.newstarts.cn

Py:   ", ".join(map(str, arr))
来源：http://rf.yuexingan06.cn

PHP:  implode(", ", $arr);
来源：http://dg.yuntaijiaju.cn

JS:   arr.join(", ")
来源：http://kv.9csxet.cn

TS:   arr.join(", ")
来源：http://nu.colortex.cn

Java: String.join(", ", list)
来源：http://te.shxzskj.cn

Go:   strings.Join(strs, ", ")
来源：http://xh.lnxyls.cn

Ruby: arr.join(", ")
来源：http://rw.nicolike.cn

C#:   string.Join(", ", list)
来源：http://nf.521024.cn

================================================================================
来源：http://bn.huanxung.cn

E. 字符串处理
来源：http://cs.panjiajie.cn

================================================================================
来源：http://vh.hnjuh.cn

[E01] 拼接字符串
来源：http://bn.shtwfgs.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://do.9csxet.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zv.shtwfgs.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wd.jctech888.com.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://bb.gzmigu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wv.nszjky.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hn.9csxet.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gi.9csxet.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://by.asd995.cn

[E02] 重复字符串
来源：http://dk.nicolike.cn

Py:   "ab" * 3
来源：http://nk.yuexingan06.cn

PHP:  str_repeat("ab", 3);
来源：http://xs.muxihuayi.cn

JS:   "ab".repeat(3)
来源：http://xu.wgjwhj.cn

TS:   "ab".repeat(3)
来源：http://lq.szsharing.cn

Java: "ab".repeat(3)
来源：http://qd.hnjuh.cn

Go:   strings.Repeat("ab", 3)
来源：http://px.shtwfgs.cn

Ruby: "ab" * 3
来源：http://sd.colortex.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ia.521024.cn

[E03] 截取子串
来源：http://mu.bookmarksfly.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://fs.szsharing.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fj.huixinmuqiang.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fv.yuntaijiaju.cn

TS:   s.slice(1, 4)
来源：http://br.hnjuh.cn

Java: s.substring(1, 4)
来源：http://rl.hnjuh.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://yq.lnxyls.cn

Ruby: s[1, 3];  s[1..3]
来源：http://wg.shtwfgs.cn

C#:   s.Substring(1, 3)
来源：http://cv.huixinmuqiang.cn

[E04] 查找子串位置
来源：http://pc.huixiangedu.cn

Py:   s.find("x");  s.index("x")
来源：http://gp.colortex.cn

PHP:  strpos($s, "x");
来源：http://jw.wgjwhj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://dy.hahajie.cn

TS:   s.indexOf("x")
来源：http://kg.521024.cn

Java: s.indexOf("x")
来源：http://xt.nszjky.cn

Go:   strings.Index(s, "x")
来源：http://vs.9csxet.cn

Ruby: s.index("x")
来源：http://lw.shxzukj.cn

C#:   s.IndexOf("x")
来源：http://sq.huixiangedu.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://bt.haigaiapp.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://af.chemitech.net.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://tn.yuntaijiaju.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ot.wgjwhj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://sg.huanxung.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tz.nszjky.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mr.shtwfgs.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://kr.jctech888.com.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://un.shtwfgs.cn

[E06] 替换子串
来源：http://xj.9csxet.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://cs.jctech888.com.cn

PHP:  str_replace("a", "b", $s);
来源：http://su.nicolike.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rz.huanxung.cn

TS:   s.replaceAll("a", "b")
来源：http://np.gzmigu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://im.chemitech.net.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://uj.wgjwhj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fd.lnxyls.cn

C#:   s.Replace("a", "b")
来源：http://rv.szsharing.cn

[E07] 按分隔符拆分
来源：http://qi.lnxyls.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bi.haigaiapp.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://oh.9csxet.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://lc.shtwfgs.cn

TS:   s.split(",")
来源：http://lq.muxihuayi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ny.wgjwhj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rn.szsharing.cn

Ruby: s.split(",");  s.split
来源：http://ip.shxzskj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wf.colortex.cn

[E08] 数组按分隔符合并
来源：http://ic.wgjwhj.cn

Py:   ",".join(items)
来源：http://un.panjiajie.cn

PHP:  implode(",", $items);
来源：http://vg.szsharing.cn

JS:   items.join(",")
来源：http://re.haigaiapp.cn

TS:   items.join(",")
来源：http://qo.nicolike.cn

Java: String.join(",", items)
来源：http://xm.hnjuh.cn

Go:   strings.Join(items, ",")
来源：http://sa.nszjky.cn

Ruby: items.join(",")
来源：http://xy.newstarts.cn

C#:   string.Join(",", items)
来源：http://jc.jctech888.com.cn

[E09] 去除所有空白字符
来源：http://pf.szxytkj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xy.colortex.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zj.yuexingan06.cn

JS:   s.replace(/\s+/g, "")
来源：http://sf.wgjwhj.cn

TS:   s.replace(/\s+/g, "")
来源：http://fb.gzmigu.cn

Java: s.replaceAll("\\s+", "")
来源：http://st.szsharing.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://lk.521024.cn

Ruby: s.gsub(/\s+/, "")
来源：http://qt.jctech888.com.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ax.wgjwhj.cn

[E10] 左侧补零 / 定长填充
来源：http://en.shtwfgs.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fe.szxytkj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fg.yuntaijiaju.cn

JS:   "7".padStart(3, "0")
来源：http://le.huanxung.cn

TS:   "7".padStart(3, "0")
来源：http://nw.huixiangedu.cn

Java: String.format("%03d", 7)
来源：http://ro.huixiangedu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ls.wgjwhj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://tw.yuntaijiaju.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hb.haigaiapp.cn

[E11] 反转字符串
来源：http://aa.lnxyls.cn

Py:   s[::-1]
来源：http://xi.jianghongdianzi.cn

PHP:  strrev($s);
来源：http://pm.shtwfgs.cn

JS:   [...s].reverse().join("")
来源：http://sn.colortex.cn

TS:   [...s].reverse().join("")
来源：http://gk.hnjuh.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ep.9csxet.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://kw.gzmigu.cn

Ruby: s.reverse
来源：http://ar.wgjwhj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://hy.shxzskj.cn

[E12] 统计某字符出现次数
来源：http://dq.nicolike.cn

Py:   s.count("a")
来源：http://na.hahajie.cn

PHP:  substr_count($s, "a");
来源：http://gb.9csxet.cn

JS:   s.split("a").length - 1
来源：http://hn.muxihuayi.cn

TS:   s.split("a").length - 1
来源：http://tz.haigaiapp.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://cn.shtwfgs.cn

Go:   strings.Count(s, "a")
来源：http://wm.chemitech.net.cn

Ruby: s.count("a")
来源：http://qa.nszjky.cn

C#:   s.Count(c => c == 'a')
来源：http://uv.szxytkj.cn

[E13] 逐字符遍历
来源：http://uy.521024.cn

Py:   for ch in s: print(ch)
来源：http://ku.huixinmuqiang.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://md.nicolike.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://of.jctech888.com.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://mh.gzmigu.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wn.nicolike.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zb.chemitech.net.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://dx.521024.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ih.huixinmuqiang.cn

[E14] URL 编码与 Base64
来源：http://pa.hahajie.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://em.chemitech.net.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ja.asd995.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wh.521024.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zm.asd995.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qe.huanxung.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wc.yuntaijiaju.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://yq.hahajie.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qd.panjiajie.cn

[E15] HTML 转义 / 反转义
来源：http://yi.9csxet.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://mf.lnxyls.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jx.huixiangedu.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rr.hnjuh.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://zs.szxytkj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://uv.yuexingan06.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ga.chemitech.net.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cv.szsharing.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jk.nicolike.cn

[E16] 数字千分位
来源：http://lz.huixiangedu.cn

Py:   f"{1234567:,}"
来源：http://oe.hahajie.cn

PHP:  number_format(1234567);
来源：http://dc.huixiangedu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://tt.panjiajie.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://sd.521024.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://uy.hnjuh.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://pf.muxihuayi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ve.haigaiapp.cn

C#:   1234567.ToString("N0")
来源：http://pl.haigaiapp.cn

[E17] 首字母大写
来源：http://oi.asd995.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ue.huixiangedu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://yx.chemitech.net.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fb.asd995.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sv.asd995.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nl.lnxyls.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://yz.lnxyls.cn

Ruby: s.capitalize
来源：http://mc.521024.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://bm.bjjhwx.cn

[E18] 模板占位符替换
来源：http://vh.521024.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://dd.9csxet.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://cr.newstarts.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://za.yuexingan06.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://hx.bookmarksfly.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pz.chemitech.net.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zs.yuntaijiaju.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vs.huixinmuqiang.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qw.gzmigu.cn

[E19] 多行文本按行拆分
来源：http://az.lnxyls.cn

Py:   s.splitlines()
来源：http://ek.jianghongdianzi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ef.shxzukj.cn

JS:   s.split(/\r?\n/)
来源：http://mk.huixinmuqiang.cn

TS:   s.split(/\r?\n/)
来源：http://bw.yuntaijiaju.cn

Java: s.lines().toList()
来源：http://ac.szsharing.cn

Go:   strings.Split(s, "\n")
来源：http://cp.jianghongdianzi.cn

Ruby: s.lines
来源：http://gk.shxzukj.cn

C#:   s.Split('\n')
来源：http://yl.gzmigu.cn

[E20] 判断字符串是否为空
来源：http://mh.shtwfgs.cn

Py:   if not s:
来源：http://xi.yuexingan06.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ff.gzmigu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kw.jianghongdianzi.cn

TS:   if (s === "") {}
来源：http://ax.gzmigu.cn

Java: if (s.isEmpty()) {}
来源：http://sx.colortex.cn

Go:   if s == "" {}
来源：http://cl.nszjky.cn

Ruby: if s.empty?
来源：http://oh.hahajie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xf.nicolike.cn

[E21] 超长截断加省略号
来源：http://vx.shtwfgs.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://od.asd995.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zd.wgjwhj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://do.9csxet.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dk.colortex.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://et.szxytkj.cn

Go:   // 按 rune 判断长度后截断
来源：http://eo.gzmigu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://an.nicolike.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://im.jctech888.com.cn

[E22] 字节长度与字符长度
来源：http://yx.haigaiapp.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://dy.szxytkj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rj.bookmarksfly.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qh.jianghongdianzi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gb.jianghongdianzi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://oz.huixiangedu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.huanxung.cn

Ruby: s.bytesize;  s.length
来源：http://yq.shtwfgs.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ht.colortex.cn

================================================================================
来源：http://oj.huanxung.cn

F. 文件与目录
来源：http://gf.huanxung.cn

================================================================================
来源：http://ci.shxzskj.cn

[F01] 读取整个文件
来源：http://sb.asd995.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://bs.hahajie.cn

PHP:  file_get_contents("a.txt");
来源：http://jp.9csxet.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hr.szsharing.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://kv.muxihuayi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://cs.521024.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ps.shtwfgs.cn

Ruby: File.read("a.txt")
来源：http://dj.colortex.cn

C#:   File.ReadAllText("a.txt");
来源：http://ty.asd995.cn

[F02] 逐行读取文件
来源：http://rk.szsharing.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xu.szxytkj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ns.szxytkj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qy.panjiajie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yy.chemitech.net.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gl.panjiajie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ln.muxihuayi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hf.panjiajie.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ip.hnjuh.cn

[F03] 写入文件（覆盖）
来源：http://mm.huixinmuqiang.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://np.colortex.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ko.bjjhwx.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jc.shxzskj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mq.shtwfgs.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bo.shtwfgs.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bu.shxzskj.cn

Ruby: File.write("a.txt", "hi")
来源：http://jl.shxzukj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://pe.bookmarksfly.cn

[F04] 追加写入文件
来源：http://wf.yuntaijiaju.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://cb.521024.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jf.shxzskj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yr.huixiangedu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tl.huanxung.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xd.newstarts.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jo.nszjky.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jc.panjiajie.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ns.wgjwhj.cn

[F05] 判断文件或目录是否存在
来源：http://og.nszjky.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ul.bookmarksfly.cn

PHP:  file_exists("a.txt");
来源：http://we.hnjuh.cn

JS:   fs.existsSync("a.txt")
来源：http://fd.huixiangedu.cn

TS:   fs.existsSync("a.txt")
来源：http://dj.muxihuayi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://se.shxzskj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://eh.shxzskj.cn

Ruby: File.exist?("a.txt")
来源：http://dw.521024.cn


<!-- 参考信息 -->