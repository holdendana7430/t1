代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pa.hahajie.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://bt.huixiangedu.cn

Go:   // 手写循环
来源：http://yw.asd995.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://cy.szxytkj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://aw.bookmarksfly.cn

[D24] 字典 / Map 基本操作
来源：http://av.jianghongdianzi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ai.jianghongdianzi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kj.huanxung.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xx.hnjuh.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://in.huixinmuqiang.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wk.bookmarksfly.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://nv.colortex.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fy.huanxung.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://bn.jianghongdianzi.cn

[D25] Set 集合去重与交并差
来源：http://xs.muxihuayi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nf.gzmigu.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ig.bookmarksfly.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rz.9csxet.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://lo.521024.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dp.asd995.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wv.shtwfgs.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://on.nicolike.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qh.hahajie.cn

[D26] 数组转字符串
来源：http://qf.haigaiapp.cn

Py:   ", ".join(map(str, arr))
来源：http://xn.wgjwhj.cn

PHP:  implode(", ", $arr);
来源：http://gp.lnxyls.cn

JS:   arr.join(", ")
来源：http://fp.panjiajie.cn

TS:   arr.join(", ")
来源：http://vs.huixiangedu.cn

Java: String.join(", ", list)
来源：http://ri.nszjky.cn

Go:   strings.Join(strs, ", ")
来源：http://ru.hnjuh.cn

Ruby: arr.join(", ")
来源：http://fp.yuntaijiaju.cn

C#:   string.Join(", ", list)
来源：http://cs.szsharing.cn

================================================================================
来源：http://mt.bookmarksfly.cn

E. 字符串处理
来源：http://cj.nicolike.cn

================================================================================
来源：http://bm.bookmarksfly.cn

[E01] 拼接字符串
来源：http://wn.newstarts.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ug.huixiangedu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ea.hahajie.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://yo.panjiajie.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gb.panjiajie.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://yz.9csxet.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rk.gzmigu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wj.huixiangedu.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nf.jctech888.com.cn

[E02] 重复字符串
来源：http://zw.yuexingan06.cn

Py:   "ab" * 3
来源：http://wh.hahajie.cn

PHP:  str_repeat("ab", 3);
来源：http://rc.haigaiapp.cn

JS:   "ab".repeat(3)
来源：http://fq.szxytkj.cn

TS:   "ab".repeat(3)
来源：http://fo.yuexingan06.cn

Java: "ab".repeat(3)
来源：http://yr.newstarts.cn

Go:   strings.Repeat("ab", 3)
来源：http://zk.521024.cn

Ruby: "ab" * 3
来源：http://ag.szsharing.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://cf.huixiangedu.cn

[E03] 截取子串
来源：http://eg.colortex.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://iz.jctech888.com.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ln.hnjuh.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rp.chemitech.net.cn

TS:   s.slice(1, 4)
来源：http://vy.nicolike.cn

Java: s.substring(1, 4)
来源：http://oh.huixiangedu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mx.jianghongdianzi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://uz.bjjhwx.cn

C#:   s.Substring(1, 3)
来源：http://gj.nicolike.cn

[E04] 查找子串位置
来源：http://yw.521024.cn

Py:   s.find("x");  s.index("x")
来源：http://nq.newstarts.cn

PHP:  strpos($s, "x");
来源：http://rc.yuntaijiaju.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vr.hnjuh.cn

TS:   s.indexOf("x")
来源：http://yf.huixiangedu.cn

Java: s.indexOf("x")
来源：http://ko.521024.cn

Go:   strings.Index(s, "x")
来源：http://hv.huanxung.cn

Ruby: s.index("x")
来源：http://jb.szsharing.cn

C#:   s.IndexOf("x")
来源：http://cw.jianghongdianzi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://hy.bjjhwx.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://es.szsharing.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://as.szxytkj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sw.szxytkj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://rd.huanxung.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ix.szxytkj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wb.nszjky.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mt.huixinmuqiang.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://lt.szxytkj.cn

[E06] 替换子串
来源：http://jv.huixiangedu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://cg.shxzskj.cn

PHP:  str_replace("a", "b", $s);
来源：http://ip.jianghongdianzi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ov.chemitech.net.cn

TS:   s.replaceAll("a", "b")
来源：http://ol.hahajie.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ut.yuexingan06.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xg.gzmigu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qr.huixinmuqiang.cn

C#:   s.Replace("a", "b")
来源：http://gh.muxihuayi.cn

[E07] 按分隔符拆分
来源：http://eb.bjjhwx.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://px.hahajie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kr.hahajie.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://iq.jctech888.com.cn

TS:   s.split(",")
来源：http://xb.yuexingan06.cn

Java: s.split(",");  s.split("\\s+")
来源：http://xx.newstarts.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wg.wgjwhj.cn

Ruby: s.split(",");  s.split
来源：http://lb.huixinmuqiang.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bu.shtwfgs.cn

