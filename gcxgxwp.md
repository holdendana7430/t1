代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://kg.jianghongdianzi.cn

JS:   arr.includes(x)
来源：http://kc.wgjwhj.cn

TS:   arr.includes(x)
来源：http://sg.colortex.cn

Java: list.contains(x)
来源：http://ni.szsharing.cn

Go:   slices.Contains(arr, x)
来源：http://wi.asd995.cn

Ruby: arr.include?(x)
来源：http://tl.colortex.cn

C#:   list.Contains(x)
来源：http://sd.shxzukj.cn

[D22] 复制数组（避免共享引用）
来源：http://us.gzmigu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gx.bookmarksfly.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://np.nszjky.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jx.nszjky.cn

TS:   [...arr];
来源：http://pt.huixiangedu.cn

Java: new ArrayList<>(list);
来源：http://nz.9csxet.cn

Go:   copied := append([]int(nil), arr...)
来源：http://vm.hnjuh.cn

Ruby: arr.dup;  arr.clone
来源：http://cn.haigaiapp.cn

C#:   new List<int>(list);
来源：http://ya.jianghongdianzi.cn

[D23] reduce 累积计算
来源：http://iy.szxytkj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://kv.shxzskj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://by.hnjuh.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hq.huanxung.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://er.nicolike.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://zh.521024.cn

Go:   // 手写循环
来源：http://tz.colortex.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dm.huixiangedu.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wh.chemitech.net.cn

[D24] 字典 / Map 基本操作
来源：http://kl.shxzukj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gt.521024.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ro.panjiajie.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kd.jctech888.com.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://pd.bjjhwx.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lz.haigaiapp.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ax.shtwfgs.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ga.shxzskj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ln.yuexingan06.cn

[D25] Set 集合去重与交并差
来源：http://jn.shxzukj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mm.shxzukj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://sb.szsharing.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ie.szsharing.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://nr.szsharing.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vx.szxytkj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ll.asd995.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://lr.huanxung.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ss.hnjuh.cn

[D26] 数组转字符串
来源：http://ex.bookmarksfly.cn

Py:   ", ".join(map(str, arr))
来源：http://pr.hahajie.cn

PHP:  implode(", ", $arr);
来源：http://xt.huixinmuqiang.cn

JS:   arr.join(", ")
来源：http://fp.yuexingan06.cn

TS:   arr.join(", ")
来源：http://do.yuntaijiaju.cn

Java: String.join(", ", list)
来源：http://hf.wgjwhj.cn

Go:   strings.Join(strs, ", ")
来源：http://gb.haigaiapp.cn

Ruby: arr.join(", ")
来源：http://px.colortex.cn

C#:   string.Join(", ", list)
来源：http://ag.jianghongdianzi.cn

================================================================================
来源：http://wq.bookmarksfly.cn

E. 字符串处理
来源：http://gh.panjiajie.cn

================================================================================
来源：http://kp.muxihuayi.cn

[E01] 拼接字符串
来源：http://su.muxihuayi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.nszjky.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tx.szxytkj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hs.yuntaijiaju.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dk.szxytkj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://km.asd995.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ms.wgjwhj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ep.colortex.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://sg.9csxet.cn

[E02] 重复字符串
来源：http://dr.jianghongdianzi.cn

Py:   "ab" * 3
来源：http://ym.huixiangedu.cn

PHP:  str_repeat("ab", 3);
来源：http://pq.newstarts.cn

JS:   "ab".repeat(3)
来源：http://pn.shxzukj.cn

TS:   "ab".repeat(3)
来源：http://hu.huixiangedu.cn

Java: "ab".repeat(3)
来源：http://xh.colortex.cn

Go:   strings.Repeat("ab", 3)
来源：http://ys.szsharing.cn

Ruby: "ab" * 3
来源：http://fc.bookmarksfly.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://uu.szxytkj.cn

[E03] 截取子串
来源：http://sr.huixinmuqiang.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zu.lnxyls.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vu.lnxyls.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yn.panjiajie.cn

TS:   s.slice(1, 4)
来源：http://oy.huixinmuqiang.cn

Java: s.substring(1, 4)
来源：http://rs.bjjhwx.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gd.szxytkj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://pv.szsharing.cn

C#:   s.Substring(1, 3)
来源：http://gg.hahajie.cn

[E04] 查找子串位置
来源：http://qj.bookmarksfly.cn

Py:   s.find("x");  s.index("x")
来源：http://ih.wgjwhj.cn

PHP:  strpos($s, "x");
来源：http://uk.panjiajie.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vu.nszjky.cn

TS:   s.indexOf("x")
来源：http://jz.yuntaijiaju.cn

Java: s.indexOf("x")
来源：http://qz.nszjky.cn

Go:   strings.Index(s, "x")
来源：http://ko.lnxyls.cn

Ruby: s.index("x")
来源：http://ov.yuexingan06.cn

