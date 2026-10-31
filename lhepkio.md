代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gi.jianghongdianzi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fu.nszjky.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hp.haigaiapp.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://dj.yuntaijiaju.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ga.shxzskj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zi.colortex.cn

[D25] Set 集合去重与交并差
来源：http://mu.newstarts.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nu.521024.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ng.haigaiapp.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://th.haigaiapp.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hv.chemitech.net.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://aw.shxzukj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ct.szsharing.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://cn.521024.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ho.gzmigu.cn

[D26] 数组转字符串
来源：http://pc.muxihuayi.cn

Py:   ", ".join(map(str, arr))
来源：http://ci.bjjhwx.cn

PHP:  implode(", ", $arr);
来源：http://gg.bookmarksfly.cn

JS:   arr.join(", ")
来源：http://ud.bookmarksfly.cn

TS:   arr.join(", ")
来源：http://bd.huixiangedu.cn

Java: String.join(", ", list)
来源：http://lo.jctech888.com.cn

Go:   strings.Join(strs, ", ")
来源：http://hi.huixinmuqiang.cn

Ruby: arr.join(", ")
来源：http://gx.yuexingan06.cn

C#:   string.Join(", ", list)
来源：http://mj.gzmigu.cn

================================================================================
来源：http://gx.szxytkj.cn

E. 字符串处理
来源：http://pr.colortex.cn

================================================================================
来源：http://zp.hnjuh.cn

[E01] 拼接字符串
来源：http://wy.nicolike.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zr.huixiangedu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://yi.9csxet.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bg.9csxet.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xb.nszjky.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rf.colortex.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://iu.wgjwhj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://so.jctech888.com.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nf.nicolike.cn

[E02] 重复字符串
来源：http://vx.gzmigu.cn

Py:   "ab" * 3
来源：http://az.muxihuayi.cn

PHP:  str_repeat("ab", 3);
来源：http://mv.huixiangedu.cn

JS:   "ab".repeat(3)
来源：http://ds.shxzukj.cn

TS:   "ab".repeat(3)
来源：http://xe.huanxung.cn

Java: "ab".repeat(3)
来源：http://ad.newstarts.cn

Go:   strings.Repeat("ab", 3)
来源：http://wz.huixiangedu.cn

Ruby: "ab" * 3
来源：http://yl.panjiajie.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hl.bookmarksfly.cn

[E03] 截取子串
来源：http://sv.nszjky.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ve.yuntaijiaju.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://yb.nszjky.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lb.wgjwhj.cn

TS:   s.slice(1, 4)
来源：http://tr.haigaiapp.cn

Java: s.substring(1, 4)
来源：http://ii.gzmigu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nw.huanxung.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ah.yuexingan06.cn

C#:   s.Substring(1, 3)
来源：http://av.szxytkj.cn

[E04] 查找子串位置
来源：http://cn.muxihuayi.cn

Py:   s.find("x");  s.index("x")
来源：http://hz.huixinmuqiang.cn

PHP:  strpos($s, "x");
来源：http://ko.nszjky.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://cj.huixiangedu.cn

TS:   s.indexOf("x")
来源：http://xl.nszjky.cn

Java: s.indexOf("x")
来源：http://xm.hnjuh.cn

Go:   strings.Index(s, "x")
来源：http://np.chemitech.net.cn

Ruby: s.index("x")
来源：http://ye.huixiangedu.cn

C#:   s.IndexOf("x")
来源：http://bc.huixiangedu.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://pd.gzmigu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qt.gzmigu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wk.hahajie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cg.jianghongdianzi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ps.szsharing.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://su.yuntaijiaju.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.chemitech.net.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qi.lnxyls.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://sg.huixiangedu.cn

[E06] 替换子串
来源：http://mf.gzmigu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wi.newstarts.cn

PHP:  str_replace("a", "b", $s);
来源：http://jx.jctech888.com.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jq.9csxet.cn

TS:   s.replaceAll("a", "b")
来源：http://al.colortex.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ji.muxihuayi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://us.bookmarksfly.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qm.huanxung.cn

C#:   s.Replace("a", "b")
来源：http://xc.shtwfgs.cn

[E07] 按分隔符拆分
来源：http://zj.huanxung.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ho.9csxet.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kj.muxihuayi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://cn.yuntaijiaju.cn

TS:   s.split(",")
来源：http://nt.haigaiapp.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ul.bookmarksfly.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zg.jianghongdianzi.cn

Ruby: s.split(",");  s.split
来源：http://zg.hnjuh.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://uh.shxzukj.cn

[E08] 数组按分隔符合并
来源：http://yg.jianghongdianzi.cn

Py:   ",".join(items)
来源：http://gq.shxzskj.cn

PHP:  implode(",", $items);
来源：http://yv.szsharing.cn

JS:   items.join(",")
来源：http://dq.asd995.cn

TS:   items.join(",")
来源：http://wv.huixinmuqiang.cn

Java: String.join(",", items)
来源：http://vf.wgjwhj.cn

