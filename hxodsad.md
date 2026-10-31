代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ss.nszjky.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://qn.newstarts.cn

Go:   // 手写循环
来源：http://ol.nszjky.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zo.bjjhwx.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qj.hnjuh.cn

[D24] 字典 / Map 基本操作
来源：http://nx.521024.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://if.bookmarksfly.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jo.yuntaijiaju.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kx.muxihuayi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://im.yuexingan06.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://he.asd995.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://sv.huanxung.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zw.yuntaijiaju.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pu.yuntaijiaju.cn

[D25] Set 集合去重与交并差
来源：http://he.jctech888.com.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://pc.shxzskj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ax.shtwfgs.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gt.huixinmuqiang.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vz.colortex.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dq.szsharing.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://bv.haigaiapp.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://be.huanxung.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nm.521024.cn

[D26] 数组转字符串
来源：http://vw.lnxyls.cn

Py:   ", ".join(map(str, arr))
来源：http://uo.yuexingan06.cn

PHP:  implode(", ", $arr);
来源：http://aa.shtwfgs.cn

JS:   arr.join(", ")
来源：http://ej.muxihuayi.cn

TS:   arr.join(", ")
来源：http://qw.wgjwhj.cn

Java: String.join(", ", list)
来源：http://jd.muxihuayi.cn

Go:   strings.Join(strs, ", ")
来源：http://yt.nszjky.cn

Ruby: arr.join(", ")
来源：http://mf.lnxyls.cn

C#:   string.Join(", ", list)
来源：http://ey.bookmarksfly.cn

================================================================================
来源：http://nn.shxzukj.cn

E. 字符串处理
来源：http://sj.huanxung.cn

================================================================================
来源：http://lz.haigaiapp.cn

[E01] 拼接字符串
来源：http://ck.panjiajie.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hu.haigaiapp.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://bk.huanxung.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mf.panjiajie.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wg.gzmigu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ox.muxihuayi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ua.wgjwhj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gy.521024.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xi.jianghongdianzi.cn

[E02] 重复字符串
来源：http://fx.chemitech.net.cn

Py:   "ab" * 3
来源：http://bv.shtwfgs.cn

PHP:  str_repeat("ab", 3);
来源：http://vo.nszjky.cn

JS:   "ab".repeat(3)
来源：http://tl.jctech888.com.cn

TS:   "ab".repeat(3)
来源：http://bc.muxihuayi.cn

Java: "ab".repeat(3)
来源：http://to.521024.cn

Go:   strings.Repeat("ab", 3)
来源：http://si.muxihuayi.cn

Ruby: "ab" * 3
来源：http://vn.szxytkj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ks.jianghongdianzi.cn

[E03] 截取子串
来源：http://yy.wgjwhj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xe.shxzukj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ng.yuntaijiaju.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jd.panjiajie.cn

TS:   s.slice(1, 4)
来源：http://xv.szsharing.cn

Java: s.substring(1, 4)
来源：http://us.bjjhwx.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xm.lnxyls.cn

Ruby: s[1, 3];  s[1..3]
来源：http://oh.wgjwhj.cn

C#:   s.Substring(1, 3)
来源：http://vj.newstarts.cn

[E04] 查找子串位置
来源：http://fa.szsharing.cn

Py:   s.find("x");  s.index("x")
来源：http://rr.521024.cn

PHP:  strpos($s, "x");
来源：http://so.yuntaijiaju.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vm.yuexingan06.cn

TS:   s.indexOf("x")
来源：http://ds.szxytkj.cn

Java: s.indexOf("x")
来源：http://fb.9csxet.cn

Go:   strings.Index(s, "x")
来源：http://cf.shtwfgs.cn

Ruby: s.index("x")
来源：http://oc.521024.cn

C#:   s.IndexOf("x")
来源：http://ef.yuntaijiaju.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://kx.shtwfgs.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hd.521024.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://tm.muxihuayi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vg.hnjuh.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://gk.shtwfgs.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://go.jctech888.com.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jd.hahajie.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zr.nicolike.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ej.nszjky.cn

[E06] 替换子串
来源：http://lb.9csxet.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kg.asd995.cn

PHP:  str_replace("a", "b", $s);
来源：http://bi.bookmarksfly.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yx.szsharing.cn

TS:   s.replaceAll("a", "b")
来源：http://gf.hahajie.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ia.asd995.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://dn.nszjky.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dl.panjiajie.cn

C#:   s.Replace("a", "b")
来源：http://tu.jctech888.com.cn

[E07] 按分隔符拆分
来源：http://tb.hnjuh.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ru.shxzukj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://do.szsharing.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://iz.lnxyls.cn

TS:   s.split(",")
来源：http://wu.nszjky.cn

Java: s.split(",");  s.split("\\s+")
来源：http://db.shxzukj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://na.nicolike.cn

Ruby: s.split(",");  s.split
来源：http://fo.bookmarksfly.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zr.bookmarksfly.cn

