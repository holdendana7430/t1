代发 wailian999

[D23] reduce 累积计算
来源：http://lo.huixinmuqiang.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://kp.shxzukj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://iw.gzmigu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nb.huixinmuqiang.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ak.lnxyls.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://kf.bjjhwx.cn

Go:   // 手写循环
来源：http://ie.shxzskj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bc.shxzskj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://di.huixinmuqiang.cn

[D24] 字典 / Map 基本操作
来源：http://lr.jctech888.com.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ms.hnjuh.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zj.muxihuayi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zw.chemitech.net.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://if.lnxyls.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jx.huanxung.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gt.shxzukj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ta.huixinmuqiang.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://js.hahajie.cn

[D25] Set 集合去重与交并差
来源：http://ur.panjiajie.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://va.gzmigu.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tw.nszjky.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ln.bookmarksfly.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qq.yuexingan06.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://sh.wgjwhj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ea.huixiangedu.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://sd.bookmarksfly.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ly.panjiajie.cn

[D26] 数组转字符串
来源：http://dh.hahajie.cn

Py:   ", ".join(map(str, arr))
来源：http://hy.bjjhwx.cn

PHP:  implode(", ", $arr);
来源：http://kt.yuntaijiaju.cn

JS:   arr.join(", ")
来源：http://ak.asd995.cn

TS:   arr.join(", ")
来源：http://if.bjjhwx.cn

Java: String.join(", ", list)
来源：http://ra.shxzukj.cn

Go:   strings.Join(strs, ", ")
来源：http://ec.yuexingan06.cn

Ruby: arr.join(", ")
来源：http://xi.shtwfgs.cn

C#:   string.Join(", ", list)
来源：http://jh.huixinmuqiang.cn

================================================================================
来源：http://fk.newstarts.cn

E. 字符串处理
来源：http://zu.nicolike.cn

================================================================================
来源：http://ps.panjiajie.cn

[E01] 拼接字符串
来源：http://fm.shtwfgs.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xo.lnxyls.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vu.hahajie.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mk.shtwfgs.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://sg.shxzukj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wx.shxzukj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ug.huixiangedu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hs.haigaiapp.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gg.yuexingan06.cn

[E02] 重复字符串
来源：http://zs.muxihuayi.cn

Py:   "ab" * 3
来源：http://mm.521024.cn

PHP:  str_repeat("ab", 3);
来源：http://jr.shxzukj.cn

JS:   "ab".repeat(3)
来源：http://lh.newstarts.cn

TS:   "ab".repeat(3)
来源：http://ga.bookmarksfly.cn

Java: "ab".repeat(3)
来源：http://cg.jianghongdianzi.cn

Go:   strings.Repeat("ab", 3)
来源：http://un.jianghongdianzi.cn

Ruby: "ab" * 3
来源：http://is.shtwfgs.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qg.nicolike.cn

[E03] 截取子串
来源：http://ja.nszjky.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://fc.huixiangedu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ss.hnjuh.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://op.newstarts.cn

TS:   s.slice(1, 4)
来源：http://mj.hahajie.cn

Java: s.substring(1, 4)
来源：http://ph.wgjwhj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://na.hahajie.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ca.shxzukj.cn

C#:   s.Substring(1, 3)
来源：http://bv.colortex.cn

[E04] 查找子串位置
来源：http://bp.szxytkj.cn

Py:   s.find("x");  s.index("x")
来源：http://ke.9csxet.cn

PHP:  strpos($s, "x");
来源：http://nq.panjiajie.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://uq.shtwfgs.cn

TS:   s.indexOf("x")
来源：http://tg.hahajie.cn

Java: s.indexOf("x")
来源：http://ai.lnxyls.cn

Go:   strings.Index(s, "x")
来源：http://mq.hahajie.cn

Ruby: s.index("x")
来源：http://qo.huixinmuqiang.cn

C#:   s.IndexOf("x")
来源：http://hz.chemitech.net.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ya.panjiajie.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ro.szxytkj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://pj.colortex.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uw.jianghongdianzi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://oa.jctech888.com.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uv.yuexingan06.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://vj.yuntaijiaju.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jw.panjiajie.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rp.jctech888.com.cn

[E06] 替换子串
来源：http://bv.shxzukj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dm.asd995.cn

PHP:  str_replace("a", "b", $s);
来源：http://qa.szsharing.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ui.haigaiapp.cn

TS:   s.replaceAll("a", "b")
来源：http://np.bjjhwx.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://us.szxytkj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xx.hnjuh.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hb.muxihuayi.cn

C#:   s.Replace("a", "b")
来源：http://sj.panjiajie.cn

[E07] 按分隔符拆分
来源：http://is.chemitech.net.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://am.chemitech.net.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://yf.shtwfgs.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://hn.huixinmuqiang.cn

TS:   s.split(",")
来源：http://qk.bjjhwx.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ks.9csxet.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://gx.shxzskj.cn

Ruby: s.split(",");  s.split
来源：http://uq.yuexingan06.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qt.nszjky.cn

