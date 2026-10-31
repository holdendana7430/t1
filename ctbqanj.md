代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://pi.muxihuayi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qz.yuexingan06.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zy.nicolike.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://em.gzmigu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://sm.521024.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lz.yuexingan06.cn

[D25] Set 集合去重与交并差
来源：http://iq.bookmarksfly.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://eg.hnjuh.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ao.colortex.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ty.shxzskj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://lk.bjjhwx.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cu.hahajie.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vt.huixiangedu.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://sy.shtwfgs.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mk.muxihuayi.cn

[D26] 数组转字符串
来源：http://ol.gzmigu.cn

Py:   ", ".join(map(str, arr))
来源：http://yu.haigaiapp.cn

PHP:  implode(", ", $arr);
来源：http://zk.szsharing.cn

JS:   arr.join(", ")
来源：http://pl.huanxung.cn

TS:   arr.join(", ")
来源：http://tt.shxzukj.cn

Java: String.join(", ", list)
来源：http://tr.newstarts.cn

Go:   strings.Join(strs, ", ")
来源：http://ov.newstarts.cn

Ruby: arr.join(", ")
来源：http://ly.szxytkj.cn

C#:   string.Join(", ", list)
来源：http://bf.shxzskj.cn

================================================================================
来源：http://mb.haigaiapp.cn

E. 字符串处理
来源：http://pu.haigaiapp.cn

================================================================================
来源：http://qc.gzmigu.cn

[E01] 拼接字符串
来源：http://ug.hahajie.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vb.jctech888.com.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ez.jctech888.com.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://pk.gzmigu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ay.gzmigu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ag.szxytkj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dn.jianghongdianzi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fo.nszjky.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://eo.521024.cn

[E02] 重复字符串
来源：http://tl.chemitech.net.cn

Py:   "ab" * 3
来源：http://tv.newstarts.cn

PHP:  str_repeat("ab", 3);
来源：http://uj.yuntaijiaju.cn

JS:   "ab".repeat(3)
来源：http://qb.lnxyls.cn

TS:   "ab".repeat(3)
来源：http://ki.gzmigu.cn

Java: "ab".repeat(3)
来源：http://wh.bookmarksfly.cn

Go:   strings.Repeat("ab", 3)
来源：http://jn.lnxyls.cn

Ruby: "ab" * 3
来源：http://jw.chemitech.net.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qh.bookmarksfly.cn

[E03] 截取子串
来源：http://ue.bookmarksfly.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://kj.muxihuayi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vm.wgjwhj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ph.bjjhwx.cn

TS:   s.slice(1, 4)
来源：http://sf.huixiangedu.cn

Java: s.substring(1, 4)
来源：http://du.hnjuh.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://yu.shxzukj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://tk.yuexingan06.cn

C#:   s.Substring(1, 3)
来源：http://hg.yuntaijiaju.cn

[E04] 查找子串位置
来源：http://pd.shxzskj.cn

Py:   s.find("x");  s.index("x")
来源：http://rt.hahajie.cn

PHP:  strpos($s, "x");
来源：http://gh.gzmigu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qn.jctech888.com.cn

TS:   s.indexOf("x")
来源：http://pz.shxzukj.cn

Java: s.indexOf("x")
来源：http://fi.chemitech.net.cn

Go:   strings.Index(s, "x")
来源：http://qa.chemitech.net.cn

Ruby: s.index("x")
来源：http://jr.newstarts.cn

C#:   s.IndexOf("x")
来源：http://we.colortex.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://rr.jianghongdianzi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://to.muxihuayi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xv.9csxet.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vx.chemitech.net.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://mv.newstarts.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fj.wgjwhj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://og.szxytkj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://bv.shtwfgs.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gb.521024.cn

[E06] 替换子串
来源：http://dz.nicolike.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xl.shxzukj.cn

PHP:  str_replace("a", "b", $s);
来源：http://xw.huixiangedu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ro.huixinmuqiang.cn

TS:   s.replaceAll("a", "b")
来源：http://as.huixiangedu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ta.huanxung.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xn.bookmarksfly.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://yb.szsharing.cn

C#:   s.Replace("a", "b")
来源：http://wb.521024.cn

[E07] 按分隔符拆分
来源：http://sl.szxytkj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pp.shxzskj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gh.haigaiapp.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ex.shxzukj.cn

TS:   s.split(",")
来源：http://hn.huanxung.cn

Java: s.split(",");  s.split("\\s+")
来源：http://xc.bookmarksfly.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bg.521024.cn

Ruby: s.split(",");  s.split
来源：http://lo.shxzskj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://aa.huixinmuqiang.cn

[E08] 数组按分隔符合并
来源：http://ah.huixinmuqiang.cn

Py:   ",".join(items)
来源：http://hy.huixiangedu.cn

PHP:  implode(",", $items);
来源：http://yo.yuntaijiaju.cn

JS:   items.join(",")
来源：http://vi.huanxung.cn

TS:   items.join(",")
来源：http://gp.colortex.cn

