代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gf.lnxyls.cn

Ruby: arr.max;  arr.min
来源：http://ic.9csxet.cn

C#:   list.Max();  list.Min()
来源：http://yi.hnjuh.cn

[D18] 扁平化嵌套数组
来源：http://af.jianghongdianzi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ka.huixinmuqiang.cn

PHP:  array_merge(...$nested);
来源：http://vv.yuntaijiaju.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dx.chemitech.net.cn

TS:   nested.flat();
来源：http://le.bookmarksfly.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ui.huixinmuqiang.cn

Go:   // 手写双层循环
来源：http://tc.yuexingan06.cn

Ruby: nested.flatten
来源：http://bu.panjiajie.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://qx.colortex.cn

[D19] 按字段分组
来源：http://kw.asd995.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kg.yuexingan06.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hc.9csxet.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://la.jctech888.com.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://nh.yuexingan06.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ux.muxihuayi.cn

Go:   // 手写 map[string][]T
来源：http://wy.521024.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ka.huanxung.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xg.jctech888.com.cn

[D20] 统计每个元素出现次数
来源：http://eb.9csxet.cn

Py:   Counter(arr)
来源：http://lf.9csxet.cn

PHP:  array_count_values($arr);
来源：http://ay.szsharing.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dd.lnxyls.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kn.huixiangedu.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://sn.muxihuayi.cn

Go:   // 手写 map[T]int
来源：http://yl.jctech888.com.cn

Ruby: arr.tally
来源：http://ou.yuexingan06.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://an.shxzskj.cn

[D21] 判断是否包含某元素
来源：http://kl.muxihuayi.cn

Py:   x in arr
来源：http://ag.wgjwhj.cn

PHP:  in_array($x, $arr, true);
来源：http://pe.panjiajie.cn

JS:   arr.includes(x)
来源：http://ic.521024.cn

TS:   arr.includes(x)
来源：http://mi.shxzukj.cn

Java: list.contains(x)
来源：http://zt.wgjwhj.cn

Go:   slices.Contains(arr, x)
来源：http://hd.hahajie.cn

Ruby: arr.include?(x)
来源：http://ye.nicolike.cn

C#:   list.Contains(x)
来源：http://ws.huixiangedu.cn

[D22] 复制数组（避免共享引用）
来源：http://xq.huanxung.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://bn.huixiangedu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kx.jctech888.com.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gy.hahajie.cn

TS:   [...arr];
来源：http://sw.hahajie.cn

Java: new ArrayList<>(list);
来源：http://so.jianghongdianzi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ei.lnxyls.cn

Ruby: arr.dup;  arr.clone
来源：http://vs.hahajie.cn

C#:   new List<int>(list);
来源：http://vr.jctech888.com.cn

[D23] reduce 累积计算
来源：http://uv.newstarts.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://on.haigaiapp.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mx.9csxet.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dp.jctech888.com.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jc.wgjwhj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ud.shxzukj.cn

Go:   // 手写循环
来源：http://mr.huixinmuqiang.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gq.newstarts.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://kg.asd995.cn

[D24] 字典 / Map 基本操作
来源：http://qx.asd995.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://df.nicolike.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zx.newstarts.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ta.szsharing.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ee.nicolike.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hq.hnjuh.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xe.shxzukj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rt.newstarts.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ve.huixiangedu.cn

[D25] Set 集合去重与交并差
来源：http://vy.huixiangedu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://uv.shxzukj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gc.nszjky.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mv.521024.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://iw.bookmarksfly.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nh.huixinmuqiang.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://dp.shtwfgs.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://yw.wgjwhj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rx.szsharing.cn

[D26] 数组转字符串
来源：http://qp.panjiajie.cn

Py:   ", ".join(map(str, arr))
来源：http://qu.521024.cn

PHP:  implode(", ", $arr);
来源：http://di.yuntaijiaju.cn

JS:   arr.join(", ")
来源：http://yw.szxytkj.cn

TS:   arr.join(", ")
来源：http://dh.haigaiapp.cn

Java: String.join(", ", list)
来源：http://fz.lnxyls.cn

Go:   strings.Join(strs, ", ")
来源：http://fk.9csxet.cn

Ruby: arr.join(", ")
来源：http://ui.hnjuh.cn

C#:   string.Join(", ", list)
来源：http://in.wgjwhj.cn

================================================================================
来源：http://xe.gzmigu.cn

E. 字符串处理
来源：http://vw.nicolike.cn

================================================================================
来源：http://vc.wgjwhj.cn

[E01] 拼接字符串
来源：http://cq.nszjky.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ai.gzmigu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zt.jctech888.com.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zn.shtwfgs.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ss.huixiangedu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gt.szxytkj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ci.asd995.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vx.hahajie.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://lg.hahajie.cn

[E02] 重复字符串
来源：http://uv.jctech888.com.cn

Py:   "ab" * 3
来源：http://fx.nicolike.cn

PHP:  str_repeat("ab", 3);
来源：http://qm.panjiajie.cn

JS:   "ab".repeat(3)
来源：http://gz.hnjuh.cn

