代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://oi.521024.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://wm.huixinmuqiang.cn

Go:   // 手写循环
来源：http://pp.jctech888.com.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qh.huixiangedu.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tf.szsharing.cn

[D24] 字典 / Map 基本操作
来源：http://uj.shxzskj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vv.jianghongdianzi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fy.panjiajie.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qb.9csxet.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://uk.nicolike.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://iw.newstarts.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ts.haigaiapp.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zr.521024.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://md.wgjwhj.cn

[D25] Set 集合去重与交并差
来源：http://jx.chemitech.net.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ix.bjjhwx.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wr.9csxet.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ck.szsharing.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mq.yuexingan06.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://pq.shxzskj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xs.nicolike.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qm.jctech888.com.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://kz.colortex.cn

[D26] 数组转字符串
来源：http://hf.yuntaijiaju.cn

Py:   ", ".join(map(str, arr))
来源：http://st.huixinmuqiang.cn

PHP:  implode(", ", $arr);
来源：http://aj.huixiangedu.cn

JS:   arr.join(", ")
来源：http://ky.nszjky.cn

TS:   arr.join(", ")
来源：http://fw.521024.cn

Java: String.join(", ", list)
来源：http://tg.wgjwhj.cn

Go:   strings.Join(strs, ", ")
来源：http://nu.nicolike.cn

Ruby: arr.join(", ")
来源：http://vo.shxzukj.cn

C#:   string.Join(", ", list)
来源：http://td.lnxyls.cn

================================================================================
来源：http://wh.szxytkj.cn

E. 字符串处理
来源：http://oj.hahajie.cn

================================================================================
来源：http://qp.muxihuayi.cn

[E01] 拼接字符串
来源：http://rh.shtwfgs.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://un.bookmarksfly.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://bo.asd995.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zb.newstarts.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gp.haigaiapp.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ee.nicolike.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gx.bjjhwx.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pz.panjiajie.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://cm.lnxyls.cn

[E02] 重复字符串
来源：http://kp.haigaiapp.cn

Py:   "ab" * 3
来源：http://pp.szxytkj.cn

PHP:  str_repeat("ab", 3);
来源：http://ga.nszjky.cn

JS:   "ab".repeat(3)
来源：http://vq.9csxet.cn

TS:   "ab".repeat(3)
来源：http://lh.chemitech.net.cn

Java: "ab".repeat(3)
来源：http://ok.hnjuh.cn

Go:   strings.Repeat("ab", 3)
来源：http://pm.gzmigu.cn

Ruby: "ab" * 3
来源：http://tz.panjiajie.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ev.shtwfgs.cn

[E03] 截取子串
来源：http://su.gzmigu.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ri.wgjwhj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://iu.521024.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zm.bookmarksfly.cn

TS:   s.slice(1, 4)
来源：http://rs.hnjuh.cn

Java: s.substring(1, 4)
来源：http://jd.hahajie.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://yy.huixinmuqiang.cn

Ruby: s[1, 3];  s[1..3]
来源：http://lc.hnjuh.cn

C#:   s.Substring(1, 3)
来源：http://em.521024.cn

[E04] 查找子串位置
来源：http://tz.huixinmuqiang.cn

Py:   s.find("x");  s.index("x")
来源：http://rw.huixiangedu.cn

PHP:  strpos($s, "x");
来源：http://pr.huixinmuqiang.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://me.shxzukj.cn

TS:   s.indexOf("x")
来源：http://kg.panjiajie.cn

Java: s.indexOf("x")
来源：http://jz.bjjhwx.cn

Go:   strings.Index(s, "x")
来源：http://kr.521024.cn

Ruby: s.index("x")
来源：http://gb.lnxyls.cn

C#:   s.IndexOf("x")
来源：http://lt.szsharing.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://zq.szsharing.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gy.bjjhwx.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://dn.hnjuh.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bq.bjjhwx.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://qt.jctech888.com.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ht.gzmigu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ka.huixiangedu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ja.huixinmuqiang.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://pe.wgjwhj.cn

[E06] 替换子串
来源：http://yk.nicolike.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fa.nszjky.cn

PHP:  str_replace("a", "b", $s);
来源：http://pj.szxytkj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ae.haigaiapp.cn

TS:   s.replaceAll("a", "b")
来源：http://pu.asd995.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bf.muxihuayi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fw.asd995.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://se.szsharing.cn

C#:   s.Replace("a", "b")
来源：http://lo.chemitech.net.cn

[E07] 按分隔符拆分
来源：http://vt.bjjhwx.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://na.shxzskj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qf.nicolike.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://tx.szsharing.cn

TS:   s.split(",")
来源：http://aw.hahajie.cn

Java: s.split(",");  s.split("\\s+")
来源：http://bo.muxihuayi.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wp.szxytkj.cn

Ruby: s.split(",");  s.split
来源：http://gv.shxzukj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ef.bookmarksfly.cn