Java: String.join(",", items)
来源：http://el.9csxet.cn

Go:   strings.Join(items, ",")
来源：http://pu.lnxyls.cn

Ruby: items.join(",")
来源：http://og.wgjwhj.cn

C#:   string.Join(",", items)
来源：http://wx.wgjwhj.cn

[E09] 去除所有空白字符
来源：http://zb.shxzukj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fr.newstarts.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ie.huanxung.cn

JS:   s.replace(/\s+/g, "")
来源：http://lp.nszjky.cn

TS:   s.replace(/\s+/g, "")
来源：http://rp.nszjky.cn

Java: s.replaceAll("\\s+", "")
来源：http://zs.huixiangedu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://rk.haigaiapp.cn

Ruby: s.gsub(/\s+/, "")
来源：http://kc.yuexingan06.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://dd.nszjky.cn

[E10] 左侧补零 / 定长填充
来源：http://es.shxzskj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qt.shxzukj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://dj.bookmarksfly.cn

JS:   "7".padStart(3, "0")
来源：http://va.jianghongdianzi.cn

TS:   "7".padStart(3, "0")
来源：http://xp.nszjky.cn

Java: String.format("%03d", 7)
来源：http://rl.colortex.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ua.lnxyls.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fz.jianghongdianzi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fz.bookmarksfly.cn

[E11] 反转字符串
来源：http://cu.yuntaijiaju.cn

Py:   s[::-1]
来源：http://th.yuexingan06.cn

PHP:  strrev($s);
来源：http://gb.shtwfgs.cn

JS:   [...s].reverse().join("")
来源：http://mo.gzmigu.cn

TS:   [...s].reverse().join("")
来源：http://ca.521024.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://cf.huanxung.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://qg.9csxet.cn

Ruby: s.reverse
来源：http://em.521024.cn

C#:   new string(s.Reverse().ToArray())
来源：http://lg.shxzskj.cn

[E12] 统计某字符出现次数
来源：http://pm.shxzskj.cn

Py:   s.count("a")
来源：http://rz.nicolike.cn

PHP:  substr_count($s, "a");
来源：http://ng.bookmarksfly.cn

JS:   s.split("a").length - 1
来源：http://ei.szxytkj.cn

TS:   s.split("a").length - 1
来源：http://fv.bjjhwx.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gk.huanxung.cn

Go:   strings.Count(s, "a")
来源：http://os.asd995.cn

Ruby: s.count("a")
来源：http://nl.hahajie.cn

C#:   s.Count(c => c == 'a')
来源：http://rt.asd995.cn

[E13] 逐字符遍历
来源：http://th.bookmarksfly.cn

Py:   for ch in s: print(ch)
来源：http://tg.huixiangedu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://yc.wgjwhj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://bz.muxihuayi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://kx.muxihuayi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vz.nszjky.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gm.huixiangedu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ci.nszjky.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://az.521024.cn

[E14] URL 编码与 Base64
来源：http://qy.jctech888.com.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ca.panjiajie.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://jn.muxihuayi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ik.chemitech.net.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zi.yuexingan06.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ch.shtwfgs.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://uz.haigaiapp.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://td.newstarts.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jj.huanxung.cn

[E15] HTML 转义 / 反转义
来源：http://hc.jianghongdianzi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://nv.colortex.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://by.gzmigu.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ht.huixiangedu.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://qb.jctech888.com.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vr.huixinmuqiang.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vj.shxzukj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ns.shxzskj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://px.szxytkj.cn

[E16] 数字千分位
来源：http://uj.gzmigu.cn

Py:   f"{1234567:,}"
来源：http://fx.muxihuayi.cn

PHP:  number_format(1234567);
来源：http://dx.muxihuayi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://vg.lnxyls.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://qi.huanxung.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nk.hnjuh.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xf.szxytkj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xb.bjjhwx.cn

C#:   1234567.ToString("N0")
来源：http://yi.jianghongdianzi.cn

[E17] 首字母大写
来源：http://as.panjiajie.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://tl.shxzskj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://tl.hnjuh.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ui.asd995.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ix.szsharing.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ax.huixinmuqiang.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://tl.szsharing.cn

Ruby: s.capitalize
来源：http://iq.yuntaijiaju.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://lg.nszjky.cn

[E18] 模板占位符替换
来源：http://pa.nicolike.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jg.521024.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://pd.hahajie.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://pj.szsharing.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://id.jianghongdianzi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pn.shtwfgs.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hn.bjjhwx.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://jy.asd995.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://sy.huanxung.cn

[E19] 多行文本按行拆分
来源：http://ez.lnxyls.cn

Py:   s.splitlines()
来源：http://as.colortex.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hm.yuntaijiaju.cn

JS:   s.split(/\r?\n/)
来源：http://yr.yuexingan06.cn

TS:   s.split(/\r?\n/)
来源：http://ti.chemitech.net.cn

Java: s.lines().toList()
来源：http://dw.huanxung.cn

Go:   strings.Split(s, "\n")
来源：http://sd.hnjuh.cn

