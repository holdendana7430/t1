代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xy.shxzskj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://rz.yuntaijiaju.cn

Go:   // 手写循环
来源：http://zl.bjjhwx.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bp.hahajie.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zj.asd995.cn

[D24] 字典 / Map 基本操作
来源：http://iu.asd995.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pg.szsharing.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vo.huanxung.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tz.wgjwhj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ek.shtwfgs.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zv.lnxyls.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mu.newstarts.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hg.colortex.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://oj.lnxyls.cn

[D25] Set 集合去重与交并差
来源：http://wy.shxzukj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zg.huanxung.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wi.jianghongdianzi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gr.huanxung.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mk.wgjwhj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xg.asd995.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vv.asd995.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://on.521024.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://tp.nicolike.cn

[D26] 数组转字符串
来源：http://xc.hahajie.cn

Py:   ", ".join(map(str, arr))
来源：http://lh.yuexingan06.cn

PHP:  implode(", ", $arr);
来源：http://hf.hahajie.cn

JS:   arr.join(", ")
来源：http://md.newstarts.cn

TS:   arr.join(", ")
来源：http://bh.haigaiapp.cn

Java: String.join(", ", list)
来源：http://qg.huixiangedu.cn

Go:   strings.Join(strs, ", ")
来源：http://bf.asd995.cn

Ruby: arr.join(", ")
来源：http://vw.haigaiapp.cn

C#:   string.Join(", ", list)
来源：http://nr.wgjwhj.cn

================================================================================
来源：http://fp.shxzskj.cn

E. 字符串处理
来源：http://ic.szsharing.cn

================================================================================
来源：http://jk.521024.cn

[E01] 拼接字符串
来源：http://yh.muxihuayi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://sq.521024.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://sz.yuexingan06.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tz.haigaiapp.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xa.jianghongdianzi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://yh.nszjky.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ba.newstarts.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mb.521024.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kj.huanxung.cn

[E02] 重复字符串
来源：http://fp.nicolike.cn

Py:   "ab" * 3
来源：http://ia.bookmarksfly.cn

PHP:  str_repeat("ab", 3);
来源：http://yh.newstarts.cn

JS:   "ab".repeat(3)
来源：http://fa.shtwfgs.cn

TS:   "ab".repeat(3)
来源：http://fa.shxzukj.cn

Java: "ab".repeat(3)
来源：http://sp.shtwfgs.cn

Go:   strings.Repeat("ab", 3)
来源：http://wi.nszjky.cn

Ruby: "ab" * 3
来源：http://xu.huixinmuqiang.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://pl.gzmigu.cn

[E03] 截取子串
来源：http://aj.nszjky.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wg.wgjwhj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://sn.colortex.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://sv.hahajie.cn

TS:   s.slice(1, 4)
来源：http://kl.shxzukj.cn

Java: s.substring(1, 4)
来源：http://va.yuntaijiaju.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rt.hahajie.cn

Ruby: s[1, 3];  s[1..3]
来源：http://lp.haigaiapp.cn

C#:   s.Substring(1, 3)
来源：http://ol.hnjuh.cn

[E04] 查找子串位置
来源：http://hi.hahajie.cn

Py:   s.find("x");  s.index("x")
来源：http://ba.haigaiapp.cn

PHP:  strpos($s, "x");
来源：http://be.yuexingan06.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ed.shxzukj.cn

TS:   s.indexOf("x")
来源：http://qa.haigaiapp.cn

Java: s.indexOf("x")
来源：http://iz.bjjhwx.cn

Go:   strings.Index(s, "x")
来源：http://ce.szxytkj.cn

Ruby: s.index("x")
来源：http://iu.yuntaijiaju.cn

C#:   s.IndexOf("x")
来源：http://pl.asd995.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ps.chemitech.net.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://pn.panjiajie.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mu.huixinmuqiang.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gr.nszjky.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ho.jianghongdianzi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vk.wgjwhj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ok.shxzukj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wd.chemitech.net.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://tr.hahajie.cn

[E06] 替换子串
来源：http://mw.muxihuayi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zx.szxytkj.cn

PHP:  str_replace("a", "b", $s);
来源：http://pd.haigaiapp.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ko.jianghongdianzi.cn

TS:   s.replaceAll("a", "b")
来源：http://uu.huixiangedu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dd.lnxyls.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://sp.szxytkj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ip.nicolike.cn

C#:   s.Replace("a", "b")
来源：http://cs.haigaiapp.cn

[E07] 按分隔符拆分
来源：http://qt.asd995.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mf.hahajie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kc.nszjky.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://se.huanxung.cn

TS:   s.split(",")
来源：http://nk.haigaiapp.cn

Java: s.split(",");  s.split("\\s+")
来源：http://uc.huixiangedu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hs.asd995.cn

Ruby: s.split(",");  s.split
来源：http://pf.huixiangedu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vu.chemitech.net.cn

[E08] 数组按分隔符合并
来源：http://gb.haigaiapp.cn