[E08] 数组按分隔符合并
来源：http://xq.jianghongdianzi.cn

Py:   ",".join(items)
来源：http://ux.hahajie.cn

PHP:  implode(",", $items);
来源：http://bf.nicolike.cn

JS:   items.join(",")
来源：http://xk.yuexingan06.cn

TS:   items.join(",")
来源：http://lt.huixinmuqiang.cn

Java: String.join(",", items)
来源：http://dk.panjiajie.cn

Go:   strings.Join(items, ",")
来源：http://wd.colortex.cn

Ruby: items.join(",")
来源：http://uo.yuexingan06.cn

C#:   string.Join(",", items)
来源：http://yk.asd995.cn

[E09] 去除所有空白字符
来源：http://nv.panjiajie.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://da.bjjhwx.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dh.panjiajie.cn

JS:   s.replace(/\s+/g, "")
来源：http://pm.colortex.cn

TS:   s.replace(/\s+/g, "")
来源：http://gt.lnxyls.cn

Java: s.replaceAll("\\s+", "")
来源：http://fq.hnjuh.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ek.szsharing.cn

Ruby: s.gsub(/\s+/, "")
来源：http://el.szxytkj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://if.gzmigu.cn

[E10] 左侧补零 / 定长填充
来源：http://eh.nszjky.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://su.wgjwhj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://sz.newstarts.cn

JS:   "7".padStart(3, "0")
来源：http://jv.hnjuh.cn

TS:   "7".padStart(3, "0")
来源：http://tg.shxzskj.cn

Java: String.format("%03d", 7)
来源：http://al.jianghongdianzi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://jh.asd995.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://je.huixiangedu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://lw.bjjhwx.cn

[E11] 反转字符串
来源：http://mo.nszjky.cn

Py:   s[::-1]
来源：http://dt.huixiangedu.cn

PHP:  strrev($s);
来源：http://zf.9csxet.cn

JS:   [...s].reverse().join("")
来源：http://pr.panjiajie.cn

TS:   [...s].reverse().join("")
来源：http://wc.nszjky.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://my.lnxyls.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://dp.colortex.cn

Ruby: s.reverse
来源：http://gc.lnxyls.cn

C#:   new string(s.Reverse().ToArray())
来源：http://hg.haigaiapp.cn

[E12] 统计某字符出现次数
来源：http://mm.lnxyls.cn

Py:   s.count("a")
来源：http://gt.gzmigu.cn

PHP:  substr_count($s, "a");
来源：http://cg.asd995.cn

JS:   s.split("a").length - 1
来源：http://eq.shtwfgs.cn

TS:   s.split("a").length - 1
来源：http://uo.muxihuayi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ap.wgjwhj.cn

Go:   strings.Count(s, "a")
来源：http://fz.huixiangedu.cn

Ruby: s.count("a")
来源：http://ku.huanxung.cn

C#:   s.Count(c => c == 'a')
来源：http://sq.bjjhwx.cn

[E13] 逐字符遍历
来源：http://fn.nicolike.cn

Py:   for ch in s: print(ch)
来源：http://qc.521024.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ul.jianghongdianzi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://yv.szsharing.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://po.bjjhwx.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://cg.newstarts.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ek.lnxyls.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://cf.bjjhwx.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hn.hnjuh.cn

[E14] URL 编码与 Base64
来源：http://rd.bjjhwx.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lv.chemitech.net.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://bn.bjjhwx.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rv.shtwfgs.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pf.huixiangedu.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ve.bookmarksfly.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ko.nszjky.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jf.bjjhwx.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://oq.hnjuh.cn

[E15] HTML 转义 / 反转义
来源：http://ga.huixiangedu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ww.haigaiapp.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ln.bookmarksfly.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bs.shxzukj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://jd.bookmarksfly.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gz.chemitech.net.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://pu.muxihuayi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pn.bookmarksfly.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://no.szxytkj.cn

[E16] 数字千分位
来源：http://he.shtwfgs.cn

Py:   f"{1234567:,}"
来源：http://tn.newstarts.cn

PHP:  number_format(1234567);
来源：http://aa.9csxet.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://bs.szsharing.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://dk.wgjwhj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://an.yuexingan06.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://tf.lnxyls.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://lm.huixinmuqiang.cn

C#:   1234567.ToString("N0")
来源：http://ms.shtwfgs.cn

[E17] 首字母大写
来源：http://wf.newstarts.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vy.asd995.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://av.gzmigu.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fo.huanxung.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dc.szsharing.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jr.gzmigu.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ra.shxzskj.cn

Ruby: s.capitalize
来源：http://tf.huixinmuqiang.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xm.nicolike.cn

[E18] 模板占位符替换
来源：http://rh.muxihuayi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://oe.yuexingan06.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://dm.hnjuh.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://lr.bjjhwx.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://il.jianghongdianzi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://cq.haigaiapp.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://pm.szxytkj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ux.huanxung.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bs.yuexingan06.cn

