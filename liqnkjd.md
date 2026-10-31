代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://eo.panjiajie.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://jx.bjjhwx.cn

Go:   // 手写循环
来源：http://pt.huixiangedu.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://rx.haigaiapp.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xu.bjjhwx.cn

[D24] 字典 / Map 基本操作
来源：http://vo.hnjuh.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://iq.yuexingan06.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mu.bjjhwx.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://st.huixinmuqiang.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wp.haigaiapp.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qf.nszjky.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fy.colortex.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pv.521024.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ai.jianghongdianzi.cn

[D25] Set 集合去重与交并差
来源：http://rn.bookmarksfly.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zm.asd995.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wy.szsharing.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://je.jianghongdianzi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gq.jctech888.com.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://up.szxytkj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tk.jianghongdianzi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ew.shxzukj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bh.newstarts.cn

[D26] 数组转字符串
来源：http://rd.lnxyls.cn

Py:   ", ".join(map(str, arr))
来源：http://yq.nszjky.cn

PHP:  implode(", ", $arr);
来源：http://lo.nicolike.cn

JS:   arr.join(", ")
来源：http://kx.lnxyls.cn

TS:   arr.join(", ")
来源：http://qf.nicolike.cn

Java: String.join(", ", list)
来源：http://jc.asd995.cn

Go:   strings.Join(strs, ", ")
来源：http://lv.jctech888.com.cn

Ruby: arr.join(", ")
来源：http://xr.9csxet.cn

C#:   string.Join(", ", list)
来源：http://em.lnxyls.cn

================================================================================
来源：http://oy.hahajie.cn

E. 字符串处理
来源：http://mb.huixiangedu.cn

================================================================================
来源：http://gz.9csxet.cn

[E01] 拼接字符串
来源：http://ih.9csxet.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://io.jctech888.com.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tl.bjjhwx.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ba.szsharing.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jy.gzmigu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vq.szsharing.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ap.szsharing.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tv.szsharing.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ac.yuntaijiaju.cn

[E02] 重复字符串
来源：http://if.jianghongdianzi.cn

Py:   "ab" * 3
来源：http://su.jianghongdianzi.cn

PHP:  str_repeat("ab", 3);
来源：http://dh.bookmarksfly.cn

JS:   "ab".repeat(3)
来源：http://zx.9csxet.cn

TS:   "ab".repeat(3)
来源：http://vq.yuexingan06.cn

Java: "ab".repeat(3)
来源：http://xa.yuntaijiaju.cn

Go:   strings.Repeat("ab", 3)
来源：http://gy.huanxung.cn

Ruby: "ab" * 3
来源：http://sj.nicolike.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://me.hnjuh.cn

[E03] 截取子串
来源：http://qd.muxihuayi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wl.9csxet.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mf.gzmigu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vw.shxzukj.cn

TS:   s.slice(1, 4)
来源：http://dx.chemitech.net.cn

Java: s.substring(1, 4)
来源：http://bt.newstarts.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://sd.huixiangedu.cn

Ruby: s[1, 3];  s[1..3]
来源：http://av.asd995.cn

C#:   s.Substring(1, 3)
来源：http://ka.shxzskj.cn

[E04] 查找子串位置
来源：http://sk.szxytkj.cn

Py:   s.find("x");  s.index("x")
来源：http://ia.yuexingan06.cn

PHP:  strpos($s, "x");
来源：http://hf.shxzukj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ap.muxihuayi.cn

TS:   s.indexOf("x")
来源：http://hh.huixinmuqiang.cn

Java: s.indexOf("x")
来源：http://ry.bookmarksfly.cn

Go:   strings.Index(s, "x")
来源：http://wg.chemitech.net.cn

Ruby: s.index("x")
来源：http://vi.colortex.cn

C#:   s.IndexOf("x")
来源：http://uk.gzmigu.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://sm.nszjky.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ia.huixiangedu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ym.huixinmuqiang.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pm.lnxyls.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ns.nicolike.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://iv.wgjwhj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://sk.shxzukj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ji.gzmigu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mq.bookmarksfly.cn

[E06] 替换子串
来源：http://do.haigaiapp.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gy.panjiajie.cn

PHP:  str_replace("a", "b", $s);
来源：http://qo.huanxung.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dk.521024.cn

TS:   s.replaceAll("a", "b")
来源：http://oy.gzmigu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ya.newstarts.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rf.shxzukj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://pi.wgjwhj.cn

C#:   s.Replace("a", "b")
来源：http://qg.bjjhwx.cn

[E07] 按分隔符拆分
来源：http://ra.521024.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://px.chemitech.net.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hr.colortex.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ut.huanxung.cn

TS:   s.split(",")
来源：http://uu.jianghongdianzi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://io.shxzukj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mz.yuntaijiaju.cn

Ruby: s.split(",");  s.split
来源：http://at.gzmigu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ci.haigaiapp.cn