Py:   ",".join(items)
来源：http://tu.jctech888.com.cn

PHP:  implode(",", $items);
来源：http://pr.shxzukj.cn

JS:   items.join(",")
来源：http://uw.huixinmuqiang.cn

TS:   items.join(",")
来源：http://tn.huixinmuqiang.cn

Java: String.join(",", items)
来源：http://mi.jianghongdianzi.cn

Go:   strings.Join(items, ",")
来源：http://ke.yuexingan06.cn

Ruby: items.join(",")
来源：http://si.nicolike.cn

C#:   string.Join(",", items)
来源：http://rm.asd995.cn

[E09] 去除所有空白字符
来源：http://rr.shxzskj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mi.newstarts.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wh.huanxung.cn

JS:   s.replace(/\s+/g, "")
来源：http://jw.nicolike.cn

TS:   s.replace(/\s+/g, "")
来源：http://xj.haigaiapp.cn

Java: s.replaceAll("\\s+", "")
来源：http://is.9csxet.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://it.yuexingan06.cn

Ruby: s.gsub(/\s+/, "")
来源：http://em.521024.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://id.hahajie.cn

[E10] 左侧补零 / 定长填充
来源：http://bq.huixiangedu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://sp.lnxyls.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tr.chemitech.net.cn

JS:   "7".padStart(3, "0")
来源：http://bj.jianghongdianzi.cn

TS:   "7".padStart(3, "0")
来源：http://ya.panjiajie.cn

Java: String.format("%03d", 7)
来源：http://ep.shxzukj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://go.lnxyls.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://nb.newstarts.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fy.shtwfgs.cn

[E11] 反转字符串
来源：http://dn.szxytkj.cn

Py:   s[::-1]
来源：http://zw.9csxet.cn

PHP:  strrev($s);
来源：http://iv.hnjuh.cn

JS:   [...s].reverse().join("")
来源：http://zb.bjjhwx.cn

TS:   [...s].reverse().join("")
来源：http://ke.huixiangedu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://uh.hnjuh.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ab.jianghongdianzi.cn

Ruby: s.reverse
来源：http://wh.hahajie.cn

C#:   new string(s.Reverse().ToArray())
来源：http://mc.huixinmuqiang.cn

[E12] 统计某字符出现次数
来源：http://ui.shxzskj.cn

Py:   s.count("a")
来源：http://lq.gzmigu.cn

PHP:  substr_count($s, "a");
来源：http://hh.huixinmuqiang.cn

JS:   s.split("a").length - 1
来源：http://fn.jctech888.com.cn

TS:   s.split("a").length - 1
来源：http://yc.colortex.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xq.chemitech.net.cn

Go:   strings.Count(s, "a")
来源：http://yl.jianghongdianzi.cn

Ruby: s.count("a")
来源：http://wj.521024.cn

C#:   s.Count(c => c == 'a')
来源：http://et.yuntaijiaju.cn

[E13] 逐字符遍历
来源：http://me.nszjky.cn

Py:   for ch in s: print(ch)
来源：http://to.muxihuayi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ip.yuexingan06.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://qp.bjjhwx.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://vh.wgjwhj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://np.asd995.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kn.colortex.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ik.nszjky.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://oi.521024.cn

[E14] URL 编码与 Base64
来源：http://lp.shtwfgs.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gs.szsharing.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://tk.jctech888.com.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://yp.huixinmuqiang.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://lh.szsharing.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://un.szsharing.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://oe.jianghongdianzi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bk.asd995.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rb.chemitech.net.cn

[E15] HTML 转义 / 反转义
来源：http://om.panjiajie.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://lc.bookmarksfly.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vc.jianghongdianzi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zy.szsharing.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://jm.huixiangedu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://on.panjiajie.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rs.bjjhwx.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://sb.huixinmuqiang.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qv.muxihuayi.cn

[E16] 数字千分位
来源：http://dd.jianghongdianzi.cn

Py:   f"{1234567:,}"
来源：http://pr.muxihuayi.cn

PHP:  number_format(1234567);
来源：http://zn.9csxet.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ny.newstarts.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://tl.gzmigu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://om.shxzukj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://on.huixiangedu.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zr.521024.cn

C#:   1234567.ToString("N0")
来源：http://lg.bjjhwx.cn

[E17] 首字母大写
来源：http://mf.lnxyls.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ko.nszjky.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://cq.shxzskj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dk.chemitech.net.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://me.huixiangedu.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ni.bookmarksfly.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vq.wgjwhj.cn

Ruby: s.capitalize
来源：http://rr.bookmarksfly.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ol.haigaiapp.cn

[E18] 模板占位符替换
来源：http://lx.bookmarksfly.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ab.521024.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gi.szxytkj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://gp.shxzskj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://fw.chemitech.net.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nc.shtwfgs.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mw.huixinmuqiang.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wx.lnxyls.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mw.shtwfgs.cn

[E19] 多行文本按行拆分
来源：http://om.hahajie.cn

