代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jf.9csxet.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://by.nszjky.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jq.9csxet.cn

Go:   // 手写 map[T]int
来源：http://li.huanxung.cn

Ruby: arr.tally
来源：http://rq.521024.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mj.panjiajie.cn

[D21] 判断是否包含某元素
来源：http://xm.chemitech.net.cn

Py:   x in arr
来源：http://nu.muxihuayi.cn

PHP:  in_array($x, $arr, true);
来源：http://ym.yuexingan06.cn

JS:   arr.includes(x)
来源：http://ab.jctech888.com.cn

TS:   arr.includes(x)
来源：http://np.hnjuh.cn

Java: list.contains(x)
来源：http://lr.szsharing.cn

Go:   slices.Contains(arr, x)
来源：http://eu.huixiangedu.cn

Ruby: arr.include?(x)
来源：http://pk.gzmigu.cn

C#:   list.Contains(x)
来源：http://ez.shxzskj.cn

[D22] 复制数组（避免共享引用）
来源：http://xd.shtwfgs.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://yk.shxzukj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vy.shtwfgs.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://uw.9csxet.cn

TS:   [...arr];
来源：http://nj.nszjky.cn

Java: new ArrayList<>(list);
来源：http://fs.huanxung.cn

Go:   copied := append([]int(nil), arr...)
来源：http://jw.bookmarksfly.cn

Ruby: arr.dup;  arr.clone
来源：http://lq.haigaiapp.cn

C#:   new List<int>(list);
来源：http://ng.asd995.cn

[D23] reduce 累积计算
来源：http://dx.panjiajie.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ui.szxytkj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://za.panjiajie.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ud.chemitech.net.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tm.haigaiapp.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://lx.jianghongdianzi.cn

Go:   // 手写循环
来源：http://kt.newstarts.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://uo.521024.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://lj.huixiangedu.cn

[D24] 字典 / Map 基本操作
来源：http://pt.yuexingan06.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hm.shxzskj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ok.jianghongdianzi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://oo.bookmarksfly.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://pe.haigaiapp.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ad.panjiajie.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ah.shtwfgs.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vx.gzmigu.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fm.bookmarksfly.cn

[D25] Set 集合去重与交并差
来源：http://mt.szxytkj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vc.asd995.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qz.shxzskj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://li.9csxet.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fl.huixiangedu.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wi.yuexingan06.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://he.hahajie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://iu.newstarts.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vd.lnxyls.cn

[D26] 数组转字符串
来源：http://to.chemitech.net.cn

Py:   ", ".join(map(str, arr))
来源：http://qa.hnjuh.cn

PHP:  implode(", ", $arr);
来源：http://oc.huanxung.cn

JS:   arr.join(", ")
来源：http://ex.521024.cn

TS:   arr.join(", ")
来源：http://jb.jctech888.com.cn

Java: String.join(", ", list)
来源：http://kl.jctech888.com.cn

Go:   strings.Join(strs, ", ")
来源：http://xh.shxzukj.cn

Ruby: arr.join(", ")
来源：http://fn.huixinmuqiang.cn

C#:   string.Join(", ", list)
来源：http://ob.shxzskj.cn

================================================================================
来源：http://lf.huixiangedu.cn

E. 字符串处理
来源：http://xf.huixinmuqiang.cn

================================================================================
来源：http://px.shxzukj.cn

[E01] 拼接字符串
来源：http://qm.yuexingan06.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://aq.chemitech.net.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ir.bjjhwx.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gx.newstarts.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tv.shxzskj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ec.muxihuayi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bj.bjjhwx.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hp.bjjhwx.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://yw.hnjuh.cn

[E02] 重复字符串
来源：http://uy.9csxet.cn

Py:   "ab" * 3
来源：http://bs.muxihuayi.cn

PHP:  str_repeat("ab", 3);
来源：http://rf.szxytkj.cn

JS:   "ab".repeat(3)
来源：http://zk.yuntaijiaju.cn

TS:   "ab".repeat(3)
来源：http://df.yuexingan06.cn

Java: "ab".repeat(3)
来源：http://fc.yuntaijiaju.cn

Go:   strings.Repeat("ab", 3)
来源：http://ja.nicolike.cn

Ruby: "ab" * 3
来源：http://ut.jctech888.com.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://bf.hahajie.cn

[E03] 截取子串
来源：http://nh.huixinmuqiang.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://me.wgjwhj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://zf.521024.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wk.jianghongdianzi.cn

TS:   s.slice(1, 4)
来源：http://nc.jianghongdianzi.cn

Java: s.substring(1, 4)
来源：http://nm.bjjhwx.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://cr.yuexingan06.cn

Ruby: s[1, 3];  s[1..3]
来源：http://jp.muxihuayi.cn

C#:   s.Substring(1, 3)
来源：http://va.yuntaijiaju.cn

[E04] 查找子串位置
来源：http://am.huixinmuqiang.cn

Py:   s.find("x");  s.index("x")
来源：http://jb.szxytkj.cn

