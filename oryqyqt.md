代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://go.szsharing.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://io.lnxyls.cn

Go:   // 手写 map[string][]T
来源：http://ui.szxytkj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://bp.jianghongdianzi.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bw.shxzskj.cn

[D20] 统计每个元素出现次数
来源：http://ob.yuntaijiaju.cn

Py:   Counter(arr)
来源：http://iv.shxzukj.cn

PHP:  array_count_values($arr);
来源：http://cf.nicolike.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://is.muxihuayi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hm.wgjwhj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://id.chemitech.net.cn

Go:   // 手写 map[T]int
来源：http://zs.panjiajie.cn

Ruby: arr.tally
来源：http://ng.jianghongdianzi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zc.shxzukj.cn

[D21] 判断是否包含某元素
来源：http://zt.521024.cn

Py:   x in arr
来源：http://up.panjiajie.cn

PHP:  in_array($x, $arr, true);
来源：http://vx.huanxung.cn

JS:   arr.includes(x)
来源：http://eo.521024.cn

TS:   arr.includes(x)
来源：http://hr.szxytkj.cn

Java: list.contains(x)
来源：http://we.hnjuh.cn

Go:   slices.Contains(arr, x)
来源：http://rg.yuexingan06.cn

Ruby: arr.include?(x)
来源：http://tw.huixiangedu.cn

C#:   list.Contains(x)
来源：http://op.muxihuayi.cn

[D22] 复制数组（避免共享引用）
来源：http://gq.bookmarksfly.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://br.jctech888.com.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://eh.9csxet.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://il.bjjhwx.cn

TS:   [...arr];
来源：http://jr.lnxyls.cn

Java: new ArrayList<>(list);
来源：http://nt.hnjuh.cn

Go:   copied := append([]int(nil), arr...)
来源：http://qf.colortex.cn

Ruby: arr.dup;  arr.clone
来源：http://pm.szsharing.cn

C#:   new List<int>(list);
来源：http://ad.huanxung.cn

[D23] reduce 累积计算
来源：http://ai.shxzskj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://kp.shxzskj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tw.lnxyls.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pj.panjiajie.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sm.521024.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://gm.yuexingan06.cn

Go:   // 手写循环
来源：http://tl.gzmigu.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jy.newstarts.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://vo.wgjwhj.cn

[D24] 字典 / Map 基本操作
来源：http://rd.nszjky.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://op.shtwfgs.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mq.muxihuayi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://eb.panjiajie.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://et.nszjky.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vv.nicolike.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://sl.bjjhwx.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://de.bjjhwx.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ep.huixiangedu.cn

[D25] Set 集合去重与交并差
来源：http://vz.panjiajie.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jp.haigaiapp.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vz.szsharing.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rx.521024.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.shxzskj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://re.bookmarksfly.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gp.lnxyls.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mw.shxzukj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ol.shtwfgs.cn

[D26] 数组转字符串
来源：http://ri.nicolike.cn

Py:   ", ".join(map(str, arr))
来源：http://ut.wgjwhj.cn

PHP:  implode(", ", $arr);
来源：http://xy.colortex.cn

JS:   arr.join(", ")
来源：http://ik.nicolike.cn

TS:   arr.join(", ")
来源：http://vg.szxytkj.cn

Java: String.join(", ", list)
来源：http://ia.asd995.cn

Go:   strings.Join(strs, ", ")
来源：http://xd.9csxet.cn

Ruby: arr.join(", ")
来源：http://ci.szsharing.cn

C#:   string.Join(", ", list)
来源：http://cr.asd995.cn

================================================================================
来源：http://bn.nszjky.cn

E. 字符串处理
来源：http://ad.yuexingan06.cn

================================================================================
来源：http://sg.panjiajie.cn

[E01] 拼接字符串
来源：http://nz.huixinmuqiang.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cj.huixinmuqiang.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hd.jianghongdianzi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://pk.yuntaijiaju.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zy.newstarts.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://sg.jctech888.com.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xn.yuexingan06.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lf.521024.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://er.hahajie.cn

[E02] 重复字符串
来源：http://hb.colortex.cn

Py:   "ab" * 3
来源：http://it.521024.cn

PHP:  str_repeat("ab", 3);
来源：http://ii.szsharing.cn

JS:   "ab".repeat(3)
来源：http://qo.bookmarksfly.cn

TS:   "ab".repeat(3)
来源：http://tm.nicolike.cn

Java: "ab".repeat(3)
来源：http://zz.9csxet.cn

Go:   strings.Repeat("ab", 3)
来源：http://ch.huixiangedu.cn

Ruby: "ab" * 3
来源：http://fi.nicolike.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://es.hnjuh.cn

[E03] 截取子串
来源：http://dt.haigaiapp.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ok.haigaiapp.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xh.yuexingan06.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ao.muxihuayi.cn

TS:   s.slice(1, 4)
来源：http://gc.chemitech.net.cn

Java: s.substring(1, 4)
来源：http://ue.yuntaijiaju.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xk.huixinmuqiang.cn

