代发 wailian999

Java: new ArrayList<>(list);
来源：http://jd.asd995.cn

Go:   copied := append([]int(nil), arr...)
来源：http://fy.szsharing.cn

Ruby: arr.dup;  arr.clone
来源：http://fo.nszjky.cn

C#:   new List<int>(list);
来源：http://tx.huanxung.cn

[D23] reduce 累积计算
来源：http://ld.asd995.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://dv.shxzukj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://of.9csxet.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gl.lnxyls.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fx.shxzukj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://zl.chemitech.net.cn

Go:   // 手写循环
来源：http://qn.shtwfgs.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qs.haigaiapp.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://iz.hnjuh.cn

[D24] 字典 / Map 基本操作
来源：http://sf.huixinmuqiang.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://lj.huanxung.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pp.panjiajie.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ao.shxzskj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://er.nszjky.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ft.jianghongdianzi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://yf.szsharing.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://dq.gzmigu.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://tk.521024.cn

[D25] Set 集合去重与交并差
来源：http://le.newstarts.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nz.jctech888.com.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bg.521024.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gg.nszjky.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dg.521024.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://gl.jctech888.com.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tq.bookmarksfly.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://lj.wgjwhj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://aw.bjjhwx.cn

[D26] 数组转字符串
来源：http://an.huanxung.cn

Py:   ", ".join(map(str, arr))
来源：http://tm.nszjky.cn

PHP:  implode(", ", $arr);
来源：http://ry.521024.cn

JS:   arr.join(", ")
来源：http://wt.shxzukj.cn

TS:   arr.join(", ")
来源：http://dc.521024.cn

Java: String.join(", ", list)
来源：http://gc.521024.cn

Go:   strings.Join(strs, ", ")
来源：http://yz.yuntaijiaju.cn

Ruby: arr.join(", ")
来源：http://bn.9csxet.cn

C#:   string.Join(", ", list)
来源：http://db.hahajie.cn

================================================================================
来源：http://kk.yuexingan06.cn

E. 字符串处理
来源：http://ok.shxzukj.cn

================================================================================
来源：http://le.huixiangedu.cn

[E01] 拼接字符串
来源：http://al.huanxung.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xi.huanxung.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fs.muxihuayi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dp.wgjwhj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://eg.asd995.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xx.newstarts.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://cg.haigaiapp.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tz.jctech888.com.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ll.hahajie.cn

[E02] 重复字符串
来源：http://oi.huixiangedu.cn

Py:   "ab" * 3
来源：http://en.colortex.cn

PHP:  str_repeat("ab", 3);
来源：http://ty.szxytkj.cn

JS:   "ab".repeat(3)
来源：http://qh.szxytkj.cn

TS:   "ab".repeat(3)
来源：http://bw.haigaiapp.cn

Java: "ab".repeat(3)
来源：http://jo.shxzukj.cn

Go:   strings.Repeat("ab", 3)
来源：http://to.chemitech.net.cn

Ruby: "ab" * 3
来源：http://nh.yuexingan06.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dw.jianghongdianzi.cn

[E03] 截取子串
来源：http://rl.gzmigu.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rj.huanxung.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qw.nszjky.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://bb.huixinmuqiang.cn

TS:   s.slice(1, 4)
来源：http://uj.bjjhwx.cn

Java: s.substring(1, 4)
来源：http://mi.newstarts.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.yuntaijiaju.cn

Ruby: s[1, 3];  s[1..3]
来源：http://yv.shxzukj.cn

C#:   s.Substring(1, 3)
来源：http://je.521024.cn

[E04] 查找子串位置
来源：http://co.shxzskj.cn

Py:   s.find("x");  s.index("x")
来源：http://mg.colortex.cn

PHP:  strpos($s, "x");
来源：http://is.huixinmuqiang.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://nj.bookmarksfly.cn

TS:   s.indexOf("x")
来源：http://fd.szxytkj.cn

Java: s.indexOf("x")
来源：http://fz.chemitech.net.cn

Go:   strings.Index(s, "x")
来源：http://wb.nicolike.cn

Ruby: s.index("x")
来源：http://mw.yuntaijiaju.cn

C#:   s.IndexOf("x")
来源：http://ht.shtwfgs.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://xj.521024.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xm.yuexingan06.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ls.muxihuayi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ks.wgjwhj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://kc.huanxung.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://va.jctech888.com.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ks.yuexingan06.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lv.gzmigu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ny.shxzukj.cn

[E06] 替换子串
来源：http://fm.nszjky.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://sc.chemitech.net.cn

PHP:  str_replace("a", "b", $s);
来源：http://pz.muxihuayi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://in.shtwfgs.cn

TS:   s.replaceAll("a", "b")
来源：http://jn.jctech888.com.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vj.jctech888.com.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ep.muxihuayi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ya.nszjky.cn

C#:   s.Replace("a", "b")
来源：http://fu.lnxyls.cn