PHP:  strpos($s, "x");
来源：http://sq.colortex.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ix.newstarts.cn

TS:   s.indexOf("x")
来源：http://ss.hahajie.cn

Java: s.indexOf("x")
来源：http://mv.newstarts.cn

Go:   strings.Index(s, "x")
来源：http://ac.9csxet.cn

Ruby: s.index("x")
来源：http://rl.lnxyls.cn

C#:   s.IndexOf("x")
来源：http://ua.9csxet.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://yc.huanxung.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qb.muxihuayi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ho.bjjhwx.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tp.nszjky.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://hf.shxzukj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gs.9csxet.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wb.shxzukj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vy.panjiajie.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rn.shtwfgs.cn

[E06] 替换子串
来源：http://au.521024.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fj.yuexingan06.cn

PHP:  str_replace("a", "b", $s);
来源：http://sr.yuntaijiaju.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://en.panjiajie.cn

TS:   s.replaceAll("a", "b")
来源：http://pk.colortex.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uf.bjjhwx.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://co.yuexingan06.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ty.shxzskj.cn

C#:   s.Replace("a", "b")
来源：http://bu.bjjhwx.cn

[E07] 按分隔符拆分
来源：http://cy.hahajie.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://sd.haigaiapp.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ts.panjiajie.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://mu.shtwfgs.cn

TS:   s.split(",")
来源：http://dx.nszjky.cn

Java: s.split(",");  s.split("\\s+")
来源：http://py.lnxyls.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://el.jianghongdianzi.cn

Ruby: s.split(",");  s.split
来源：http://hm.jctech888.com.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kh.szsharing.cn

[E08] 数组按分隔符合并
来源：http://rr.9csxet.cn

Py:   ",".join(items)
来源：http://ss.jianghongdianzi.cn

PHP:  implode(",", $items);
来源：http://ho.gzmigu.cn

JS:   items.join(",")
来源：http://uo.shtwfgs.cn

TS:   items.join(",")
来源：http://cc.shxzukj.cn

Java: String.join(",", items)
来源：http://fs.haigaiapp.cn

Go:   strings.Join(items, ",")
来源：http://xl.lnxyls.cn

Ruby: items.join(",")
来源：http://un.nszjky.cn

C#:   string.Join(",", items)
来源：http://dc.9csxet.cn

[E09] 去除所有空白字符
来源：http://zy.huanxung.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://sx.jctech888.com.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://oa.nicolike.cn

JS:   s.replace(/\s+/g, "")
来源：http://gz.bjjhwx.cn

TS:   s.replace(/\s+/g, "")
来源：http://jk.haigaiapp.cn

Java: s.replaceAll("\\s+", "")
来源：http://ce.bjjhwx.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://hw.shxzskj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://gn.9csxet.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://tg.yuexingan06.cn

[E10] 左侧补零 / 定长填充
来源：http://xi.yuntaijiaju.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hi.hnjuh.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bs.huixiangedu.cn

JS:   "7".padStart(3, "0")
来源：http://mg.hahajie.cn

TS:   "7".padStart(3, "0")
来源：http://qy.yuexingan06.cn

Java: String.format("%03d", 7)
来源：http://sk.hnjuh.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://qb.yuntaijiaju.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vx.szxytkj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://nr.newstarts.cn

[E11] 反转字符串
来源：http://vw.muxihuayi.cn

Py:   s[::-1]
来源：http://oh.wgjwhj.cn

PHP:  strrev($s);
来源：http://qy.shxzukj.cn

JS:   [...s].reverse().join("")
来源：http://wf.szxytkj.cn

TS:   [...s].reverse().join("")
来源：http://yf.szsharing.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://np.hahajie.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://sd.bjjhwx.cn

Ruby: s.reverse
来源：http://ww.nicolike.cn

C#:   new string(s.Reverse().ToArray())
来源：http://mu.bookmarksfly.cn

[E12] 统计某字符出现次数
来源：http://jk.9csxet.cn

Py:   s.count("a")
来源：http://gb.shxzukj.cn

PHP:  substr_count($s, "a");
来源：http://mw.lnxyls.cn

JS:   s.split("a").length - 1
来源：http://cb.hnjuh.cn

TS:   s.split("a").length - 1
来源：http://vf.yuntaijiaju.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xw.shxzukj.cn

Go:   strings.Count(s, "a")
来源：http://ma.hnjuh.cn

Ruby: s.count("a")
来源：http://zc.shxzukj.cn

C#:   s.Count(c => c == 'a')
来源：http://iw.yuntaijiaju.cn

[E13] 逐字符遍历
来源：http://kr.nicolike.cn

Py:   for ch in s: print(ch)
来源：http://ib.panjiajie.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zg.521024.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://nt.hahajie.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://pm.jianghongdianzi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fr.9csxet.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wo.yuexingan06.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://rs.colortex.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ze.hahajie.cn

