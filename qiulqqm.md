代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mm.huixiangedu.cn

[D24] 字典 / Map 基本操作
来源：http://bf.newstarts.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qx.hnjuh.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ln.haigaiapp.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://en.huixinmuqiang.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://be.newstarts.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://yh.chemitech.net.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://kl.chemitech.net.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zs.shxzskj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ty.bookmarksfly.cn

[D25] Set 集合去重与交并差
来源：http://ma.lnxyls.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ne.chemitech.net.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://lq.haigaiapp.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://nt.haigaiapp.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://md.wgjwhj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bj.shxzukj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vx.chemitech.net.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pe.newstarts.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zn.521024.cn

[D26] 数组转字符串
来源：http://rq.yuntaijiaju.cn

Py:   ", ".join(map(str, arr))
来源：http://fn.jctech888.com.cn

PHP:  implode(", ", $arr);
来源：http://nj.chemitech.net.cn

JS:   arr.join(", ")
来源：http://tn.asd995.cn

TS:   arr.join(", ")
来源：http://lg.hnjuh.cn

Java: String.join(", ", list)
来源：http://tz.szsharing.cn

Go:   strings.Join(strs, ", ")
来源：http://hf.haigaiapp.cn

Ruby: arr.join(", ")
来源：http://ei.shtwfgs.cn

C#:   string.Join(", ", list)
来源：http://ea.shxzukj.cn

================================================================================
来源：http://mn.huixiangedu.cn

E. 字符串处理
来源：http://rv.nszjky.cn

================================================================================
来源：http://ac.shtwfgs.cn

[E01] 拼接字符串
来源：http://jg.asd995.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ar.colortex.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rg.nicolike.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hn.bjjhwx.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ig.9csxet.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wn.haigaiapp.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://it.szxytkj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fp.hnjuh.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://do.asd995.cn

[E02] 重复字符串
来源：http://xs.huanxung.cn

Py:   "ab" * 3
来源：http://gx.yuexingan06.cn

PHP:  str_repeat("ab", 3);
来源：http://ru.huixinmuqiang.cn

JS:   "ab".repeat(3)
来源：http://xf.9csxet.cn

TS:   "ab".repeat(3)
来源：http://ku.shtwfgs.cn

Java: "ab".repeat(3)
来源：http://zt.huanxung.cn

Go:   strings.Repeat("ab", 3)
来源：http://hi.shtwfgs.cn

Ruby: "ab" * 3
来源：http://uy.huixinmuqiang.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hr.shxzukj.cn

[E03] 截取子串
来源：http://ja.jianghongdianzi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://fg.asd995.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://lh.chemitech.net.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://po.shxzskj.cn

TS:   s.slice(1, 4)
来源：http://ro.nicolike.cn

Java: s.substring(1, 4)
来源：http://cl.hnjuh.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rq.huanxung.cn

Ruby: s[1, 3];  s[1..3]
来源：http://bo.chemitech.net.cn

C#:   s.Substring(1, 3)
来源：http://st.panjiajie.cn

[E04] 查找子串位置
来源：http://qs.yuntaijiaju.cn

Py:   s.find("x");  s.index("x")
来源：http://fi.bookmarksfly.cn

PHP:  strpos($s, "x");
来源：http://dq.asd995.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://es.9csxet.cn

TS:   s.indexOf("x")
来源：http://bi.nszjky.cn

Java: s.indexOf("x")
来源：http://en.nicolike.cn

Go:   strings.Index(s, "x")
来源：http://el.wgjwhj.cn

Ruby: s.index("x")
来源：http://vy.hahajie.cn

C#:   s.IndexOf("x")
来源：http://jq.bookmarksfly.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://cj.muxihuayi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xn.shtwfgs.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kl.bookmarksfly.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ke.huanxung.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ji.nicolike.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gj.szsharing.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://rq.panjiajie.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ce.szxytkj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ji.muxihuayi.cn

[E06] 替换子串
来源：http://fz.yuexingan06.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fq.huanxung.cn

PHP:  str_replace("a", "b", $s);
来源：http://cz.colortex.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fl.bookmarksfly.cn

TS:   s.replaceAll("a", "b")
来源：http://gy.panjiajie.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xk.huixiangedu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fv.bjjhwx.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nq.nicolike.cn

C#:   s.Replace("a", "b")
来源：http://vg.colortex.cn

[E07] 按分隔符拆分
来源：http://ey.521024.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ul.lnxyls.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bt.wgjwhj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://xf.huixiangedu.cn

TS:   s.split(",")
来源：http://il.asd995.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ke.521024.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wh.haigaiapp.cn

Ruby: s.split(",");  s.split
来源：http://ty.shxzskj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://po.muxihuayi.cn

[E08] 数组按分隔符合并
来源：http://mg.jctech888.com.cn

Py:   ",".join(items)
来源：http://hw.shxzskj.cn

PHP:  implode(",", $items);
来源：http://ak.gzmigu.cn

