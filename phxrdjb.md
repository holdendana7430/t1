代发 wailian999

[D23] reduce 累积计算
来源：http://ru.yuntaijiaju.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://fq.chemitech.net.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ns.bjjhwx.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vr.huixinmuqiang.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ti.yuntaijiaju.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://cw.asd995.cn

Go:   // 手写循环
来源：http://ww.szxytkj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://za.colortex.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ib.521024.cn

[D24] 字典 / Map 基本操作
来源：http://ll.yuexingan06.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vx.bookmarksfly.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://eg.jianghongdianzi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://iu.shxzskj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qq.wgjwhj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mv.lnxyls.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ym.asd995.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cr.jctech888.com.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vp.asd995.cn

[D25] Set 集合去重与交并差
来源：http://dk.yuntaijiaju.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rq.lnxyls.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wx.szxytkj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rv.shxzskj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://cu.bjjhwx.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://sl.hnjuh.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hd.panjiajie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pi.hahajie.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mn.wgjwhj.cn

[D26] 数组转字符串
来源：http://re.newstarts.cn

Py:   ", ".join(map(str, arr))
来源：http://eo.shtwfgs.cn

PHP:  implode(", ", $arr);
来源：http://js.lnxyls.cn

JS:   arr.join(", ")
来源：http://mp.huixinmuqiang.cn

TS:   arr.join(", ")
来源：http://cd.yuntaijiaju.cn

Java: String.join(", ", list)
来源：http://xh.colortex.cn

Go:   strings.Join(strs, ", ")
来源：http://rh.hnjuh.cn

Ruby: arr.join(", ")
来源：http://gn.wgjwhj.cn

C#:   string.Join(", ", list)
来源：http://nu.szxytkj.cn

================================================================================
来源：http://ke.huanxung.cn

E. 字符串处理
来源：http://ey.colortex.cn

================================================================================
来源：http://st.colortex.cn

[E01] 拼接字符串
来源：http://wf.hnjuh.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fb.lnxyls.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://bo.9csxet.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fi.jctech888.com.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jy.hahajie.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wm.colortex.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bk.gzmigu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zp.chemitech.net.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ty.jianghongdianzi.cn

[E02] 重复字符串
来源：http://lr.huixinmuqiang.cn

Py:   "ab" * 3
来源：http://gz.chemitech.net.cn

PHP:  str_repeat("ab", 3);
来源：http://jk.huixiangedu.cn

JS:   "ab".repeat(3)
来源：http://dg.hnjuh.cn

TS:   "ab".repeat(3)
来源：http://zr.muxihuayi.cn

Java: "ab".repeat(3)
来源：http://ok.yuexingan06.cn

Go:   strings.Repeat("ab", 3)
来源：http://cg.colortex.cn

Ruby: "ab" * 3
来源：http://zh.huixinmuqiang.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://le.yuexingan06.cn

[E03] 截取子串
来源：http://fx.bjjhwx.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ko.nicolike.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bf.huanxung.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://kw.shxzskj.cn

TS:   s.slice(1, 4)
来源：http://wj.nicolike.cn

Java: s.substring(1, 4)
来源：http://tm.shtwfgs.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fn.nicolike.cn

Ruby: s[1, 3];  s[1..3]
来源：http://mk.bjjhwx.cn

C#:   s.Substring(1, 3)
来源：http://gg.shxzskj.cn

[E04] 查找子串位置
来源：http://eb.nicolike.cn

Py:   s.find("x");  s.index("x")
来源：http://nz.haigaiapp.cn

PHP:  strpos($s, "x");
来源：http://ok.9csxet.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://dk.chemitech.net.cn

TS:   s.indexOf("x")
来源：http://yx.yuntaijiaju.cn

Java: s.indexOf("x")
来源：http://fc.9csxet.cn

Go:   strings.Index(s, "x")
来源：http://rn.szxytkj.cn

Ruby: s.index("x")
来源：http://ql.asd995.cn

C#:   s.IndexOf("x")
来源：http://rn.521024.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://yv.asd995.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://iz.shxzukj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bl.9csxet.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ba.nicolike.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ia.jctech888.com.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qj.9csxet.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dd.shxzukj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ay.huanxung.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dk.shtwfgs.cn

[E06] 替换子串
来源：http://lx.hahajie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://nf.szsharing.cn

PHP:  str_replace("a", "b", $s);
来源：http://pv.huanxung.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nv.chemitech.net.cn

TS:   s.replaceAll("a", "b")
来源：http://qv.521024.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://oi.szsharing.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rq.bjjhwx.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://aj.muxihuayi.cn

C#:   s.Replace("a", "b")
来源：http://ty.521024.cn

[E07] 按分隔符拆分
来源：http://mg.szsharing.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xi.hahajie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://if.hahajie.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://st.gzmigu.cn

TS:   s.split(",")
来源：http://zs.shtwfgs.cn

Java: s.split(",");  s.split("\\s+")
来源：http://jc.gzmigu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ap.newstarts.cn