[E07] 按分隔符拆分
来源：http://cc.asd995.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rk.jctech888.com.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xu.521024.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://vo.yuexingan06.cn

TS:   s.split(",")
来源：http://cy.szxytkj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://zo.haigaiapp.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://aa.yuexingan06.cn

Ruby: s.split(",");  s.split
来源：http://ly.jctech888.com.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dt.9csxet.cn

[E08] 数组按分隔符合并
来源：http://em.521024.cn

Py:   ",".join(items)
来源：http://ae.huanxung.cn

PHP:  implode(",", $items);
来源：http://yl.huixiangedu.cn

JS:   items.join(",")
来源：http://ub.muxihuayi.cn

TS:   items.join(",")
来源：http://iu.yuntaijiaju.cn

Java: String.join(",", items)
来源：http://re.chemitech.net.cn

Go:   strings.Join(items, ",")
来源：http://wx.yuexingan06.cn

Ruby: items.join(",")
来源：http://md.szsharing.cn

C#:   string.Join(",", items)
来源：http://on.bjjhwx.cn

[E09] 去除所有空白字符
来源：http://tx.nicolike.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://sx.bjjhwx.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dm.shtwfgs.cn

JS:   s.replace(/\s+/g, "")
来源：http://yu.asd995.cn

TS:   s.replace(/\s+/g, "")
来源：http://wi.hahajie.cn

Java: s.replaceAll("\\s+", "")
来源：http://bb.bookmarksfly.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://rk.asd995.cn

Ruby: s.gsub(/\s+/, "")
来源：http://jx.newstarts.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://tq.yuexingan06.cn

[E10] 左侧补零 / 定长填充
来源：http://ek.yuntaijiaju.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://nu.huixinmuqiang.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ir.lnxyls.cn

JS:   "7".padStart(3, "0")
来源：http://fe.yuntaijiaju.cn

TS:   "7".padStart(3, "0")
来源：http://zb.jianghongdianzi.cn

Java: String.format("%03d", 7)
来源：http://wb.521024.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://vz.bookmarksfly.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wm.gzmigu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wm.lnxyls.cn

[E11] 反转字符串
来源：http://az.haigaiapp.cn

Py:   s[::-1]
来源：http://ht.haigaiapp.cn

PHP:  strrev($s);
来源：http://qq.asd995.cn

JS:   [...s].reverse().join("")
来源：http://ji.gzmigu.cn

TS:   [...s].reverse().join("")
来源：http://tn.huixiangedu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ds.haigaiapp.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://yz.szsharing.cn

Ruby: s.reverse
来源：http://rb.haigaiapp.cn

C#:   new string(s.Reverse().ToArray())
来源：http://xm.hnjuh.cn

[E12] 统计某字符出现次数
来源：http://oz.hahajie.cn

Py:   s.count("a")
来源：http://lq.shxzukj.cn

PHP:  substr_count($s, "a");
来源：http://tt.521024.cn

JS:   s.split("a").length - 1
来源：http://ix.jianghongdianzi.cn

TS:   s.split("a").length - 1
来源：http://nh.chemitech.net.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fa.nszjky.cn

Go:   strings.Count(s, "a")
来源：http://di.muxihuayi.cn

Ruby: s.count("a")
来源：http://di.asd995.cn

C#:   s.Count(c => c == 'a')
来源：http://mo.huanxung.cn

[E13] 逐字符遍历
来源：http://cr.hnjuh.cn

Py:   for ch in s: print(ch)
来源：http://nq.hnjuh.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ex.shxzukj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://lr.shxzukj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://yh.lnxyls.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fu.asd995.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://lf.haigaiapp.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://mj.newstarts.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xd.hahajie.cn

[E14] URL 编码与 Base64
来源：http://il.panjiajie.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gb.9csxet.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://qd.jianghongdianzi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://al.gzmigu.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://av.szxytkj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mg.yuexingan06.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://uc.shtwfgs.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ls.shxzukj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fx.huanxung.cn

[E15] HTML 转义 / 反转义
来源：http://fw.shxzukj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://dr.panjiajie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zi.521024.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mo.muxihuayi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://as.9csxet.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wd.szxytkj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gc.jianghongdianzi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ib.521024.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://xw.jianghongdianzi.cn

[E16] 数字千分位
来源：http://nq.yuntaijiaju.cn

Py:   f"{1234567:,}"
来源：http://hs.huixiangedu.cn

PHP:  number_format(1234567);
来源：http://rc.nicolike.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://gq.colortex.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://hr.huanxung.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jh.hahajie.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://uw.jctech888.com.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ue.shxzukj.cn

C#:   1234567.ToString("N0")
来源：http://bq.muxihuayi.cn

[E17] 首字母大写
来源：http://dp.szxytkj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vm.haigaiapp.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://iy.shxzukj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ol.jianghongdianzi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hb.szxytkj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bt.chemitech.net.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rw.gzmigu.cn

Ruby: s.capitalize
来源：http://oj.wgjwhj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jp.jianghongdianzi.cn

