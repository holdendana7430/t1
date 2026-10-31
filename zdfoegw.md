代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nz.yuexingan06.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://kp.bookmarksfly.cn

Go:   // 手写循环
来源：http://cn.9csxet.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mx.hahajie.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gu.panjiajie.cn

[D24] 字典 / Map 基本操作
来源：http://gq.newstarts.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://co.bookmarksfly.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://dr.nicolike.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rf.szxytkj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xc.yuntaijiaju.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://is.nicolike.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://cn.yuntaijiaju.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ai.panjiajie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gt.yuntaijiaju.cn

[D25] Set 集合去重与交并差
来源：http://sa.shxzukj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lq.shtwfgs.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ai.huixiangedu.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://uh.shtwfgs.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://an.huixinmuqiang.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ls.chemitech.net.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tg.521024.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dh.bjjhwx.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://eo.asd995.cn

[D26] 数组转字符串
来源：http://qb.bjjhwx.cn

Py:   ", ".join(map(str, arr))
来源：http://zk.asd995.cn

PHP:  implode(", ", $arr);
来源：http://mx.lnxyls.cn

JS:   arr.join(", ")
来源：http://sf.wgjwhj.cn

TS:   arr.join(", ")
来源：http://hj.shxzukj.cn

Java: String.join(", ", list)
来源：http://ha.521024.cn

Go:   strings.Join(strs, ", ")
来源：http://li.yuntaijiaju.cn

Ruby: arr.join(", ")
来源：http://ou.nszjky.cn

C#:   string.Join(", ", list)
来源：http://qy.asd995.cn

================================================================================
来源：http://dm.521024.cn

E. 字符串处理
来源：http://ce.haigaiapp.cn

================================================================================
来源：http://ns.yuntaijiaju.cn

[E01] 拼接字符串
来源：http://bl.szsharing.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vl.chemitech.net.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://kf.haigaiapp.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gb.hahajie.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qp.huixinmuqiang.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ga.bookmarksfly.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wj.haigaiapp.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ef.huanxung.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://tg.bookmarksfly.cn

[E02] 重复字符串
来源：http://lw.yuntaijiaju.cn

Py:   "ab" * 3
来源：http://sn.gzmigu.cn

PHP:  str_repeat("ab", 3);
来源：http://qt.chemitech.net.cn

JS:   "ab".repeat(3)
来源：http://uy.hahajie.cn

TS:   "ab".repeat(3)
来源：http://kv.haigaiapp.cn

Java: "ab".repeat(3)
来源：http://cv.yuntaijiaju.cn

Go:   strings.Repeat("ab", 3)
来源：http://ml.wgjwhj.cn

Ruby: "ab" * 3
来源：http://mc.huanxung.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://se.shxzukj.cn

[E03] 截取子串
来源：http://eq.9csxet.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://bb.bjjhwx.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://px.bjjhwx.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yc.szxytkj.cn

TS:   s.slice(1, 4)
来源：http://ab.chemitech.net.cn

Java: s.substring(1, 4)
来源：http://qc.newstarts.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://yd.szsharing.cn

Ruby: s[1, 3];  s[1..3]
来源：http://xf.yuntaijiaju.cn

C#:   s.Substring(1, 3)
来源：http://vw.haigaiapp.cn

[E04] 查找子串位置
来源：http://dd.panjiajie.cn

Py:   s.find("x");  s.index("x")
来源：http://oe.haigaiapp.cn

PHP:  strpos($s, "x");
来源：http://ft.hnjuh.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vt.521024.cn

TS:   s.indexOf("x")
来源：http://ki.haigaiapp.cn

Java: s.indexOf("x")
来源：http://dr.yuntaijiaju.cn

Go:   strings.Index(s, "x")
来源：http://tb.panjiajie.cn

Ruby: s.index("x")
来源：http://wp.huixiangedu.cn

C#:   s.IndexOf("x")
来源：http://lo.lnxyls.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://pu.muxihuayi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://vh.muxihuayi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ya.9csxet.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ba.haigaiapp.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://vu.yuntaijiaju.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://we.shtwfgs.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://th.muxihuayi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qs.szxytkj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://sv.newstarts.cn

[E06] 替换子串
来源：http://yc.nicolike.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://tr.521024.cn

PHP:  str_replace("a", "b", $s);
来源：http://km.bjjhwx.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sz.lnxyls.cn

TS:   s.replaceAll("a", "b")
来源：http://fg.bjjhwx.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vj.jianghongdianzi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://pu.hahajie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ny.hahajie.cn

C#:   s.Replace("a", "b")
来源：http://kh.colortex.cn

[E07] 按分隔符拆分
来源：http://dv.521024.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wv.haigaiapp.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://aq.shtwfgs.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://sq.bjjhwx.cn

TS:   s.split(",")
来源：http://vh.hnjuh.cn

Java: s.split(",");  s.split("\\s+")
来源：http://dl.gzmigu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xs.yuexingan06.cn