Ruby: s.split(",");  s.split
来源：http://ub.szxytkj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ox.nicolike.cn

[E08] 数组按分隔符合并
来源：http://tf.bjjhwx.cn

Py:   ",".join(items)
来源：http://xq.haigaiapp.cn

PHP:  implode(",", $items);
来源：http://kt.jianghongdianzi.cn

JS:   items.join(",")
来源：http://tf.muxihuayi.cn

TS:   items.join(",")
来源：http://gp.jianghongdianzi.cn

Java: String.join(",", items)
来源：http://ql.jianghongdianzi.cn

Go:   strings.Join(items, ",")
来源：http://qx.chemitech.net.cn

Ruby: items.join(",")
来源：http://yr.shtwfgs.cn

C#:   string.Join(",", items)
来源：http://li.yuexingan06.cn

[E09] 去除所有空白字符
来源：http://sf.yuexingan06.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wq.shxzukj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ef.szxytkj.cn

JS:   s.replace(/\s+/g, "")
来源：http://vn.jctech888.com.cn

TS:   s.replace(/\s+/g, "")
来源：http://mt.nicolike.cn

Java: s.replaceAll("\\s+", "")
来源：http://wp.jctech888.com.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://bx.521024.cn

Ruby: s.gsub(/\s+/, "")
来源：http://lu.huanxung.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ns.hahajie.cn

[E10] 左侧补零 / 定长填充
来源：http://ho.hahajie.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ji.bjjhwx.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fw.nicolike.cn

JS:   "7".padStart(3, "0")
来源：http://sf.hahajie.cn

TS:   "7".padStart(3, "0")
来源：http://hy.haigaiapp.cn

Java: String.format("%03d", 7)
来源：http://sh.panjiajie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://li.yuntaijiaju.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ye.yuntaijiaju.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ze.521024.cn

[E11] 反转字符串
来源：http://sp.521024.cn

Py:   s[::-1]
来源：http://ld.521024.cn

PHP:  strrev($s);
来源：http://kb.nszjky.cn

JS:   [...s].reverse().join("")
来源：http://cf.gzmigu.cn

TS:   [...s].reverse().join("")
来源：http://zi.nszjky.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ic.jctech888.com.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ad.szsharing.cn

Ruby: s.reverse
来源：http://gk.521024.cn

C#:   new string(s.Reverse().ToArray())
来源：http://tc.haigaiapp.cn

[E12] 统计某字符出现次数
来源：http://qi.nicolike.cn

Py:   s.count("a")
来源：http://qq.nicolike.cn

PHP:  substr_count($s, "a");
来源：http://sd.chemitech.net.cn

JS:   s.split("a").length - 1
来源：http://ha.huanxung.cn

TS:   s.split("a").length - 1
来源：http://df.9csxet.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rk.shxzukj.cn

Go:   strings.Count(s, "a")
来源：http://xj.bjjhwx.cn

Ruby: s.count("a")
来源：http://xo.gzmigu.cn

C#:   s.Count(c => c == 'a')
来源：http://yj.chemitech.net.cn

[E13] 逐字符遍历
来源：http://rm.bookmarksfly.cn

Py:   for ch in s: print(ch)
来源：http://vv.muxihuayi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://sg.chemitech.net.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://mz.colortex.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://zv.huixinmuqiang.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gi.jctech888.com.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wx.yuntaijiaju.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://cj.newstarts.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://it.newstarts.cn

[E14] URL 编码与 Base64
来源：http://pk.muxihuayi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xu.haigaiapp.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://it.huixiangedu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://se.nszjky.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tr.muxihuayi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mv.9csxet.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wo.szxytkj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bh.jianghongdianzi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bh.jctech888.com.cn

[E15] HTML 转义 / 反转义
来源：http://ae.panjiajie.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ao.jctech888.com.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ai.gzmigu.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://it.haigaiapp.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://wp.hahajie.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mq.newstarts.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://nr.9csxet.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://dw.yuntaijiaju.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://dh.szsharing.cn

[E16] 数字千分位
来源：http://ql.huixiangedu.cn

Py:   f"{1234567:,}"
来源：http://yr.hahajie.cn

PHP:  number_format(1234567);
来源：http://sj.haigaiapp.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://jp.huixiangedu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://zy.lnxyls.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ii.lnxyls.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://uc.shxzukj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://de.shxzukj.cn

C#:   1234567.ToString("N0")
来源：http://el.muxihuayi.cn

[E17] 首字母大写
来源：http://sr.shxzskj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://yz.yuexingan06.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://vo.bookmarksfly.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ia.szsharing.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bg.panjiajie.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rz.muxihuayi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hk.huixinmuqiang.cn

Ruby: s.capitalize
来源：http://kl.nicolike.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jt.jianghongdianzi.cn

[E18] 模板占位符替换
来源：http://jo.wgjwhj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vn.szsharing.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mu.haigaiapp.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://wi.jianghongdianzi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://vj.bjjhwx.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ap.gzmigu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ip.haigaiapp.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://po.521024.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://il.muxihuayi.cn

