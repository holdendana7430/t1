代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://au.bookmarksfly.cn

[D24] 字典 / Map 基本操作
来源：http://om.yuexingan06.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://nh.hahajie.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kd.nszjky.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ko.asd995.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://eb.newstarts.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ic.shxzukj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xz.9csxet.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qi.bjjhwx.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fk.jctech888.com.cn

[D25] Set 集合去重与交并差
来源：http://or.panjiajie.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://or.huixinmuqiang.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://sx.yuexingan06.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://sk.521024.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fh.haigaiapp.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://iv.chemitech.net.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qw.shxzskj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pc.shxzskj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://az.nicolike.cn

[D26] 数组转字符串
来源：http://ah.521024.cn

Py:   ", ".join(map(str, arr))
来源：http://ka.wgjwhj.cn

PHP:  implode(", ", $arr);
来源：http://bd.colortex.cn

JS:   arr.join(", ")
来源：http://vs.huixinmuqiang.cn

TS:   arr.join(", ")
来源：http://ow.jctech888.com.cn

Java: String.join(", ", list)
来源：http://pi.asd995.cn

Go:   strings.Join(strs, ", ")
来源：http://cz.haigaiapp.cn

Ruby: arr.join(", ")
来源：http://no.szxytkj.cn

C#:   string.Join(", ", list)
来源：http://kx.szsharing.cn

================================================================================
来源：http://gm.huixiangedu.cn

E. 字符串处理
来源：http://gh.haigaiapp.cn

================================================================================
来源：http://og.shxzukj.cn

[E01] 拼接字符串
来源：http://oa.hahajie.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://su.wgjwhj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vx.shxzukj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://pz.huanxung.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://pk.bookmarksfly.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tw.bookmarksfly.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zs.szxytkj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xs.panjiajie.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://uu.shtwfgs.cn

[E02] 重复字符串
来源：http://dp.yuexingan06.cn

Py:   "ab" * 3
来源：http://ts.521024.cn

PHP:  str_repeat("ab", 3);
来源：http://ep.shtwfgs.cn

JS:   "ab".repeat(3)
来源：http://dd.newstarts.cn

TS:   "ab".repeat(3)
来源：http://sr.bookmarksfly.cn

Java: "ab".repeat(3)
来源：http://yl.9csxet.cn

Go:   strings.Repeat("ab", 3)
来源：http://av.gzmigu.cn

Ruby: "ab" * 3
来源：http://sn.hnjuh.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://uc.jctech888.com.cn

[E03] 截取子串
来源：http://yx.shtwfgs.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://py.haigaiapp.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ux.yuexingan06.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://le.huixinmuqiang.cn

TS:   s.slice(1, 4)
来源：http://yd.huanxung.cn

Java: s.substring(1, 4)
来源：http://mn.muxihuayi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fc.hnjuh.cn

Ruby: s[1, 3];  s[1..3]
来源：http://bp.newstarts.cn

C#:   s.Substring(1, 3)
来源：http://cx.muxihuayi.cn

[E04] 查找子串位置
来源：http://cd.bjjhwx.cn

Py:   s.find("x");  s.index("x")
来源：http://ga.haigaiapp.cn

PHP:  strpos($s, "x");
来源：http://mn.panjiajie.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zq.nszjky.cn

TS:   s.indexOf("x")
来源：http://zf.shxzskj.cn

Java: s.indexOf("x")
来源：http://tp.huanxung.cn

Go:   strings.Index(s, "x")
来源：http://zb.gzmigu.cn

Ruby: s.index("x")
来源：http://qp.bookmarksfly.cn

C#:   s.IndexOf("x")
来源：http://sf.muxihuayi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://va.lnxyls.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://kr.shxzskj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bk.huixinmuqiang.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ik.nszjky.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ec.newstarts.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tx.chemitech.net.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://vx.shxzukj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://nw.jianghongdianzi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://je.521024.cn

[E06] 替换子串
来源：http://ow.hahajie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fq.huixinmuqiang.cn

PHP:  str_replace("a", "b", $s);
来源：http://vm.colortex.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rl.huixinmuqiang.cn

TS:   s.replaceAll("a", "b")
来源：http://vl.huixinmuqiang.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ks.jctech888.com.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://cy.shxzukj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://pl.huixinmuqiang.cn

C#:   s.Replace("a", "b")
来源：http://za.huanxung.cn

[E07] 按分隔符拆分
来源：http://rg.huixiangedu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vw.shtwfgs.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://co.9csxet.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ha.yuntaijiaju.cn

TS:   s.split(",")
来源：http://qd.newstarts.cn

Java: s.split(",");  s.split("\\s+")
来源：http://sw.szxytkj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://su.newstarts.cn

Ruby: s.split(",");  s.split
来源：http://th.521024.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gb.chemitech.net.cn

[E08] 数组按分隔符合并
来源：http://yz.wgjwhj.cn

Py:   ",".join(items)
来源：http://ra.huixiangedu.cn

