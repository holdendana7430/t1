代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rw.lnxyls.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://hn.hahajie.cn

Go:   // 手写循环
来源：http://gk.lnxyls.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ks.asd995.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://vq.haigaiapp.cn

[D24] 字典 / Map 基本操作
来源：http://va.jianghongdianzi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jl.jctech888.com.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kv.asd995.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vv.hnjuh.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qg.panjiajie.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ww.bookmarksfly.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qu.gzmigu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gk.hnjuh.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qk.panjiajie.cn

[D25] Set 集合去重与交并差
来源：http://tb.shxzukj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://em.bookmarksfly.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://lx.jianghongdianzi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zr.hahajie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://sk.bjjhwx.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://si.hahajie.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://uh.gzmigu.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wr.colortex.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mg.nicolike.cn

[D26] 数组转字符串
来源：http://aw.colortex.cn

Py:   ", ".join(map(str, arr))
来源：http://vl.yuntaijiaju.cn

PHP:  implode(", ", $arr);
来源：http://le.shxzukj.cn

JS:   arr.join(", ")
来源：http://oz.szxytkj.cn

TS:   arr.join(", ")
来源：http://dv.muxihuayi.cn

Java: String.join(", ", list)
来源：http://vg.newstarts.cn

Go:   strings.Join(strs, ", ")
来源：http://uv.shxzskj.cn

Ruby: arr.join(", ")
来源：http://lh.haigaiapp.cn

C#:   string.Join(", ", list)
来源：http://nw.nszjky.cn

================================================================================
来源：http://gr.haigaiapp.cn

E. 字符串处理
来源：http://fl.bookmarksfly.cn

================================================================================
来源：http://yu.szsharing.cn

[E01] 拼接字符串
来源：http://se.huanxung.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ar.wgjwhj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dm.szsharing.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dz.nicolike.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ba.newstarts.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gf.hnjuh.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tk.panjiajie.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tl.gzmigu.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gf.shtwfgs.cn

[E02] 重复字符串
来源：http://vx.jianghongdianzi.cn

Py:   "ab" * 3
来源：http://lp.panjiajie.cn

PHP:  str_repeat("ab", 3);
来源：http://ji.nszjky.cn

JS:   "ab".repeat(3)
来源：http://tp.hnjuh.cn

TS:   "ab".repeat(3)
来源：http://tt.wgjwhj.cn

Java: "ab".repeat(3)
来源：http://xl.gzmigu.cn

Go:   strings.Repeat("ab", 3)
来源：http://pq.asd995.cn

Ruby: "ab" * 3
来源：http://ys.yuexingan06.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://of.huixiangedu.cn

[E03] 截取子串
来源：http://gr.hnjuh.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://sq.bookmarksfly.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tv.lnxyls.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://pf.chemitech.net.cn

TS:   s.slice(1, 4)
来源：http://ob.hahajie.cn

Java: s.substring(1, 4)
来源：http://uw.bjjhwx.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hw.bjjhwx.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ae.asd995.cn

C#:   s.Substring(1, 3)
来源：http://uq.bjjhwx.cn

[E04] 查找子串位置
来源：http://ds.chemitech.net.cn

Py:   s.find("x");  s.index("x")
来源：http://ee.huixiangedu.cn

PHP:  strpos($s, "x");
来源：http://ir.gzmigu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ok.hahajie.cn

TS:   s.indexOf("x")
来源：http://ot.muxihuayi.cn

Java: s.indexOf("x")
来源：http://qv.colortex.cn

Go:   strings.Index(s, "x")
来源：http://ax.chemitech.net.cn

Ruby: s.index("x")
来源：http://be.muxihuayi.cn

C#:   s.IndexOf("x")
来源：http://un.huixinmuqiang.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://oc.panjiajie.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jc.szsharing.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://pn.newstarts.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yy.shtwfgs.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://hl.bjjhwx.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ay.yuntaijiaju.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://oa.szxytkj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ja.jctech888.com.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qg.bjjhwx.cn

[E06] 替换子串
来源：http://ss.huixiangedu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ti.huixinmuqiang.cn

PHP:  str_replace("a", "b", $s);
来源：http://qg.asd995.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://df.lnxyls.cn

TS:   s.replaceAll("a", "b")
来源：http://pl.nicolike.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sk.bookmarksfly.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://uq.lnxyls.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vm.gzmigu.cn

C#:   s.Replace("a", "b")
来源：http://dj.yuexingan06.cn

[E07] 按分隔符拆分
来源：http://oi.bookmarksfly.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://sw.gzmigu.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vy.shxzskj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://wy.szxytkj.cn

TS:   s.split(",")
来源：http://ss.hnjuh.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ll.shxzskj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ra.shxzskj.cn

Ruby: s.split(",");  s.split
来源：http://wg.nicolike.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mg.yuexingan06.cn