[E19] 多行文本按行拆分
来源：http://fv.9csxet.cn

Py:   s.splitlines()
来源：http://lx.wgjwhj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nu.yuntaijiaju.cn

JS:   s.split(/\r?\n/)
来源：http://he.jianghongdianzi.cn

TS:   s.split(/\r?\n/)
来源：http://ae.yuntaijiaju.cn

Java: s.lines().toList()
来源：http://xa.panjiajie.cn

Go:   strings.Split(s, "\n")
来源：http://pq.bjjhwx.cn

Ruby: s.lines
来源：http://si.wgjwhj.cn

C#:   s.Split('\n')
来源：http://ov.shxzskj.cn

[E20] 判断字符串是否为空
来源：http://bk.hnjuh.cn

Py:   if not s:
来源：http://iv.newstarts.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zm.shxzukj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fl.huixinmuqiang.cn

TS:   if (s === "") {}
来源：http://fr.chemitech.net.cn

Java: if (s.isEmpty()) {}
来源：http://oy.jctech888.com.cn

Go:   if s == "" {}
来源：http://dm.colortex.cn

Ruby: if s.empty?
来源：http://au.chemitech.net.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qz.bookmarksfly.cn

[E21] 超长截断加省略号
来源：http://ao.chemitech.net.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hi.szxytkj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qj.yuexingan06.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kz.lnxyls.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gf.shxzukj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tk.nszjky.cn

Go:   // 按 rune 判断长度后截断
来源：http://xl.nszjky.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://di.chemitech.net.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kk.bjjhwx.cn

[E22] 字节长度与字符长度
来源：http://hj.nszjky.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://do.huixiangedu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yy.jianghongdianzi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gr.521024.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://id.9csxet.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://an.asd995.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ia.hahajie.cn

Ruby: s.bytesize;  s.length
来源：http://je.muxihuayi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dg.panjiajie.cn

================================================================================
来源：http://vf.huixinmuqiang.cn

F. 文件与目录
来源：http://hk.muxihuayi.cn

================================================================================
来源：http://bj.jianghongdianzi.cn

[F01] 读取整个文件
来源：http://gg.panjiajie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nx.gzmigu.cn

PHP:  file_get_contents("a.txt");
来源：http://yz.muxihuayi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kf.szxytkj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vk.yuexingan06.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://nf.yuexingan06.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ow.9csxet.cn

Ruby: File.read("a.txt")
来源：http://pp.haigaiapp.cn

C#:   File.ReadAllText("a.txt");
来源：http://vh.haigaiapp.cn

[F02] 逐行读取文件
来源：http://ut.wgjwhj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pb.nicolike.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qv.hnjuh.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zg.shtwfgs.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kb.hahajie.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ac.521024.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ou.huixiangedu.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rp.hahajie.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://yp.szsharing.cn

[F03] 写入文件（覆盖）
来源：http://kg.9csxet.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gf.huixiangedu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://tj.jianghongdianzi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pr.hahajie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://az.9csxet.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jk.huixinmuqiang.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://dt.bookmarksfly.cn

Ruby: File.write("a.txt", "hi")
来源：http://pd.muxihuayi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://uo.lnxyls.cn

[F04] 追加写入文件
来源：http://ah.huixiangedu.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ue.huixiangedu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://te.asd995.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cd.asd995.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wj.yuntaijiaju.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://co.huixiangedu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vo.huixinmuqiang.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vd.9csxet.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://pn.wgjwhj.cn

[F05] 判断文件或目录是否存在
来源：http://zr.shxzukj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ga.lnxyls.cn

PHP:  file_exists("a.txt");
来源：http://qm.bjjhwx.cn

JS:   fs.existsSync("a.txt")
来源：http://vx.huixiangedu.cn

TS:   fs.existsSync("a.txt")
来源：http://ti.newstarts.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://dl.shxzskj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ne.chemitech.net.cn

Ruby: File.exist?("a.txt")
来源：http://vv.szxytkj.cn

C#:   File.Exists("a.txt")
来源：http://ld.huanxung.cn

[F06] 删除文件
来源：http://st.haigaiapp.cn

Py:   os.remove("a.txt")
来源：http://zz.gzmigu.cn

PHP:  unlink("a.txt");
来源：http://pf.huixinmuqiang.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ij.jianghongdianzi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://pz.gzmigu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yg.521024.cn

Go:   os.Remove("a.txt")
来源：http://tg.szxytkj.cn

Ruby: File.delete("a.txt")
来源：http://ms.nszjky.cn

C#:   File.Delete("a.txt");
来源：http://xl.yuntaijiaju.cn

[F07] 创建目录（含多级）
来源：http://nz.shtwfgs.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mp.muxihuayi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hg.asd995.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://no.lnxyls.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ws.gzmigu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ef.jianghongdianzi.cn


<!-- 参考信息 -->