PHP:  implode(",", $items);
来源：http://eu.yuexingan06.cn

JS:   items.join(",")
来源：http://or.huixiangedu.cn

TS:   items.join(",")
来源：http://oi.shxzukj.cn

Java: String.join(",", items)
来源：http://zh.lnxyls.cn

Go:   strings.Join(items, ",")
来源：http://gz.jianghongdianzi.cn

Ruby: items.join(",")
来源：http://js.nicolike.cn

C#:   string.Join(",", items)
来源：http://ny.yuntaijiaju.cn

[E09] 去除所有空白字符
来源：http://th.asd995.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kd.panjiajie.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://li.colortex.cn

JS:   s.replace(/\s+/g, "")
来源：http://du.szsharing.cn

TS:   s.replace(/\s+/g, "")
来源：http://cz.shtwfgs.cn

Java: s.replaceAll("\\s+", "")
来源：http://os.szxytkj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://cj.muxihuayi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://dv.521024.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vg.hnjuh.cn

[E10] 左侧补零 / 定长填充
来源：http://to.bookmarksfly.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://pk.shxzukj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ct.szsharing.cn

JS:   "7".padStart(3, "0")
来源：http://je.haigaiapp.cn

TS:   "7".padStart(3, "0")
来源：http://uk.bookmarksfly.cn

Java: String.format("%03d", 7)
来源：http://dv.szsharing.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://vc.haigaiapp.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hh.nicolike.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://uf.hahajie.cn

[E11] 反转字符串
来源：http://pi.bjjhwx.cn

Py:   s[::-1]
来源：http://rw.huixinmuqiang.cn

PHP:  strrev($s);
来源：http://ax.colortex.cn

JS:   [...s].reverse().join("")
来源：http://jw.hahajie.cn

TS:   [...s].reverse().join("")
来源：http://ak.hnjuh.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://kw.bjjhwx.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://eu.bjjhwx.cn

Ruby: s.reverse
来源：http://zr.hnjuh.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ge.chemitech.net.cn

[E12] 统计某字符出现次数
来源：http://jo.panjiajie.cn

Py:   s.count("a")
来源：http://gc.gzmigu.cn

PHP:  substr_count($s, "a");
来源：http://wf.shtwfgs.cn

JS:   s.split("a").length - 1
来源：http://gz.jianghongdianzi.cn

TS:   s.split("a").length - 1
来源：http://ek.huixinmuqiang.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mp.szxytkj.cn

Go:   strings.Count(s, "a")
来源：http://gq.bjjhwx.cn

Ruby: s.count("a")
来源：http://bj.wgjwhj.cn

C#:   s.Count(c => c == 'a')
来源：http://rx.gzmigu.cn

[E13] 逐字符遍历
来源：http://oe.newstarts.cn

Py:   for ch in s: print(ch)
来源：http://li.521024.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tz.huixinmuqiang.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://sh.huanxung.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://uo.bjjhwx.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://oo.nszjky.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://er.colortex.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://oi.hahajie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://pn.newstarts.cn

[E14] URL 编码与 Base64
来源：http://rz.wgjwhj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ig.9csxet.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://qb.wgjwhj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hr.huanxung.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://lg.newstarts.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://yj.9csxet.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ie.asd995.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jz.panjiajie.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gs.yuntaijiaju.cn

[E15] HTML 转义 / 反转义
来源：http://hh.jctech888.com.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ss.hahajie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zo.yuntaijiaju.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ex.asd995.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://gk.chemitech.net.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qe.hahajie.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://sv.9csxet.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wg.nicolike.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://yu.nicolike.cn

[E16] 数字千分位
来源：http://jc.521024.cn

Py:   f"{1234567:,}"
来源：http://xk.lnxyls.cn

PHP:  number_format(1234567);
来源：http://cs.hnjuh.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://eb.bookmarksfly.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://tp.shxzukj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xi.haigaiapp.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ts.shxzukj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fu.nicolike.cn

C#:   1234567.ToString("N0")
来源：http://bd.szxytkj.cn

[E17] 首字母大写
来源：http://ph.hnjuh.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gt.huanxung.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://fy.9csxet.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ud.shxzukj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zw.asd995.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hm.haigaiapp.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ex.521024.cn

Ruby: s.capitalize
来源：http://ah.szxytkj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ru.szxytkj.cn

[E18] 模板占位符替换
来源：http://ie.bjjhwx.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qp.9csxet.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://lb.hnjuh.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://pl.chemitech.net.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://in.nszjky.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://dy.hnjuh.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fn.huixiangedu.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zb.haigaiapp.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ln.szsharing.cn

[E19] 多行文本按行拆分
来源：http://tb.bookmarksfly.cn

Py:   s.splitlines()
来源：http://mz.muxihuayi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rd.szsharing.cn

JS:   s.split(/\r?\n/)
来源：http://wd.huixiangedu.cn