Ruby: s.split(",");  s.split
来源：http://yx.gzmigu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fi.muxihuayi.cn

[E08] 数组按分隔符合并
来源：http://be.huixiangedu.cn

Py:   ",".join(items)
来源：http://ay.hnjuh.cn

PHP:  implode(",", $items);
来源：http://ah.muxihuayi.cn

JS:   items.join(",")
来源：http://qu.szsharing.cn

TS:   items.join(",")
来源：http://za.muxihuayi.cn

Java: String.join(",", items)
来源：http://ii.nicolike.cn

Go:   strings.Join(items, ",")
来源：http://iz.huixiangedu.cn

Ruby: items.join(",")
来源：http://ud.shtwfgs.cn

C#:   string.Join(",", items)
来源：http://oo.jctech888.com.cn

[E09] 去除所有空白字符
来源：http://jk.bookmarksfly.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://as.chemitech.net.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://pj.hahajie.cn

JS:   s.replace(/\s+/g, "")
来源：http://fx.szsharing.cn

TS:   s.replace(/\s+/g, "")
来源：http://xl.panjiajie.cn

Java: s.replaceAll("\\s+", "")
来源：http://xr.muxihuayi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://it.shxzukj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://te.521024.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mv.huanxung.cn

[E10] 左侧补零 / 定长填充
来源：http://yf.muxihuayi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dx.huixiangedu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://cf.colortex.cn

JS:   "7".padStart(3, "0")
来源：http://uz.yuntaijiaju.cn

TS:   "7".padStart(3, "0")
来源：http://on.bjjhwx.cn

Java: String.format("%03d", 7)
来源：http://ai.panjiajie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://bu.muxihuayi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vi.shxzskj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cw.hnjuh.cn

[E11] 反转字符串
来源：http://eb.asd995.cn

Py:   s[::-1]
来源：http://jm.nszjky.cn

PHP:  strrev($s);
来源：http://gv.szxytkj.cn

JS:   [...s].reverse().join("")
来源：http://ep.nicolike.cn

TS:   [...s].reverse().join("")
来源：http://gn.nicolike.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://hc.bjjhwx.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://dp.haigaiapp.cn

Ruby: s.reverse
来源：http://qb.huixiangedu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ra.panjiajie.cn

[E12] 统计某字符出现次数
来源：http://np.huixinmuqiang.cn

Py:   s.count("a")
来源：http://ia.hahajie.cn

PHP:  substr_count($s, "a");
来源：http://cf.huanxung.cn

JS:   s.split("a").length - 1
来源：http://ws.521024.cn

TS:   s.split("a").length - 1
来源：http://vy.shtwfgs.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ot.szxytkj.cn

Go:   strings.Count(s, "a")
来源：http://cw.jctech888.com.cn

Ruby: s.count("a")
来源：http://cu.521024.cn

C#:   s.Count(c => c == 'a')
来源：http://hy.jctech888.com.cn

[E13] 逐字符遍历
来源：http://vi.muxihuayi.cn

Py:   for ch in s: print(ch)
来源：http://pr.wgjwhj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xp.shxzukj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ql.wgjwhj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://cn.bjjhwx.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ut.shxzskj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://lt.hnjuh.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://sp.521024.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ku.9csxet.cn

[E14] URL 编码与 Base64
来源：http://ox.yuexingan06.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kr.nicolike.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://eo.yuntaijiaju.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gh.szsharing.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ob.colortex.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vk.bookmarksfly.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mj.yuntaijiaju.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ol.521024.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://lu.nicolike.cn

[E15] HTML 转义 / 反转义
来源：http://ud.bjjhwx.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://sf.panjiajie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mj.bjjhwx.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://st.9csxet.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://gh.hnjuh.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://pt.hahajie.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gy.shtwfgs.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://by.chemitech.net.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jc.yuntaijiaju.cn

[E16] 数字千分位
来源：http://cs.chemitech.net.cn

Py:   f"{1234567:,}"
来源：http://ie.chemitech.net.cn

PHP:  number_format(1234567);
来源：http://xo.huixiangedu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://jb.hnjuh.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://qj.shtwfgs.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://az.wgjwhj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lx.yuntaijiaju.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bj.shxzukj.cn

C#:   1234567.ToString("N0")
来源：http://bu.gzmigu.cn

[E17] 首字母大写
来源：http://vd.gzmigu.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://yr.haigaiapp.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://zx.nicolike.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wo.chemitech.net.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uk.nszjky.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qy.hnjuh.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hm.yuexingan06.cn

Ruby: s.capitalize
来源：http://yf.newstarts.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fa.panjiajie.cn

[E18] 模板占位符替换
来源：http://zt.yuntaijiaju.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://nv.9csxet.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://es.shxzukj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://oo.colortex.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://eb.521024.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://iu.newstarts.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://te.shtwfgs.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ui.colortex.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hp.huixiangedu.cn

[E19] 多行文本按行拆分
来源：http://yh.jianghongdianzi.cn

