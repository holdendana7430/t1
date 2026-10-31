代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xp.lnxyls.cn

[D24] 字典 / Map 基本操作
来源：http://va.shxzskj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ip.panjiajie.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kp.gzmigu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ee.huixinmuqiang.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fp.shxzskj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xh.lnxyls.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fm.bjjhwx.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vh.shtwfgs.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ee.jctech888.com.cn

[D25] Set 集合去重与交并差
来源：http://tx.bookmarksfly.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://cs.9csxet.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vf.shxzskj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rm.shxzskj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ux.huixinmuqiang.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ox.yuntaijiaju.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jc.panjiajie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ob.huixinmuqiang.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vt.nicolike.cn

[D26] 数组转字符串
来源：http://so.haigaiapp.cn

Py:   ", ".join(map(str, arr))
来源：http://ab.newstarts.cn

PHP:  implode(", ", $arr);
来源：http://bu.yuexingan06.cn

JS:   arr.join(", ")
来源：http://gg.521024.cn

TS:   arr.join(", ")
来源：http://jb.hnjuh.cn

Java: String.join(", ", list)
来源：http://mc.shtwfgs.cn

Go:   strings.Join(strs, ", ")
来源：http://ft.haigaiapp.cn

Ruby: arr.join(", ")
来源：http://kn.hnjuh.cn

C#:   string.Join(", ", list)
来源：http://fs.huixiangedu.cn

================================================================================
来源：http://tb.szsharing.cn

E. 字符串处理
来源：http://le.shtwfgs.cn

================================================================================
来源：http://sg.bjjhwx.cn

[E01] 拼接字符串
来源：http://ya.huixiangedu.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://sy.shxzukj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ov.huanxung.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hn.asd995.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ob.colortex.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vz.521024.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://od.newstarts.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hk.haigaiapp.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ok.hnjuh.cn

[E02] 重复字符串
来源：http://fg.huanxung.cn

Py:   "ab" * 3
来源：http://uh.hahajie.cn

PHP:  str_repeat("ab", 3);
来源：http://iq.bookmarksfly.cn

JS:   "ab".repeat(3)
来源：http://ok.newstarts.cn

TS:   "ab".repeat(3)
来源：http://jh.bjjhwx.cn

Java: "ab".repeat(3)
来源：http://tx.hahajie.cn

Go:   strings.Repeat("ab", 3)
来源：http://wd.lnxyls.cn

Ruby: "ab" * 3
来源：http://pt.yuexingan06.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ed.yuntaijiaju.cn

[E03] 截取子串
来源：http://em.shxzskj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jx.muxihuayi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://oz.jianghongdianzi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zu.szsharing.cn

TS:   s.slice(1, 4)
来源：http://zf.shxzukj.cn

Java: s.substring(1, 4)
来源：http://tm.newstarts.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jb.colortex.cn

Ruby: s[1, 3];  s[1..3]
来源：http://sn.hahajie.cn

C#:   s.Substring(1, 3)
来源：http://gx.shtwfgs.cn

[E04] 查找子串位置
来源：http://mi.colortex.cn

Py:   s.find("x");  s.index("x")
来源：http://jy.lnxyls.cn

PHP:  strpos($s, "x");
来源：http://nl.bookmarksfly.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mn.shxzskj.cn

TS:   s.indexOf("x")
来源：http://cx.shxzukj.cn

Java: s.indexOf("x")
来源：http://bt.shxzskj.cn

Go:   strings.Index(s, "x")
来源：http://la.asd995.cn

Ruby: s.index("x")
来源：http://nl.haigaiapp.cn

C#:   s.IndexOf("x")
来源：http://rs.colortex.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://dw.jctech888.com.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jg.hahajie.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://he.nszjky.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hp.szsharing.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://lu.jianghongdianzi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bk.wgjwhj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fh.huanxung.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://nf.9csxet.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hh.asd995.cn

[E06] 替换子串
来源：http://pb.gzmigu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ib.gzmigu.cn

PHP:  str_replace("a", "b", $s);
来源：http://vi.yuexingan06.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jb.szxytkj.cn

TS:   s.replaceAll("a", "b")
来源：http://se.bookmarksfly.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://se.yuexingan06.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vw.szsharing.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hi.yuexingan06.cn

C#:   s.Replace("a", "b")
来源：http://oc.szxytkj.cn

[E07] 按分隔符拆分
来源：http://rk.shxzukj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lw.521024.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gx.hahajie.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://yd.bjjhwx.cn

TS:   s.split(",")
来源：http://xz.szxytkj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://mn.haigaiapp.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://my.colortex.cn

Ruby: s.split(",");  s.split
来源：http://wk.yuntaijiaju.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yb.521024.cn

[E08] 数组按分隔符合并
来源：http://bp.9csxet.cn

Py:   ",".join(items)
来源：http://yn.hahajie.cn

PHP:  implode(",", $items);
来源：http://mk.colortex.cn