TS:   s.split(/\r?\n/)
来源：http://ra.shtwfgs.cn

Java: s.lines().toList()
来源：http://rz.nszjky.cn

Go:   strings.Split(s, "\n")
来源：http://yj.bookmarksfly.cn

Ruby: s.lines
来源：http://qo.hnjuh.cn

C#:   s.Split('\n')
来源：http://dp.shxzukj.cn

[E20] 判断字符串是否为空
来源：http://nd.huixinmuqiang.cn

Py:   if not s:
来源：http://sn.panjiajie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://gy.gzmigu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fy.muxihuayi.cn

TS:   if (s === "") {}
来源：http://vq.muxihuayi.cn

Java: if (s.isEmpty()) {}
来源：http://ek.chemitech.net.cn

Go:   if s == "" {}
来源：http://ex.shxzukj.cn

Ruby: if s.empty?
来源：http://bj.chemitech.net.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fa.hahajie.cn

[E21] 超长截断加省略号
来源：http://fp.hahajie.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ph.shtwfgs.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mf.yuntaijiaju.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vs.hnjuh.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://es.panjiajie.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xw.hahajie.cn

Go:   // 按 rune 判断长度后截断
来源：http://th.521024.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://oz.bookmarksfly.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vr.szsharing.cn

[E22] 字节长度与字符长度
来源：http://zn.bookmarksfly.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ff.wgjwhj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mz.shtwfgs.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fw.jianghongdianzi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ie.521024.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ya.9csxet.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fs.colortex.cn

Ruby: s.bytesize;  s.length
来源：http://dv.jctech888.com.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ap.yuntaijiaju.cn

================================================================================
来源：http://dm.muxihuayi.cn

F. 文件与目录
来源：http://oc.nicolike.cn

================================================================================
来源：http://wp.gzmigu.cn

[F01] 读取整个文件
来源：http://yx.huixiangedu.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rc.gzmigu.cn

PHP:  file_get_contents("a.txt");
来源：http://am.huixiangedu.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lq.nszjky.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ax.huixiangedu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://nl.bookmarksfly.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://oh.haigaiapp.cn

Ruby: File.read("a.txt")
来源：http://fn.shxzukj.cn

C#:   File.ReadAllText("a.txt");
来源：http://xp.colortex.cn

[F02] 逐行读取文件
来源：http://xg.gzmigu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bm.szxytkj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cs.hnjuh.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ti.colortex.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://db.muxihuayi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://py.lnxyls.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xz.asd995.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zm.hahajie.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ld.huanxung.cn

[F03] 写入文件（覆盖）
来源：http://fp.jctech888.com.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://kn.huanxung.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://fc.hahajie.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://is.newstarts.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lm.9csxet.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dk.bjjhwx.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bt.bjjhwx.cn

Ruby: File.write("a.txt", "hi")
来源：http://zh.jctech888.com.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bf.nicolike.cn

[F04] 追加写入文件
来源：http://qh.gzmigu.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jr.bjjhwx.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xw.huixinmuqiang.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vp.hahajie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nu.haigaiapp.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://yj.colortex.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://yb.jctech888.com.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://db.jctech888.com.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://km.huanxung.cn

[F05] 判断文件或目录是否存在
来源：http://bn.huixiangedu.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dl.asd995.cn

PHP:  file_exists("a.txt");
来源：http://hp.huixiangedu.cn

JS:   fs.existsSync("a.txt")
来源：http://gp.huixinmuqiang.cn

TS:   fs.existsSync("a.txt")
来源：http://yi.panjiajie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://dd.szxytkj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mk.szsharing.cn

Ruby: File.exist?("a.txt")
来源：http://ke.hahajie.cn

C#:   File.Exists("a.txt")
来源：http://ot.shtwfgs.cn

[F06] 删除文件
来源：http://kr.newstarts.cn

Py:   os.remove("a.txt")
来源：http://sj.haigaiapp.cn

PHP:  unlink("a.txt");
来源：http://bs.wgjwhj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://sv.colortex.cn

TS:   fs.unlinkSync("a.txt")
来源：http://pb.hahajie.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://op.huixiangedu.cn

Go:   os.Remove("a.txt")
来源：http://lx.huanxung.cn

Ruby: File.delete("a.txt")
来源：http://lr.shxzukj.cn

C#:   File.Delete("a.txt");
来源：http://xt.colortex.cn

[F07] 创建目录（含多级）
来源：http://vw.asd995.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gd.muxihuayi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://yo.colortex.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pt.yuexingan06.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://if.gzmigu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://yc.panjiajie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zg.nszjky.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gh.bjjhwx.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://cl.szsharing.cn

[F08] 遍历目录
来源：http://jl.szsharing.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://af.521024.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wp.gzmigu.cn

JS:   fs.readdirSync("dir")
来源：http://jn.jianghongdianzi.cn

TS:   fs.readdirSync("dir")
来源：http://mj.9csxet.cn


<!-- 参考信息 -->