[E08] 数组按分隔符合并
来源：http://zt.yuexingan06.cn

Py:   ",".join(items)
来源：http://tu.asd995.cn

PHP:  implode(",", $items);
来源：http://fk.hnjuh.cn

JS:   items.join(",")
来源：http://gz.huanxung.cn

TS:   items.join(",")
来源：http://tu.hnjuh.cn

Java: String.join(",", items)
来源：http://lp.huixiangedu.cn

Go:   strings.Join(items, ",")
来源：http://wg.huixiangedu.cn

Ruby: items.join(",")
来源：http://dh.lnxyls.cn

C#:   string.Join(",", items)
来源：http://kh.colortex.cn

[E09] 去除所有空白字符
来源：http://zb.shtwfgs.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mm.shxzukj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zq.chemitech.net.cn

JS:   s.replace(/\s+/g, "")
来源：http://wz.szsharing.cn

TS:   s.replace(/\s+/g, "")
来源：http://mo.521024.cn

Java: s.replaceAll("\\s+", "")
来源：http://po.colortex.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://iv.nszjky.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ob.huanxung.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cp.shxzukj.cn

[E10] 左侧补零 / 定长填充
来源：http://ol.haigaiapp.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://if.jctech888.com.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bq.szxytkj.cn

JS:   "7".padStart(3, "0")
来源：http://af.asd995.cn

TS:   "7".padStart(3, "0")
来源：http://tw.szsharing.cn

Java: String.format("%03d", 7)
来源：http://kb.wgjwhj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://qz.szsharing.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://bv.colortex.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://dv.muxihuayi.cn

[E11] 反转字符串
来源：http://zf.huixiangedu.cn

Py:   s[::-1]
来源：http://mk.shxzukj.cn

PHP:  strrev($s);
来源：http://bm.gzmigu.cn

JS:   [...s].reverse().join("")
来源：http://ja.nszjky.cn

TS:   [...s].reverse().join("")
来源：http://rr.jianghongdianzi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://it.lnxyls.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ji.lnxyls.cn

Ruby: s.reverse
来源：http://wp.jctech888.com.cn

C#:   new string(s.Reverse().ToArray())
来源：http://eh.szsharing.cn

[E12] 统计某字符出现次数
来源：http://dr.huixinmuqiang.cn

Py:   s.count("a")
来源：http://rw.jctech888.com.cn

PHP:  substr_count($s, "a");
来源：http://mm.yuexingan06.cn

JS:   s.split("a").length - 1
来源：http://gg.shxzukj.cn

TS:   s.split("a").length - 1
来源：http://xa.bjjhwx.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hx.chemitech.net.cn

Go:   strings.Count(s, "a")
来源：http://un.jianghongdianzi.cn

Ruby: s.count("a")
来源：http://bt.wgjwhj.cn

C#:   s.Count(c => c == 'a')
来源：http://iy.shxzukj.cn

[E13] 逐字符遍历
来源：http://nq.asd995.cn

Py:   for ch in s: print(ch)
来源：http://qk.yuntaijiaju.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://sq.nszjky.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://yn.muxihuayi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://lq.colortex.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://nn.huixinmuqiang.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://cm.9csxet.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://yu.haigaiapp.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://az.yuexingan06.cn

[E14] URL 编码与 Base64
来源：http://fr.lnxyls.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://dy.shxzskj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://vi.lnxyls.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ju.huixinmuqiang.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://kv.hahajie.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lb.muxihuayi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://at.szsharing.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fb.nicolike.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://yk.huixiangedu.cn

[E15] HTML 转义 / 反转义
来源：http://vh.nszjky.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://dg.9csxet.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://cy.colortex.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pp.jctech888.com.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://td.bookmarksfly.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wm.huixinmuqiang.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xb.szxytkj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://kh.newstarts.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cs.huixiangedu.cn

[E16] 数字千分位
来源：http://et.jctech888.com.cn

Py:   f"{1234567:,}"
来源：http://qk.hnjuh.cn

PHP:  number_format(1234567);
来源：http://zs.gzmigu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://mu.panjiajie.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://nm.521024.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nw.huixinmuqiang.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vk.nicolike.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://iw.newstarts.cn

C#:   1234567.ToString("N0")
来源：http://iy.521024.cn

[E17] 首字母大写
来源：http://eu.newstarts.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://yb.yuexingan06.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://tn.chemitech.net.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xp.shxzskj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oi.bjjhwx.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://di.nicolike.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ab.szsharing.cn

Ruby: s.capitalize
来源：http://al.huixiangedu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ax.hnjuh.cn

[E18] 模板占位符替换
来源：http://bk.shxzukj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ou.bookmarksfly.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qf.szxytkj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://lu.szxytkj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://vj.chemitech.net.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://sa.bjjhwx.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xy.muxihuayi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://tf.bookmarksfly.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xt.521024.cn

[E19] 多行文本按行拆分
来源：http://eh.nicolike.cn