Py:   s.splitlines()
来源：http://nz.shxzskj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://di.newstarts.cn

JS:   s.split(/\r?\n/)
来源：http://hq.bookmarksfly.cn

TS:   s.split(/\r?\n/)
来源：http://zq.huixiangedu.cn

Java: s.lines().toList()
来源：http://pd.nszjky.cn

Go:   strings.Split(s, "\n")
来源：http://io.szsharing.cn

Ruby: s.lines
来源：http://xk.muxihuayi.cn

C#:   s.Split('\n')
来源：http://hs.shxzukj.cn

[E20] 判断字符串是否为空
来源：http://iy.shtwfgs.cn

Py:   if not s:
来源：http://gh.yuntaijiaju.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jk.hnjuh.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ge.hnjuh.cn

TS:   if (s === "") {}
来源：http://yn.jianghongdianzi.cn

Java: if (s.isEmpty()) {}
来源：http://lh.panjiajie.cn

Go:   if s == "" {}
来源：http://uc.chemitech.net.cn

Ruby: if s.empty?
来源：http://ce.colortex.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jh.9csxet.cn

[E21] 超长截断加省略号
来源：http://mk.asd995.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://dz.lnxyls.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bu.shxzukj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://an.szsharing.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://eh.asd995.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bm.bookmarksfly.cn

Go:   // 按 rune 判断长度后截断
来源：http://bg.szsharing.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qq.szxytkj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zx.bookmarksfly.cn

[E22] 字节长度与字符长度
来源：http://dz.jianghongdianzi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qj.jianghongdianzi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tb.szsharing.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://yy.bjjhwx.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zs.bookmarksfly.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xq.szsharing.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hr.huixiangedu.cn

Ruby: s.bytesize;  s.length
来源：http://no.yuexingan06.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ho.huixiangedu.cn

================================================================================
来源：http://vk.muxihuayi.cn

F. 文件与目录
来源：http://jy.jianghongdianzi.cn

================================================================================
来源：http://dt.shxzskj.cn

[F01] 读取整个文件
来源：http://ip.hahajie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ry.hahajie.cn

PHP:  file_get_contents("a.txt");
来源：http://fn.nszjky.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fu.yuexingan06.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ql.huanxung.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ov.huixiangedu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jk.521024.cn

Ruby: File.read("a.txt")
来源：http://jc.hnjuh.cn

C#:   File.ReadAllText("a.txt");
来源：http://zl.gzmigu.cn

[F02] 逐行读取文件
来源：http://im.huixiangedu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qa.shxzukj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ej.szxytkj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ny.nszjky.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yl.jianghongdianzi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jt.shxzukj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://iu.521024.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ky.panjiajie.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://cr.huixinmuqiang.cn

[F03] 写入文件（覆盖）
来源：http://xb.asd995.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://sp.bjjhwx.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://lw.huixiangedu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qc.huixiangedu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zx.jianghongdianzi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gm.huixinmuqiang.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ja.nszjky.cn

Ruby: File.write("a.txt", "hi")
来源：http://gy.wgjwhj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ov.chemitech.net.cn

[F04] 追加写入文件
来源：http://pn.haigaiapp.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://yi.newstarts.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kx.huixiangedu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hh.shtwfgs.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xe.521024.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zv.chemitech.net.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jd.nszjky.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://po.yuexingan06.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://su.yuexingan06.cn

[F05] 判断文件或目录是否存在
来源：http://uf.bjjhwx.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hw.yuntaijiaju.cn

PHP:  file_exists("a.txt");
来源：http://eg.9csxet.cn

JS:   fs.existsSync("a.txt")
来源：http://us.lnxyls.cn

TS:   fs.existsSync("a.txt")
来源：http://lz.shxzskj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://pr.lnxyls.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tw.chemitech.net.cn

Ruby: File.exist?("a.txt")
来源：http://po.shxzukj.cn

C#:   File.Exists("a.txt")
来源：http://mx.panjiajie.cn

[F06] 删除文件
来源：http://mx.huanxung.cn

Py:   os.remove("a.txt")
来源：http://ep.asd995.cn

PHP:  unlink("a.txt");
来源：http://rx.hnjuh.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ra.hahajie.cn

TS:   fs.unlinkSync("a.txt")
来源：http://vv.521024.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ep.nszjky.cn

Go:   os.Remove("a.txt")
来源：http://zs.bjjhwx.cn

Ruby: File.delete("a.txt")
来源：http://qu.9csxet.cn

C#:   File.Delete("a.txt");
来源：http://se.huixinmuqiang.cn

[F07] 创建目录（含多级）
来源：http://cl.lnxyls.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jl.szxytkj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zn.yuexingan06.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vy.shtwfgs.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ng.9csxet.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://pr.bookmarksfly.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ct.chemitech.net.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ff.jianghongdianzi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://lk.nicolike.cn

[F08] 遍历目录
来源：http://fd.asd995.cn


<!-- 参考信息 -->