C#:   s.IndexOf("x")
来源：http://tx.asd995.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://zc.muxihuayi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ff.haigaiapp.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ax.shxzskj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ek.9csxet.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://wj.gzmigu.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rw.hnjuh.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://of.szxytkj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qf.hahajie.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://od.jianghongdianzi.cn

[E06] 替换子串
来源：http://vm.yuntaijiaju.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://iq.gzmigu.cn

PHP:  str_replace("a", "b", $s);
来源：http://bu.bjjhwx.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://md.shtwfgs.cn

TS:   s.replaceAll("a", "b")
来源：http://vw.yuexingan06.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ag.szxytkj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qg.lnxyls.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://tx.lnxyls.cn

C#:   s.Replace("a", "b")
来源：http://yp.colortex.cn

[E07] 按分隔符拆分
来源：http://hy.asd995.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zj.shtwfgs.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://av.muxihuayi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://wf.asd995.cn

TS:   s.split(",")
来源：http://uu.521024.cn

Java: s.split(",");  s.split("\\s+")
来源：http://md.huanxung.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xe.shxzskj.cn

Ruby: s.split(",");  s.split
来源：http://zm.lnxyls.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jz.panjiajie.cn

[E08] 数组按分隔符合并
来源：http://zy.huixinmuqiang.cn

Py:   ",".join(items)
来源：http://hk.szsharing.cn

PHP:  implode(",", $items);
来源：http://ba.nicolike.cn

JS:   items.join(",")
来源：http://ya.shxzukj.cn

TS:   items.join(",")
来源：http://id.wgjwhj.cn

Java: String.join(",", items)
来源：http://jq.bookmarksfly.cn

Go:   strings.Join(items, ",")
来源：http://tc.nicolike.cn

Ruby: items.join(",")
来源：http://xo.hahajie.cn

C#:   string.Join(",", items)
来源：http://ek.521024.cn

[E09] 去除所有空白字符
来源：http://yz.panjiajie.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://py.nicolike.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vo.huanxung.cn

JS:   s.replace(/\s+/g, "")
来源：http://eq.szxytkj.cn

TS:   s.replace(/\s+/g, "")
来源：http://fl.wgjwhj.cn

Java: s.replaceAll("\\s+", "")
来源：http://ut.hahajie.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ln.wgjwhj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://tz.muxihuayi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fb.bjjhwx.cn

[E10] 左侧补零 / 定长填充
来源：http://uz.wgjwhj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fu.hahajie.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ko.nicolike.cn

JS:   "7".padStart(3, "0")
来源：http://ia.bookmarksfly.cn

TS:   "7".padStart(3, "0")
来源：http://uq.521024.cn

Java: String.format("%03d", 7)
来源：http://ng.hahajie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://go.gzmigu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jz.bjjhwx.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://le.szsharing.cn

[E11] 反转字符串
来源：http://ok.shxzukj.cn

Py:   s[::-1]
来源：http://oq.asd995.cn

PHP:  strrev($s);
来源：http://yq.yuexingan06.cn

JS:   [...s].reverse().join("")
来源：http://mh.wgjwhj.cn

TS:   [...s].reverse().join("")
来源：http://al.521024.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://kf.shtwfgs.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://bx.yuexingan06.cn

Ruby: s.reverse
来源：http://vq.colortex.cn

C#:   new string(s.Reverse().ToArray())
来源：http://uu.yuexingan06.cn

[E12] 统计某字符出现次数
来源：http://sv.jianghongdianzi.cn

Py:   s.count("a")
来源：http://gp.nszjky.cn

PHP:  substr_count($s, "a");
来源：http://jc.bookmarksfly.cn

JS:   s.split("a").length - 1
来源：http://yv.9csxet.cn

TS:   s.split("a").length - 1
来源：http://yz.shxzskj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ct.jctech888.com.cn

Go:   strings.Count(s, "a")
来源：http://kd.shtwfgs.cn

Ruby: s.count("a")
来源：http://su.shxzukj.cn

C#:   s.Count(c => c == 'a')
来源：http://un.huanxung.cn

[E13] 逐字符遍历
来源：http://mx.bookmarksfly.cn

Py:   for ch in s: print(ch)
来源：http://cs.bjjhwx.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://un.shxzskj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://cs.yuexingan06.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://wd.yuntaijiaju.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vo.muxihuayi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://yy.bookmarksfly.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ha.wgjwhj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ib.haigaiapp.cn

[E14] URL 编码与 Base64
来源：http://ae.asd995.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pd.jianghongdianzi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://yx.wgjwhj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ca.yuntaijiaju.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tj.yuntaijiaju.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vh.shtwfgs.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://nx.521024.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wh.gzmigu.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rl.huixiangedu.cn

[E15] HTML 转义 / 反转义
来源：http://ub.shtwfgs.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://qq.huixiangedu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://sx.gzmigu.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://it.hnjuh.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://cx.newstarts.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bc.colortex.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ak.chemitech.net.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ry.bookmarksfly.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fc.wgjwhj.cn

[E16] 数字千分位
来源：http://ra.chemitech.net.cn