TS:   "ab".repeat(3)
来源：http://oh.panjiajie.cn

Java: "ab".repeat(3)
来源：http://kl.shtwfgs.cn

Go:   strings.Repeat("ab", 3)
来源：http://uu.panjiajie.cn

Ruby: "ab" * 3
来源：http://no.jctech888.com.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://bb.jctech888.com.cn

[E03] 截取子串
来源：http://oe.szxytkj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://uh.shxzskj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://zk.yuexingan06.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xe.9csxet.cn

TS:   s.slice(1, 4)
来源：http://zc.szxytkj.cn

Java: s.substring(1, 4)
来源：http://rn.muxihuayi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://uc.szsharing.cn

Ruby: s[1, 3];  s[1..3]
来源：http://tf.shxzskj.cn

C#:   s.Substring(1, 3)
来源：http://gb.shxzukj.cn

[E04] 查找子串位置
来源：http://jx.szxytkj.cn

Py:   s.find("x");  s.index("x")
来源：http://dy.muxihuayi.cn

PHP:  strpos($s, "x");
来源：http://vw.huanxung.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mv.shxzukj.cn

TS:   s.indexOf("x")
来源：http://ig.gzmigu.cn

Java: s.indexOf("x")
来源：http://fa.shtwfgs.cn

Go:   strings.Index(s, "x")
来源：http://pm.yuntaijiaju.cn

Ruby: s.index("x")
来源：http://mk.shxzukj.cn

C#:   s.IndexOf("x")
来源：http://aw.hnjuh.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://wp.lnxyls.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://sa.huixinmuqiang.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vz.hnjuh.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bw.newstarts.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://oh.shxzskj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ok.colortex.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tb.nicolike.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://dj.yuexingan06.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://df.newstarts.cn

[E06] 替换子串
来源：http://vz.jianghongdianzi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://oq.newstarts.cn

PHP:  str_replace("a", "b", $s);
来源：http://cr.jctech888.com.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gc.nszjky.cn

TS:   s.replaceAll("a", "b")
来源：http://gv.hnjuh.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://iw.wgjwhj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ak.shxzukj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ab.colortex.cn

C#:   s.Replace("a", "b")
来源：http://jn.huanxung.cn

[E07] 按分隔符拆分
来源：http://cn.szsharing.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ww.shxzskj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fv.jianghongdianzi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://tt.lnxyls.cn

TS:   s.split(",")
来源：http://ji.huixiangedu.cn

Java: s.split(",");  s.split("\\s+")
来源：http://fl.nicolike.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pr.wgjwhj.cn

Ruby: s.split(",");  s.split
来源：http://jy.huanxung.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://er.shxzukj.cn

[E08] 数组按分隔符合并
来源：http://nf.szsharing.cn

Py:   ",".join(items)
来源：http://bn.newstarts.cn

PHP:  implode(",", $items);
来源：http://tq.yuntaijiaju.cn

JS:   items.join(",")
来源：http://db.huixinmuqiang.cn

TS:   items.join(",")
来源：http://of.521024.cn

Java: String.join(",", items)
来源：http://tb.szxytkj.cn

Go:   strings.Join(items, ",")
来源：http://rx.huixiangedu.cn

Ruby: items.join(",")
来源：http://mc.lnxyls.cn

C#:   string.Join(",", items)
来源：http://zx.chemitech.net.cn

[E09] 去除所有空白字符
来源：http://zw.lnxyls.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ak.colortex.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ui.huixinmuqiang.cn

JS:   s.replace(/\s+/g, "")
来源：http://oi.huixiangedu.cn

TS:   s.replace(/\s+/g, "")
来源：http://uy.chemitech.net.cn

Java: s.replaceAll("\\s+", "")
来源：http://qr.shtwfgs.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://cf.asd995.cn

Ruby: s.gsub(/\s+/, "")
来源：http://oq.szxytkj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qf.muxihuayi.cn

[E10] 左侧补零 / 定长填充
来源：http://wc.nszjky.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://yp.521024.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zm.haigaiapp.cn

JS:   "7".padStart(3, "0")
来源：http://nn.chemitech.net.cn

TS:   "7".padStart(3, "0")
来源：http://yl.yuexingan06.cn

Java: String.format("%03d", 7)
来源：http://ue.yuexingan06.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://nb.wgjwhj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fa.huixiangedu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bh.wgjwhj.cn

[E11] 反转字符串
来源：http://hr.huixiangedu.cn

Py:   s[::-1]
来源：http://kr.muxihuayi.cn

PHP:  strrev($s);
来源：http://vx.yuexingan06.cn

JS:   [...s].reverse().join("")
来源：http://ud.newstarts.cn

TS:   [...s].reverse().join("")
来源：http://ke.wgjwhj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://lc.wgjwhj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://op.huanxung.cn

Ruby: s.reverse
来源：http://my.shxzukj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://md.bookmarksfly.cn

[E12] 统计某字符出现次数
来源：http://um.huixiangedu.cn

Py:   s.count("a")
来源：http://ms.colortex.cn

