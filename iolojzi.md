代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://to.huixiangedu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jt.szsharing.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vv.asd995.cn

Go:   // 手写 map[T]int
来源：http://ta.lnxyls.cn

Ruby: arr.tally
来源：http://vj.nicolike.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ft.newstarts.cn

[D21] 判断是否包含某元素
来源：http://qw.newstarts.cn

Py:   x in arr
来源：http://yf.jianghongdianzi.cn

PHP:  in_array($x, $arr, true);
来源：http://pe.9csxet.cn

JS:   arr.includes(x)
来源：http://ii.shtwfgs.cn

TS:   arr.includes(x)
来源：http://ck.9csxet.cn

Java: list.contains(x)
来源：http://qp.jctech888.com.cn

Go:   slices.Contains(arr, x)
来源：http://dg.huixinmuqiang.cn

Ruby: arr.include?(x)
来源：http://ju.huanxung.cn

C#:   list.Contains(x)
来源：http://va.9csxet.cn

[D22] 复制数组（避免共享引用）
来源：http://kp.521024.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://si.huixinmuqiang.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://me.lnxyls.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fy.lnxyls.cn

TS:   [...arr];
来源：http://dh.muxihuayi.cn

Java: new ArrayList<>(list);
来源：http://om.panjiajie.cn

Go:   copied := append([]int(nil), arr...)
来源：http://uy.bookmarksfly.cn

Ruby: arr.dup;  arr.clone
来源：http://cv.jctech888.com.cn

C#:   new List<int>(list);
来源：http://zv.muxihuayi.cn

[D23] reduce 累积计算
来源：http://li.panjiajie.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://to.asd995.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ec.jctech888.com.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ie.asd995.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cw.szxytkj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://kd.shtwfgs.cn

Go:   // 手写循环
来源：http://pv.muxihuayi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://nq.shtwfgs.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rk.panjiajie.cn

[D24] 字典 / Map 基本操作
来源：http://ct.chemitech.net.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://cy.huanxung.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xc.huanxung.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hc.newstarts.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fs.huanxung.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bn.lnxyls.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rl.szxytkj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://af.asd995.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://uc.huanxung.cn

[D25] Set 集合去重与交并差
来源：http://nj.colortex.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wt.asd995.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rp.nszjky.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://dd.colortex.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://sx.panjiajie.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://fs.colortex.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://na.newstarts.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dz.panjiajie.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://gk.chemitech.net.cn

[D26] 数组转字符串
来源：http://gw.bookmarksfly.cn

Py:   ", ".join(map(str, arr))
来源：http://vj.wgjwhj.cn

PHP:  implode(", ", $arr);
来源：http://qa.gzmigu.cn

JS:   arr.join(", ")
来源：http://zi.wgjwhj.cn

TS:   arr.join(", ")
来源：http://me.asd995.cn

Java: String.join(", ", list)
来源：http://rf.jianghongdianzi.cn

Go:   strings.Join(strs, ", ")
来源：http://bh.colortex.cn

Ruby: arr.join(", ")
来源：http://vn.muxihuayi.cn

C#:   string.Join(", ", list)
来源：http://ep.521024.cn

================================================================================
来源：http://xn.shtwfgs.cn

E. 字符串处理
来源：http://qw.shtwfgs.cn

================================================================================
来源：http://yy.yuntaijiaju.cn

[E01] 拼接字符串
来源：http://zx.gzmigu.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bg.shxzskj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://yc.szxytkj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qn.szsharing.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vn.wgjwhj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qa.9csxet.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yk.hahajie.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ak.panjiajie.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://iq.colortex.cn

[E02] 重复字符串
来源：http://ta.nicolike.cn

Py:   "ab" * 3
来源：http://fg.muxihuayi.cn

PHP:  str_repeat("ab", 3);
来源：http://fx.yuexingan06.cn

JS:   "ab".repeat(3)
来源：http://fk.szsharing.cn

TS:   "ab".repeat(3)
来源：http://dj.szsharing.cn

Java: "ab".repeat(3)
来源：http://zz.9csxet.cn

Go:   strings.Repeat("ab", 3)
来源：http://xz.9csxet.cn

Ruby: "ab" * 3
来源：http://cc.lnxyls.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://kv.shtwfgs.cn

[E03] 截取子串
来源：http://hy.yuexingan06.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zi.gzmigu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://cz.szxytkj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rh.shxzukj.cn

TS:   s.slice(1, 4)
来源：http://km.jianghongdianzi.cn

Java: s.substring(1, 4)
来源：http://lh.gzmigu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ef.yuexingan06.cn

Ruby: s[1, 3];  s[1..3]
来源：http://hx.wgjwhj.cn

C#:   s.Substring(1, 3)
来源：http://qu.lnxyls.cn

[E04] 查找子串位置
来源：http://ju.hnjuh.cn

Py:   s.find("x");  s.index("x")
来源：http://zf.huixinmuqiang.cn