Ruby: s[1, 3];  s[1..3]
来源：http://hy.newstarts.cn

C#:   s.Substring(1, 3)
来源：http://vl.asd995.cn

[E04] 查找子串位置
来源：http://wm.szxytkj.cn

Py:   s.find("x");  s.index("x")
来源：http://vc.szsharing.cn

PHP:  strpos($s, "x");
来源：http://yb.haigaiapp.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ea.jctech888.com.cn

TS:   s.indexOf("x")
来源：http://dy.nszjky.cn

Java: s.indexOf("x")
来源：http://la.jctech888.com.cn

Go:   strings.Index(s, "x")
来源：http://di.gzmigu.cn

Ruby: s.index("x")
来源：http://cu.yuexingan06.cn

C#:   s.IndexOf("x")
来源：http://jc.chemitech.net.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://xh.colortex.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jn.shtwfgs.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qx.gzmigu.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pf.asd995.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://uj.szsharing.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://le.shtwfgs.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ts.shxzukj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://sk.colortex.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ux.shtwfgs.cn

[E06] 替换子串
来源：http://io.hahajie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dn.shtwfgs.cn

PHP:  str_replace("a", "b", $s);
来源：http://ee.hahajie.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://om.shxzskj.cn

TS:   s.replaceAll("a", "b")
来源：http://yv.muxihuayi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uo.huanxung.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://yu.shxzukj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://sf.bookmarksfly.cn

C#:   s.Replace("a", "b")
来源：http://lr.colortex.cn

[E07] 按分隔符拆分
来源：http://qs.yuntaijiaju.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://dc.colortex.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gb.wgjwhj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://yn.bjjhwx.cn

TS:   s.split(",")
来源：http://wm.nszjky.cn

Java: s.split(",");  s.split("\\s+")
来源：http://jo.521024.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xt.bjjhwx.cn

Ruby: s.split(",");  s.split
来源：http://ye.huixinmuqiang.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://so.muxihuayi.cn

[E08] 数组按分隔符合并
来源：http://ys.gzmigu.cn

Py:   ",".join(items)
来源：http://mu.jianghongdianzi.cn

PHP:  implode(",", $items);
来源：http://cd.jctech888.com.cn

JS:   items.join(",")
来源：http://af.jianghongdianzi.cn

TS:   items.join(",")
来源：http://ti.bookmarksfly.cn

Java: String.join(",", items)
来源：http://po.huixinmuqiang.cn

Go:   strings.Join(items, ",")
来源：http://ot.colortex.cn

Ruby: items.join(",")
来源：http://zi.lnxyls.cn

C#:   string.Join(",", items)
来源：http://pc.yuexingan06.cn

[E09] 去除所有空白字符
来源：http://ry.szsharing.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fl.nicolike.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://uz.muxihuayi.cn

JS:   s.replace(/\s+/g, "")
来源：http://dv.huanxung.cn

TS:   s.replace(/\s+/g, "")
来源：http://in.haigaiapp.cn

Java: s.replaceAll("\\s+", "")
来源：http://cx.huixinmuqiang.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://jp.hnjuh.cn

Ruby: s.gsub(/\s+/, "")
来源：http://tv.shxzukj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ww.szsharing.cn

[E10] 左侧补零 / 定长填充
来源：http://lb.gzmigu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fz.hahajie.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://on.lnxyls.cn

JS:   "7".padStart(3, "0")
来源：http://we.hahajie.cn

TS:   "7".padStart(3, "0")
来源：http://pb.muxihuayi.cn

Java: String.format("%03d", 7)
来源：http://dh.shxzskj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://gg.jianghongdianzi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://gz.panjiajie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://dw.shxzskj.cn

[E11] 反转字符串
来源：http://rv.hahajie.cn

Py:   s[::-1]
来源：http://nu.521024.cn

PHP:  strrev($s);
来源：http://hn.panjiajie.cn

JS:   [...s].reverse().join("")
来源：http://rv.yuntaijiaju.cn

TS:   [...s].reverse().join("")
来源：http://ur.szsharing.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ub.panjiajie.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://bp.lnxyls.cn

Ruby: s.reverse
来源：http://ol.nszjky.cn

C#:   new string(s.Reverse().ToArray())
来源：http://bn.wgjwhj.cn

[E12] 统计某字符出现次数
来源：http://ju.haigaiapp.cn

Py:   s.count("a")
来源：http://kr.shxzskj.cn

PHP:  substr_count($s, "a");
来源：http://qx.lnxyls.cn

JS:   s.split("a").length - 1
来源：http://ie.huanxung.cn

TS:   s.split("a").length - 1
来源：http://aj.nszjky.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qj.hnjuh.cn

Go:   strings.Count(s, "a")
来源：http://rh.yuexingan06.cn

Ruby: s.count("a")
来源：http://pi.yuntaijiaju.cn

C#:   s.Count(c => c == 'a')
来源：http://wm.szsharing.cn

[E13] 逐字符遍历
来源：http://sw.wgjwhj.cn

