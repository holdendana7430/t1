代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rn.szsharing.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://pl.lnxyls.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rz.nicolike.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ka.huanxung.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kh.muxihuayi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ju.shtwfgs.cn

[D25] Set 集合去重与交并差
来源：http://hv.huanxung.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ef.shtwfgs.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://cj.haigaiapp.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jh.bjjhwx.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ql.jctech888.com.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ob.panjiajie.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ze.asd995.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://us.huanxung.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lj.9csxet.cn

[D26] 数组转字符串
来源：http://mt.shxzukj.cn

Py:   ", ".join(map(str, arr))
来源：http://bd.shxzskj.cn

PHP:  implode(", ", $arr);
来源：http://oc.gzmigu.cn

JS:   arr.join(", ")
来源：http://ao.huanxung.cn

TS:   arr.join(", ")
来源：http://jo.yuntaijiaju.cn

Java: String.join(", ", list)
来源：http://gt.huixiangedu.cn

Go:   strings.Join(strs, ", ")
来源：http://kc.wgjwhj.cn

Ruby: arr.join(", ")
来源：http://wr.szxytkj.cn

C#:   string.Join(", ", list)
来源：http://cq.haigaiapp.cn

================================================================================
来源：http://fv.bjjhwx.cn

E. 字符串处理
来源：http://mx.shxzskj.cn

================================================================================
来源：http://xp.szsharing.cn

[E01] 拼接字符串
来源：http://nu.hahajie.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ou.shxzukj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://nr.wgjwhj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gv.szsharing.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rb.huanxung.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://eo.shxzukj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://il.yuntaijiaju.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://od.jianghongdianzi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ky.newstarts.cn

[E02] 重复字符串
来源：http://tv.huanxung.cn

Py:   "ab" * 3
来源：http://jt.yuntaijiaju.cn

PHP:  str_repeat("ab", 3);
来源：http://aa.huixiangedu.cn

JS:   "ab".repeat(3)
来源：http://zx.bjjhwx.cn

TS:   "ab".repeat(3)
来源：http://fe.hahajie.cn

Java: "ab".repeat(3)
来源：http://oy.shtwfgs.cn

Go:   strings.Repeat("ab", 3)
来源：http://oj.wgjwhj.cn

Ruby: "ab" * 3
来源：http://ry.gzmigu.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ga.shxzskj.cn

[E03] 截取子串
来源：http://rh.521024.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://eq.lnxyls.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ke.521024.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hv.nicolike.cn

TS:   s.slice(1, 4)
来源：http://hy.colortex.cn

Java: s.substring(1, 4)
来源：http://gh.bookmarksfly.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rd.szxytkj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://mf.shxzukj.cn

C#:   s.Substring(1, 3)
来源：http://wr.nszjky.cn

[E04] 查找子串位置
来源：http://tj.huixinmuqiang.cn

Py:   s.find("x");  s.index("x")
来源：http://af.jianghongdianzi.cn

PHP:  strpos($s, "x");
来源：http://us.chemitech.net.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ll.wgjwhj.cn

TS:   s.indexOf("x")
来源：http://hx.shtwfgs.cn

Java: s.indexOf("x")
来源：http://ub.yuntaijiaju.cn

Go:   strings.Index(s, "x")
来源：http://ok.huixiangedu.cn

Ruby: s.index("x")
来源：http://yy.newstarts.cn

C#:   s.IndexOf("x")
来源：http://pv.haigaiapp.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://uv.shxzukj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mr.huixiangedu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fc.muxihuayi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ua.521024.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ij.bookmarksfly.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://iu.huixinmuqiang.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qh.szsharing.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://yg.huixiangedu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://pa.hahajie.cn

[E06] 替换子串
来源：http://wd.szxytkj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gr.shxzskj.cn

PHP:  str_replace("a", "b", $s);
来源：http://yj.jctech888.com.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ma.shxzskj.cn

TS:   s.replaceAll("a", "b")
来源：http://hg.szsharing.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ia.521024.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.shxzukj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ql.jianghongdianzi.cn

C#:   s.Replace("a", "b")
来源：http://ji.chemitech.net.cn

[E07] 按分隔符拆分
来源：http://ts.wgjwhj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ha.yuntaijiaju.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tw.muxihuayi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ef.shxzukj.cn

TS:   s.split(",")
来源：http://gn.huixinmuqiang.cn

Java: s.split(",");  s.split("\\s+")
来源：http://td.szxytkj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://sp.bjjhwx.cn

Ruby: s.split(",");  s.split
来源：http://ay.huixinmuqiang.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://nv.nicolike.cn

[E08] 数组按分隔符合并
来源：http://rb.bookmarksfly.cn

Py:   ",".join(items)
来源：http://ol.chemitech.net.cn

PHP:  implode(",", $items);
来源：http://fz.hnjuh.cn

JS:   items.join(",")
来源：http://lc.muxihuayi.cn

TS:   items.join(",")
来源：http://gh.shtwfgs.cn