[E08] 数组按分隔符合并
来源：http://nm.huanxung.cn

Py:   ",".join(items)
来源：http://bv.bookmarksfly.cn

PHP:  implode(",", $items);
来源：http://su.asd995.cn

JS:   items.join(",")
来源：http://re.szsharing.cn

TS:   items.join(",")
来源：http://ay.panjiajie.cn

Java: String.join(",", items)
来源：http://om.huixinmuqiang.cn

Go:   strings.Join(items, ",")
来源：http://ax.szxytkj.cn

Ruby: items.join(",")
来源：http://da.shtwfgs.cn

C#:   string.Join(",", items)
来源：http://tj.hahajie.cn

[E09] 去除所有空白字符
来源：http://qp.bjjhwx.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zt.hnjuh.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zc.yuexingan06.cn

JS:   s.replace(/\s+/g, "")
来源：http://iz.wgjwhj.cn

TS:   s.replace(/\s+/g, "")
来源：http://uj.bjjhwx.cn

Java: s.replaceAll("\\s+", "")
来源：http://td.shxzskj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://rt.huanxung.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ma.521024.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ca.nicolike.cn

[E10] 左侧补零 / 定长填充
来源：http://me.bookmarksfly.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kn.hnjuh.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xx.bjjhwx.cn

JS:   "7".padStart(3, "0")
来源：http://ew.asd995.cn

TS:   "7".padStart(3, "0")
来源：http://wx.szsharing.cn

Java: String.format("%03d", 7)
来源：http://uz.chemitech.net.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://wi.yuntaijiaju.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lw.haigaiapp.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bm.szxytkj.cn

[E11] 反转字符串
来源：http://ey.huanxung.cn

Py:   s[::-1]
来源：http://sz.shxzukj.cn

PHP:  strrev($s);
来源：http://ht.lnxyls.cn

JS:   [...s].reverse().join("")
来源：http://gt.9csxet.cn

TS:   [...s].reverse().join("")
来源：http://vv.nszjky.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://vz.gzmigu.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://zj.yuntaijiaju.cn

Ruby: s.reverse
来源：http://zo.colortex.cn

C#:   new string(s.Reverse().ToArray())
来源：http://qx.huixiangedu.cn

[E12] 统计某字符出现次数
来源：http://mw.nicolike.cn

Py:   s.count("a")
来源：http://ps.yuntaijiaju.cn

PHP:  substr_count($s, "a");
来源：http://st.haigaiapp.cn

JS:   s.split("a").length - 1
来源：http://yb.haigaiapp.cn

TS:   s.split("a").length - 1
来源：http://kq.panjiajie.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ly.521024.cn

Go:   strings.Count(s, "a")
来源：http://si.gzmigu.cn

Ruby: s.count("a")
来源：http://yb.hahajie.cn

C#:   s.Count(c => c == 'a')
来源：http://an.gzmigu.cn

[E13] 逐字符遍历
来源：http://wb.newstarts.cn

Py:   for ch in s: print(ch)
来源：http://bu.shxzskj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xn.nicolike.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://jw.shxzukj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://il.huixinmuqiang.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://by.hahajie.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mc.chemitech.net.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://sv.wgjwhj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://eg.huanxung.cn

[E14] URL 编码与 Base64
来源：http://mg.gzmigu.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://yr.huixiangedu.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://qn.nicolike.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qj.shxzukj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://lo.bookmarksfly.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://dk.panjiajie.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gl.asd995.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mj.521024.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://uu.muxihuayi.cn

[E15] HTML 转义 / 反转义
来源：http://pp.yuexingan06.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ot.huixiangedu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rl.wgjwhj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hf.9csxet.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ck.shxzukj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ym.haigaiapp.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ry.haigaiapp.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://no.szxytkj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mn.lnxyls.cn

[E16] 数字千分位
来源：http://ha.hnjuh.cn

Py:   f"{1234567:,}"
来源：http://ep.szxytkj.cn

PHP:  number_format(1234567);
来源：http://mu.shtwfgs.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://oz.yuexingan06.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://kx.szsharing.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bm.colortex.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ej.haigaiapp.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ig.yuntaijiaju.cn

C#:   1234567.ToString("N0")
来源：http://te.bookmarksfly.cn

[E17] 首字母大写
来源：http://ln.huanxung.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://im.jctech888.com.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://pj.haigaiapp.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nv.gzmigu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yh.gzmigu.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://su.bjjhwx.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lv.yuntaijiaju.cn

Ruby: s.capitalize
来源：http://pk.gzmigu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ta.yuntaijiaju.cn

[E18] 模板占位符替换
来源：http://ut.huixiangedu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://el.huanxung.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nl.asd995.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ex.nszjky.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://fh.newstarts.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://at.szxytkj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kn.nicolike.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ja.haigaiapp.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ey.huixiangedu.cn

[E19] 多行文本按行拆分
来源：http://cr.muxihuayi.cn