JS:   items.join(",")
来源：http://ta.chemitech.net.cn

TS:   items.join(",")
来源：http://pv.asd995.cn

Java: String.join(",", items)
来源：http://ja.hnjuh.cn

Go:   strings.Join(items, ",")
来源：http://cm.521024.cn

Ruby: items.join(",")
来源：http://jr.nicolike.cn

C#:   string.Join(",", items)
来源：http://se.gzmigu.cn

[E09] 去除所有空白字符
来源：http://zb.bjjhwx.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://gk.521024.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ww.szxytkj.cn

JS:   s.replace(/\s+/g, "")
来源：http://ag.hahajie.cn

TS:   s.replace(/\s+/g, "")
来源：http://pp.9csxet.cn

Java: s.replaceAll("\\s+", "")
来源：http://lg.nicolike.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://am.hahajie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://en.jianghongdianzi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fo.nicolike.cn

[E10] 左侧补零 / 定长填充
来源：http://nc.szsharing.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zt.nicolike.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xv.huixinmuqiang.cn

JS:   "7".padStart(3, "0")
来源：http://lj.shxzskj.cn

TS:   "7".padStart(3, "0")
来源：http://zu.huixinmuqiang.cn

Java: String.format("%03d", 7)
来源：http://pp.huixinmuqiang.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ft.wgjwhj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wz.bookmarksfly.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zx.shxzskj.cn

[E11] 反转字符串
来源：http://hg.colortex.cn

Py:   s[::-1]
来源：http://wv.colortex.cn

PHP:  strrev($s);
来源：http://dg.shtwfgs.cn

JS:   [...s].reverse().join("")
来源：http://cm.muxihuayi.cn

TS:   [...s].reverse().join("")
来源：http://ge.shxzukj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ro.panjiajie.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ta.wgjwhj.cn

Ruby: s.reverse
来源：http://gy.szsharing.cn

C#:   new string(s.Reverse().ToArray())
来源：http://nk.huixiangedu.cn

[E12] 统计某字符出现次数
来源：http://zf.bjjhwx.cn

Py:   s.count("a")
来源：http://os.huixinmuqiang.cn

PHP:  substr_count($s, "a");
来源：http://by.gzmigu.cn

JS:   s.split("a").length - 1
来源：http://dl.nicolike.cn

TS:   s.split("a").length - 1
来源：http://ll.lnxyls.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xg.yuntaijiaju.cn

Go:   strings.Count(s, "a")
来源：http://fr.521024.cn

Ruby: s.count("a")
来源：http://ql.wgjwhj.cn

C#:   s.Count(c => c == 'a')
来源：http://vy.colortex.cn

[E13] 逐字符遍历
来源：http://iy.huanxung.cn

Py:   for ch in s: print(ch)
来源：http://tt.shxzukj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://il.huixinmuqiang.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://xp.asd995.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://uw.521024.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://nw.hahajie.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fp.jctech888.com.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://wa.lnxyls.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gp.gzmigu.cn

[E14] URL 编码与 Base64
来源：http://zq.nicolike.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://go.shxzukj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://pe.yuntaijiaju.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://is.hahajie.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tt.shxzukj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://pm.chemitech.net.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cf.jctech888.com.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://it.muxihuayi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jt.asd995.cn

[E15] HTML 转义 / 反转义
来源：http://oh.bookmarksfly.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://uf.szsharing.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://sg.shtwfgs.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://te.chemitech.net.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://jl.huixinmuqiang.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xj.newstarts.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://dg.szsharing.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pa.9csxet.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lm.nszjky.cn

[E16] 数字千分位
来源：http://ey.shxzukj.cn

Py:   f"{1234567:,}"
来源：http://ym.newstarts.cn

PHP:  number_format(1234567);
来源：http://yg.huanxung.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://xk.nicolike.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://wu.nicolike.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wl.hahajie.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://dq.nszjky.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fm.huanxung.cn

C#:   1234567.ToString("N0")
来源：http://bb.jctech888.com.cn

[E17] 首字母大写
来源：http://zw.huixiangedu.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vw.chemitech.net.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://nb.muxihuayi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ob.shxzskj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://su.gzmigu.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ik.yuntaijiaju.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://cs.szsharing.cn

Ruby: s.capitalize
来源：http://si.huanxung.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xl.shxzukj.cn

[E18] 模板占位符替换
来源：http://qd.huixiangedu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kj.haigaiapp.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://io.yuntaijiaju.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://qz.521024.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://fu.yuexingan06.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ud.shtwfgs.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vo.shtwfgs.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hj.huixinmuqiang.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gu.haigaiapp.cn

[E19] 多行文本按行拆分
来源：http://us.bookmarksfly.cn

Py:   s.splitlines()
来源：http://fy.huixinmuqiang.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hp.wgjwhj.cn

JS:   s.split(/\r?\n/)
来源：http://ds.521024.cn

TS:   s.split(/\r?\n/)
来源：http://mh.huixinmuqiang.cn