Py:   s.splitlines()
来源：http://kk.huixinmuqiang.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://sy.shtwfgs.cn

JS:   s.split(/\r?\n/)
来源：http://ub.shtwfgs.cn

TS:   s.split(/\r?\n/)
来源：http://hh.muxihuayi.cn

Java: s.lines().toList()
来源：http://ls.bookmarksfly.cn

Go:   strings.Split(s, "\n")
来源：http://gg.colortex.cn

Ruby: s.lines
来源：http://lb.szxytkj.cn

C#:   s.Split('\n')
来源：http://em.shxzukj.cn

[E20] 判断字符串是否为空
来源：http://lx.colortex.cn

Py:   if not s:
来源：http://kd.hahajie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ew.huixiangedu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ts.szxytkj.cn

TS:   if (s === "") {}
来源：http://vf.shxzskj.cn

Java: if (s.isEmpty()) {}
来源：http://kx.colortex.cn

Go:   if s == "" {}
来源：http://px.newstarts.cn

Ruby: if s.empty?
来源：http://qr.asd995.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rh.nszjky.cn

[E21] 超长截断加省略号
来源：http://os.lnxyls.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rs.jianghongdianzi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jv.muxihuayi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nv.haigaiapp.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://al.hnjuh.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://yp.huixinmuqiang.cn

Go:   // 按 rune 判断长度后截断
来源：http://su.wgjwhj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://zl.hnjuh.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://iy.huanxung.cn

[E22] 字节长度与字符长度
来源：http://ik.shxzukj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://tp.huanxung.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vf.bookmarksfly.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ox.colortex.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rf.asd995.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xu.szsharing.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vr.huixiangedu.cn

Ruby: s.bytesize;  s.length
来源：http://qi.9csxet.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cr.newstarts.cn

================================================================================
来源：http://pz.szxytkj.cn

F. 文件与目录
来源：http://lp.shxzukj.cn

================================================================================
来源：http://ru.nszjky.cn

[F01] 读取整个文件
来源：http://nf.szxytkj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ag.muxihuayi.cn

PHP:  file_get_contents("a.txt");
来源：http://dk.muxihuayi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://tk.shxzukj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ak.9csxet.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://rv.lnxyls.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tc.huixinmuqiang.cn

Ruby: File.read("a.txt")
来源：http://ve.521024.cn

C#:   File.ReadAllText("a.txt");
来源：http://pz.huanxung.cn

[F02] 逐行读取文件
来源：http://kl.huixiangedu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fc.haigaiapp.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rn.gzmigu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://aa.yuexingan06.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rl.haigaiapp.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://iw.521024.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ib.jctech888.com.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gt.hahajie.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://kl.jctech888.com.cn

[F03] 写入文件（覆盖）
来源：http://xs.shtwfgs.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://nv.yuexingan06.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://di.colortex.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nv.lnxyls.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fa.yuntaijiaju.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://td.huixiangedu.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://su.jianghongdianzi.cn

Ruby: File.write("a.txt", "hi")
来源：http://ux.521024.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vv.haigaiapp.cn

[F04] 追加写入文件
来源：http://dm.shxzskj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rl.yuntaijiaju.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://za.jianghongdianzi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qe.muxihuayi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uc.chemitech.net.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xg.huixinmuqiang.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hh.huixiangedu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://su.chemitech.net.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://cf.yuexingan06.cn

[F05] 判断文件或目录是否存在
来源：http://ct.9csxet.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jg.szsharing.cn

PHP:  file_exists("a.txt");
来源：http://mi.huixinmuqiang.cn

JS:   fs.existsSync("a.txt")
来源：http://br.hnjuh.cn

TS:   fs.existsSync("a.txt")
来源：http://qc.gzmigu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ni.shxzskj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tz.szxytkj.cn

Ruby: File.exist?("a.txt")
来源：http://an.huanxung.cn

C#:   File.Exists("a.txt")
来源：http://sd.shxzskj.cn

[F06] 删除文件
来源：http://hb.szxytkj.cn

Py:   os.remove("a.txt")
来源：http://mg.bjjhwx.cn

PHP:  unlink("a.txt");
来源：http://vp.szxytkj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://tc.hahajie.cn

TS:   fs.unlinkSync("a.txt")
来源：http://tz.szsharing.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zo.nicolike.cn

Go:   os.Remove("a.txt")
来源：http://mr.shxzskj.cn

Ruby: File.delete("a.txt")
来源：http://lu.hnjuh.cn

C#:   File.Delete("a.txt");
来源：http://qu.haigaiapp.cn

[F07] 创建目录（含多级）
来源：http://up.nicolike.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tx.huanxung.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rb.haigaiapp.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://td.yuexingan06.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mw.panjiajie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kn.lnxyls.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ay.nicolike.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ku.asd995.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ur.nicolike.cn

[F08] 遍历目录
来源：http://af.shtwfgs.cn


<!-- 参考信息 -->