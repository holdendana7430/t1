代发 wailian999

Java: new ArrayList<>(list);
来源：http://ah.shxzukj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://sz.huixiangedu.cn

Ruby: arr.dup;  arr.clone
来源：http://zj.shxzukj.cn

C#:   new List<int>(list);
来源：http://qb.yuexingan06.cn

[D23] reduce 累积计算
来源：http://dv.9csxet.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://tx.9csxet.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://is.lnxyls.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mj.chemitech.net.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ki.521024.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://xi.shxzukj.cn

Go:   // 手写循环
来源：http://zq.asd995.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fr.szxytkj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://eu.bjjhwx.cn

[D24] 字典 / Map 基本操作
来源：http://fb.shtwfgs.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gc.shxzskj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qv.szsharing.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://er.asd995.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://sr.chemitech.net.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ko.yuntaijiaju.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bt.wgjwhj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://dv.newstarts.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://tu.szxytkj.cn

[D25] Set 集合去重与交并差
来源：http://wq.szsharing.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://dl.bjjhwx.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gh.wgjwhj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://dm.newstarts.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hd.huanxung.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://sb.newstarts.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://eo.shxzukj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gq.haigaiapp.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ge.hahajie.cn

[D26] 数组转字符串
来源：http://yx.lnxyls.cn

Py:   ", ".join(map(str, arr))
来源：http://zk.colortex.cn

PHP:  implode(", ", $arr);
来源：http://nu.newstarts.cn

JS:   arr.join(", ")
来源：http://an.shxzukj.cn

TS:   arr.join(", ")
来源：http://ku.wgjwhj.cn

Java: String.join(", ", list)
来源：http://ym.szsharing.cn

Go:   strings.Join(strs, ", ")
来源：http://jv.521024.cn

Ruby: arr.join(", ")
来源：http://jb.nicolike.cn

C#:   string.Join(", ", list)
来源：http://eu.chemitech.net.cn

================================================================================
来源：http://nn.521024.cn

E. 字符串处理
来源：http://rb.lnxyls.cn

================================================================================
来源：http://rp.shxzskj.cn

[E01] 拼接字符串
来源：http://rc.huanxung.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mf.asd995.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rj.hahajie.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://sw.chemitech.net.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://cd.colortex.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ld.hahajie.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tu.huixinmuqiang.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xq.chemitech.net.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wd.hahajie.cn

[E02] 重复字符串
来源：http://nz.bjjhwx.cn

Py:   "ab" * 3
来源：http://hd.yuexingan06.cn

PHP:  str_repeat("ab", 3);
来源：http://kd.asd995.cn

JS:   "ab".repeat(3)
来源：http://ul.muxihuayi.cn

TS:   "ab".repeat(3)
来源：http://mu.chemitech.net.cn

Java: "ab".repeat(3)
来源：http://vq.shtwfgs.cn

Go:   strings.Repeat("ab", 3)
来源：http://wk.jctech888.com.cn

Ruby: "ab" * 3
来源：http://li.521024.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ls.yuexingan06.cn

[E03] 截取子串
来源：http://gn.huanxung.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ni.hnjuh.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://zn.szxytkj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://kn.nicolike.cn

TS:   s.slice(1, 4)
来源：http://kj.jianghongdianzi.cn

Java: s.substring(1, 4)
来源：http://bm.huixiangedu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://yg.nicolike.cn

Ruby: s[1, 3];  s[1..3]
来源：http://qv.lnxyls.cn

C#:   s.Substring(1, 3)
来源：http://uw.huixinmuqiang.cn

[E04] 查找子串位置
来源：http://tb.shxzskj.cn

Py:   s.find("x");  s.index("x")
来源：http://ce.shxzukj.cn

PHP:  strpos($s, "x");
来源：http://dn.nicolike.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://yk.muxihuayi.cn

TS:   s.indexOf("x")
来源：http://yq.bjjhwx.cn

Java: s.indexOf("x")
来源：http://ew.newstarts.cn

Go:   strings.Index(s, "x")
来源：http://id.colortex.cn

Ruby: s.index("x")
来源：http://lx.colortex.cn

C#:   s.IndexOf("x")
来源：http://ha.jctech888.com.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://uh.newstarts.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dg.jctech888.com.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ww.shxzukj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sl.szsharing.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://br.gzmigu.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nm.szxytkj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://sn.nszjky.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://os.shxzskj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ai.shtwfgs.cn

[E06] 替换子串
来源：http://kz.asd995.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gd.huanxung.cn

PHP:  str_replace("a", "b", $s);
来源：http://vl.asd995.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kv.szxytkj.cn

TS:   s.replaceAll("a", "b")
来源：http://dx.yuntaijiaju.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ab.521024.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hj.bookmarksfly.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://oj.hahajie.cn

C#:   s.Replace("a", "b")
来源：http://os.colortex.cn

[E07] 按分隔符拆分
来源：http://vw.nicolike.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hx.lnxyls.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://lf.huixiangedu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://bh.wgjwhj.cn