[E19] 多行文本按行拆分
来源：http://ev.gzmigu.cn

Py:   s.splitlines()
来源：http://lf.gzmigu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://db.jctech888.com.cn

JS:   s.split(/\r?\n/)
来源：http://wk.hnjuh.cn

TS:   s.split(/\r?\n/)
来源：http://qe.panjiajie.cn

Java: s.lines().toList()
来源：http://qw.yuexingan06.cn

Go:   strings.Split(s, "\n")
来源：http://nc.nszjky.cn

Ruby: s.lines
来源：http://hh.hahajie.cn

C#:   s.Split('\n')
来源：http://sn.521024.cn

[E20] 判断字符串是否为空
来源：http://ve.huixiangedu.cn

Py:   if not s:
来源：http://ed.newstarts.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ft.colortex.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ff.asd995.cn

TS:   if (s === "") {}
来源：http://df.bookmarksfly.cn

Java: if (s.isEmpty()) {}
来源：http://om.muxihuayi.cn

Go:   if s == "" {}
来源：http://ft.jianghongdianzi.cn

Ruby: if s.empty?
来源：http://wj.huanxung.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rn.szsharing.cn

[E21] 超长截断加省略号
来源：http://fo.huixiangedu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ve.wgjwhj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://dk.yuexingan06.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tq.huanxung.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://su.newstarts.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hs.hnjuh.cn

Go:   // 按 rune 判断长度后截断
来源：http://iq.wgjwhj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hr.gzmigu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://dz.huixinmuqiang.cn

[E22] 字节长度与字符长度
来源：http://ue.lnxyls.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://go.haigaiapp.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jp.521024.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fx.nszjky.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ew.huanxung.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xt.hnjuh.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://iq.haigaiapp.cn

Ruby: s.bytesize;  s.length
来源：http://ez.huixinmuqiang.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ta.asd995.cn

================================================================================
来源：http://jc.huixinmuqiang.cn

F. 文件与目录
来源：http://mu.colortex.cn

================================================================================
来源：http://lk.newstarts.cn

[F01] 读取整个文件
来源：http://hn.jianghongdianzi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ei.huixiangedu.cn

PHP:  file_get_contents("a.txt");
来源：http://sa.shtwfgs.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wu.hahajie.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://dv.newstarts.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://dj.huanxung.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ai.szsharing.cn

Ruby: File.read("a.txt")
来源：http://ld.hnjuh.cn

C#:   File.ReadAllText("a.txt");
来源：http://gs.jianghongdianzi.cn

[F02] 逐行读取文件
来源：http://oa.newstarts.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gl.9csxet.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qz.lnxyls.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xl.bjjhwx.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fb.lnxyls.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xu.bookmarksfly.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://px.521024.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gm.huixinmuqiang.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://al.huixiangedu.cn

[F03] 写入文件（覆盖）
来源：http://lc.newstarts.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://es.yuntaijiaju.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://xm.asd995.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ax.newstarts.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://te.nszjky.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ou.lnxyls.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vb.muxihuayi.cn

Ruby: File.write("a.txt", "hi")
来源：http://lk.nicolike.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cb.nszjky.cn

[F04] 追加写入文件
来源：http://xn.yuntaijiaju.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wx.huixinmuqiang.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ej.muxihuayi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://em.asd995.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wc.huanxung.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://yt.shtwfgs.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vs.shxzukj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://io.shxzukj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ik.chemitech.net.cn

[F05] 判断文件或目录是否存在
来源：http://hi.panjiajie.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pp.newstarts.cn

PHP:  file_exists("a.txt");
来源：http://ad.muxihuayi.cn

JS:   fs.existsSync("a.txt")
来源：http://lx.shtwfgs.cn

TS:   fs.existsSync("a.txt")
来源：http://wh.newstarts.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ar.panjiajie.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ao.shxzskj.cn

Ruby: File.exist?("a.txt")
来源：http://pl.haigaiapp.cn

C#:   File.Exists("a.txt")
来源：http://vq.panjiajie.cn

[F06] 删除文件
来源：http://hy.shtwfgs.cn

Py:   os.remove("a.txt")
来源：http://ap.huixinmuqiang.cn

PHP:  unlink("a.txt");
来源：http://gw.bookmarksfly.cn

JS:   fs.unlinkSync("a.txt")
来源：http://op.nszjky.cn

TS:   fs.unlinkSync("a.txt")
来源：http://pu.huanxung.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://up.huanxung.cn

Go:   os.Remove("a.txt")
来源：http://nw.shxzukj.cn

Ruby: File.delete("a.txt")
来源：http://yl.muxihuayi.cn

C#:   File.Delete("a.txt");
来源：http://mi.yuntaijiaju.cn

[F07] 创建目录（含多级）
来源：http://vn.jctech888.com.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gh.lnxyls.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mw.bjjhwx.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ha.nszjky.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bz.nicolike.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gc.shxzskj.cn


<!-- 参考信息 -->