[E18] 模板占位符替换
来源：http://cd.asd995.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hj.hnjuh.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ka.bjjhwx.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://yz.yuntaijiaju.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://zb.shxzukj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://yr.hnjuh.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://eo.wgjwhj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rq.jianghongdianzi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ob.newstarts.cn

[E19] 多行文本按行拆分
来源：http://xc.colortex.cn

Py:   s.splitlines()
来源：http://ht.newstarts.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ed.shtwfgs.cn

JS:   s.split(/\r?\n/)
来源：http://xo.szsharing.cn

TS:   s.split(/\r?\n/)
来源：http://vq.jctech888.com.cn

Java: s.lines().toList()
来源：http://be.nicolike.cn

Go:   strings.Split(s, "\n")
来源：http://xr.szsharing.cn

Ruby: s.lines
来源：http://lg.jianghongdianzi.cn

C#:   s.Split('\n')
来源：http://ip.haigaiapp.cn

[E20] 判断字符串是否为空
来源：http://ir.gzmigu.cn

Py:   if not s:
来源：http://ha.nicolike.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ph.shtwfgs.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wd.szxytkj.cn

TS:   if (s === "") {}
来源：http://ve.shxzukj.cn

Java: if (s.isEmpty()) {}
来源：http://vt.nszjky.cn

Go:   if s == "" {}
来源：http://ay.huixiangedu.cn

Ruby: if s.empty?
来源：http://ss.yuexingan06.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dl.bjjhwx.cn

[E21] 超长截断加省略号
来源：http://tc.muxihuayi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://jr.haigaiapp.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://nq.chemitech.net.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://eo.nicolike.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://eq.szxytkj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pe.asd995.cn

Go:   // 按 rune 判断长度后截断
来源：http://lq.huixiangedu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tx.asd995.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://np.huixinmuqiang.cn

[E22] 字节长度与字符长度
来源：http://xv.jctech888.com.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hk.shxzukj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://eb.haigaiapp.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://tv.hahajie.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pz.asd995.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://za.9csxet.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://oc.newstarts.cn

Ruby: s.bytesize;  s.length
来源：http://gp.huixiangedu.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kz.szsharing.cn

================================================================================
来源：http://bc.gzmigu.cn

F. 文件与目录
来源：http://pg.hahajie.cn

================================================================================
来源：http://th.521024.cn

[F01] 读取整个文件
来源：http://cr.bjjhwx.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ae.bookmarksfly.cn

PHP:  file_get_contents("a.txt");
来源：http://lj.panjiajie.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://cv.colortex.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jl.9csxet.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ez.nszjky.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://me.chemitech.net.cn

Ruby: File.read("a.txt")
来源：http://ri.yuexingan06.cn

C#:   File.ReadAllText("a.txt");
来源：http://rx.huixiangedu.cn

[F02] 逐行读取文件
来源：http://jk.muxihuayi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://zc.chemitech.net.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dw.jctech888.com.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ip.hnjuh.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ym.asd995.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pc.bjjhwx.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hq.hnjuh.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ve.newstarts.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ny.colortex.cn

[F03] 写入文件（覆盖）
来源：http://se.yuexingan06.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://yh.wgjwhj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://yc.szsharing.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://st.shxzukj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mg.shtwfgs.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vl.gzmigu.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rr.521024.cn

Ruby: File.write("a.txt", "hi")
来源：http://yo.hahajie.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lx.haigaiapp.cn

[F04] 追加写入文件
来源：http://is.haigaiapp.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://sc.panjiajie.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ll.shtwfgs.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ap.gzmigu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ds.newstarts.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://nz.szsharing.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ju.haigaiapp.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fi.gzmigu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lf.bookmarksfly.cn

[F05] 判断文件或目录是否存在
来源：http://cu.huixinmuqiang.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gq.yuexingan06.cn

PHP:  file_exists("a.txt");
来源：http://ob.shxzukj.cn

JS:   fs.existsSync("a.txt")
来源：http://qh.muxihuayi.cn

TS:   fs.existsSync("a.txt")
来源：http://ar.9csxet.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://xe.panjiajie.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ig.lnxyls.cn

Ruby: File.exist?("a.txt")
来源：http://gf.9csxet.cn

C#:   File.Exists("a.txt")
来源：http://yy.hnjuh.cn

[F06] 删除文件
来源：http://yr.panjiajie.cn

Py:   os.remove("a.txt")
来源：http://gx.haigaiapp.cn

PHP:  unlink("a.txt");
来源：http://ye.gzmigu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://mb.shxzskj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://mu.hahajie.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://eq.chemitech.net.cn

Go:   os.Remove("a.txt")
来源：http://ep.jctech888.com.cn

Ruby: File.delete("a.txt")
来源：http://lv.huixinmuqiang.cn

C#:   File.Delete("a.txt");
来源：http://cy.bookmarksfly.cn

[F07] 创建目录（含多级）
来源：http://qi.gzmigu.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qy.nicolike.cn


<!-- 参考信息 -->