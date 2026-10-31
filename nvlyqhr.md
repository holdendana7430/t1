代发 wailian999

Ruby: arr.tally
来源：http://cl.yuexingan06.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mk.lnxyls.cn

[D21] 判断是否包含某元素
来源：http://tq.9csxet.cn

Py:   x in arr
来源：http://eg.chemitech.net.cn

PHP:  in_array($x, $arr, true);
来源：http://rr.newstarts.cn

JS:   arr.includes(x)
来源：http://vu.colortex.cn

TS:   arr.includes(x)
来源：http://jf.szxytkj.cn

Java: list.contains(x)
来源：http://fl.colortex.cn

Go:   slices.Contains(arr, x)
来源：http://in.shtwfgs.cn

Ruby: arr.include?(x)
来源：http://hr.hahajie.cn

C#:   list.Contains(x)
来源：http://pw.panjiajie.cn

[D22] 复制数组（避免共享引用）
来源：http://xc.szsharing.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zn.panjiajie.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wc.wgjwhj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://tj.panjiajie.cn

TS:   [...arr];
来源：http://cd.521024.cn

Java: new ArrayList<>(list);
来源：http://tx.shxzskj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://qb.chemitech.net.cn

Ruby: arr.dup;  arr.clone
来源：http://mo.nicolike.cn

C#:   new List<int>(list);
来源：http://lb.hnjuh.cn

[D23] reduce 累积计算
来源：http://wo.yuexingan06.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ub.bjjhwx.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://nu.newstarts.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ms.colortex.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qh.huixinmuqiang.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://po.hahajie.cn

Go:   // 手写循环
来源：http://te.newstarts.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://iq.nicolike.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://yc.lnxyls.cn

[D24] 字典 / Map 基本操作
来源：http://sw.asd995.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wb.newstarts.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mf.521024.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://sy.gzmigu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bp.nszjky.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jz.nszjky.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://uy.chemitech.net.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://os.panjiajie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ko.yuntaijiaju.cn

[D25] Set 集合去重与交并差
来源：http://uw.lnxyls.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ph.bjjhwx.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gg.bjjhwx.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ar.bjjhwx.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://br.nicolike.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://fv.haigaiapp.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://yn.shtwfgs.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hg.newstarts.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ue.shxzskj.cn

[D26] 数组转字符串
来源：http://ws.yuexingan06.cn

Py:   ", ".join(map(str, arr))
来源：http://ct.521024.cn

PHP:  implode(", ", $arr);
来源：http://jt.shxzskj.cn

JS:   arr.join(", ")
来源：http://sc.hnjuh.cn

TS:   arr.join(", ")
来源：http://kj.yuntaijiaju.cn

Java: String.join(", ", list)
来源：http://tq.szxytkj.cn

Go:   strings.Join(strs, ", ")
来源：http://dr.hahajie.cn

Ruby: arr.join(", ")
来源：http://dn.yuexingan06.cn

C#:   string.Join(", ", list)
来源：http://dk.bjjhwx.cn

================================================================================
来源：http://vo.hnjuh.cn

E. 字符串处理
来源：http://vw.haigaiapp.cn

================================================================================
来源：http://sf.panjiajie.cn

[E01] 拼接字符串
来源：http://dq.muxihuayi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ab.hahajie.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fz.hnjuh.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://rk.bjjhwx.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://lp.haigaiapp.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://sg.bjjhwx.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://is.shxzukj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://od.huixiangedu.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://pd.shxzskj.cn

[E02] 重复字符串
来源：http://tk.shxzukj.cn

Py:   "ab" * 3
来源：http://mg.bjjhwx.cn

PHP:  str_repeat("ab", 3);
来源：http://fu.hnjuh.cn

JS:   "ab".repeat(3)
来源：http://jg.521024.cn

TS:   "ab".repeat(3)
来源：http://it.muxihuayi.cn

Java: "ab".repeat(3)
来源：http://mr.hnjuh.cn

Go:   strings.Repeat("ab", 3)
来源：http://ro.yuntaijiaju.cn

Ruby: "ab" * 3
来源：http://oo.nszjky.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://sg.nicolike.cn

[E03] 截取子串
来源：http://ng.lnxyls.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ce.521024.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vw.shtwfgs.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://oa.panjiajie.cn

TS:   s.slice(1, 4)
来源：http://mf.hahajie.cn

Java: s.substring(1, 4)
来源：http://qm.haigaiapp.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kw.nszjky.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ha.chemitech.net.cn

C#:   s.Substring(1, 3)
来源：http://yt.haigaiapp.cn

[E04] 查找子串位置
来源：http://aw.nicolike.cn

Py:   s.find("x");  s.index("x")
来源：http://fy.muxihuayi.cn

PHP:  strpos($s, "x");
来源：http://rl.bookmarksfly.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://yw.muxihuayi.cn

TS:   s.indexOf("x")
来源：http://ug.newstarts.cn

Java: s.indexOf("x")
来源：http://mq.szxytkj.cn