Java: String.join(",", items)
来源：http://au.huixinmuqiang.cn

Go:   strings.Join(items, ",")
来源：http://la.nszjky.cn

Ruby: items.join(",")
来源：http://ep.chemitech.net.cn

C#:   string.Join(",", items)
来源：http://hn.nszjky.cn

[E09] 去除所有空白字符
来源：http://wx.yuexingan06.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ts.gzmigu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fm.jctech888.com.cn

JS:   s.replace(/\s+/g, "")
来源：http://xb.muxihuayi.cn

TS:   s.replace(/\s+/g, "")
来源：http://vm.shxzukj.cn

Java: s.replaceAll("\\s+", "")
来源：http://eh.shxzukj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://by.muxihuayi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://br.hnjuh.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ex.lnxyls.cn

[E10] 左侧补零 / 定长填充
来源：http://ov.nicolike.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://or.szxytkj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://cj.asd995.cn

JS:   "7".padStart(3, "0")
来源：http://jv.haigaiapp.cn

TS:   "7".padStart(3, "0")
来源：http://vy.shxzukj.cn

Java: String.format("%03d", 7)
来源：http://gi.szxytkj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://vo.shxzskj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mm.muxihuayi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cq.huixiangedu.cn

[E11] 反转字符串
来源：http://vq.szsharing.cn

Py:   s[::-1]
来源：http://hy.huixiangedu.cn

PHP:  strrev($s);
来源：http://md.jianghongdianzi.cn

JS:   [...s].reverse().join("")
来源：http://wx.szsharing.cn

TS:   [...s].reverse().join("")
来源：http://zx.wgjwhj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://kg.szxytkj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ku.colortex.cn

Ruby: s.reverse
来源：http://cn.chemitech.net.cn

C#:   new string(s.Reverse().ToArray())
来源：http://cs.521024.cn

[E12] 统计某字符出现次数
来源：http://rz.9csxet.cn

Py:   s.count("a")
来源：http://ft.9csxet.cn

PHP:  substr_count($s, "a");
来源：http://jl.haigaiapp.cn

JS:   s.split("a").length - 1
来源：http://ei.colortex.cn

TS:   s.split("a").length - 1
来源：http://kd.haigaiapp.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hk.yuntaijiaju.cn

Go:   strings.Count(s, "a")
来源：http://qf.huanxung.cn

Ruby: s.count("a")
来源：http://ki.hahajie.cn

C#:   s.Count(c => c == 'a')
来源：http://mv.gzmigu.cn

[E13] 逐字符遍历
来源：http://nz.muxihuayi.cn

Py:   for ch in s: print(ch)
来源：http://yg.hnjuh.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://sc.jianghongdianzi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://dw.9csxet.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://iz.huixinmuqiang.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vf.shxzukj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hx.nszjky.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://he.wgjwhj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://up.gzmigu.cn

[E14] URL 编码与 Base64
来源：http://iq.asd995.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://sk.huixiangedu.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://os.huanxung.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gf.bjjhwx.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xi.huixinmuqiang.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wf.nicolike.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cn.haigaiapp.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kj.colortex.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vr.yuntaijiaju.cn

[E15] HTML 转义 / 反转义
来源：http://bz.jianghongdianzi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://lm.szxytkj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ub.yuntaijiaju.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pp.lnxyls.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://je.haigaiapp.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://et.521024.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mo.jctech888.com.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://eu.yuntaijiaju.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ni.jctech888.com.cn

[E16] 数字千分位
来源：http://qe.chemitech.net.cn

Py:   f"{1234567:,}"
来源：http://bd.colortex.cn

PHP:  number_format(1234567);
来源：http://eg.jctech888.com.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://rv.jctech888.com.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://sd.521024.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qs.9csxet.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://gu.hahajie.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xc.521024.cn

C#:   1234567.ToString("N0")
来源：http://er.jctech888.com.cn

[E17] 首字母大写
来源：http://yi.huixinmuqiang.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hp.lnxyls.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://zi.gzmigu.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ow.asd995.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ne.bookmarksfly.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jo.hnjuh.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lr.muxihuayi.cn

Ruby: s.capitalize
来源：http://bx.wgjwhj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tu.521024.cn

[E18] 模板占位符替换
来源：http://im.9csxet.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jp.yuexingan06.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ga.hnjuh.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ol.nicolike.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://pw.521024.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://uy.gzmigu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://cr.shxzskj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mz.colortex.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://cn.9csxet.cn

[E19] 多行文本按行拆分
来源：http://by.huixinmuqiang.cn

Py:   s.splitlines()
来源：http://xn.shtwfgs.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://sp.yuexingan06.cn

JS:   s.split(/\r?\n/)
来源：http://nw.chemitech.net.cn

TS:   s.split(/\r?\n/)
来源：http://oh.asd995.cn

Java: s.lines().toList()
来源：http://zp.huanxung.cn

Go:   strings.Split(s, "\n")
来源：http://eg.huixinmuqiang.cn