[E08] 数组按分隔符合并
来源：http://ky.szxytkj.cn

Py:   ",".join(items)
来源：http://ng.szxytkj.cn

PHP:  implode(",", $items);
来源：http://rt.szsharing.cn

JS:   items.join(",")
来源：http://qu.szxytkj.cn

TS:   items.join(",")
来源：http://ks.shtwfgs.cn

Java: String.join(",", items)
来源：http://uf.hahajie.cn

Go:   strings.Join(items, ",")
来源：http://wi.yuexingan06.cn

Ruby: items.join(",")
来源：http://rq.colortex.cn

C#:   string.Join(",", items)
来源：http://au.panjiajie.cn

[E09] 去除所有空白字符
来源：http://ot.huixinmuqiang.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vd.wgjwhj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qs.chemitech.net.cn

JS:   s.replace(/\s+/g, "")
来源：http://qq.yuntaijiaju.cn

TS:   s.replace(/\s+/g, "")
来源：http://ft.newstarts.cn

Java: s.replaceAll("\\s+", "")
来源：http://ke.szxytkj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://cd.hahajie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://gx.shxzskj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gl.huixiangedu.cn

[E10] 左侧补零 / 定长填充
来源：http://lf.huixiangedu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://iv.wgjwhj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ya.huixiangedu.cn

JS:   "7".padStart(3, "0")
来源：http://jk.shxzskj.cn

TS:   "7".padStart(3, "0")
来源：http://tt.newstarts.cn

Java: String.format("%03d", 7)
来源：http://nq.szsharing.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://df.hahajie.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://or.nszjky.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://yk.shxzukj.cn

[E11] 反转字符串
来源：http://nu.asd995.cn

Py:   s[::-1]
来源：http://ee.bjjhwx.cn

PHP:  strrev($s);
来源：http://oj.jianghongdianzi.cn

JS:   [...s].reverse().join("")
来源：http://wr.nszjky.cn

TS:   [...s].reverse().join("")
来源：http://gf.9csxet.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://tb.szsharing.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://tj.shtwfgs.cn

Ruby: s.reverse
来源：http://hq.huanxung.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ci.asd995.cn

[E12] 统计某字符出现次数
来源：http://mk.nszjky.cn

Py:   s.count("a")
来源：http://lq.muxihuayi.cn

PHP:  substr_count($s, "a");
来源：http://pd.521024.cn

JS:   s.split("a").length - 1
来源：http://ze.nicolike.cn

TS:   s.split("a").length - 1
来源：http://ox.szsharing.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ey.bookmarksfly.cn

Go:   strings.Count(s, "a")
来源：http://yp.521024.cn

Ruby: s.count("a")
来源：http://tb.gzmigu.cn

C#:   s.Count(c => c == 'a')
来源：http://ac.shxzskj.cn

[E13] 逐字符遍历
来源：http://kl.yuexingan06.cn

Py:   for ch in s: print(ch)
来源：http://vo.hnjuh.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kx.521024.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://jb.bookmarksfly.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://kp.jianghongdianzi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fb.colortex.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ts.huanxung.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ui.gzmigu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://pz.szxytkj.cn

[E14] URL 编码与 Base64
来源：http://vz.szxytkj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fn.hnjuh.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://kz.newstarts.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qg.colortex.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xc.bjjhwx.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qw.jianghongdianzi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://lz.panjiajie.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://pw.muxihuayi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fk.yuntaijiaju.cn

[E15] HTML 转义 / 反转义
来源：http://fh.9csxet.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://kd.jianghongdianzi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://uw.yuexingan06.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://va.hnjuh.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://wv.chemitech.net.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tn.shtwfgs.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ll.bjjhwx.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wu.521024.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ne.szxytkj.cn

[E16] 数字千分位
来源：http://yx.shxzskj.cn

Py:   f"{1234567:,}"
来源：http://xx.huixinmuqiang.cn

PHP:  number_format(1234567);
来源：http://zh.haigaiapp.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://fh.nszjky.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://vz.huixiangedu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gl.yuntaijiaju.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://kg.shxzukj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wt.shtwfgs.cn

C#:   1234567.ToString("N0")
来源：http://ra.nszjky.cn

[E17] 首字母大写
来源：http://nt.shtwfgs.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qk.asd995.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://vz.szxytkj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mv.hahajie.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pm.521024.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://lr.jianghongdianzi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ny.huanxung.cn

Ruby: s.capitalize
来源：http://tm.newstarts.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ig.jianghongdianzi.cn

[E18] 模板占位符替换
来源：http://bg.yuntaijiaju.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xt.huixinmuqiang.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ey.hahajie.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ds.chemitech.net.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://iu.yuntaijiaju.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gk.shxzukj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bp.gzmigu.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fg.panjiajie.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wc.yuntaijiaju.cn

[E19] 多行文本按行拆分
来源：http://vo.nicolike.cn

