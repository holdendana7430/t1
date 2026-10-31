代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://vm.jctech888.com.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://et.chemitech.net.cn

Go:   // 手写 map[string][]T
来源：http://cq.colortex.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://oe.chemitech.net.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://tj.huixiangedu.cn

[D20] 统计每个元素出现次数
来源：http://lw.shtwfgs.cn

Py:   Counter(arr)
来源：http://hr.hnjuh.cn

PHP:  array_count_values($arr);
来源：http://jx.huixiangedu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ue.chemitech.net.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ln.panjiajie.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ye.nszjky.cn

Go:   // 手写 map[T]int
来源：http://wh.gzmigu.cn

Ruby: arr.tally
来源：http://lc.asd995.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ke.shxzukj.cn

[D21] 判断是否包含某元素
来源：http://iy.szsharing.cn

Py:   x in arr
来源：http://qa.muxihuayi.cn

PHP:  in_array($x, $arr, true);
来源：http://ue.huixiangedu.cn

JS:   arr.includes(x)
来源：http://ww.shxzskj.cn

TS:   arr.includes(x)
来源：http://vh.nszjky.cn

Java: list.contains(x)
来源：http://at.szxytkj.cn

Go:   slices.Contains(arr, x)
来源：http://wh.chemitech.net.cn

Ruby: arr.include?(x)
来源：http://ec.hahajie.cn

C#:   list.Contains(x)
来源：http://wb.chemitech.net.cn

[D22] 复制数组（避免共享引用）
来源：http://zf.newstarts.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gt.shxzskj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jx.muxihuayi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ay.wgjwhj.cn

TS:   [...arr];
来源：http://yk.muxihuayi.cn

Java: new ArrayList<>(list);
来源：http://op.hnjuh.cn

Go:   copied := append([]int(nil), arr...)
来源：http://di.yuntaijiaju.cn

Ruby: arr.dup;  arr.clone
来源：http://fy.asd995.cn

C#:   new List<int>(list);
来源：http://pf.9csxet.cn

[D23] reduce 累积计算
来源：http://vp.muxihuayi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xz.nicolike.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://iv.9csxet.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ym.yuntaijiaju.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kn.szxytkj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://nr.szsharing.cn

Go:   // 手写循环
来源：http://xt.muxihuayi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ji.asd995.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xr.shtwfgs.cn

[D24] 字典 / Map 基本操作
来源：http://rl.jctech888.com.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://tr.huanxung.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://lf.chemitech.net.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ci.huixiangedu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://tq.gzmigu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fd.jctech888.com.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bj.bjjhwx.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ng.huixinmuqiang.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ms.hahajie.cn

[D25] Set 集合去重与交并差
来源：http://ld.jianghongdianzi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vd.newstarts.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://nq.521024.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ob.yuexingan06.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ug.yuexingan06.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://lq.nszjky.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ll.yuexingan06.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://oz.yuntaijiaju.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mr.chemitech.net.cn

[D26] 数组转字符串
来源：http://ki.panjiajie.cn

Py:   ", ".join(map(str, arr))
来源：http://kn.jianghongdianzi.cn

PHP:  implode(", ", $arr);
来源：http://sf.lnxyls.cn

JS:   arr.join(", ")
来源：http://ig.nicolike.cn

TS:   arr.join(", ")
来源：http://vr.bookmarksfly.cn

Java: String.join(", ", list)
来源：http://fs.muxihuayi.cn

Go:   strings.Join(strs, ", ")
来源：http://mf.jctech888.com.cn

Ruby: arr.join(", ")
来源：http://pw.chemitech.net.cn

C#:   string.Join(", ", list)
来源：http://bg.yuntaijiaju.cn

================================================================================
来源：http://vj.szsharing.cn

E. 字符串处理
来源：http://bh.gzmigu.cn

================================================================================
来源：http://ym.lnxyls.cn

[E01] 拼接字符串
来源：http://bd.szxytkj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rg.jctech888.com.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://gp.9csxet.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xx.yuntaijiaju.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://is.newstarts.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rk.wgjwhj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vo.huanxung.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gw.szxytkj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jr.huanxung.cn

[E02] 重复字符串
来源：http://py.asd995.cn

Py:   "ab" * 3
来源：http://yf.hahajie.cn

PHP:  str_repeat("ab", 3);
来源：http://cj.bjjhwx.cn

JS:   "ab".repeat(3)
来源：http://dv.nicolike.cn

TS:   "ab".repeat(3)
来源：http://pd.panjiajie.cn

Java: "ab".repeat(3)
来源：http://ve.huixinmuqiang.cn

Go:   strings.Repeat("ab", 3)
来源：http://dk.haigaiapp.cn

Ruby: "ab" * 3
来源：http://zg.9csxet.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qo.bookmarksfly.cn

[E03] 截取子串
来源：http://ii.szxytkj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://uj.9csxet.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ru.wgjwhj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ee.yuexingan06.cn

TS:   s.slice(1, 4)
来源：http://oa.yuexingan06.cn

Java: s.substring(1, 4)
来源：http://du.huixiangedu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://id.bjjhwx.cn