Go:   strings.Join(items, ",")
来源：http://ag.jctech888.com.cn

Ruby: items.join(",")
来源：http://dq.jctech888.com.cn

C#:   string.Join(",", items)
来源：http://gu.hahajie.cn

[E09] 去除所有空白字符
来源：http://dm.nicolike.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ez.huixinmuqiang.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ft.shxzskj.cn

JS:   s.replace(/\s+/g, "")
来源：http://zq.jctech888.com.cn

TS:   s.replace(/\s+/g, "")
来源：http://qq.bjjhwx.cn

Java: s.replaceAll("\\s+", "")
来源：http://br.asd995.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ov.yuntaijiaju.cn

Ruby: s.gsub(/\s+/, "")
来源：http://sj.bookmarksfly.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fs.hahajie.cn

[E10] 左侧补零 / 定长填充
来源：http://uf.jianghongdianzi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://nv.jianghongdianzi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://um.colortex.cn

JS:   "7".padStart(3, "0")
来源：http://da.asd995.cn

TS:   "7".padStart(3, "0")
来源：http://up.newstarts.cn

Java: String.format("%03d", 7)
来源：http://wl.521024.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ac.colortex.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qf.newstarts.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ia.szxytkj.cn

[E11] 反转字符串
来源：http://ov.panjiajie.cn

Py:   s[::-1]
来源：http://xf.shxzukj.cn

PHP:  strrev($s);
来源：http://ko.nszjky.cn

JS:   [...s].reverse().join("")
来源：http://ix.jctech888.com.cn

TS:   [...s].reverse().join("")
来源：http://ti.newstarts.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ao.lnxyls.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://uy.asd995.cn

Ruby: s.reverse
来源：http://id.panjiajie.cn

C#:   new string(s.Reverse().ToArray())
来源：http://yg.haigaiapp.cn

[E12] 统计某字符出现次数
来源：http://yn.bjjhwx.cn

Py:   s.count("a")
来源：http://rb.jianghongdianzi.cn

PHP:  substr_count($s, "a");
来源：http://bv.wgjwhj.cn

JS:   s.split("a").length - 1
来源：http://yz.wgjwhj.cn

TS:   s.split("a").length - 1
来源：http://eg.nicolike.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qh.hahajie.cn

Go:   strings.Count(s, "a")
来源：http://vm.shxzskj.cn

Ruby: s.count("a")
来源：http://pt.huixiangedu.cn

C#:   s.Count(c => c == 'a')
来源：http://jh.lnxyls.cn

[E13] 逐字符遍历
来源：http://oz.wgjwhj.cn

Py:   for ch in s: print(ch)
来源：http://rv.yuntaijiaju.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ft.shtwfgs.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://go.muxihuayi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://gf.jctech888.com.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://da.szxytkj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tm.jianghongdianzi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://pf.hahajie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://tk.9csxet.cn

[E14] URL 编码与 Base64
来源：http://is.yuexingan06.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wt.huixinmuqiang.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ut.9csxet.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://df.huanxung.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tu.huanxung.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ji.521024.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://lw.521024.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qc.haigaiapp.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://df.yuexingan06.cn

[E15] HTML 转义 / 反转义
来源：http://jz.shtwfgs.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ad.newstarts.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ul.yuexingan06.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hb.haigaiapp.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://wd.haigaiapp.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ue.muxihuayi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ob.asd995.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pl.hnjuh.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://dw.shtwfgs.cn

[E16] 数字千分位
来源：http://om.gzmigu.cn

Py:   f"{1234567:,}"
来源：http://bb.nicolike.cn

PHP:  number_format(1234567);
来源：http://la.szsharing.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://gw.haigaiapp.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://uz.colortex.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fl.shtwfgs.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://gq.hnjuh.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fj.gzmigu.cn

C#:   1234567.ToString("N0")
来源：http://sl.huanxung.cn

[E17] 首字母大写
来源：http://fu.wgjwhj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://uw.shxzskj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://fr.chemitech.net.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yi.nszjky.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kr.yuexingan06.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mo.huanxung.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vz.shtwfgs.cn

Ruby: s.capitalize
来源：http://kn.9csxet.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zr.gzmigu.cn

[E18] 模板占位符替换
来源：http://dd.lnxyls.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bg.yuntaijiaju.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ls.asd995.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://gf.szxytkj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://gl.szxytkj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gq.yuexingan06.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mm.nicolike.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://po.hnjuh.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://tw.panjiajie.cn

[E19] 多行文本按行拆分
来源：http://yn.shxzukj.cn

Py:   s.splitlines()
来源：http://lp.nicolike.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://eo.yuntaijiaju.cn

JS:   s.split(/\r?\n/)
来源：http://ou.szsharing.cn

TS:   s.split(/\r?\n/)
来源：http://lj.huixinmuqiang.cn

Java: s.lines().toList()
来源：http://nr.yuexingan06.cn

Go:   strings.Split(s, "\n")
来源：http://do.jianghongdianzi.cn