[E08] 数组按分隔符合并
来源：http://pv.hnjuh.cn

Py:   ",".join(items)
来源：http://ot.wgjwhj.cn

PHP:  implode(",", $items);
来源：http://ny.hnjuh.cn

JS:   items.join(",")
来源：http://hc.muxihuayi.cn

TS:   items.join(",")
来源：http://li.521024.cn

Java: String.join(",", items)
来源：http://bm.nszjky.cn

Go:   strings.Join(items, ",")
来源：http://xl.asd995.cn

Ruby: items.join(",")
来源：http://sc.hahajie.cn

C#:   string.Join(",", items)
来源：http://lp.lnxyls.cn

[E09] 去除所有空白字符
来源：http://ei.newstarts.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nc.nszjky.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jr.yuntaijiaju.cn

JS:   s.replace(/\s+/g, "")
来源：http://xy.wgjwhj.cn

TS:   s.replace(/\s+/g, "")
来源：http://wa.huixinmuqiang.cn

Java: s.replaceAll("\\s+", "")
来源：http://zc.panjiajie.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://xu.asd995.cn

Ruby: s.gsub(/\s+/, "")
来源：http://qk.lnxyls.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vc.colortex.cn

[E10] 左侧补零 / 定长填充
来源：http://on.hahajie.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mx.wgjwhj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jz.hnjuh.cn

JS:   "7".padStart(3, "0")
来源：http://il.hahajie.cn

TS:   "7".padStart(3, "0")
来源：http://bc.bookmarksfly.cn

Java: String.format("%03d", 7)
来源：http://ip.9csxet.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://jb.521024.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lx.yuexingan06.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rn.nszjky.cn

[E11] 反转字符串
来源：http://qy.colortex.cn

Py:   s[::-1]
来源：http://fz.asd995.cn

PHP:  strrev($s);
来源：http://us.shtwfgs.cn

JS:   [...s].reverse().join("")
来源：http://pm.hahajie.cn

TS:   [...s].reverse().join("")
来源：http://eh.huanxung.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ma.muxihuayi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ct.hahajie.cn

Ruby: s.reverse
来源：http://ar.521024.cn

C#:   new string(s.Reverse().ToArray())
来源：http://mx.shxzukj.cn

[E12] 统计某字符出现次数
来源：http://sq.bjjhwx.cn

Py:   s.count("a")
来源：http://xm.nszjky.cn

PHP:  substr_count($s, "a");
来源：http://zm.shxzskj.cn

JS:   s.split("a").length - 1
来源：http://ah.shtwfgs.cn

TS:   s.split("a").length - 1
来源：http://gb.haigaiapp.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://pd.9csxet.cn

Go:   strings.Count(s, "a")
来源：http://on.9csxet.cn

Ruby: s.count("a")
来源：http://dv.yuntaijiaju.cn

C#:   s.Count(c => c == 'a')
来源：http://hp.haigaiapp.cn

[E13] 逐字符遍历
来源：http://xq.asd995.cn

Py:   for ch in s: print(ch)
来源：http://ti.huixinmuqiang.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://cu.gzmigu.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ui.huixinmuqiang.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://gk.shtwfgs.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://en.shxzukj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://bc.szxytkj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://oh.muxihuayi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://yt.huixiangedu.cn

[E14] URL 编码与 Base64
来源：http://ez.lnxyls.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://cw.jianghongdianzi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://tn.shxzukj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mq.szxytkj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ze.jianghongdianzi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://pm.jctech888.com.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fz.shxzskj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://uy.gzmigu.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rm.huanxung.cn

[E15] HTML 转义 / 反转义
来源：http://md.muxihuayi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ny.hnjuh.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ht.huixinmuqiang.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hc.lnxyls.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://qi.bjjhwx.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wn.hnjuh.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xm.nszjky.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ck.hahajie.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://tv.huixinmuqiang.cn

[E16] 数字千分位
来源：http://um.colortex.cn

Py:   f"{1234567:,}"
来源：http://ik.chemitech.net.cn

PHP:  number_format(1234567);
来源：http://ze.lnxyls.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://kg.bjjhwx.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://tz.bjjhwx.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://kl.jianghongdianzi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ch.521024.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://on.bookmarksfly.cn

C#:   1234567.ToString("N0")
来源：http://lc.shtwfgs.cn

[E17] 首字母大写
来源：http://ec.huixiangedu.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xy.huixiangedu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ty.gzmigu.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sy.bookmarksfly.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zh.muxihuayi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://sx.yuexingan06.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lw.huixiangedu.cn

Ruby: s.capitalize
来源：http://am.9csxet.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vp.asd995.cn

[E18] 模板占位符替换
来源：http://ju.szsharing.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://iv.yuntaijiaju.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wd.nicolike.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://yp.newstarts.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://jz.shxzukj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://oo.jctech888.com.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wz.521024.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vl.nicolike.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bw.nicolike.cn

[E19] 多行文本按行拆分
来源：http://aj.szsharing.cn