PHP:  strpos($s, "x");
来源：http://ff.lnxyls.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://cz.wgjwhj.cn

TS:   s.indexOf("x")
来源：http://tl.bookmarksfly.cn

Java: s.indexOf("x")
来源：http://pj.newstarts.cn

Go:   strings.Index(s, "x")
来源：http://yd.huixinmuqiang.cn

Ruby: s.index("x")
来源：http://tl.nicolike.cn

C#:   s.IndexOf("x")
来源：http://wp.newstarts.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ov.yuexingan06.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ch.haigaiapp.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://tf.yuntaijiaju.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fv.bjjhwx.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ft.huixinmuqiang.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pj.nicolike.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pb.haigaiapp.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://sx.szsharing.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://se.hahajie.cn

[E06] 替换子串
来源：http://cz.shtwfgs.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xs.nicolike.cn

PHP:  str_replace("a", "b", $s);
来源：http://mn.lnxyls.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pk.bookmarksfly.cn

TS:   s.replaceAll("a", "b")
来源：http://ij.hnjuh.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gq.hahajie.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qe.gzmigu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://er.szxytkj.cn

C#:   s.Replace("a", "b")
来源：http://yd.bjjhwx.cn

[E07] 按分隔符拆分
来源：http://uh.yuexingan06.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gd.haigaiapp.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://za.szxytkj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://zu.hahajie.cn

TS:   s.split(",")
来源：http://pf.lnxyls.cn

Java: s.split(",");  s.split("\\s+")
来源：http://il.wgjwhj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ro.shxzskj.cn

Ruby: s.split(",");  s.split
来源：http://kv.huanxung.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dm.shtwfgs.cn

[E08] 数组按分隔符合并
来源：http://pb.yuexingan06.cn

Py:   ",".join(items)
来源：http://tk.asd995.cn

PHP:  implode(",", $items);
来源：http://re.muxihuayi.cn

JS:   items.join(",")
来源：http://yc.bjjhwx.cn

TS:   items.join(",")
来源：http://lm.wgjwhj.cn

Java: String.join(",", items)
来源：http://lk.yuexingan06.cn

Go:   strings.Join(items, ",")
来源：http://kj.shxzukj.cn

Ruby: items.join(",")
来源：http://eq.gzmigu.cn

C#:   string.Join(",", items)
来源：http://xi.bookmarksfly.cn

[E09] 去除所有空白字符
来源：http://og.huanxung.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://yn.yuexingan06.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://pg.yuexingan06.cn

JS:   s.replace(/\s+/g, "")
来源：http://ph.hahajie.cn

TS:   s.replace(/\s+/g, "")
来源：http://nk.shxzukj.cn

Java: s.replaceAll("\\s+", "")
来源：http://gd.shxzukj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://if.jianghongdianzi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ih.asd995.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://st.jctech888.com.cn

[E10] 左侧补零 / 定长填充
来源：http://sq.szsharing.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fo.haigaiapp.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://de.szxytkj.cn

JS:   "7".padStart(3, "0")
来源：http://ke.newstarts.cn

TS:   "7".padStart(3, "0")
来源：http://ah.huixinmuqiang.cn

Java: String.format("%03d", 7)
来源：http://vz.nszjky.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://hg.hnjuh.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qx.panjiajie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bi.huixiangedu.cn

[E11] 反转字符串
来源：http://ao.szxytkj.cn

Py:   s[::-1]
来源：http://cm.szsharing.cn

PHP:  strrev($s);
来源：http://lj.521024.cn

JS:   [...s].reverse().join("")
来源：http://wu.hnjuh.cn

TS:   [...s].reverse().join("")
来源：http://ug.muxihuayi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://mr.bookmarksfly.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://vf.szsharing.cn

Ruby: s.reverse
来源：http://fv.szxytkj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ov.bjjhwx.cn

[E12] 统计某字符出现次数
来源：http://ux.shxzskj.cn

Py:   s.count("a")
来源：http://hj.shxzskj.cn

PHP:  substr_count($s, "a");
来源：http://ix.shxzskj.cn

JS:   s.split("a").length - 1
来源：http://bz.huixiangedu.cn

TS:   s.split("a").length - 1
来源：http://an.jianghongdianzi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://pm.bjjhwx.cn

Go:   strings.Count(s, "a")
来源：http://ex.shxzukj.cn

Ruby: s.count("a")
来源：http://jy.shxzukj.cn

C#:   s.Count(c => c == 'a')
来源：http://fs.jianghongdianzi.cn

[E13] 逐字符遍历
来源：http://ve.huixinmuqiang.cn

Py:   for ch in s: print(ch)
来源：http://xi.yuexingan06.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ty.huixiangedu.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://gy.huanxung.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://za.bjjhwx.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://uj.huanxung.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hv.hnjuh.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://sk.muxihuayi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://pf.chemitech.net.cn