[E08] 数组按分隔符合并
来源：http://qu.jianghongdianzi.cn

Py:   ",".join(items)
来源：http://jw.9csxet.cn

PHP:  implode(",", $items);
来源：http://jh.haigaiapp.cn

JS:   items.join(",")
来源：http://ej.hahajie.cn

TS:   items.join(",")
来源：http://uy.chemitech.net.cn

Java: String.join(",", items)
来源：http://nh.nszjky.cn

Go:   strings.Join(items, ",")
来源：http://hs.szxytkj.cn

Ruby: items.join(",")
来源：http://vp.muxihuayi.cn

C#:   string.Join(",", items)
来源：http://cj.lnxyls.cn

[E09] 去除所有空白字符
来源：http://vw.nszjky.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://oa.asd995.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ki.hahajie.cn

JS:   s.replace(/\s+/g, "")
来源：http://uh.szxytkj.cn

TS:   s.replace(/\s+/g, "")
来源：http://kq.shtwfgs.cn

Java: s.replaceAll("\\s+", "")
来源：http://ut.szsharing.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://cj.shxzskj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://vt.nicolike.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xz.9csxet.cn

[E10] 左侧补零 / 定长填充
来源：http://xo.jctech888.com.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.jianghongdianzi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ob.yuexingan06.cn

JS:   "7".padStart(3, "0")
来源：http://hp.colortex.cn

TS:   "7".padStart(3, "0")
来源：http://yg.muxihuayi.cn

Java: String.format("%03d", 7)
来源：http://gn.asd995.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://tc.yuntaijiaju.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://nf.bjjhwx.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ir.nszjky.cn

[E11] 反转字符串
来源：http://yd.panjiajie.cn

Py:   s[::-1]
来源：http://ab.colortex.cn

PHP:  strrev($s);
来源：http://wd.szxytkj.cn

JS:   [...s].reverse().join("")
来源：http://hs.asd995.cn

TS:   [...s].reverse().join("")
来源：http://dm.bookmarksfly.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://rh.yuntaijiaju.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://mc.wgjwhj.cn

Ruby: s.reverse
来源：http://zb.colortex.cn

C#:   new string(s.Reverse().ToArray())
来源：http://af.nicolike.cn

[E12] 统计某字符出现次数
来源：http://xz.bjjhwx.cn

Py:   s.count("a")
来源：http://ot.yuexingan06.cn

PHP:  substr_count($s, "a");
来源：http://og.shtwfgs.cn

JS:   s.split("a").length - 1
来源：http://oy.nicolike.cn

TS:   s.split("a").length - 1
来源：http://nk.asd995.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yj.shtwfgs.cn

Go:   strings.Count(s, "a")
来源：http://zt.jctech888.com.cn

Ruby: s.count("a")
来源：http://jp.huixinmuqiang.cn

C#:   s.Count(c => c == 'a')
来源：http://qu.hahajie.cn

[E13] 逐字符遍历
来源：http://sn.shtwfgs.cn

Py:   for ch in s: print(ch)
来源：http://bo.hnjuh.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ig.jctech888.com.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ql.nicolike.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ok.521024.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://sy.hahajie.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xz.panjiajie.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://dn.gzmigu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ob.jctech888.com.cn

[E14] URL 编码与 Base64
来源：http://au.nicolike.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://er.muxihuayi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ja.huanxung.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vl.huanxung.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mk.yuexingan06.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bk.newstarts.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vy.szxytkj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wa.9csxet.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://oc.jctech888.com.cn

[E15] HTML 转义 / 反转义
来源：http://mt.shxzukj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://mo.jctech888.com.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wj.newstarts.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ju.jctech888.com.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://gu.yuntaijiaju.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://aq.hahajie.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qh.huanxung.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ej.huanxung.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://oq.muxihuayi.cn

[E16] 数字千分位
来源：http://mb.szxytkj.cn

Py:   f"{1234567:,}"
来源：http://uj.9csxet.cn

PHP:  number_format(1234567);
来源：http://qo.9csxet.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://dg.9csxet.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://yg.asd995.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fa.huixiangedu.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rs.shxzukj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://po.haigaiapp.cn

C#:   1234567.ToString("N0")
来源：http://gw.wgjwhj.cn

[E17] 首字母大写
来源：http://ef.asd995.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fo.wgjwhj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ph.nicolike.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ld.asd995.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zt.chemitech.net.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ci.hahajie.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ci.gzmigu.cn

Ruby: s.capitalize
来源：http://ix.yuntaijiaju.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xa.chemitech.net.cn

[E18] 模板占位符替换
来源：http://eh.newstarts.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fe.szxytkj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://oo.newstarts.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://hv.wgjwhj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://dn.muxihuayi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://il.521024.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ag.huanxung.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ne.521024.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://uu.jianghongdianzi.cn

[E19] 多行文本按行拆分
来源：http://yk.521024.cn