Ruby: s[1, 3];  s[1..3]
来源：http://qg.jctech888.com.cn

C#:   s.Substring(1, 3)
来源：http://uq.panjiajie.cn

[E04] 查找子串位置
来源：http://lh.huanxung.cn

Py:   s.find("x");  s.index("x")
来源：http://hd.hnjuh.cn

PHP:  strpos($s, "x");
来源：http://yy.szxytkj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://os.chemitech.net.cn

TS:   s.indexOf("x")
来源：http://nv.haigaiapp.cn

Java: s.indexOf("x")
来源：http://jt.hahajie.cn

Go:   strings.Index(s, "x")
来源：http://kb.lnxyls.cn

Ruby: s.index("x")
来源：http://mt.shxzskj.cn

C#:   s.IndexOf("x")
来源：http://wq.shxzskj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://nz.newstarts.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zr.huixinmuqiang.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://cv.muxihuayi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cs.shxzskj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://pg.colortex.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jw.bjjhwx.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://op.shtwfgs.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tw.jianghongdianzi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fj.shxzskj.cn

[E06] 替换子串
来源：http://nu.521024.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ev.muxihuayi.cn

PHP:  str_replace("a", "b", $s);
来源：http://kk.jianghongdianzi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ay.panjiajie.cn

TS:   s.replaceAll("a", "b")
来源：http://rd.huixiangedu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://om.nicolike.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vo.chemitech.net.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kk.shxzukj.cn

C#:   s.Replace("a", "b")
来源：http://gs.wgjwhj.cn

[E07] 按分隔符拆分
来源：http://cf.yuntaijiaju.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mz.bookmarksfly.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zx.newstarts.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://lp.bookmarksfly.cn

TS:   s.split(",")
来源：http://iu.9csxet.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ky.haigaiapp.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://gd.newstarts.cn

Ruby: s.split(",");  s.split
来源：http://er.yuntaijiaju.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://oy.9csxet.cn

[E08] 数组按分隔符合并
来源：http://ac.bjjhwx.cn

Py:   ",".join(items)
来源：http://fd.hahajie.cn

PHP:  implode(",", $items);
来源：http://hz.huixiangedu.cn

JS:   items.join(",")
来源：http://gv.shtwfgs.cn

TS:   items.join(",")
来源：http://rw.gzmigu.cn

Java: String.join(",", items)
来源：http://bz.bookmarksfly.cn

Go:   strings.Join(items, ",")
来源：http://lh.nicolike.cn

Ruby: items.join(",")
来源：http://kl.huixinmuqiang.cn

C#:   string.Join(",", items)
来源：http://qk.9csxet.cn

[E09] 去除所有空白字符
来源：http://ym.bookmarksfly.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xg.shxzskj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://en.shtwfgs.cn

JS:   s.replace(/\s+/g, "")
来源：http://vs.wgjwhj.cn

TS:   s.replace(/\s+/g, "")
来源：http://fv.521024.cn

Java: s.replaceAll("\\s+", "")
来源：http://fh.haigaiapp.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://tg.huanxung.cn

Ruby: s.gsub(/\s+/, "")
来源：http://we.jianghongdianzi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://pe.szxytkj.cn

[E10] 左侧补零 / 定长填充
来源：http://tk.bookmarksfly.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ai.szxytkj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://eh.szxytkj.cn

JS:   "7".padStart(3, "0")
来源：http://pj.yuexingan06.cn

TS:   "7".padStart(3, "0")
来源：http://lp.hnjuh.cn

Java: String.format("%03d", 7)
来源：http://yc.shxzskj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://un.hahajie.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xn.colortex.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://oc.yuexingan06.cn

[E11] 反转字符串
来源：http://wx.shxzukj.cn

Py:   s[::-1]
来源：http://yg.huixinmuqiang.cn

PHP:  strrev($s);
来源：http://wv.shxzukj.cn

JS:   [...s].reverse().join("")
来源：http://ja.wgjwhj.cn

TS:   [...s].reverse().join("")
来源：http://cx.yuexingan06.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://vx.muxihuayi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://yn.shtwfgs.cn

Ruby: s.reverse
来源：http://rw.huanxung.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ei.bookmarksfly.cn

[E12] 统计某字符出现次数
来源：http://kd.shtwfgs.cn

Py:   s.count("a")
来源：http://vd.huixiangedu.cn

PHP:  substr_count($s, "a");
来源：http://wk.yuntaijiaju.cn

JS:   s.split("a").length - 1
来源：http://he.hahajie.cn

TS:   s.split("a").length - 1
来源：http://ac.jianghongdianzi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://cd.bookmarksfly.cn

Go:   strings.Count(s, "a")
来源：http://vt.newstarts.cn

Ruby: s.count("a")
来源：http://ip.nicolike.cn

C#:   s.Count(c => c == 'a')
来源：http://nz.szsharing.cn

[E13] 逐字符遍历
来源：http://iv.bjjhwx.cn

