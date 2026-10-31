代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://zy.yuexingan06.cn

Ruby: arr.include?(x)
来源：http://ul.nszjky.cn

C#:   list.Contains(x)
来源：http://eq.nicolike.cn

[D22] 复制数组（避免共享引用）
来源：http://nu.chemitech.net.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jv.hnjuh.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mv.jctech888.com.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ho.szsharing.cn

TS:   [...arr];
来源：http://oq.nszjky.cn

Java: new ArrayList<>(list);
来源：http://nm.panjiajie.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ym.haigaiapp.cn

Ruby: arr.dup;  arr.clone
来源：http://ra.huanxung.cn

C#:   new List<int>(list);
来源：http://aw.panjiajie.cn

[D23] reduce 累积计算
来源：http://mo.szxytkj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lf.bjjhwx.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fv.newstarts.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dz.gzmigu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jd.nszjky.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://bq.shxzukj.cn

Go:   // 手写循环
来源：http://iw.chemitech.net.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fj.hnjuh.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zv.9csxet.cn

[D24] 字典 / Map 基本操作
来源：http://eq.shxzukj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ps.jianghongdianzi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ha.haigaiapp.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://aa.shxzskj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bj.wgjwhj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://kq.szsharing.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rs.newstarts.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ez.lnxyls.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kv.newstarts.cn

[D25] Set 集合去重与交并差
来源：http://ox.szsharing.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://og.huixinmuqiang.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rh.chemitech.net.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://om.9csxet.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fb.521024.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rq.huixiangedu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xr.bookmarksfly.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dz.haigaiapp.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hh.szsharing.cn

[D26] 数组转字符串
来源：http://sl.shtwfgs.cn

Py:   ", ".join(map(str, arr))
来源：http://vm.panjiajie.cn

PHP:  implode(", ", $arr);
来源：http://jt.huanxung.cn

JS:   arr.join(", ")
来源：http://mi.lnxyls.cn

TS:   arr.join(", ")
来源：http://om.wgjwhj.cn

Java: String.join(", ", list)
来源：http://jq.shxzukj.cn

Go:   strings.Join(strs, ", ")
来源：http://ud.haigaiapp.cn

Ruby: arr.join(", ")
来源：http://an.nicolike.cn

C#:   string.Join(", ", list)
来源：http://nx.jctech888.com.cn

================================================================================
来源：http://yj.bjjhwx.cn

E. 字符串处理
来源：http://xc.huixinmuqiang.cn

================================================================================
来源：http://je.shxzskj.cn

[E01] 拼接字符串
来源：http://xb.wgjwhj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://nh.colortex.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://oo.gzmigu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ws.jctech888.com.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://oz.lnxyls.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://dj.bookmarksfly.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ar.gzmigu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ro.muxihuayi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bm.yuntaijiaju.cn

[E02] 重复字符串
来源：http://vw.hnjuh.cn

Py:   "ab" * 3
来源：http://ye.jianghongdianzi.cn

PHP:  str_repeat("ab", 3);
来源：http://mt.nszjky.cn

JS:   "ab".repeat(3)
来源：http://pz.shtwfgs.cn

TS:   "ab".repeat(3)
来源：http://uu.nszjky.cn

Java: "ab".repeat(3)
来源：http://ql.hnjuh.cn

Go:   strings.Repeat("ab", 3)
来源：http://br.gzmigu.cn

Ruby: "ab" * 3
来源：http://gv.shxzukj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://uf.newstarts.cn

[E03] 截取子串
来源：http://qr.asd995.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ri.haigaiapp.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://uk.hahajie.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://iu.nszjky.cn

TS:   s.slice(1, 4)
来源：http://oc.muxihuayi.cn

Java: s.substring(1, 4)
来源：http://fv.hnjuh.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://sh.lnxyls.cn

Ruby: s[1, 3];  s[1..3]
来源：http://hz.shxzskj.cn

C#:   s.Substring(1, 3)
来源：http://aj.hahajie.cn

[E04] 查找子串位置
来源：http://xm.shxzskj.cn

Py:   s.find("x");  s.index("x")
来源：http://ul.huanxung.cn

PHP:  strpos($s, "x");
来源：http://jj.yuntaijiaju.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gm.hnjuh.cn

TS:   s.indexOf("x")
来源：http://sw.panjiajie.cn

Java: s.indexOf("x")
来源：http://nm.9csxet.cn

Go:   strings.Index(s, "x")
来源：http://ms.gzmigu.cn

Ruby: s.index("x")
来源：http://xr.colortex.cn

C#:   s.IndexOf("x")
来源：http://wm.bookmarksfly.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://pb.asd995.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gq.chemitech.net.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vj.szxytkj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yo.huanxung.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://xr.haigaiapp.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ox.gzmigu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://nm.nszjky.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tn.gzmigu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qn.hnjuh.cn

[E06] 替换子串
来源：http://eo.lnxyls.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kr.jianghongdianzi.cn