JS:   items.join(",")
来源：http://vq.hnjuh.cn

TS:   items.join(",")
来源：http://iw.szxytkj.cn

Java: String.join(",", items)
来源：http://ql.nszjky.cn

Go:   strings.Join(items, ",")
来源：http://wd.panjiajie.cn

Ruby: items.join(",")
来源：http://cn.yuexingan06.cn

C#:   string.Join(",", items)
来源：http://lv.bookmarksfly.cn

[E09] 去除所有空白字符
来源：http://ia.huixinmuqiang.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ig.bookmarksfly.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xt.chemitech.net.cn

JS:   s.replace(/\s+/g, "")
来源：http://or.huixiangedu.cn

TS:   s.replace(/\s+/g, "")
来源：http://wy.nicolike.cn

Java: s.replaceAll("\\s+", "")
来源：http://cr.bookmarksfly.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://en.jianghongdianzi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://jn.huixinmuqiang.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://to.hnjuh.cn

[E10] 左侧补零 / 定长填充
来源：http://yr.shxzukj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wa.huanxung.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://sq.shxzukj.cn

JS:   "7".padStart(3, "0")
来源：http://xb.asd995.cn

TS:   "7".padStart(3, "0")
来源：http://kj.shxzskj.cn

Java: String.format("%03d", 7)
来源：http://si.521024.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://rb.521024.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rn.nicolike.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://pc.szxytkj.cn

[E11] 反转字符串
来源：http://aq.huanxung.cn

Py:   s[::-1]
来源：http://mt.muxihuayi.cn

PHP:  strrev($s);
来源：http://dc.shtwfgs.cn

JS:   [...s].reverse().join("")
来源：http://zi.hahajie.cn

TS:   [...s].reverse().join("")
来源：http://vd.yuexingan06.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://no.521024.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://wv.hnjuh.cn

Ruby: s.reverse
来源：http://jh.shxzskj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://zj.huixinmuqiang.cn

[E12] 统计某字符出现次数
来源：http://ep.yuexingan06.cn

Py:   s.count("a")
来源：http://qx.bookmarksfly.cn

PHP:  substr_count($s, "a");
来源：http://ex.yuntaijiaju.cn

JS:   s.split("a").length - 1
来源：http://ja.wgjwhj.cn

TS:   s.split("a").length - 1
来源：http://zn.muxihuayi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://bv.shtwfgs.cn

Go:   strings.Count(s, "a")
来源：http://pi.jianghongdianzi.cn

Ruby: s.count("a")
来源：http://gg.521024.cn

C#:   s.Count(c => c == 'a')
来源：http://ep.jianghongdianzi.cn

[E13] 逐字符遍历
来源：http://dj.nszjky.cn

Py:   for ch in s: print(ch)
来源：http://ur.jctech888.com.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zy.huixinmuqiang.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ti.nszjky.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://hr.lnxyls.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ew.panjiajie.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mu.bookmarksfly.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://va.jianghongdianzi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://yz.chemitech.net.cn

[E14] URL 编码与 Base64
来源：http://dh.huanxung.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://uh.hahajie.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ac.newstarts.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fa.szxytkj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gw.nicolike.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ku.shtwfgs.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://og.muxihuayi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jj.asd995.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://pz.hnjuh.cn

[E15] HTML 转义 / 反转义
来源：http://he.asd995.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://kc.bookmarksfly.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://nq.shtwfgs.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vy.nszjky.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://dg.chemitech.net.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tm.asd995.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ky.yuntaijiaju.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gj.newstarts.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://df.jctech888.com.cn

[E16] 数字千分位
来源：http://rb.yuexingan06.cn

Py:   f"{1234567:,}"
来源：http://xa.asd995.cn

PHP:  number_format(1234567);
来源：http://ec.9csxet.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://aj.szxytkj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ll.bjjhwx.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ph.colortex.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ue.shxzukj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ge.lnxyls.cn

C#:   1234567.ToString("N0")
来源：http://nw.521024.cn

[E17] 首字母大写
来源：http://vy.nicolike.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hm.hahajie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://yw.gzmigu.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ax.huixinmuqiang.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uk.huixiangedu.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zf.jctech888.com.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zb.asd995.cn

Ruby: s.capitalize
来源：http://zi.yuexingan06.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ji.bjjhwx.cn

[E18] 模板占位符替换
来源：http://ug.shxzskj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wt.haigaiapp.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zq.lnxyls.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://tn.panjiajie.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://sr.chemitech.net.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fq.chemitech.net.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ln.shxzskj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://te.panjiajie.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://tn.yuexingan06.cn

[E19] 多行文本按行拆分
来源：http://do.nicolike.cn

Py:   s.splitlines()
来源：http://oa.szsharing.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ji.hahajie.cn

JS:   s.split(/\r?\n/)
来源：http://fq.colortex.cn

TS:   s.split(/\r?\n/)
来源：http://cx.haigaiapp.cn