TS:   s.split(",")
来源：http://os.wgjwhj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://np.nszjky.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://yr.bookmarksfly.cn

Ruby: s.split(",");  s.split
来源：http://mo.shtwfgs.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bg.jctech888.com.cn

[E08] 数组按分隔符合并
来源：http://wl.haigaiapp.cn

Py:   ",".join(items)
来源：http://bc.szxytkj.cn

PHP:  implode(",", $items);
来源：http://ce.nszjky.cn

JS:   items.join(",")
来源：http://ke.nszjky.cn

TS:   items.join(",")
来源：http://cy.nszjky.cn

Java: String.join(",", items)
来源：http://mg.muxihuayi.cn

Go:   strings.Join(items, ",")
来源：http://xp.szxytkj.cn

Ruby: items.join(",")
来源：http://qp.yuexingan06.cn

C#:   string.Join(",", items)
来源：http://hu.wgjwhj.cn

[E09] 去除所有空白字符
来源：http://tn.hahajie.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lr.bjjhwx.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ac.chemitech.net.cn

JS:   s.replace(/\s+/g, "")
来源：http://qy.yuntaijiaju.cn

TS:   s.replace(/\s+/g, "")
来源：http://qs.9csxet.cn

Java: s.replaceAll("\\s+", "")
来源：http://ji.asd995.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://vq.bjjhwx.cn

Ruby: s.gsub(/\s+/, "")
来源：http://wb.newstarts.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cl.jianghongdianzi.cn

[E10] 左侧补零 / 定长填充
来源：http://mj.bookmarksfly.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ka.jctech888.com.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://on.szsharing.cn

JS:   "7".padStart(3, "0")
来源：http://zi.colortex.cn

TS:   "7".padStart(3, "0")
来源：http://th.shtwfgs.cn

Java: String.format("%03d", 7)
来源：http://ks.asd995.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://yt.shxzukj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ii.hahajie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://gz.bjjhwx.cn

[E11] 反转字符串
来源：http://nx.szxytkj.cn

Py:   s[::-1]
来源：http://ou.huixiangedu.cn

PHP:  strrev($s);
来源：http://yh.huixiangedu.cn

JS:   [...s].reverse().join("")
来源：http://vd.szsharing.cn

TS:   [...s].reverse().join("")
来源：http://kz.9csxet.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://hn.newstarts.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://qq.shtwfgs.cn

Ruby: s.reverse
来源：http://ne.colortex.cn

C#:   new string(s.Reverse().ToArray())
来源：http://sg.lnxyls.cn

[E12] 统计某字符出现次数
来源：http://xj.shxzukj.cn

Py:   s.count("a")
来源：http://rl.huanxung.cn

PHP:  substr_count($s, "a");
来源：http://ks.chemitech.net.cn

JS:   s.split("a").length - 1
来源：http://pb.gzmigu.cn

TS:   s.split("a").length - 1
来源：http://mi.muxihuayi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://px.panjiajie.cn

Go:   strings.Count(s, "a")
来源：http://rx.nicolike.cn

Ruby: s.count("a")
来源：http://xt.9csxet.cn

C#:   s.Count(c => c == 'a')
来源：http://ql.wgjwhj.cn

[E13] 逐字符遍历
来源：http://rv.muxihuayi.cn

Py:   for ch in s: print(ch)
来源：http://zm.huixinmuqiang.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qh.szxytkj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://zf.szxytkj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ht.colortex.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ll.bjjhwx.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ew.asd995.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://uq.chemitech.net.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gt.huixinmuqiang.cn

[E14] URL 编码与 Base64
来源：http://vg.shxzukj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fd.chemitech.net.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://km.hnjuh.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ow.gzmigu.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hh.jctech888.com.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xd.shxzskj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hn.haigaiapp.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vv.wgjwhj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://cv.asd995.cn

[E15] HTML 转义 / 反转义
来源：http://az.huanxung.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://by.521024.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://tb.gzmigu.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jn.huixiangedu.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ja.chemitech.net.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tz.lnxyls.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ob.asd995.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://sf.nszjky.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ax.shxzskj.cn

[E16] 数字千分位
来源：http://ur.hahajie.cn

Py:   f"{1234567:,}"
来源：http://be.wgjwhj.cn

PHP:  number_format(1234567);
来源：http://wz.szsharing.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://zp.gzmigu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://xa.yuexingan06.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://pe.asd995.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ln.hnjuh.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gn.huixinmuqiang.cn

C#:   1234567.ToString("N0")
来源：http://lm.yuexingan06.cn

[E17] 首字母大写
来源：http://mz.jianghongdianzi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ma.shxzskj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://mk.lnxyls.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://av.huixiangedu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pf.muxihuayi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ur.szxytkj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://yb.shxzukj.cn

Ruby: s.capitalize
来源：http://ek.yuexingan06.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rs.panjiajie.cn

[E18] 模板占位符替换
来源：http://bz.huixiangedu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://sv.huixinmuqiang.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gl.lnxyls.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ie.chemitech.net.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://kq.panjiajie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ai.muxihuayi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lg.nicolike.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://or.shxzskj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vh.nszjky.cn