Java: s.lines().toList()
来源：http://fe.szxytkj.cn

Go:   strings.Split(s, "\n")
来源：http://gq.shtwfgs.cn

Ruby: s.lines
来源：http://kt.huixiangedu.cn

C#:   s.Split('\n')
来源：http://cb.shxzukj.cn

[E20] 判断字符串是否为空
来源：http://cf.haigaiapp.cn

Py:   if not s:
来源：http://ds.szxytkj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://pq.bjjhwx.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://bh.hahajie.cn

TS:   if (s === "") {}
来源：http://wm.shtwfgs.cn

Java: if (s.isEmpty()) {}
来源：http://yp.chemitech.net.cn

Go:   if s == "" {}
来源：http://mv.panjiajie.cn

Ruby: if s.empty?
来源：http://rv.panjiajie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ap.bookmarksfly.cn

[E21] 超长截断加省略号
来源：http://gu.jctech888.com.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mp.asd995.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://il.wgjwhj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fs.newstarts.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://aq.szxytkj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ks.nicolike.cn

Go:   // 按 rune 判断长度后截断
来源：http://oj.huixiangedu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cn.bjjhwx.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qa.panjiajie.cn

[E22] 字节长度与字符长度
来源：http://hh.hahajie.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ey.9csxet.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ye.nicolike.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://kn.bjjhwx.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jw.huixiangedu.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zu.szsharing.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://as.jctech888.com.cn

Ruby: s.bytesize;  s.length
来源：http://gg.haigaiapp.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gz.newstarts.cn

================================================================================
来源：http://df.shtwfgs.cn

F. 文件与目录
来源：http://xq.lnxyls.cn

================================================================================
来源：http://am.jianghongdianzi.cn

[F01] 读取整个文件
来源：http://mp.shtwfgs.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qi.panjiajie.cn

PHP:  file_get_contents("a.txt");
来源：http://ck.huanxung.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xt.521024.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://uq.yuntaijiaju.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://cw.nszjky.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://cx.jianghongdianzi.cn

Ruby: File.read("a.txt")
来源：http://hy.huixinmuqiang.cn

C#:   File.ReadAllText("a.txt");
来源：http://rl.huixinmuqiang.cn

[F02] 逐行读取文件
来源：http://ll.yuexingan06.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://uw.muxihuayi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://nk.huanxung.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bs.szxytkj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xu.jianghongdianzi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://cm.panjiajie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jp.nszjky.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zp.nicolike.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vx.huixiangedu.cn

[F03] 写入文件（覆盖）
来源：http://nz.huanxung.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cg.panjiajie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://xl.huixiangedu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bb.szsharing.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ih.hnjuh.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ej.shtwfgs.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kh.bjjhwx.cn

Ruby: File.write("a.txt", "hi")
来源：http://ip.newstarts.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ea.huanxung.cn

[F04] 追加写入文件
来源：http://na.panjiajie.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://za.newstarts.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rc.bjjhwx.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jo.shtwfgs.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lk.bjjhwx.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gm.bookmarksfly.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wo.huixinmuqiang.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nu.shtwfgs.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dl.panjiajie.cn

[F05] 判断文件或目录是否存在
来源：http://eu.shtwfgs.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://iv.lnxyls.cn

PHP:  file_exists("a.txt");
来源：http://mz.shxzukj.cn

JS:   fs.existsSync("a.txt")
来源：http://fx.colortex.cn

TS:   fs.existsSync("a.txt")
来源：http://xe.colortex.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://im.yuntaijiaju.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ot.nicolike.cn

Ruby: File.exist?("a.txt")
来源：http://ym.huixinmuqiang.cn

C#:   File.Exists("a.txt")
来源：http://ld.huanxung.cn

[F06] 删除文件
来源：http://xd.asd995.cn

Py:   os.remove("a.txt")
来源：http://jh.bjjhwx.cn

PHP:  unlink("a.txt");
来源：http://gh.jctech888.com.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ua.bjjhwx.cn

TS:   fs.unlinkSync("a.txt")
来源：http://mp.nszjky.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fr.jianghongdianzi.cn

Go:   os.Remove("a.txt")
来源：http://js.newstarts.cn

Ruby: File.delete("a.txt")
来源：http://hk.jctech888.com.cn

C#:   File.Delete("a.txt");
来源：http://rj.shtwfgs.cn

[F07] 创建目录（含多级）
来源：http://ua.szxytkj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fu.nszjky.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pj.chemitech.net.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hy.wgjwhj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dg.panjiajie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fi.szsharing.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://yz.huanxung.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xh.huixiangedu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://yu.shxzukj.cn

[F08] 遍历目录
来源：http://vg.szsharing.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://kv.hahajie.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://yi.jianghongdianzi.cn

JS:   fs.readdirSync("dir")
来源：http://bb.9csxet.cn

TS:   fs.readdirSync("dir")
来源：http://fm.panjiajie.cn


<!-- 参考信息 -->