PHP:  substr_count($s, "a");
来源：http://fm.shtwfgs.cn

JS:   s.split("a").length - 1
来源：http://ax.521024.cn

TS:   s.split("a").length - 1
来源：http://hd.shtwfgs.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ty.lnxyls.cn

Go:   strings.Count(s, "a")
来源：http://zp.huixinmuqiang.cn

Ruby: s.count("a")
来源：http://es.huixinmuqiang.cn

C#:   s.Count(c => c == 'a')
来源：http://ci.huixinmuqiang.cn

[E13] 逐字符遍历
来源：http://mi.hnjuh.cn

Py:   for ch in s: print(ch)
来源：http://th.asd995.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ym.shxzukj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ja.szsharing.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://xp.szxytkj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ys.szsharing.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xl.nicolike.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://fl.shxzukj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://uy.lnxyls.cn

[E14] URL 编码与 Base64
来源：http://xz.lnxyls.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wx.nszjky.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://zu.shxzskj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://os.panjiajie.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zu.szxytkj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zw.wgjwhj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ce.colortex.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://be.hahajie.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://iq.shxzukj.cn

[E15] HTML 转义 / 反转义
来源：http://ux.asd995.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://fy.newstarts.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gr.szxytkj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://el.nszjky.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://wy.huanxung.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://lk.shxzukj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bo.wgjwhj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://uv.bjjhwx.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://eb.bjjhwx.cn

[E16] 数字千分位
来源：http://uq.newstarts.cn

Py:   f"{1234567:,}"
来源：http://nt.nicolike.cn

PHP:  number_format(1234567);
来源：http://xf.nicolike.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://hp.newstarts.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://xu.nszjky.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://kz.jctech888.com.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://aw.jianghongdianzi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qy.9csxet.cn

C#:   1234567.ToString("N0")
来源：http://ip.lnxyls.cn

[E17] 首字母大写
来源：http://se.hahajie.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nv.bookmarksfly.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://vj.hnjuh.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pw.huixinmuqiang.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yl.szsharing.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://yz.bjjhwx.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hj.szxytkj.cn

Ruby: s.capitalize
来源：http://mf.shtwfgs.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fq.colortex.cn

[E18] 模板占位符替换
来源：http://pk.lnxyls.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bu.huanxung.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://he.szsharing.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://gw.lnxyls.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://wd.szsharing.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qm.shxzukj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://sy.nszjky.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vx.9csxet.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yx.szsharing.cn

[E19] 多行文本按行拆分
来源：http://wy.bjjhwx.cn

Py:   s.splitlines()
来源：http://pw.bookmarksfly.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rz.shxzskj.cn

JS:   s.split(/\r?\n/)
来源：http://cs.asd995.cn

TS:   s.split(/\r?\n/)
来源：http://kf.panjiajie.cn

Java: s.lines().toList()
来源：http://it.haigaiapp.cn

Go:   strings.Split(s, "\n")
来源：http://ab.haigaiapp.cn

Ruby: s.lines
来源：http://uh.asd995.cn

C#:   s.Split('\n')
来源：http://mc.huanxung.cn

[E20] 判断字符串是否为空
来源：http://tv.newstarts.cn

Py:   if not s:
来源：http://cc.colortex.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://iw.huixinmuqiang.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ip.asd995.cn

TS:   if (s === "") {}
来源：http://bm.muxihuayi.cn

Java: if (s.isEmpty()) {}
来源：http://qz.asd995.cn

Go:   if s == "" {}
来源：http://kl.shtwfgs.cn

Ruby: if s.empty?
来源：http://db.bookmarksfly.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://py.huixiangedu.cn

[E21] 超长截断加省略号
来源：http://fl.jctech888.com.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://of.newstarts.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://aa.jctech888.com.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://co.bjjhwx.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://og.shxzskj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hf.gzmigu.cn

Go:   // 按 rune 判断长度后截断
来源：http://ll.hnjuh.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xg.bookmarksfly.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qk.hahajie.cn

[E22] 字节长度与字符长度
来源：http://uc.muxihuayi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bi.lnxyls.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yg.521024.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qq.shxzskj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gq.huanxung.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qy.9csxet.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vb.bjjhwx.cn

Ruby: s.bytesize;  s.length
来源：http://pr.huixinmuqiang.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ef.chemitech.net.cn

================================================================================
来源：http://ph.shtwfgs.cn

F. 文件与目录
来源：http://pg.hnjuh.cn

================================================================================
来源：http://td.wgjwhj.cn

[F01] 读取整个文件
来源：http://od.lnxyls.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gk.szsharing.cn

PHP:  file_get_contents("a.txt");
来源：http://de.bookmarksfly.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hl.521024.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hx.yuexingan06.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://sz.nicolike.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://cy.jianghongdianzi.cn

Ruby: File.read("a.txt")
来源：http://pk.yuexingan06.cn

C#:   File.ReadAllText("a.txt");
来源：http://bq.hahajie.cn

[F02] 逐行读取文件
来源：http://qb.szsharing.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xh.hnjuh.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xm.lnxyls.cn


<!-- 参考信息 -->