[E19] 多行文本按行拆分
来源：http://xg.shtwfgs.cn

Py:   s.splitlines()
来源：http://qp.huixiangedu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://oy.shxzukj.cn

JS:   s.split(/\r?\n/)
来源：http://xn.haigaiapp.cn

TS:   s.split(/\r?\n/)
来源：http://lv.shtwfgs.cn

Java: s.lines().toList()
来源：http://fp.colortex.cn

Go:   strings.Split(s, "\n")
来源：http://zw.hnjuh.cn

Ruby: s.lines
来源：http://uy.jianghongdianzi.cn

C#:   s.Split('\n')
来源：http://qp.gzmigu.cn

[E20] 判断字符串是否为空
来源：http://ah.szsharing.cn

Py:   if not s:
来源：http://oz.wgjwhj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hm.szxytkj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tj.shxzskj.cn

TS:   if (s === "") {}
来源：http://as.szsharing.cn

Java: if (s.isEmpty()) {}
来源：http://eq.lnxyls.cn

Go:   if s == "" {}
来源：http://jc.szxytkj.cn

Ruby: if s.empty?
来源：http://iz.jianghongdianzi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jl.lnxyls.cn

[E21] 超长截断加省略号
来源：http://me.jianghongdianzi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://fi.gzmigu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ux.shxzskj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fx.lnxyls.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rb.asd995.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wf.huixinmuqiang.cn

Go:   // 按 rune 判断长度后截断
来源：http://pb.lnxyls.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://zt.yuntaijiaju.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vj.panjiajie.cn

[E22] 字节长度与字符长度
来源：http://po.asd995.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hx.huixiangedu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ht.shtwfgs.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ns.shxzskj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jd.asd995.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xd.shtwfgs.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ej.huixiangedu.cn

Ruby: s.bytesize;  s.length
来源：http://hn.jianghongdianzi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xj.bookmarksfly.cn

================================================================================
来源：http://dz.gzmigu.cn

F. 文件与目录
来源：http://dl.nszjky.cn

================================================================================
来源：http://hz.huixinmuqiang.cn

[F01] 读取整个文件
来源：http://np.jianghongdianzi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://uv.chemitech.net.cn

PHP:  file_get_contents("a.txt");
来源：http://yx.wgjwhj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rx.szxytkj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://og.huixinmuqiang.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://zt.muxihuayi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pq.muxihuayi.cn

Ruby: File.read("a.txt")
来源：http://kp.szxytkj.cn

C#:   File.ReadAllText("a.txt");
来源：http://gp.yuntaijiaju.cn

[F02] 逐行读取文件
来源：http://bj.jianghongdianzi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ux.chemitech.net.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.yuntaijiaju.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ny.shtwfgs.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fs.521024.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bl.nicolike.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rh.szxytkj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rn.bookmarksfly.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ai.huanxung.cn

[F03] 写入文件（覆盖）
来源：http://js.shxzskj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gm.shxzukj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://et.huixinmuqiang.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zm.muxihuayi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xc.wgjwhj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://oo.szsharing.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://he.gzmigu.cn

Ruby: File.write("a.txt", "hi")
来源：http://xp.newstarts.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://rb.shtwfgs.cn

[F04] 追加写入文件
来源：http://kp.shxzukj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://fx.huanxung.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://om.bookmarksfly.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pm.9csxet.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wz.jctech888.com.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://nn.shxzukj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vx.shxzukj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yd.bjjhwx.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dd.shxzskj.cn

[F05] 判断文件或目录是否存在
来源：http://vr.wgjwhj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hk.colortex.cn

PHP:  file_exists("a.txt");
来源：http://ly.colortex.cn

JS:   fs.existsSync("a.txt")
来源：http://wl.hnjuh.cn

TS:   fs.existsSync("a.txt")
来源：http://cy.shxzukj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://su.asd995.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wl.bjjhwx.cn

Ruby: File.exist?("a.txt")
来源：http://ff.chemitech.net.cn

C#:   File.Exists("a.txt")
来源：http://jf.haigaiapp.cn

[F06] 删除文件
来源：http://pg.nicolike.cn

Py:   os.remove("a.txt")
来源：http://rz.szsharing.cn

PHP:  unlink("a.txt");
来源：http://yr.jctech888.com.cn

JS:   fs.unlinkSync("a.txt")
来源：http://xe.yuntaijiaju.cn

TS:   fs.unlinkSync("a.txt")
来源：http://cb.shxzskj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://sz.yuexingan06.cn

Go:   os.Remove("a.txt")
来源：http://dw.lnxyls.cn

Ruby: File.delete("a.txt")
来源：http://qx.jctech888.com.cn

C#:   File.Delete("a.txt");
来源：http://ku.huanxung.cn

[F07] 创建目录（含多级）
来源：http://in.huanxung.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://na.jctech888.com.cn


<!-- 参考信息 -->