Ruby: s.lines
来源：http://kr.panjiajie.cn

C#:   s.Split('\n')
来源：http://uo.chemitech.net.cn

[E20] 判断字符串是否为空
来源：http://vo.muxihuayi.cn

Py:   if not s:
来源：http://dl.nicolike.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://so.yuntaijiaju.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fp.jianghongdianzi.cn

TS:   if (s === "") {}
来源：http://wq.colortex.cn

Java: if (s.isEmpty()) {}
来源：http://jf.huixiangedu.cn

Go:   if s == "" {}
来源：http://gm.nicolike.cn

Ruby: if s.empty?
来源：http://je.huanxung.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mh.newstarts.cn

[E21] 超长截断加省略号
来源：http://ba.asd995.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://su.521024.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://sn.muxihuayi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ec.bookmarksfly.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uz.521024.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://kz.panjiajie.cn

Go:   // 按 rune 判断长度后截断
来源：http://su.hahajie.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wu.hahajie.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://yg.jctech888.com.cn

[E22] 字节长度与字符长度
来源：http://kg.shtwfgs.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pq.chemitech.net.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hx.hnjuh.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jg.yuexingan06.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hp.yuexingan06.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zo.shxzukj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mg.hahajie.cn

Ruby: s.bytesize;  s.length
来源：http://qh.yuexingan06.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vb.huixiangedu.cn

================================================================================
来源：http://ln.szxytkj.cn

F. 文件与目录
来源：http://lq.jianghongdianzi.cn

================================================================================
来源：http://zw.shtwfgs.cn

[F01] 读取整个文件
来源：http://xk.asd995.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://bd.wgjwhj.cn

PHP:  file_get_contents("a.txt");
来源：http://zi.9csxet.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://an.huixinmuqiang.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lo.jianghongdianzi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://hh.jianghongdianzi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kk.szxytkj.cn

Ruby: File.read("a.txt")
来源：http://em.nszjky.cn

C#:   File.ReadAllText("a.txt");
来源：http://je.huixinmuqiang.cn

[F02] 逐行读取文件
来源：http://zy.newstarts.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bv.gzmigu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hw.hahajie.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qp.huixiangedu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://na.muxihuayi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xq.lnxyls.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://oo.huanxung.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ek.gzmigu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bg.nicolike.cn

[F03] 写入文件（覆盖）
来源：http://sy.shtwfgs.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ix.yuexingan06.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://vx.bjjhwx.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jb.lnxyls.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ai.shxzskj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://oq.szxytkj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gc.colortex.cn

Ruby: File.write("a.txt", "hi")
来源：http://uz.haigaiapp.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://yf.wgjwhj.cn

[F04] 追加写入文件
来源：http://wz.asd995.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vj.wgjwhj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jt.wgjwhj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://er.chemitech.net.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gs.hahajie.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fe.521024.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dh.521024.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nu.huixinmuqiang.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ks.9csxet.cn

[F05] 判断文件或目录是否存在
来源：http://af.huanxung.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mv.shxzskj.cn

PHP:  file_exists("a.txt");
来源：http://jp.lnxyls.cn

JS:   fs.existsSync("a.txt")
来源：http://mr.newstarts.cn

TS:   fs.existsSync("a.txt")
来源：http://wt.hahajie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://bf.hahajie.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zp.colortex.cn

Ruby: File.exist?("a.txt")
来源：http://ps.shxzskj.cn

C#:   File.Exists("a.txt")
来源：http://nd.chemitech.net.cn

[F06] 删除文件
来源：http://gp.bookmarksfly.cn

Py:   os.remove("a.txt")
来源：http://xg.shxzukj.cn

PHP:  unlink("a.txt");
来源：http://zr.bjjhwx.cn

JS:   fs.unlinkSync("a.txt")
来源：http://md.nszjky.cn

TS:   fs.unlinkSync("a.txt")
来源：http://dh.yuexingan06.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rz.muxihuayi.cn

Go:   os.Remove("a.txt")
来源：http://da.panjiajie.cn

Ruby: File.delete("a.txt")
来源：http://pl.nszjky.cn

C#:   File.Delete("a.txt");
来源：http://lf.gzmigu.cn

[F07] 创建目录（含多级）
来源：http://pk.shxzskj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tf.chemitech.net.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cy.hnjuh.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pe.shxzukj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yl.jianghongdianzi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xs.haigaiapp.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://pq.bookmarksfly.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ei.9csxet.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zv.asd995.cn

[F08] 遍历目录
来源：http://ij.huanxung.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://sq.hnjuh.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bd.szsharing.cn

JS:   fs.readdirSync("dir")
来源：http://aw.newstarts.cn

TS:   fs.readdirSync("dir")
来源：http://ev.nicolike.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ft.haigaiapp.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://bh.huixinmuqiang.cn

Ruby: Dir.children("dir")
来源：http://gr.nszjky.cn

C#:   Directory.GetFiles("dir")
来源：http://zu.haigaiapp.cn


<!-- 参考信息 -->