Py:   s.splitlines()
来源：http://go.shxzukj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://yq.bjjhwx.cn

JS:   s.split(/\r?\n/)
来源：http://rm.hnjuh.cn

TS:   s.split(/\r?\n/)
来源：http://fd.shxzukj.cn

Java: s.lines().toList()
来源：http://ig.wgjwhj.cn

Go:   strings.Split(s, "\n")
来源：http://vk.jctech888.com.cn

Ruby: s.lines
来源：http://gh.asd995.cn

C#:   s.Split('\n')
来源：http://hq.colortex.cn

[E20] 判断字符串是否为空
来源：http://vq.chemitech.net.cn

Py:   if not s:
来源：http://nc.yuntaijiaju.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://nu.jctech888.com.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ey.jianghongdianzi.cn

TS:   if (s === "") {}
来源：http://xn.colortex.cn

Java: if (s.isEmpty()) {}
来源：http://tc.9csxet.cn

Go:   if s == "" {}
来源：http://rd.bjjhwx.cn

Ruby: if s.empty?
来源：http://fi.bookmarksfly.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bn.huixinmuqiang.cn

[E21] 超长截断加省略号
来源：http://dc.haigaiapp.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xk.szsharing.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://eh.panjiajie.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sj.huixinmuqiang.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uy.szsharing.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bn.asd995.cn

Go:   // 按 rune 判断长度后截断
来源：http://wi.huanxung.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wz.szxytkj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://eo.jctech888.com.cn

[E22] 字节长度与字符长度
来源：http://ep.huanxung.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bc.huixiangedu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jy.bjjhwx.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ng.newstarts.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bj.bookmarksfly.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zg.bjjhwx.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rm.bjjhwx.cn

Ruby: s.bytesize;  s.length
来源：http://ry.jianghongdianzi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wt.muxihuayi.cn

================================================================================
来源：http://po.colortex.cn

F. 文件与目录
来源：http://vx.jianghongdianzi.cn

================================================================================
来源：http://tq.haigaiapp.cn

[F01] 读取整个文件
来源：http://sa.panjiajie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hn.gzmigu.cn

PHP:  file_get_contents("a.txt");
来源：http://yc.newstarts.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wc.nszjky.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zs.colortex.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://pz.yuntaijiaju.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ue.lnxyls.cn

Ruby: File.read("a.txt")
来源：http://zj.lnxyls.cn

C#:   File.ReadAllText("a.txt");
来源：http://wt.shxzskj.cn

[F02] 逐行读取文件
来源：http://tg.gzmigu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xr.shxzukj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://lw.jctech888.com.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://oi.chemitech.net.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tz.jctech888.com.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://oq.yuexingan06.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xn.nszjky.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wx.jianghongdianzi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://kr.hahajie.cn

[F03] 写入文件（覆盖）
来源：http://wo.shxzskj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ro.yuexingan06.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://us.newstarts.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://oo.yuexingan06.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ya.gzmigu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lq.muxihuayi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ew.hnjuh.cn

Ruby: File.write("a.txt", "hi")
来源：http://ex.jianghongdianzi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ey.chemitech.net.cn

[F04] 追加写入文件
来源：http://up.colortex.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dp.newstarts.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gn.jctech888.com.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://of.jctech888.com.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ij.521024.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://sx.bookmarksfly.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bd.haigaiapp.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vc.jianghongdianzi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://is.huixiangedu.cn

[F05] 判断文件或目录是否存在
来源：http://sr.muxihuayi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ko.jctech888.com.cn

PHP:  file_exists("a.txt");
来源：http://uy.muxihuayi.cn

JS:   fs.existsSync("a.txt")
来源：http://mo.asd995.cn

TS:   fs.existsSync("a.txt")
来源：http://zc.huixiangedu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ni.huixinmuqiang.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mp.newstarts.cn

Ruby: File.exist?("a.txt")
来源：http://qc.jctech888.com.cn

C#:   File.Exists("a.txt")
来源：http://rm.9csxet.cn

[F06] 删除文件
来源：http://be.lnxyls.cn

Py:   os.remove("a.txt")
来源：http://px.szsharing.cn

PHP:  unlink("a.txt");
来源：http://or.huixiangedu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ji.lnxyls.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ob.521024.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gk.asd995.cn

Go:   os.Remove("a.txt")
来源：http://mv.jctech888.com.cn

Ruby: File.delete("a.txt")
来源：http://ue.szxytkj.cn

C#:   File.Delete("a.txt");
来源：http://nz.huixinmuqiang.cn

[F07] 创建目录（含多级）
来源：http://kr.muxihuayi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vb.hnjuh.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ql.yuexingan06.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qv.chemitech.net.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ae.haigaiapp.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ng.shxzukj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mq.huanxung.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gx.colortex.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://re.nszjky.cn

[F08] 遍历目录
来源：http://sf.haigaiapp.cn


<!-- 参考信息 -->