Java: s.lines().toList()
来源：http://gt.muxihuayi.cn

Go:   strings.Split(s, "\n")
来源：http://fw.szxytkj.cn

Ruby: s.lines
来源：http://dz.szsharing.cn

C#:   s.Split('\n')
来源：http://ci.szxytkj.cn

[E20] 判断字符串是否为空
来源：http://cn.haigaiapp.cn

Py:   if not s:
来源：http://rg.jctech888.com.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wm.muxihuayi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ih.panjiajie.cn

TS:   if (s === "") {}
来源：http://xb.bjjhwx.cn

Java: if (s.isEmpty()) {}
来源：http://as.asd995.cn

Go:   if s == "" {}
来源：http://oi.nicolike.cn

Ruby: if s.empty?
来源：http://bn.bjjhwx.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qj.9csxet.cn

[E21] 超长截断加省略号
来源：http://xi.9csxet.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://pz.huixinmuqiang.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ht.yuntaijiaju.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://iz.szsharing.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xu.shtwfgs.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://og.asd995.cn

Go:   // 按 rune 判断长度后截断
来源：http://ne.wgjwhj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yb.gzmigu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gj.haigaiapp.cn

[E22] 字节长度与字符长度
来源：http://rj.9csxet.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ln.wgjwhj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qq.colortex.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hp.hahajie.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://am.jctech888.com.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jp.szxytkj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vd.asd995.cn

Ruby: s.bytesize;  s.length
来源：http://wg.bookmarksfly.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://so.shtwfgs.cn

================================================================================
来源：http://cq.shxzukj.cn

F. 文件与目录
来源：http://uo.chemitech.net.cn

================================================================================
来源：http://vz.szxytkj.cn

[F01] 读取整个文件
来源：http://no.szsharing.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qb.bjjhwx.cn

PHP:  file_get_contents("a.txt");
来源：http://bx.jianghongdianzi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://od.huixiangedu.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://km.yuexingan06.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://eu.newstarts.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://op.wgjwhj.cn

Ruby: File.read("a.txt")
来源：http://cf.nicolike.cn

C#:   File.ReadAllText("a.txt");
来源：http://xb.panjiajie.cn

[F02] 逐行读取文件
来源：http://hn.9csxet.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rk.bjjhwx.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pw.shtwfgs.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rs.lnxyls.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vq.bjjhwx.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wv.jctech888.com.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://au.muxihuayi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://of.bookmarksfly.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hl.lnxyls.cn

[F03] 写入文件（覆盖）
来源：http://un.shxzskj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://to.jctech888.com.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://bm.huixiangedu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hm.bookmarksfly.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ae.nszjky.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rt.bookmarksfly.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://pa.huanxung.cn

Ruby: File.write("a.txt", "hi")
来源：http://xk.jianghongdianzi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xa.muxihuayi.cn

[F04] 追加写入文件
来源：http://cu.gzmigu.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gy.haigaiapp.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ho.szxytkj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fr.lnxyls.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ll.lnxyls.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jl.9csxet.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://aj.jianghongdianzi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xv.bjjhwx.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://al.szxytkj.cn

[F05] 判断文件或目录是否存在
来源：http://xa.521024.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vs.shtwfgs.cn

PHP:  file_exists("a.txt");
来源：http://kc.shxzukj.cn

JS:   fs.existsSync("a.txt")
来源：http://fe.panjiajie.cn

TS:   fs.existsSync("a.txt")
来源：http://kh.jianghongdianzi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://qv.yuexingan06.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jf.nicolike.cn

Ruby: File.exist?("a.txt")
来源：http://zc.9csxet.cn

C#:   File.Exists("a.txt")
来源：http://cs.huixinmuqiang.cn

[F06] 删除文件
来源：http://hg.newstarts.cn

Py:   os.remove("a.txt")
来源：http://tk.huanxung.cn

PHP:  unlink("a.txt");
来源：http://ag.muxihuayi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://my.9csxet.cn

TS:   fs.unlinkSync("a.txt")
来源：http://fz.panjiajie.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://nb.huixinmuqiang.cn

Go:   os.Remove("a.txt")
来源：http://ke.jctech888.com.cn

Ruby: File.delete("a.txt")
来源：http://dk.yuexingan06.cn

C#:   File.Delete("a.txt");
来源：http://mt.muxihuayi.cn

[F07] 创建目录（含多级）
来源：http://rm.szsharing.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://uj.gzmigu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rr.bookmarksfly.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zs.bookmarksfly.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ci.huanxung.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dq.panjiajie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fi.shxzukj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ja.bjjhwx.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wh.asd995.cn

[F08] 遍历目录
来源：http://zy.szxytkj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://zm.asd995.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ct.shxzskj.cn

JS:   fs.readdirSync("dir")
来源：http://gu.521024.cn

TS:   fs.readdirSync("dir")
来源：http://xq.szsharing.cn


<!-- 参考信息 -->