[E14] URL 编码与 Base64
来源：http://fe.yuexingan06.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qc.hahajie.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://vp.gzmigu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wu.wgjwhj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fh.nicolike.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://nb.huixinmuqiang.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://di.hahajie.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ko.bjjhwx.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://sv.asd995.cn

[E15] HTML 转义 / 反转义
来源：http://wm.newstarts.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://sv.shxzukj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ia.hahajie.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vb.chemitech.net.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ci.colortex.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ib.nszjky.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wl.gzmigu.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ve.lnxyls.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://il.szxytkj.cn

[E16] 数字千分位
来源：http://ay.hahajie.cn

Py:   f"{1234567:,}"
来源：http://sy.szsharing.cn

PHP:  number_format(1234567);
来源：http://jw.szxytkj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ky.huixiangedu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://yu.shxzskj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://eg.hnjuh.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://eg.hnjuh.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tp.yuexingan06.cn

C#:   1234567.ToString("N0")
来源：http://sh.wgjwhj.cn

[E17] 首字母大写
来源：http://yq.bookmarksfly.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://sx.huixinmuqiang.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://vw.9csxet.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ig.hahajie.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zp.huixinmuqiang.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ra.hahajie.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qs.nszjky.cn

Ruby: s.capitalize
来源：http://lj.yuntaijiaju.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dx.huixinmuqiang.cn

[E18] 模板占位符替换
来源：http://rs.shxzskj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mn.hnjuh.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zj.bookmarksfly.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://cd.szxytkj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://mb.colortex.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zl.jianghongdianzi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://re.jianghongdianzi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vy.nszjky.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qj.panjiajie.cn

[E19] 多行文本按行拆分
来源：http://pq.panjiajie.cn

Py:   s.splitlines()
来源：http://uv.szxytkj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mz.huixinmuqiang.cn

JS:   s.split(/\r?\n/)
来源：http://kl.lnxyls.cn

TS:   s.split(/\r?\n/)
来源：http://gs.panjiajie.cn

Java: s.lines().toList()
来源：http://md.bjjhwx.cn

Go:   strings.Split(s, "\n")
来源：http://qa.shxzskj.cn

Ruby: s.lines
来源：http://wd.wgjwhj.cn

C#:   s.Split('\n')
来源：http://td.yuexingan06.cn

[E20] 判断字符串是否为空
来源：http://ij.yuexingan06.cn

Py:   if not s:
来源：http://rn.bjjhwx.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ai.521024.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ma.bookmarksfly.cn

TS:   if (s === "") {}
来源：http://ho.hahajie.cn

Java: if (s.isEmpty()) {}
来源：http://rz.shxzskj.cn

Go:   if s == "" {}
来源：http://lk.chemitech.net.cn

Ruby: if s.empty?
来源：http://vn.shxzskj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://he.shxzukj.cn

[E21] 超长截断加省略号
来源：http://xo.newstarts.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ea.asd995.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://yw.muxihuayi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dd.jctech888.com.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://do.shxzukj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ka.nicolike.cn

Go:   // 按 rune 判断长度后截断
来源：http://oi.huixinmuqiang.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://kz.jianghongdianzi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tu.colortex.cn

[E22] 字节长度与字符长度
来源：http://dk.nicolike.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zk.jctech888.com.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wg.gzmigu.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://es.gzmigu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://eu.asd995.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vk.shxzskj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ig.huixinmuqiang.cn

Ruby: s.bytesize;  s.length
来源：http://yn.huixiangedu.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://up.gzmigu.cn

================================================================================
来源：http://kj.colortex.cn

F. 文件与目录
来源：http://si.lnxyls.cn

================================================================================
来源：http://va.lnxyls.cn

[F01] 读取整个文件
来源：http://cp.521024.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://kv.gzmigu.cn

PHP:  file_get_contents("a.txt");
来源：http://bf.9csxet.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://nc.521024.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rv.szxytkj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://xv.9csxet.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vl.yuexingan06.cn

Ruby: File.read("a.txt")
来源：http://vc.jctech888.com.cn

C#:   File.ReadAllText("a.txt");
来源：http://zm.muxihuayi.cn

[F02] 逐行读取文件
来源：http://hp.colortex.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ey.lnxyls.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qz.jianghongdianzi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ar.hnjuh.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ki.chemitech.net.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://us.muxihuayi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wc.chemitech.net.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://os.huixinmuqiang.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://kt.colortex.cn

[F03] 写入文件（覆盖）
来源：http://mi.nszjky.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xr.newstarts.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://fk.521024.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vv.hnjuh.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://er.szsharing.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qw.lnxyls.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ds.bookmarksfly.cn

Ruby: File.write("a.txt", "hi")
来源：http://zv.szxytkj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wu.huanxung.cn

[F04] 追加写入文件
来源：http://cx.jianghongdianzi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dg.haigaiapp.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://sz.szxytkj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kr.newstarts.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mt.yuexingan06.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://yh.haigaiapp.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hp.jianghongdianzi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ej.yuexingan06.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kk.521024.cn


<!-- 参考信息 -->