Ruby: s.lines
来源：http://gz.nicolike.cn

C#:   s.Split('\n')
来源：http://hr.panjiajie.cn

[E20] 判断字符串是否为空
来源：http://ar.yuntaijiaju.cn

Py:   if not s:
来源：http://uj.nszjky.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ye.huixiangedu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://sm.bjjhwx.cn

TS:   if (s === "") {}
来源：http://ci.lnxyls.cn

Java: if (s.isEmpty()) {}
来源：http://br.huixiangedu.cn

Go:   if s == "" {}
来源：http://bj.9csxet.cn

Ruby: if s.empty?
来源：http://er.nszjky.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dp.chemitech.net.cn

[E21] 超长截断加省略号
来源：http://li.nicolike.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://pf.huixinmuqiang.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vb.huanxung.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zu.521024.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ex.jctech888.com.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://nf.9csxet.cn

Go:   // 按 rune 判断长度后截断
来源：http://fx.shxzukj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fw.521024.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://sn.colortex.cn

[E22] 字节长度与字符长度
来源：http://kn.shtwfgs.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jf.muxihuayi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ph.shtwfgs.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zs.shtwfgs.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ij.jctech888.com.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zo.nszjky.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gx.nicolike.cn

Ruby: s.bytesize;  s.length
来源：http://ed.shxzukj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xm.521024.cn

================================================================================
来源：http://fp.newstarts.cn

F. 文件与目录
来源：http://or.chemitech.net.cn

================================================================================
来源：http://kq.bjjhwx.cn

[F01] 读取整个文件
来源：http://se.bookmarksfly.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mi.muxihuayi.cn

PHP:  file_get_contents("a.txt");
来源：http://do.jctech888.com.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jo.wgjwhj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ow.shxzskj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ym.jianghongdianzi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ag.huixinmuqiang.cn

Ruby: File.read("a.txt")
来源：http://ed.lnxyls.cn

C#:   File.ReadAllText("a.txt");
来源：http://cl.9csxet.cn

[F02] 逐行读取文件
来源：http://bd.wgjwhj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ek.yuexingan06.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vo.hahajie.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pe.colortex.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://af.wgjwhj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ai.panjiajie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lb.lnxyls.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qv.szxytkj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qj.jianghongdianzi.cn

[F03] 写入文件（覆盖）
来源：http://ne.muxihuayi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jb.yuntaijiaju.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ul.huixinmuqiang.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mt.huanxung.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qo.huixiangedu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://pn.szxytkj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tn.gzmigu.cn

Ruby: File.write("a.txt", "hi")
来源：http://ch.gzmigu.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://yi.colortex.cn

[F04] 追加写入文件
来源：http://qt.bjjhwx.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://sr.yuntaijiaju.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mq.huanxung.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vf.hnjuh.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mo.jianghongdianzi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://by.bjjhwx.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jr.521024.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jz.newstarts.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://or.asd995.cn

[F05] 判断文件或目录是否存在
来源：http://hx.shxzukj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://eb.hnjuh.cn

PHP:  file_exists("a.txt");
来源：http://gr.bjjhwx.cn

JS:   fs.existsSync("a.txt")
来源：http://ow.huixinmuqiang.cn

TS:   fs.existsSync("a.txt")
来源：http://sw.huixiangedu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://oa.haigaiapp.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ls.huanxung.cn

Ruby: File.exist?("a.txt")
来源：http://bc.hnjuh.cn

C#:   File.Exists("a.txt")
来源：http://lk.haigaiapp.cn

[F06] 删除文件
来源：http://pi.shxzskj.cn

Py:   os.remove("a.txt")
来源：http://gz.muxihuayi.cn

PHP:  unlink("a.txt");
来源：http://sq.panjiajie.cn

JS:   fs.unlinkSync("a.txt")
来源：http://er.haigaiapp.cn

TS:   fs.unlinkSync("a.txt")
来源：http://at.chemitech.net.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yi.huixinmuqiang.cn

Go:   os.Remove("a.txt")
来源：http://ym.newstarts.cn

Ruby: File.delete("a.txt")
来源：http://lf.hnjuh.cn

C#:   File.Delete("a.txt");
来源：http://of.huixiangedu.cn

[F07] 创建目录（含多级）
来源：http://xh.nicolike.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sl.huixinmuqiang.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dg.gzmigu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gf.huixinmuqiang.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qt.huanxung.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qd.521024.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rj.521024.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dl.shxzskj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://di.521024.cn

[F08] 遍历目录
来源：http://pd.chemitech.net.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://zq.shtwfgs.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://sd.huanxung.cn

JS:   fs.readdirSync("dir")
来源：http://sd.nicolike.cn

TS:   fs.readdirSync("dir")
来源：http://tn.nszjky.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://uv.yuexingan06.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://af.yuexingan06.cn

Ruby: Dir.children("dir")
来源：http://iv.huanxung.cn

C#:   Directory.GetFiles("dir")
来源：http://cw.newstarts.cn


<!-- 参考信息 -->