Py:   f"{1234567:,}"
来源：http://dp.9csxet.cn

PHP:  number_format(1234567);
来源：http://ly.muxihuayi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://vi.asd995.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://em.lnxyls.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://dt.newstarts.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://pa.bjjhwx.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wi.colortex.cn

C#:   1234567.ToString("N0")
来源：http://hw.shtwfgs.cn

[E17] 首字母大写
来源：http://pg.hahajie.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xs.huixiangedu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://np.hnjuh.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gq.asd995.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://my.shtwfgs.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://pm.hnjuh.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://yt.jctech888.com.cn

Ruby: s.capitalize
来源：http://dp.huixiangedu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://am.wgjwhj.cn

[E18] 模板占位符替换
来源：http://pl.szxytkj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mr.gzmigu.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qs.colortex.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ki.yuntaijiaju.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://gq.asd995.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xc.bjjhwx.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ed.szsharing.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qm.bjjhwx.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://oj.haigaiapp.cn

[E19] 多行文本按行拆分
来源：http://pw.szsharing.cn

Py:   s.splitlines()
来源：http://iq.szxytkj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://oj.521024.cn

JS:   s.split(/\r?\n/)
来源：http://bx.huixinmuqiang.cn

TS:   s.split(/\r?\n/)
来源：http://mt.lnxyls.cn

Java: s.lines().toList()
来源：http://zp.yuexingan06.cn

Go:   strings.Split(s, "\n")
来源：http://qf.huixinmuqiang.cn

Ruby: s.lines
来源：http://pj.jctech888.com.cn

C#:   s.Split('\n')
来源：http://pc.colortex.cn

[E20] 判断字符串是否为空
来源：http://ir.bookmarksfly.cn

Py:   if not s:
来源：http://gp.gzmigu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ku.shxzukj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://sv.chemitech.net.cn

TS:   if (s === "") {}
来源：http://fa.colortex.cn

Java: if (s.isEmpty()) {}
来源：http://zl.colortex.cn

Go:   if s == "" {}
来源：http://gb.wgjwhj.cn

Ruby: if s.empty?
来源：http://uu.jianghongdianzi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://iy.colortex.cn

[E21] 超长截断加省略号
来源：http://kj.huixinmuqiang.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lj.hahajie.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://je.huixiangedu.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jo.jctech888.com.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yl.521024.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mg.haigaiapp.cn

Go:   // 按 rune 判断长度后截断
来源：http://vx.szxytkj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wi.szxytkj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://pr.jctech888.com.cn

[E22] 字节长度与字符长度
来源：http://gb.shtwfgs.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vs.szsharing.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://iu.muxihuayi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ut.bjjhwx.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ll.bookmarksfly.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ek.muxihuayi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ao.muxihuayi.cn

Ruby: s.bytesize;  s.length
来源：http://mg.huixiangedu.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ke.gzmigu.cn

================================================================================
来源：http://sl.gzmigu.cn

F. 文件与目录
来源：http://mt.shxzukj.cn

================================================================================
来源：http://mh.jianghongdianzi.cn

[F01] 读取整个文件
来源：http://gg.9csxet.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nv.9csxet.cn

PHP:  file_get_contents("a.txt");
来源：http://hi.yuexingan06.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://eo.hnjuh.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://cd.muxihuayi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://hb.shxzukj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://uz.shxzskj.cn

Ruby: File.read("a.txt")
来源：http://fq.panjiajie.cn

C#:   File.ReadAllText("a.txt");
来源：http://rx.521024.cn

[F02] 逐行读取文件
来源：http://ef.panjiajie.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ix.bjjhwx.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ku.bjjhwx.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dv.huanxung.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sl.hahajie.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bv.huixiangedu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ad.hnjuh.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bz.huixiangedu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://sy.lnxyls.cn

[F03] 写入文件（覆盖）
来源：http://bo.hahajie.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://up.jianghongdianzi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ba.hahajie.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hv.huanxung.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bb.jctech888.com.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fx.hahajie.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://oi.nicolike.cn

Ruby: File.write("a.txt", "hi")
来源：http://md.bjjhwx.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nf.panjiajie.cn

[F04] 追加写入文件
来源：http://qo.colortex.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tm.chemitech.net.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fb.hnjuh.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zr.huixinmuqiang.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lr.gzmigu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lz.muxihuayi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zd.panjiajie.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fv.huixinmuqiang.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jf.bjjhwx.cn

[F05] 判断文件或目录是否存在
来源：http://ed.hahajie.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xu.chemitech.net.cn

PHP:  file_exists("a.txt");
来源：http://am.yuntaijiaju.cn

JS:   fs.existsSync("a.txt")
来源：http://yx.shxzskj.cn

TS:   fs.existsSync("a.txt")
来源：http://ef.yuexingan06.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://bm.yuexingan06.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pn.shtwfgs.cn

Ruby: File.exist?("a.txt")
来源：http://et.yuntaijiaju.cn


<!-- 参考信息 -->