Py:   s.splitlines()
来源：http://ki.asd995.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xe.shtwfgs.cn

JS:   s.split(/\r?\n/)
来源：http://jc.muxihuayi.cn

TS:   s.split(/\r?\n/)
来源：http://hz.panjiajie.cn

Java: s.lines().toList()
来源：http://je.wgjwhj.cn

Go:   strings.Split(s, "\n")
来源：http://xi.huanxung.cn

Ruby: s.lines
来源：http://kc.shxzskj.cn

C#:   s.Split('\n')
来源：http://jk.asd995.cn

[E20] 判断字符串是否为空
来源：http://gh.huixinmuqiang.cn

Py:   if not s:
来源：http://br.bjjhwx.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bm.muxihuayi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qh.huixinmuqiang.cn

TS:   if (s === "") {}
来源：http://jx.yuexingan06.cn

Java: if (s.isEmpty()) {}
来源：http://gl.gzmigu.cn

Go:   if s == "" {}
来源：http://hv.szxytkj.cn

Ruby: if s.empty?
来源：http://ld.shxzukj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rz.wgjwhj.cn

[E21] 超长截断加省略号
来源：http://cb.hnjuh.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qy.colortex.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://yv.muxihuayi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rw.shxzukj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://br.nszjky.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xc.shtwfgs.cn

Go:   // 按 rune 判断长度后截断
来源：http://sc.hnjuh.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ay.newstarts.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://sr.shxzukj.cn

[E22] 字节长度与字符长度
来源：http://le.nicolike.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://np.shtwfgs.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nn.gzmigu.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ls.9csxet.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zr.yuntaijiaju.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://nh.bjjhwx.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dz.shxzskj.cn

Ruby: s.bytesize;  s.length
来源：http://st.hahajie.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kx.521024.cn

================================================================================
来源：http://td.chemitech.net.cn

F. 文件与目录
来源：http://eu.jianghongdianzi.cn

================================================================================
来源：http://yb.huixiangedu.cn

[F01] 读取整个文件
来源：http://zl.bjjhwx.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dx.chemitech.net.cn

PHP:  file_get_contents("a.txt");
来源：http://ou.newstarts.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://td.yuntaijiaju.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jt.huanxung.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://pg.jctech888.com.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hn.yuntaijiaju.cn

Ruby: File.read("a.txt")
来源：http://ln.shxzskj.cn

C#:   File.ReadAllText("a.txt");
来源：http://vd.huixiangedu.cn

[F02] 逐行读取文件
来源：http://tq.9csxet.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qy.9csxet.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wf.521024.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://we.yuntaijiaju.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ur.hnjuh.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gx.haigaiapp.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ud.jctech888.com.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://uj.wgjwhj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wr.huanxung.cn

[F03] 写入文件（覆盖）
来源：http://bb.521024.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zf.jianghongdianzi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ww.hahajie.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ut.asd995.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kn.nicolike.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://yz.yuexingan06.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fv.gzmigu.cn

Ruby: File.write("a.txt", "hi")
来源：http://ui.haigaiapp.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xn.bjjhwx.cn

[F04] 追加写入文件
来源：http://ce.huanxung.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wz.shxzukj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xt.shxzskj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bz.gzmigu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wh.colortex.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rf.shxzukj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://cx.lnxyls.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yo.9csxet.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lu.colortex.cn

[F05] 判断文件或目录是否存在
来源：http://jv.asd995.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://sb.jianghongdianzi.cn

PHP:  file_exists("a.txt");
来源：http://zo.shtwfgs.cn

JS:   fs.existsSync("a.txt")
来源：http://mh.hnjuh.cn

TS:   fs.existsSync("a.txt")
来源：http://ct.huixinmuqiang.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://lw.huixinmuqiang.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ve.shtwfgs.cn

Ruby: File.exist?("a.txt")
来源：http://ur.panjiajie.cn

C#:   File.Exists("a.txt")
来源：http://qz.jianghongdianzi.cn

[F06] 删除文件
来源：http://le.huixinmuqiang.cn

Py:   os.remove("a.txt")
来源：http://we.colortex.cn

PHP:  unlink("a.txt");
来源：http://bn.chemitech.net.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ap.gzmigu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://gf.9csxet.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fk.jctech888.com.cn

Go:   os.Remove("a.txt")
来源：http://eo.huixinmuqiang.cn

Ruby: File.delete("a.txt")
来源：http://kg.shxzukj.cn

C#:   File.Delete("a.txt");
来源：http://tt.9csxet.cn

[F07] 创建目录（含多级）
来源：http://wc.szsharing.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fn.chemitech.net.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xg.shxzukj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ss.wgjwhj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://er.huanxung.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ng.lnxyls.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rb.521024.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ec.huixiangedu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rs.huixiangedu.cn

[F08] 遍历目录
来源：http://ic.nszjky.cn


<!-- 参考信息 -->