Ruby: s.lines
来源：http://hk.panjiajie.cn

C#:   s.Split('\n')
来源：http://ym.yuexingan06.cn

[E20] 判断字符串是否为空
来源：http://gz.yuexingan06.cn

Py:   if not s:
来源：http://ze.huixiangedu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://sv.yuntaijiaju.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xj.szxytkj.cn

TS:   if (s === "") {}
来源：http://nv.hnjuh.cn

Java: if (s.isEmpty()) {}
来源：http://at.panjiajie.cn

Go:   if s == "" {}
来源：http://gm.huixiangedu.cn

Ruby: if s.empty?
来源：http://br.newstarts.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://id.nicolike.cn

[E21] 超长截断加省略号
来源：http://jx.bjjhwx.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kb.newstarts.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://nx.jctech888.com.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ke.jianghongdianzi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dm.yuexingan06.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dn.huixiangedu.cn

Go:   // 按 rune 判断长度后截断
来源：http://hb.shxzukj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vj.haigaiapp.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://nb.bjjhwx.cn

[E22] 字节长度与字符长度
来源：http://dx.szsharing.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://yv.haigaiapp.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yi.jctech888.com.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://yy.nicolike.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yb.yuntaijiaju.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ss.newstarts.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xp.jctech888.com.cn

Ruby: s.bytesize;  s.length
来源：http://gn.huixiangedu.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://su.9csxet.cn

================================================================================
来源：http://wi.newstarts.cn

F. 文件与目录
来源：http://sw.9csxet.cn

================================================================================
来源：http://is.haigaiapp.cn

[F01] 读取整个文件
来源：http://vf.haigaiapp.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mt.hnjuh.cn

PHP:  file_get_contents("a.txt");
来源：http://nm.jctech888.com.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://sd.colortex.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jv.nszjky.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://bb.bookmarksfly.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pi.yuexingan06.cn

Ruby: File.read("a.txt")
来源：http://wz.yuntaijiaju.cn

C#:   File.ReadAllText("a.txt");
来源：http://hy.wgjwhj.cn

[F02] 逐行读取文件
来源：http://rm.panjiajie.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fs.huixiangedu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qq.asd995.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qa.shtwfgs.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ch.szxytkj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ln.yuntaijiaju.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jk.jianghongdianzi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://no.szxytkj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ek.9csxet.cn

[F03] 写入文件（覆盖）
来源：http://zm.bjjhwx.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pd.huixiangedu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ix.haigaiapp.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tf.9csxet.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ov.bjjhwx.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xd.nicolike.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wo.wgjwhj.cn

Ruby: File.write("a.txt", "hi")
来源：http://mk.shtwfgs.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://fc.panjiajie.cn

[F04] 追加写入文件
来源：http://ol.colortex.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://da.yuntaijiaju.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rv.nicolike.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ny.yuntaijiaju.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://co.bookmarksfly.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://tm.huanxung.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wr.chemitech.net.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wb.shxzskj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://sc.huanxung.cn

[F05] 判断文件或目录是否存在
来源：http://oy.newstarts.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://zk.asd995.cn

PHP:  file_exists("a.txt");
来源：http://ga.haigaiapp.cn

JS:   fs.existsSync("a.txt")
来源：http://uc.szxytkj.cn

TS:   fs.existsSync("a.txt")
来源：http://ry.9csxet.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://gw.nszjky.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tk.panjiajie.cn

Ruby: File.exist?("a.txt")
来源：http://db.huanxung.cn

C#:   File.Exists("a.txt")
来源：http://lp.hahajie.cn

[F06] 删除文件
来源：http://pp.hahajie.cn

Py:   os.remove("a.txt")
来源：http://ae.521024.cn

PHP:  unlink("a.txt");
来源：http://kt.jianghongdianzi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://aa.hahajie.cn

TS:   fs.unlinkSync("a.txt")
来源：http://yn.asd995.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://js.yuexingan06.cn

Go:   os.Remove("a.txt")
来源：http://dx.bjjhwx.cn

Ruby: File.delete("a.txt")
来源：http://he.haigaiapp.cn

C#:   File.Delete("a.txt");
来源：http://by.huixiangedu.cn

[F07] 创建目录（含多级）
来源：http://cs.haigaiapp.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sk.nicolike.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rz.shxzskj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nt.chemitech.net.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://me.lnxyls.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ov.panjiajie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wi.huixinmuqiang.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gc.muxihuayi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qf.nicolike.cn

[F08] 遍历目录
来源：http://se.jianghongdianzi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://of.haigaiapp.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ya.shtwfgs.cn

JS:   fs.readdirSync("dir")
来源：http://je.shxzukj.cn

TS:   fs.readdirSync("dir")
来源：http://ac.wgjwhj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wr.jianghongdianzi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://wv.shxzskj.cn

Ruby: Dir.children("dir")
来源：http://rv.hnjuh.cn

C#:   Directory.GetFiles("dir")
来源：http://xo.521024.cn


<!-- 参考信息 -->