Py:   s.splitlines()
来源：http://mb.asd995.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://un.muxihuayi.cn

JS:   s.split(/\r?\n/)
来源：http://do.jctech888.com.cn

TS:   s.split(/\r?\n/)
来源：http://ke.asd995.cn

Java: s.lines().toList()
来源：http://wi.shxzskj.cn

Go:   strings.Split(s, "\n")
来源：http://vh.bjjhwx.cn

Ruby: s.lines
来源：http://ie.panjiajie.cn

C#:   s.Split('\n')
来源：http://he.huixiangedu.cn

[E20] 判断字符串是否为空
来源：http://qs.colortex.cn

Py:   if not s:
来源：http://ul.panjiajie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://se.colortex.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://le.hnjuh.cn

TS:   if (s === "") {}
来源：http://ct.asd995.cn

Java: if (s.isEmpty()) {}
来源：http://vc.szxytkj.cn

Go:   if s == "" {}
来源：http://ov.szsharing.cn

Ruby: if s.empty?
来源：http://rq.yuexingan06.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ae.shxzskj.cn

[E21] 超长截断加省略号
来源：http://vr.wgjwhj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ij.yuexingan06.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ut.521024.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bz.newstarts.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jf.jctech888.com.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://oz.haigaiapp.cn

Go:   // 按 rune 判断长度后截断
来源：http://qp.shtwfgs.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ub.yuexingan06.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://nc.nicolike.cn

[E22] 字节长度与字符长度
来源：http://if.nszjky.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xs.chemitech.net.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rp.shxzukj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://kn.9csxet.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://za.huixiangedu.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ig.521024.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zw.nicolike.cn

Ruby: s.bytesize;  s.length
来源：http://xo.szsharing.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vo.nszjky.cn

================================================================================
来源：http://ly.nszjky.cn

F. 文件与目录
来源：http://tl.szsharing.cn

================================================================================
来源：http://vb.hnjuh.cn

[F01] 读取整个文件
来源：http://nx.huanxung.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://yl.nszjky.cn

PHP:  file_get_contents("a.txt");
来源：http://dv.jctech888.com.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://to.yuntaijiaju.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ue.shxzukj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://sw.szxytkj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hp.shtwfgs.cn

Ruby: File.read("a.txt")
来源：http://io.nszjky.cn

C#:   File.ReadAllText("a.txt");
来源：http://ay.newstarts.cn

[F02] 逐行读取文件
来源：http://kb.shxzskj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pe.shxzskj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bs.chemitech.net.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xl.9csxet.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tv.jianghongdianzi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dd.newstarts.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ah.hnjuh.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kv.shtwfgs.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wq.nszjky.cn

[F03] 写入文件（覆盖）
来源：http://qe.newstarts.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ws.hnjuh.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://qb.newstarts.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ub.hahajie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ne.jctech888.com.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zr.panjiajie.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://oc.shxzskj.cn

Ruby: File.write("a.txt", "hi")
来源：http://ru.shxzskj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ds.chemitech.net.cn

[F04] 追加写入文件
来源：http://hc.szsharing.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xm.hnjuh.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cv.nicolike.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vv.gzmigu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hj.haigaiapp.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://kv.colortex.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lf.lnxyls.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zz.521024.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hr.huanxung.cn

[F05] 判断文件或目录是否存在
来源：http://ru.hnjuh.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tt.huixinmuqiang.cn

PHP:  file_exists("a.txt");
来源：http://hc.521024.cn

JS:   fs.existsSync("a.txt")
来源：http://vp.yuexingan06.cn

TS:   fs.existsSync("a.txt")
来源：http://yr.muxihuayi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ic.hnjuh.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://uz.shxzukj.cn

Ruby: File.exist?("a.txt")
来源：http://iv.yuntaijiaju.cn

C#:   File.Exists("a.txt")
来源：http://fl.szxytkj.cn

[F06] 删除文件
来源：http://fr.colortex.cn

Py:   os.remove("a.txt")
来源：http://ni.chemitech.net.cn

PHP:  unlink("a.txt");
来源：http://pn.shxzukj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://et.hnjuh.cn

TS:   fs.unlinkSync("a.txt")
来源：http://we.jctech888.com.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://no.szxytkj.cn

Go:   os.Remove("a.txt")
来源：http://we.521024.cn

Ruby: File.delete("a.txt")
来源：http://sx.jianghongdianzi.cn

C#:   File.Delete("a.txt");
来源：http://gu.hnjuh.cn

[F07] 创建目录（含多级）
来源：http://yq.szxytkj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://aj.asd995.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://sy.szxytkj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qq.yuntaijiaju.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qs.chemitech.net.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gm.huixiangedu.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hl.9csxet.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xi.shxzskj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fg.newstarts.cn

[F08] 遍历目录
来源：http://mt.huixinmuqiang.cn


<!-- 参考信息 -->