Py:   for ch in s: print(ch)
来源：http://ma.jctech888.com.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ri.gzmigu.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://tt.panjiajie.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ff.muxihuayi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://pe.hahajie.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://cg.shxzukj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://bd.jianghongdianzi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://uz.muxihuayi.cn

[E14] URL 编码与 Base64
来源：http://zw.521024.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lk.chemitech.net.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://hl.wgjwhj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://nd.9csxet.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hu.shxzukj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://im.haigaiapp.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mb.shxzukj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kq.shxzskj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bx.nicolike.cn

[E15] HTML 转义 / 反转义
来源：http://xx.hnjuh.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://pv.hnjuh.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://no.hahajie.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vn.shtwfgs.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://kh.jianghongdianzi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hu.jianghongdianzi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://uf.colortex.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://kv.bjjhwx.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fe.szsharing.cn

[E16] 数字千分位
来源：http://nq.shtwfgs.cn

Py:   f"{1234567:,}"
来源：http://yw.panjiajie.cn

PHP:  number_format(1234567);
来源：http://wq.szsharing.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://tn.bjjhwx.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://br.lnxyls.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hv.chemitech.net.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yc.shxzukj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://od.shxzukj.cn

C#:   1234567.ToString("N0")
来源：http://xg.bookmarksfly.cn

[E17] 首字母大写
来源：http://qy.wgjwhj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ws.colortex.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://qs.shxzukj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mb.chemitech.net.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gy.yuexingan06.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ip.gzmigu.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qj.hnjuh.cn

Ruby: s.capitalize
来源：http://fc.newstarts.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tb.newstarts.cn

[E18] 模板占位符替换
来源：http://go.haigaiapp.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jq.yuntaijiaju.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://py.wgjwhj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ye.nicolike.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ta.huixiangedu.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pi.nszjky.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gl.huanxung.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://op.yuexingan06.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://cm.yuexingan06.cn

[E19] 多行文本按行拆分
来源：http://wb.szxytkj.cn

Py:   s.splitlines()
来源：http://jg.jctech888.com.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dg.shxzukj.cn

JS:   s.split(/\r?\n/)
来源：http://ou.hahajie.cn

TS:   s.split(/\r?\n/)
来源：http://xm.lnxyls.cn

Java: s.lines().toList()
来源：http://ko.bookmarksfly.cn

Go:   strings.Split(s, "\n")
来源：http://bl.shxzskj.cn

Ruby: s.lines
来源：http://cv.gzmigu.cn

C#:   s.Split('\n')
来源：http://cz.szsharing.cn

[E20] 判断字符串是否为空
来源：http://mf.jctech888.com.cn

Py:   if not s:
来源：http://xe.jianghongdianzi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ix.wgjwhj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rn.lnxyls.cn

TS:   if (s === "") {}
来源：http://eq.panjiajie.cn

Java: if (s.isEmpty()) {}
来源：http://po.yuntaijiaju.cn

Go:   if s == "" {}
来源：http://kg.521024.cn

Ruby: if s.empty?
来源：http://he.bookmarksfly.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qz.huanxung.cn

[E21] 超长截断加省略号
来源：http://zw.shxzukj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ku.haigaiapp.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ls.shtwfgs.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://oz.9csxet.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rh.shtwfgs.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zo.shxzukj.cn

Go:   // 按 rune 判断长度后截断
来源：http://sw.shtwfgs.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fr.chemitech.net.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://sv.9csxet.cn

[E22] 字节长度与字符长度
来源：http://oz.yuexingan06.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://oh.wgjwhj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dp.nicolike.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ol.nszjky.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://kv.521024.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://tu.huixinmuqiang.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ez.bjjhwx.cn

Ruby: s.bytesize;  s.length
来源：http://ru.shxzskj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://st.newstarts.cn

================================================================================
来源：http://gx.muxihuayi.cn

F. 文件与目录
来源：http://rz.gzmigu.cn

================================================================================
来源：http://yb.bookmarksfly.cn

[F01] 读取整个文件
来源：http://lc.521024.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rn.colortex.cn

PHP:  file_get_contents("a.txt");
来源：http://cs.521024.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://cs.hnjuh.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vp.huanxung.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://pk.panjiajie.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://cv.haigaiapp.cn

Ruby: File.read("a.txt")
来源：http://tf.shxzukj.cn

C#:   File.ReadAllText("a.txt");
来源：http://gd.wgjwhj.cn

[F02] 逐行读取文件
来源：http://cv.haigaiapp.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://go.9csxet.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://uh.chemitech.net.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ve.bookmarksfly.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://de.hahajie.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.szsharing.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bc.jctech888.com.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mz.huixiangedu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ow.colortex.cn

[F03] 写入文件（覆盖）
来源：http://bu.haigaiapp.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://oo.chemitech.net.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ak.bookmarksfly.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nb.colortex.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zt.szsharing.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fc.bjjhwx.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://yf.shxzskj.cn

Ruby: File.write("a.txt", "hi")
来源：http://ol.jianghongdianzi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://pv.shxzukj.cn

[F04] 追加写入文件
来源：http://fs.szsharing.cn


<!-- 参考信息 -->