Go:   strings.Index(s, "x")
来源：http://vw.shtwfgs.cn

Ruby: s.index("x")
来源：http://bk.muxihuayi.cn

C#:   s.IndexOf("x")
来源：http://xq.colortex.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://hd.colortex.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://iy.huanxung.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qe.huanxung.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ag.nicolike.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://vc.9csxet.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cu.hahajie.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ml.shxzskj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ad.bjjhwx.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ad.panjiajie.cn

[E06] 替换子串
来源：http://dd.shxzskj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ug.colortex.cn

PHP:  str_replace("a", "b", $s);
来源：http://nz.521024.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://su.haigaiapp.cn

TS:   s.replaceAll("a", "b")
来源：http://wd.521024.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://go.hnjuh.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xy.haigaiapp.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://cr.hahajie.cn

C#:   s.Replace("a", "b")
来源：http://cs.shxzukj.cn

[E07] 按分隔符拆分
来源：http://wv.bjjhwx.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lr.panjiajie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kp.chemitech.net.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://oq.nszjky.cn

TS:   s.split(",")
来源：http://vm.chemitech.net.cn

Java: s.split(",");  s.split("\\s+")
来源：http://mx.jctech888.com.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://eg.haigaiapp.cn

Ruby: s.split(",");  s.split
来源：http://va.9csxet.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qm.jctech888.com.cn

[E08] 数组按分隔符合并
来源：http://bd.521024.cn

Py:   ",".join(items)
来源：http://hr.shxzukj.cn

PHP:  implode(",", $items);
来源：http://ws.nicolike.cn

JS:   items.join(",")
来源：http://po.bookmarksfly.cn

TS:   items.join(",")
来源：http://xp.panjiajie.cn

Java: String.join(",", items)
来源：http://lp.nszjky.cn

Go:   strings.Join(items, ",")
来源：http://cs.bookmarksfly.cn

Ruby: items.join(",")
来源：http://ui.jianghongdianzi.cn

C#:   string.Join(",", items)
来源：http://sk.newstarts.cn

[E09] 去除所有空白字符
来源：http://tb.9csxet.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ro.huixiangedu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ln.szxytkj.cn

JS:   s.replace(/\s+/g, "")
来源：http://hf.colortex.cn

TS:   s.replace(/\s+/g, "")
来源：http://ey.hahajie.cn

Java: s.replaceAll("\\s+", "")
来源：http://sz.chemitech.net.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://xb.shxzskj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://jm.szsharing.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fu.hnjuh.cn

[E10] 左侧补零 / 定长填充
来源：http://ia.nszjky.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gu.jctech888.com.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ai.521024.cn

JS:   "7".padStart(3, "0")
来源：http://ch.haigaiapp.cn

TS:   "7".padStart(3, "0")
来源：http://wr.szsharing.cn

Java: String.format("%03d", 7)
来源：http://oo.szxytkj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://so.huixinmuqiang.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://yc.yuntaijiaju.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://nm.szsharing.cn

[E11] 反转字符串
来源：http://ow.asd995.cn

Py:   s[::-1]
来源：http://gr.huixiangedu.cn

PHP:  strrev($s);
来源：http://mg.shxzskj.cn

JS:   [...s].reverse().join("")
来源：http://wm.nicolike.cn

TS:   [...s].reverse().join("")
来源：http://og.gzmigu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://zw.hnjuh.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ri.wgjwhj.cn

Ruby: s.reverse
来源：http://mo.nicolike.cn

C#:   new string(s.Reverse().ToArray())
来源：http://sb.shtwfgs.cn

[E12] 统计某字符出现次数
来源：http://ui.hahajie.cn

Py:   s.count("a")
来源：http://ab.bookmarksfly.cn

PHP:  substr_count($s, "a");
来源：http://xw.szxytkj.cn

JS:   s.split("a").length - 1
来源：http://cb.nicolike.cn

TS:   s.split("a").length - 1
来源：http://rw.9csxet.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://go.shxzukj.cn

Go:   strings.Count(s, "a")
来源：http://bw.lnxyls.cn

Ruby: s.count("a")
来源：http://sj.hahajie.cn

C#:   s.Count(c => c == 'a')
来源：http://cq.shxzskj.cn

[E13] 逐字符遍历
来源：http://jf.colortex.cn

Py:   for ch in s: print(ch)
来源：http://wb.huixiangedu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zk.nicolike.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ut.nicolike.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://dn.panjiajie.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mw.jianghongdianzi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ow.colortex.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ev.newstarts.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ue.shxzskj.cn

[E14] URL 编码与 Base64
来源：http://fv.shtwfgs.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://bl.hahajie.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ci.521024.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ra.yuexingan06.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fa.szsharing.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ry.jctech888.com.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mj.huanxung.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://lp.shxzskj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://aq.szxytkj.cn