Py:   for ch in s: print(ch)
来源：http://lm.huanxung.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rq.muxihuayi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://fl.muxihuayi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://fi.shtwfgs.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://sh.yuntaijiaju.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://dx.lnxyls.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://zy.newstarts.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jn.jianghongdianzi.cn

[E14] URL 编码与 Base64
来源：http://il.huanxung.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fb.haigaiapp.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://lf.gzmigu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fd.nszjky.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fl.bjjhwx.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ep.wgjwhj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ks.huixiangedu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ou.bjjhwx.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hj.yuexingan06.cn

[E15] HTML 转义 / 反转义
来源：http://kr.yuntaijiaju.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ag.gzmigu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://on.panjiajie.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hi.shtwfgs.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://gt.huixiangedu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ee.yuexingan06.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vq.newstarts.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ww.yuexingan06.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wp.newstarts.cn

[E16] 数字千分位
来源：http://nc.wgjwhj.cn

Py:   f"{1234567:,}"
来源：http://bu.newstarts.cn

PHP:  number_format(1234567);
来源：http://ul.nicolike.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://zm.521024.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://we.huixiangedu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://an.bookmarksfly.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rg.hahajie.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://oc.szsharing.cn

C#:   1234567.ToString("N0")
来源：http://gv.panjiajie.cn

[E17] 首字母大写
来源：http://fn.gzmigu.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nw.yuexingan06.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://pt.huanxung.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ta.gzmigu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://im.szxytkj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fm.nicolike.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://yl.huixiangedu.cn

Ruby: s.capitalize
来源：http://hu.yuexingan06.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wb.wgjwhj.cn

[E18] 模板占位符替换
来源：http://hk.jianghongdianzi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://id.wgjwhj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ce.huanxung.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://gy.newstarts.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://dz.panjiajie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vo.nszjky.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://je.yuexingan06.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kg.9csxet.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jd.muxihuayi.cn

[E19] 多行文本按行拆分
来源：http://rn.gzmigu.cn

Py:   s.splitlines()
来源：http://rx.jctech888.com.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ms.szxytkj.cn

JS:   s.split(/\r?\n/)
来源：http://ul.521024.cn

TS:   s.split(/\r?\n/)
来源：http://mz.asd995.cn

Java: s.lines().toList()
来源：http://ov.9csxet.cn

Go:   strings.Split(s, "\n")
来源：http://ue.bjjhwx.cn

Ruby: s.lines
来源：http://ka.yuntaijiaju.cn

C#:   s.Split('\n')
来源：http://pg.hahajie.cn

[E20] 判断字符串是否为空
来源：http://ti.shtwfgs.cn

Py:   if not s:
来源：http://vg.521024.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yn.haigaiapp.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://oq.haigaiapp.cn

TS:   if (s === "") {}
来源：http://gu.szxytkj.cn

Java: if (s.isEmpty()) {}
来源：http://cw.muxihuayi.cn

Go:   if s == "" {}
来源：http://hn.asd995.cn

Ruby: if s.empty?
来源：http://zt.hahajie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qo.lnxyls.cn

[E21] 超长截断加省略号
来源：http://ec.jctech888.com.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zw.shxzskj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://po.nszjky.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mg.hahajie.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dw.asd995.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ex.521024.cn

Go:   // 按 rune 判断长度后截断
来源：http://sf.bookmarksfly.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://kb.jianghongdianzi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hx.521024.cn

[E22] 字节长度与字符长度
来源：http://au.huixinmuqiang.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://id.521024.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ug.nicolike.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ax.muxihuayi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://im.asd995.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://tg.jianghongdianzi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://nu.wgjwhj.cn

Ruby: s.bytesize;  s.length
来源：http://nz.szxytkj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ad.asd995.cn

================================================================================
来源：http://ab.nicolike.cn

F. 文件与目录
来源：http://yy.panjiajie.cn

================================================================================
来源：http://kg.yuntaijiaju.cn

[F01] 读取整个文件
来源：http://kt.shtwfgs.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ea.gzmigu.cn

PHP:  file_get_contents("a.txt");
来源：http://av.521024.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ci.asd995.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qa.bjjhwx.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://gp.bjjhwx.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://or.wgjwhj.cn

Ruby: File.read("a.txt")
来源：http://cr.hahajie.cn

C#:   File.ReadAllText("a.txt");
来源：http://iu.nicolike.cn

[F02] 逐行读取文件
来源：http://sx.asd995.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bb.panjiajie.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xd.panjiajie.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://is.nszjky.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jm.hahajie.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://im.szsharing.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xg.yuexingan06.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ta.shxzskj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xq.muxihuayi.cn

[F03] 写入文件（覆盖）
来源：http://ye.panjiajie.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://yh.lnxyls.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://xk.gzmigu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qp.szsharing.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ni.haigaiapp.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rl.shxzskj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kb.9csxet.cn

Ruby: File.write("a.txt", "hi")
来源：http://rd.yuntaijiaju.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://kr.szsharing.cn

[F04] 追加写入文件
来源：http://ty.lnxyls.cn


<!-- 参考信息 -->