PHP:  str_replace("a", "b", $s);
来源：http://vi.shtwfgs.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://do.shxzukj.cn

TS:   s.replaceAll("a", "b")
来源：http://zc.colortex.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ml.9csxet.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ml.bookmarksfly.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nv.nszjky.cn

C#:   s.Replace("a", "b")
来源：http://tg.gzmigu.cn

[E07] 按分隔符拆分
来源：http://je.9csxet.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://at.panjiajie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://yx.shxzskj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://mo.shxzskj.cn

TS:   s.split(",")
来源：http://au.muxihuayi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://zc.asd995.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ec.shxzskj.cn

Ruby: s.split(",");  s.split
来源：http://lv.chemitech.net.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vk.newstarts.cn

[E08] 数组按分隔符合并
来源：http://ir.huixiangedu.cn

Py:   ",".join(items)
来源：http://ff.nszjky.cn

PHP:  implode(",", $items);
来源：http://ow.colortex.cn

JS:   items.join(",")
来源：http://hp.9csxet.cn

TS:   items.join(",")
来源：http://oz.muxihuayi.cn

Java: String.join(",", items)
来源：http://sb.521024.cn

Go:   strings.Join(items, ",")
来源：http://kp.bjjhwx.cn

Ruby: items.join(",")
来源：http://lm.521024.cn

C#:   string.Join(",", items)
来源：http://yr.muxihuayi.cn

[E09] 去除所有空白字符
来源：http://vy.bookmarksfly.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://dm.gzmigu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ym.szsharing.cn

JS:   s.replace(/\s+/g, "")
来源：http://ri.jctech888.com.cn

TS:   s.replace(/\s+/g, "")
来源：http://kl.szxytkj.cn

Java: s.replaceAll("\\s+", "")
来源：http://pp.bjjhwx.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://cs.chemitech.net.cn

Ruby: s.gsub(/\s+/, "")
来源：http://gg.shtwfgs.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gv.huixiangedu.cn

[E10] 左侧补零 / 定长填充
来源：http://ld.wgjwhj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vq.9csxet.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tc.szxytkj.cn

JS:   "7".padStart(3, "0")
来源：http://np.yuntaijiaju.cn

TS:   "7".padStart(3, "0")
来源：http://ab.nicolike.cn

Java: String.format("%03d", 7)
来源：http://xr.hahajie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://wg.jctech888.com.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vu.521024.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://pg.huanxung.cn

[E11] 反转字符串
来源：http://eq.gzmigu.cn

Py:   s[::-1]
来源：http://yw.yuntaijiaju.cn

PHP:  strrev($s);
来源：http://le.shxzukj.cn

JS:   [...s].reverse().join("")
来源：http://zi.wgjwhj.cn

TS:   [...s].reverse().join("")
来源：http://kz.bjjhwx.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://vo.chemitech.net.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://lw.nszjky.cn

Ruby: s.reverse
来源：http://ro.shxzukj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://fg.szxytkj.cn

[E12] 统计某字符出现次数
来源：http://gi.bookmarksfly.cn

Py:   s.count("a")
来源：http://ul.nicolike.cn

PHP:  substr_count($s, "a");
来源：http://gw.muxihuayi.cn

JS:   s.split("a").length - 1
来源：http://dq.shtwfgs.cn

TS:   s.split("a").length - 1
来源：http://gb.yuntaijiaju.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://sy.gzmigu.cn

Go:   strings.Count(s, "a")
来源：http://ii.panjiajie.cn

Ruby: s.count("a")
来源：http://dc.hahajie.cn

C#:   s.Count(c => c == 'a')
来源：http://ou.huixinmuqiang.cn

[E13] 逐字符遍历
来源：http://qy.shtwfgs.cn

Py:   for ch in s: print(ch)
来源：http://zk.huixiangedu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.chemitech.net.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://rk.hnjuh.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://tr.shxzukj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://so.newstarts.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gr.nicolike.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://sa.asd995.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://lh.jianghongdianzi.cn

[E14] URL 编码与 Base64
来源：http://ph.9csxet.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pd.chemitech.net.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://sz.yuexingan06.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://cy.wgjwhj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://oz.shxzskj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ho.hahajie.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://oc.chemitech.net.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fg.9csxet.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mi.huanxung.cn

[E15] HTML 转义 / 反转义
来源：http://uv.panjiajie.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://re.bookmarksfly.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://pj.yuntaijiaju.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://sa.huixiangedu.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://so.jctech888.com.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://aq.lnxyls.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hr.shtwfgs.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://yt.yuexingan06.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://pl.yuexingan06.cn

[E16] 数字千分位
来源：http://bt.bjjhwx.cn

Py:   f"{1234567:,}"
来源：http://rg.huanxung.cn

PHP:  number_format(1234567);
来源：http://rg.chemitech.net.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.shxzukj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ii.jianghongdianzi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://pb.colortex.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vp.jianghongdianzi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ov.newstarts.cn