[E15] HTML 转义 / 反转义
来源：http://cs.wgjwhj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://im.newstarts.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rx.gzmigu.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pc.haigaiapp.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://sx.jianghongdianzi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gl.newstarts.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bg.hnjuh.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://df.asd995.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hn.yuexingan06.cn

[E16] 数字千分位
来源：http://au.wgjwhj.cn

Py:   f"{1234567:,}"
来源：http://cs.haigaiapp.cn

PHP:  number_format(1234567);
来源：http://mn.jianghongdianzi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://av.hahajie.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ep.bookmarksfly.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://iw.gzmigu.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ak.szsharing.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://uj.huixiangedu.cn

C#:   1234567.ToString("N0")
来源：http://jn.huanxung.cn

[E17] 首字母大写
来源：http://qr.wgjwhj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bm.panjiajie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://hw.yuexingan06.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bx.huixinmuqiang.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wb.521024.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://oa.haigaiapp.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ae.chemitech.net.cn

Ruby: s.capitalize
来源：http://sl.wgjwhj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jh.wgjwhj.cn

[E18] 模板占位符替换
来源：http://jr.9csxet.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zc.szxytkj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hv.huixinmuqiang.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ne.szxytkj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://dy.shtwfgs.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://cc.huanxung.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lk.muxihuayi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gc.9csxet.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bc.bookmarksfly.cn

[E19] 多行文本按行拆分
来源：http://ry.9csxet.cn

Py:   s.splitlines()
来源：http://zb.nszjky.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ds.huixinmuqiang.cn

JS:   s.split(/\r?\n/)
来源：http://xa.bookmarksfly.cn

TS:   s.split(/\r?\n/)
来源：http://ge.newstarts.cn

Java: s.lines().toList()
来源：http://zi.szxytkj.cn

Go:   strings.Split(s, "\n")
来源：http://ow.szsharing.cn

Ruby: s.lines
来源：http://yy.jctech888.com.cn

C#:   s.Split('\n')
来源：http://ea.szsharing.cn

[E20] 判断字符串是否为空
来源：http://oq.jianghongdianzi.cn

Py:   if not s:
来源：http://rg.newstarts.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qj.gzmigu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wi.lnxyls.cn

TS:   if (s === "") {}
来源：http://nv.bjjhwx.cn

Java: if (s.isEmpty()) {}
来源：http://qa.hahajie.cn

Go:   if s == "" {}
来源：http://lj.yuntaijiaju.cn

Ruby: if s.empty?
来源：http://jj.jianghongdianzi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://pu.chemitech.net.cn

[E21] 超长截断加省略号
来源：http://hs.huanxung.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://tc.9csxet.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ga.shxzskj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pz.521024.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vm.asd995.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jg.bookmarksfly.cn

Go:   // 按 rune 判断长度后截断
来源：http://sd.panjiajie.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gl.asd995.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jw.hahajie.cn

[E22] 字节长度与字符长度
来源：http://jq.hnjuh.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ue.521024.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yz.lnxyls.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vl.jctech888.com.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wq.huanxung.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yn.gzmigu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fh.gzmigu.cn

Ruby: s.bytesize;  s.length
来源：http://gy.yuexingan06.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cz.colortex.cn

================================================================================
来源：http://oz.jctech888.com.cn

F. 文件与目录
来源：http://go.jctech888.com.cn

================================================================================
来源：http://ft.yuexingan06.cn

[F01] 读取整个文件
来源：http://ic.yuntaijiaju.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gg.shxzskj.cn

PHP:  file_get_contents("a.txt");
来源：http://ba.yuexingan06.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jw.newstarts.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fc.521024.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://gj.shxzukj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://bc.nszjky.cn

Ruby: File.read("a.txt")
来源：http://im.szxytkj.cn

C#:   File.ReadAllText("a.txt");
来源：http://eb.szxytkj.cn

[F02] 逐行读取文件
来源：http://fo.hahajie.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://at.jctech888.com.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kj.haigaiapp.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://oi.9csxet.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gh.colortex.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mx.hnjuh.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ls.bjjhwx.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://uo.9csxet.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://cj.szxytkj.cn

[F03] 写入文件（覆盖）
来源：http://ih.huixiangedu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://em.gzmigu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://fv.bjjhwx.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ie.shtwfgs.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tf.szxytkj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xz.szxytkj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rn.yuntaijiaju.cn

Ruby: File.write("a.txt", "hi")
来源：http://si.chemitech.net.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cg.yuexingan06.cn

[F04] 追加写入文件
来源：http://yc.jianghongdianzi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ep.szxytkj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dg.hnjuh.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mz.colortex.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jr.jianghongdianzi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ze.yuexingan06.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ro.huanxung.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gr.9csxet.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://sg.szsharing.cn

[F05] 判断文件或目录是否存在
来源：http://ky.yuntaijiaju.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fn.chemitech.net.cn

PHP:  file_exists("a.txt");
来源：http://js.szsharing.cn

JS:   fs.existsSync("a.txt")
来源：http://np.9csxet.cn


<!-- 参考信息 -->