[E14] URL 编码与 Base64
来源：http://kj.bookmarksfly.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://re.shtwfgs.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://dl.hnjuh.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://sy.yuntaijiaju.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nf.shxzukj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://sn.nszjky.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://oi.bookmarksfly.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://co.yuntaijiaju.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dr.9csxet.cn

[E15] HTML 转义 / 反转义
来源：http://es.gzmigu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://qk.asd995.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fl.colortex.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://sq.yuntaijiaju.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://in.521024.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kg.szsharing.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://tu.gzmigu.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ff.wgjwhj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ih.hahajie.cn

[E16] 数字千分位
来源：http://op.bookmarksfly.cn

Py:   f"{1234567:,}"
来源：http://zy.asd995.cn

PHP:  number_format(1234567);
来源：http://be.muxihuayi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://pe.shxzukj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://rr.nszjky.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fm.jctech888.com.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hf.bookmarksfly.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://lt.huanxung.cn

C#:   1234567.ToString("N0")
来源：http://de.szsharing.cn

[E17] 首字母大写
来源：http://ur.yuexingan06.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://pt.nszjky.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://nc.chemitech.net.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yx.huixiangedu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ar.chemitech.net.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://cw.muxihuayi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qx.newstarts.cn

Ruby: s.capitalize
来源：http://he.hnjuh.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gv.9csxet.cn

[E18] 模板占位符替换
来源：http://gy.521024.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bj.colortex.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://cv.colortex.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ng.yuexingan06.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://li.hahajie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gb.newstarts.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hg.bjjhwx.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dp.huixiangedu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://sz.huixiangedu.cn

[E19] 多行文本按行拆分
来源：http://ek.panjiajie.cn

Py:   s.splitlines()
来源：http://ml.shtwfgs.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://sk.newstarts.cn

JS:   s.split(/\r?\n/)
来源：http://kj.jianghongdianzi.cn

TS:   s.split(/\r?\n/)
来源：http://lz.newstarts.cn

Java: s.lines().toList()
来源：http://sy.jianghongdianzi.cn

Go:   strings.Split(s, "\n")
来源：http://fj.nicolike.cn

Ruby: s.lines
来源：http://fv.lnxyls.cn

C#:   s.Split('\n')
来源：http://tm.asd995.cn

[E20] 判断字符串是否为空
来源：http://wh.muxihuayi.cn

Py:   if not s:
来源：http://rp.szxytkj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vj.huixiangedu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://pi.shtwfgs.cn

TS:   if (s === "") {}
来源：http://fh.newstarts.cn

Java: if (s.isEmpty()) {}
来源：http://yh.gzmigu.cn

Go:   if s == "" {}
来源：http://yd.huixiangedu.cn

Ruby: if s.empty?
来源：http://hx.yuntaijiaju.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fx.colortex.cn

[E21] 超长截断加省略号
来源：http://qn.haigaiapp.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vo.szxytkj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hf.hnjuh.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://st.newstarts.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yr.hahajie.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vi.newstarts.cn

Go:   // 按 rune 判断长度后截断
来源：http://fl.haigaiapp.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://js.panjiajie.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hj.bookmarksfly.cn

[E22] 字节长度与字符长度
来源：http://fe.szxytkj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://el.shxzukj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zq.chemitech.net.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://bm.shxzskj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qf.9csxet.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rp.shxzukj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kj.wgjwhj.cn

Ruby: s.bytesize;  s.length
来源：http://zu.jctech888.com.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bq.haigaiapp.cn

================================================================================
来源：http://uc.panjiajie.cn

F. 文件与目录
来源：http://qj.bookmarksfly.cn

================================================================================
来源：http://bm.yuntaijiaju.cn

[F01] 读取整个文件
来源：http://qx.muxihuayi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://yj.lnxyls.cn

PHP:  file_get_contents("a.txt");
来源：http://qx.shxzukj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ep.yuexingan06.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fn.shxzukj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://cs.jianghongdianzi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jy.shtwfgs.cn

Ruby: File.read("a.txt")
来源：http://sd.shxzukj.cn

C#:   File.ReadAllText("a.txt");
来源：http://tu.colortex.cn

[F02] 逐行读取文件
来源：http://fj.wgjwhj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fh.nicolike.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qv.nszjky.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rh.yuntaijiaju.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ck.chemitech.net.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://nj.hahajie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ms.521024.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://as.shxzskj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lq.panjiajie.cn

[F03] 写入文件（覆盖）
来源：http://il.newstarts.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://lq.gzmigu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://gn.szsharing.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mx.nszjky.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fa.panjiajie.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vz.yuntaijiaju.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qc.shxzukj.cn

Ruby: File.write("a.txt", "hi")
来源：http://uk.gzmigu.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ax.shxzukj.cn

[F04] 追加写入文件
来源：http://wf.jctech888.com.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hq.muxihuayi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dd.hnjuh.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cz.jianghongdianzi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://es.nicolike.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xp.wgjwhj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ei.haigaiapp.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qm.nszjky.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://an.lnxyls.cn


<!-- 参考信息 -->