C#:   1234567.ToString("N0")
来源：http://cf.huixinmuqiang.cn

[E17] 首字母大写
来源：http://ra.lnxyls.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://eg.shxzukj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://na.bookmarksfly.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uv.szxytkj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ej.bjjhwx.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hx.nszjky.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hx.521024.cn

Ruby: s.capitalize
来源：http://us.yuntaijiaju.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://az.shxzskj.cn

[E18] 模板占位符替换
来源：http://sc.lnxyls.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kd.nicolike.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://cx.nicolike.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://tw.nicolike.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://rp.nszjky.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://cx.huanxung.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ow.9csxet.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xd.newstarts.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ax.chemitech.net.cn

[E19] 多行文本按行拆分
来源：http://ph.huixiangedu.cn

Py:   s.splitlines()
来源：http://vt.shtwfgs.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hk.gzmigu.cn

JS:   s.split(/\r?\n/)
来源：http://os.521024.cn

TS:   s.split(/\r?\n/)
来源：http://ok.gzmigu.cn

Java: s.lines().toList()
来源：http://pm.yuntaijiaju.cn

Go:   strings.Split(s, "\n")
来源：http://dd.nszjky.cn

Ruby: s.lines
来源：http://ma.bookmarksfly.cn

C#:   s.Split('\n')
来源：http://of.huixinmuqiang.cn

[E20] 判断字符串是否为空
来源：http://km.bjjhwx.cn

Py:   if not s:
来源：http://vp.bookmarksfly.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vh.haigaiapp.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vn.jctech888.com.cn

TS:   if (s === "") {}
来源：http://kl.521024.cn

Java: if (s.isEmpty()) {}
来源：http://kb.nicolike.cn

Go:   if s == "" {}
来源：http://ym.hahajie.cn

Ruby: if s.empty?
来源：http://le.jctech888.com.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vn.huixinmuqiang.cn

[E21] 超长截断加省略号
来源：http://di.muxihuayi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://su.szxytkj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://nb.hnjuh.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rj.nicolike.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ym.nicolike.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gs.bookmarksfly.cn

Go:   // 按 rune 判断长度后截断
来源：http://it.9csxet.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ye.9csxet.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tm.colortex.cn

[E22] 字节长度与字符长度
来源：http://ku.nszjky.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vg.jctech888.com.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ym.szxytkj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pn.asd995.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nm.nszjky.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://on.nicolike.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://te.lnxyls.cn

Ruby: s.bytesize;  s.length
来源：http://mj.bookmarksfly.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ss.hnjuh.cn

================================================================================
来源：http://hx.hnjuh.cn

F. 文件与目录
来源：http://ye.yuntaijiaju.cn

================================================================================
来源：http://ij.hahajie.cn

[F01] 读取整个文件
来源：http://bf.9csxet.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://yy.huixinmuqiang.cn

PHP:  file_get_contents("a.txt");
来源：http://ki.asd995.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://yk.shtwfgs.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ek.hahajie.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://jo.lnxyls.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://sc.asd995.cn

Ruby: File.read("a.txt")
来源：http://vw.gzmigu.cn

C#:   File.ReadAllText("a.txt");
来源：http://rd.bjjhwx.cn

[F02] 逐行读取文件
来源：http://sn.newstarts.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://zd.bookmarksfly.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wk.521024.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vd.bjjhwx.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sj.nicolike.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mt.nicolike.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hm.yuntaijiaju.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mf.shxzukj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://it.9csxet.cn

[F03] 写入文件（覆盖）
来源：http://mp.hnjuh.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ej.9csxet.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://cp.shtwfgs.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://iu.huanxung.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dp.huanxung.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://if.colortex.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://pf.jctech888.com.cn

Ruby: File.write("a.txt", "hi")
来源：http://vu.muxihuayi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mo.asd995.cn

[F04] 追加写入文件
来源：http://av.jctech888.com.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://yd.colortex.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bs.panjiajie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yf.yuntaijiaju.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sr.nicolike.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://di.newstarts.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ft.huanxung.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://we.nicolike.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rb.huixiangedu.cn

[F05] 判断文件或目录是否存在
来源：http://lq.bjjhwx.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://uv.jctech888.com.cn

PHP:  file_exists("a.txt");
来源：http://nw.gzmigu.cn

JS:   fs.existsSync("a.txt")
来源：http://io.huixiangedu.cn

TS:   fs.existsSync("a.txt")
来源：http://io.nszjky.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ei.szsharing.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vu.shxzskj.cn

Ruby: File.exist?("a.txt")
来源：http://ta.chemitech.net.cn

C#:   File.Exists("a.txt")
来源：http://bl.wgjwhj.cn

[F06] 删除文件
来源：http://ll.szsharing.cn

Py:   os.remove("a.txt")
来源：http://mb.521024.cn

PHP:  unlink("a.txt");
来源：http://kh.yuntaijiaju.cn


<!-- 参考信息 -->