Py:   s.splitlines()
来源：http://wr.szxytkj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cd.asd995.cn

JS:   s.split(/\r?\n/)
来源：http://tl.huixiangedu.cn

TS:   s.split(/\r?\n/)
来源：http://jd.hnjuh.cn

Java: s.lines().toList()
来源：http://qn.lnxyls.cn

Go:   strings.Split(s, "\n")
来源：http://jv.bjjhwx.cn

Ruby: s.lines
来源：http://mj.newstarts.cn

C#:   s.Split('\n')
来源：http://yq.newstarts.cn

[E20] 判断字符串是否为空
来源：http://ni.521024.cn

Py:   if not s:
来源：http://xk.panjiajie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cj.shtwfgs.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://na.haigaiapp.cn

TS:   if (s === "") {}
来源：http://bi.521024.cn

Java: if (s.isEmpty()) {}
来源：http://eh.panjiajie.cn

Go:   if s == "" {}
来源：http://zt.yuexingan06.cn

Ruby: if s.empty?
来源：http://iw.huanxung.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://lu.shxzskj.cn

[E21] 超长截断加省略号
来源：http://ct.newstarts.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nq.jianghongdianzi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://nl.shxzukj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yd.bjjhwx.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wf.nicolike.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ce.newstarts.cn

Go:   // 按 rune 判断长度后截断
来源：http://pz.9csxet.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xf.huixiangedu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ew.9csxet.cn

[E22] 字节长度与字符长度
来源：http://ea.nszjky.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://uo.wgjwhj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ee.panjiajie.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ji.haigaiapp.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cm.jctech888.com.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bl.newstarts.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ui.shxzukj.cn

Ruby: s.bytesize;  s.length
来源：http://ek.shtwfgs.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://iz.panjiajie.cn

================================================================================
来源：http://ny.muxihuayi.cn

F. 文件与目录
来源：http://kc.szsharing.cn

================================================================================
来源：http://bm.yuntaijiaju.cn

[F01] 读取整个文件
来源：http://ew.521024.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fa.yuexingan06.cn

PHP:  file_get_contents("a.txt");
来源：http://xe.lnxyls.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://uo.9csxet.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ow.szsharing.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://xd.asd995.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://th.colortex.cn

Ruby: File.read("a.txt")
来源：http://me.bookmarksfly.cn

C#:   File.ReadAllText("a.txt");
来源：http://vl.haigaiapp.cn

[F02] 逐行读取文件
来源：http://pp.wgjwhj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hi.yuntaijiaju.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xs.shtwfgs.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ib.shxzukj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jg.shxzskj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://nc.muxihuayi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gl.shtwfgs.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dw.shxzukj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xs.newstarts.cn

[F03] 写入文件（覆盖）
来源：http://ib.szsharing.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://au.shtwfgs.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ih.yuexingan06.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bw.muxihuayi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dz.lnxyls.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mu.lnxyls.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://en.yuntaijiaju.cn

Ruby: File.write("a.txt", "hi")
来源：http://wm.szxytkj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bf.shtwfgs.cn

[F04] 追加写入文件
来源：http://xv.szxytkj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ec.gzmigu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tn.bjjhwx.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pc.huixiangedu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ec.hahajie.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://pw.muxihuayi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://yq.gzmigu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rp.hahajie.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://cl.bookmarksfly.cn

[F05] 判断文件或目录是否存在
来源：http://kj.colortex.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kh.colortex.cn

PHP:  file_exists("a.txt");
来源：http://ln.hahajie.cn

JS:   fs.existsSync("a.txt")
来源：http://xy.hnjuh.cn

TS:   fs.existsSync("a.txt")
来源：http://km.9csxet.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://xv.shxzukj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://sv.bookmarksfly.cn

Ruby: File.exist?("a.txt")
来源：http://nu.bookmarksfly.cn

C#:   File.Exists("a.txt")
来源：http://ll.shxzskj.cn

[F06] 删除文件
来源：http://tu.hnjuh.cn

Py:   os.remove("a.txt")
来源：http://ee.szxytkj.cn

PHP:  unlink("a.txt");
来源：http://ly.panjiajie.cn

JS:   fs.unlinkSync("a.txt")
来源：http://bc.shxzukj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://il.jctech888.com.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gg.shxzskj.cn

Go:   os.Remove("a.txt")
来源：http://zx.muxihuayi.cn

Ruby: File.delete("a.txt")
来源：http://gf.yuntaijiaju.cn

C#:   File.Delete("a.txt");
来源：http://dr.newstarts.cn

[F07] 创建目录（含多级）
来源：http://mr.jctech888.com.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sq.asd995.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tk.asd995.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dc.chemitech.net.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fb.521024.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://nm.huanxung.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://pl.haigaiapp.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zx.bookmarksfly.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jr.huixiangedu.cn

[F08] 遍历目录
来源：http://ps.huanxung.cn


<!-- 参考信息 -->