Py:   s.splitlines()
来源：http://tx.nicolike.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hg.gzmigu.cn

JS:   s.split(/\r?\n/)
来源：http://hz.szxytkj.cn

TS:   s.split(/\r?\n/)
来源：http://qf.shtwfgs.cn

Java: s.lines().toList()
来源：http://nh.bjjhwx.cn

Go:   strings.Split(s, "\n")
来源：http://es.shtwfgs.cn

Ruby: s.lines
来源：http://qb.shxzukj.cn

C#:   s.Split('\n')
来源：http://bi.hahajie.cn

[E20] 判断字符串是否为空
来源：http://ou.yuntaijiaju.cn

Py:   if not s:
来源：http://uf.shxzskj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rl.asd995.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://cv.521024.cn

TS:   if (s === "") {}
来源：http://if.gzmigu.cn

Java: if (s.isEmpty()) {}
来源：http://gu.szxytkj.cn

Go:   if s == "" {}
来源：http://mi.chemitech.net.cn

Ruby: if s.empty?
来源：http://tl.wgjwhj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ye.szsharing.cn

[E21] 超长截断加省略号
来源：http://pr.9csxet.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ci.szxytkj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://eb.wgjwhj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ut.huixinmuqiang.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://am.gzmigu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hq.huixinmuqiang.cn

Go:   // 按 rune 判断长度后截断
来源：http://fn.wgjwhj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yg.szsharing.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://yt.shxzukj.cn

[E22] 字节长度与字符长度
来源：http://sn.asd995.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gm.9csxet.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ig.bookmarksfly.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jd.jianghongdianzi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yg.huixinmuqiang.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vh.jianghongdianzi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wq.haigaiapp.cn

Ruby: s.bytesize;  s.length
来源：http://lp.gzmigu.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wt.wgjwhj.cn

================================================================================
来源：http://um.newstarts.cn

F. 文件与目录
来源：http://cd.nicolike.cn

================================================================================
来源：http://wm.bookmarksfly.cn

[F01] 读取整个文件
来源：http://ys.shxzukj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rq.shtwfgs.cn

PHP:  file_get_contents("a.txt");
来源：http://nm.szxytkj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rh.yuntaijiaju.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://pf.colortex.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://zl.bookmarksfly.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://bo.shtwfgs.cn

Ruby: File.read("a.txt")
来源：http://jd.muxihuayi.cn

C#:   File.ReadAllText("a.txt");
来源：http://hq.asd995.cn

[F02] 逐行读取文件
来源：http://kn.szsharing.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://sg.huanxung.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ue.bjjhwx.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://oi.lnxyls.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gg.hahajie.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wi.szsharing.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ze.huixinmuqiang.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://cq.hahajie.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dn.haigaiapp.cn

[F03] 写入文件（覆盖）
来源：http://zn.muxihuayi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ho.haigaiapp.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://yx.huixiangedu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zn.lnxyls.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ug.huixinmuqiang.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jj.jctech888.com.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nf.nszjky.cn

Ruby: File.write("a.txt", "hi")
来源：http://ku.hnjuh.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ii.hahajie.cn

[F04] 追加写入文件
来源：http://sp.szsharing.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://if.szsharing.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ie.chemitech.net.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cf.521024.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ju.colortex.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ni.yuexingan06.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dr.shxzskj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xj.jianghongdianzi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://em.chemitech.net.cn

[F05] 判断文件或目录是否存在
来源：http://ai.haigaiapp.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vo.szsharing.cn

PHP:  file_exists("a.txt");
来源：http://mk.huanxung.cn

JS:   fs.existsSync("a.txt")
来源：http://bo.newstarts.cn

TS:   fs.existsSync("a.txt")
来源：http://cb.panjiajie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://at.wgjwhj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://cy.9csxet.cn

Ruby: File.exist?("a.txt")
来源：http://eh.jctech888.com.cn

C#:   File.Exists("a.txt")
来源：http://ai.asd995.cn

[F06] 删除文件
来源：http://vi.shxzskj.cn

Py:   os.remove("a.txt")
来源：http://tn.szxytkj.cn

PHP:  unlink("a.txt");
来源：http://kw.muxihuayi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://el.asd995.cn

TS:   fs.unlinkSync("a.txt")
来源：http://zy.yuexingan06.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://cj.newstarts.cn

Go:   os.Remove("a.txt")
来源：http://ww.huixinmuqiang.cn

Ruby: File.delete("a.txt")
来源：http://cx.huixiangedu.cn

C#:   File.Delete("a.txt");
来源：http://vi.hahajie.cn

[F07] 创建目录（含多级）
来源：http://av.nicolike.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wm.lnxyls.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cq.shtwfgs.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sc.shxzskj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ti.haigaiapp.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vp.9csxet.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rx.panjiajie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ng.shxzukj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ua.panjiajie.cn

[F08] 遍历目录
来源：http://bt.shxzskj.cn


<!-- 参考信息 -->