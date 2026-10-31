代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://um.huanxung.cn

Go:   // 手写双层循环
来源：http://gs.9csxet.cn

Ruby: nested.flatten
来源：http://ko.jctech888.com.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ww.haigaiapp.cn

[D19] 按字段分组
来源：http://pk.jctech888.com.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kg.shxzukj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hm.wgjwhj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://go.lnxyls.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://kq.hahajie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ik.shxzskj.cn

Go:   // 手写 map[string][]T
来源：http://it.shxzukj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://wm.szxytkj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lj.hahajie.cn

[D20] 统计每个元素出现次数
来源：http://tm.haigaiapp.cn

Py:   Counter(arr)
来源：http://hn.huixiangedu.cn

PHP:  array_count_values($arr);
来源：http://nn.chemitech.net.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oa.nicolike.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://me.yuntaijiaju.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zo.jctech888.com.cn

Go:   // 手写 map[T]int
来源：http://ja.lnxyls.cn

Ruby: arr.tally
来源：http://kz.wgjwhj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://nk.wgjwhj.cn

[D21] 判断是否包含某元素
来源：http://oc.hahajie.cn

Py:   x in arr
来源：http://rp.huanxung.cn

PHP:  in_array($x, $arr, true);
来源：http://uo.yuexingan06.cn

JS:   arr.includes(x)
来源：http://zg.yuntaijiaju.cn

TS:   arr.includes(x)
来源：http://qc.szxytkj.cn

Java: list.contains(x)
来源：http://ew.asd995.cn

Go:   slices.Contains(arr, x)
来源：http://pk.9csxet.cn

Ruby: arr.include?(x)
来源：http://xt.szxytkj.cn

C#:   list.Contains(x)
来源：http://dq.521024.cn

[D22] 复制数组（避免共享引用）
来源：http://qw.gzmigu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://up.bookmarksfly.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://or.panjiajie.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ct.hnjuh.cn

TS:   [...arr];
来源：http://ea.bjjhwx.cn

Java: new ArrayList<>(list);
来源：http://dk.huixinmuqiang.cn

Go:   copied := append([]int(nil), arr...)
来源：http://vn.nicolike.cn

Ruby: arr.dup;  arr.clone
来源：http://jy.9csxet.cn

C#:   new List<int>(list);
来源：http://vt.jianghongdianzi.cn

[D23] reduce 累积计算
来源：http://hn.colortex.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ap.panjiajie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wl.newstarts.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tk.bookmarksfly.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sf.szxytkj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://su.chemitech.net.cn

Go:   // 手写循环
来源：http://ja.jctech888.com.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://yt.bookmarksfly.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zb.asd995.cn

[D24] 字典 / Map 基本操作
来源：http://fz.newstarts.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ta.shxzukj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qp.huanxung.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ak.haigaiapp.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bt.nszjky.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ze.521024.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://be.wgjwhj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hd.hahajie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mp.shxzskj.cn

[D25] Set 集合去重与交并差
来源：http://vy.9csxet.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://cf.shtwfgs.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://sy.jianghongdianzi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wg.bjjhwx.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xu.hahajie.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hy.chemitech.net.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ki.521024.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bk.bjjhwx.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rd.szxytkj.cn

[D26] 数组转字符串
来源：http://ac.haigaiapp.cn

Py:   ", ".join(map(str, arr))
来源：http://hj.yuntaijiaju.cn

PHP:  implode(", ", $arr);
来源：http://jx.huixiangedu.cn

JS:   arr.join(", ")
来源：http://pm.huixiangedu.cn

TS:   arr.join(", ")
来源：http://je.hahajie.cn

Java: String.join(", ", list)
来源：http://tn.nszjky.cn

Go:   strings.Join(strs, ", ")
来源：http://so.jianghongdianzi.cn

Ruby: arr.join(", ")
来源：http://gx.yuntaijiaju.cn

C#:   string.Join(", ", list)
来源：http://ya.szxytkj.cn

================================================================================
来源：http://hx.hahajie.cn

E. 字符串处理
来源：http://zh.huanxung.cn

================================================================================
来源：http://zy.bjjhwx.cn

[E01] 拼接字符串
来源：http://ub.shxzskj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wh.yuexingan06.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://nt.hahajie.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dx.lnxyls.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xt.shtwfgs.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://eo.chemitech.net.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://re.wgjwhj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vy.jianghongdianzi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://yl.yuexingan06.cn

[E02] 重复字符串
来源：http://vf.asd995.cn

Py:   "ab" * 3
来源：http://ke.chemitech.net.cn

PHP:  str_repeat("ab", 3);
来源：http://cr.panjiajie.cn

JS:   "ab".repeat(3)
来源：http://by.shxzukj.cn

TS:   "ab".repeat(3)
来源：http://ml.521024.cn

Java: "ab".repeat(3)
来源：http://vs.nicolike.cn

Go:   strings.Repeat("ab", 3)
来源：http://bk.colortex.cn

Ruby: "ab" * 3
来源：http://ug.bjjhwx.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ql.huanxung.cn

[E03] 截取子串
来源：http://vi.wgjwhj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yh.nszjky.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gi.haigaiapp.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mk.szxytkj.cn

TS:   s.slice(1, 4)
来源：http://yt.lnxyls.cn

Java: s.substring(1, 4)
来源：http://up.bookmarksfly.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ui.haigaiapp.cn

Ruby: s[1, 3];  s[1..3]
来源：http://lz.lnxyls.cn

C#:   s.Substring(1, 3)
来源：http://wr.chemitech.net.cn

[E04] 查找子串位置
来源：http://rr.haigaiapp.cn

Py:   s.find("x");  s.index("x")
来源：http://cd.jctech888.com.cn

PHP:  strpos($s, "x");
来源：http://gm.haigaiapp.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rc.nszjky.cn

TS:   s.indexOf("x")
来源：http://rc.yuntaijiaju.cn

Java: s.indexOf("x")
来源：http://vp.colortex.cn

Go:   strings.Index(s, "x")
来源：http://yg.muxihuayi.cn

Ruby: s.index("x")
来源：http://zo.huanxung.cn

C#:   s.IndexOf("x")
来源：http://wd.colortex.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://xa.jctech888.com.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://om.bookmarksfly.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vn.jctech888.com.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gz.nszjky.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://qq.shxzukj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pi.chemitech.net.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ya.chemitech.net.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ec.shxzskj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://tf.colortex.cn

[E06] 替换子串
来源：http://zm.panjiajie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://po.huixiangedu.cn

PHP:  str_replace("a", "b", $s);
来源：http://tb.huanxung.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mu.hahajie.cn

TS:   s.replaceAll("a", "b")
来源：http://qq.nicolike.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wf.asd995.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://im.chemitech.net.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://af.asd995.cn

C#:   s.Replace("a", "b")
来源：http://cu.hnjuh.cn

[E07] 按分隔符拆分
来源：http://de.szxytkj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jc.jctech888.com.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gv.chemitech.net.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://jy.wgjwhj.cn

TS:   s.split(",")
来源：http://av.bjjhwx.cn

Java: s.split(",");  s.split("\\s+")
来源：http://jn.jctech888.com.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jj.asd995.cn

Ruby: s.split(",");  s.split
来源：http://ua.shtwfgs.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pl.hahajie.cn

[E08] 数组按分隔符合并
来源：http://lv.9csxet.cn

Py:   ",".join(items)
来源：http://gs.chemitech.net.cn

PHP:  implode(",", $items);
来源：http://nt.haigaiapp.cn

JS:   items.join(",")
来源：http://js.yuexingan06.cn

TS:   items.join(",")
来源：http://mf.shxzskj.cn

Java: String.join(",", items)
来源：http://qu.yuntaijiaju.cn

Go:   strings.Join(items, ",")
来源：http://om.nszjky.cn

Ruby: items.join(",")
来源：http://oi.chemitech.net.cn

C#:   string.Join(",", items)
来源：http://hu.huanxung.cn

[E09] 去除所有空白字符
来源：http://qn.chemitech.net.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://cl.nicolike.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://kx.chemitech.net.cn

JS:   s.replace(/\s+/g, "")
来源：http://af.hnjuh.cn

TS:   s.replace(/\s+/g, "")
来源：http://su.bjjhwx.cn

Java: s.replaceAll("\\s+", "")
来源：http://zx.shtwfgs.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://pw.nicolike.cn

Ruby: s.gsub(/\s+/, "")
来源：http://dv.hnjuh.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lu.yuntaijiaju.cn

[E10] 左侧补零 / 定长填充
来源：http://mk.colortex.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://pd.huixinmuqiang.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ic.jianghongdianzi.cn

JS:   "7".padStart(3, "0")
来源：http://cd.yuntaijiaju.cn

TS:   "7".padStart(3, "0")
来源：http://lc.yuntaijiaju.cn

Java: String.format("%03d", 7)
来源：http://is.nicolike.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://la.nszjky.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://th.colortex.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xf.yuntaijiaju.cn

[E11] 反转字符串
来源：http://dp.colortex.cn

Py:   s[::-1]
来源：http://kn.huixiangedu.cn

PHP:  strrev($s);
来源：http://qv.asd995.cn

JS:   [...s].reverse().join("")
来源：http://hy.lnxyls.cn

TS:   [...s].reverse().join("")
来源：http://kw.gzmigu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://fv.yuexingan06.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ca.jianghongdianzi.cn

Ruby: s.reverse
来源：http://ze.huixinmuqiang.cn

C#:   new string(s.Reverse().ToArray())
来源：http://kc.hnjuh.cn

[E12] 统计某字符出现次数
来源：http://cu.jctech888.com.cn

Py:   s.count("a")
来源：http://sk.huanxung.cn

PHP:  substr_count($s, "a");
来源：http://os.jctech888.com.cn

JS:   s.split("a").length - 1
来源：http://il.colortex.cn

TS:   s.split("a").length - 1
来源：http://gj.shxzskj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wi.huixiangedu.cn

Go:   strings.Count(s, "a")
来源：http://nn.panjiajie.cn

Ruby: s.count("a")
来源：http://xp.szxytkj.cn

C#:   s.Count(c => c == 'a')
来源：http://of.shxzukj.cn

[E13] 逐字符遍历
来源：http://cq.newstarts.cn

Py:   for ch in s: print(ch)
来源：http://be.hnjuh.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hu.huanxung.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://sm.szxytkj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ts.shxzukj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gr.muxihuayi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rz.jianghongdianzi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://gm.haigaiapp.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mj.jianghongdianzi.cn

[E14] URL 编码与 Base64
来源：http://in.yuexingan06.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xh.muxihuayi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://af.szsharing.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://uj.yuexingan06.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://yp.muxihuayi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kc.colortex.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jt.asd995.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://lx.hnjuh.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dg.szsharing.cn

[E15] HTML 转义 / 反转义
来源：http://hu.gzmigu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://xy.muxihuayi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rb.nicolike.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://eq.bjjhwx.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ta.shtwfgs.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vi.shxzskj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://so.9csxet.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jr.9csxet.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fb.yuexingan06.cn

[E16] 数字千分位
来源：http://mo.muxihuayi.cn

Py:   f"{1234567:,}"
来源：http://vw.panjiajie.cn

PHP:  number_format(1234567);
来源：http://cb.haigaiapp.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://nw.huanxung.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://gk.bjjhwx.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://kz.haigaiapp.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rm.muxihuayi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hs.colortex.cn

C#:   1234567.ToString("N0")
来源：http://jw.shxzukj.cn

[E17] 首字母大写
来源：http://ue.nszjky.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://on.szsharing.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://rm.bjjhwx.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vg.huixiangedu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ct.hahajie.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jk.asd995.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kj.lnxyls.cn

Ruby: s.capitalize
来源：http://tv.huanxung.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qv.yuexingan06.cn

[E18] 模板占位符替换
来源：http://ax.521024.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ao.newstarts.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nx.hnjuh.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zi.colortex.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://me.panjiajie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ng.yuexingan06.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://to.hnjuh.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://to.gzmigu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ke.9csxet.cn

[E19] 多行文本按行拆分
来源：http://uo.szxytkj.cn

Py:   s.splitlines()
来源：http://mo.lnxyls.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vh.gzmigu.cn

JS:   s.split(/\r?\n/)
来源：http://oc.wgjwhj.cn

TS:   s.split(/\r?\n/)
来源：http://jx.shxzskj.cn

Java: s.lines().toList()
来源：http://mz.nszjky.cn

Go:   strings.Split(s, "\n")
来源：http://om.shxzskj.cn

Ruby: s.lines
来源：http://za.huanxung.cn

C#:   s.Split('\n')
来源：http://qk.hahajie.cn

[E20] 判断字符串是否为空
来源：http://wr.muxihuayi.cn

Py:   if not s:
来源：http://xc.asd995.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rz.nszjky.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ez.haigaiapp.cn

TS:   if (s === "") {}
来源：http://aw.colortex.cn

Java: if (s.isEmpty()) {}
来源：http://sv.521024.cn

Go:   if s == "" {}
来源：http://tj.shxzskj.cn

Ruby: if s.empty?
来源：http://br.yuexingan06.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ac.panjiajie.cn

[E21] 超长截断加省略号
来源：http://kh.jctech888.com.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://di.huixiangedu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vc.shxzukj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zu.yuntaijiaju.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cc.hahajie.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ee.lnxyls.cn

Go:   // 按 rune 判断长度后截断
来源：http://ds.yuexingan06.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tq.lnxyls.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xz.hnjuh.cn

[E22] 字节长度与字符长度
来源：http://wg.521024.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pd.shtwfgs.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wi.szxytkj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://cg.shxzukj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://me.shxzukj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wo.lnxyls.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wj.gzmigu.cn

Ruby: s.bytesize;  s.length
来源：http://vk.asd995.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://nq.jianghongdianzi.cn

================================================================================
来源：http://mj.muxihuayi.cn

F. 文件与目录
来源：http://qe.muxihuayi.cn

================================================================================
来源：http://py.nszjky.cn

[F01] 读取整个文件
来源：http://wb.nszjky.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mr.haigaiapp.cn

PHP:  file_get_contents("a.txt");
来源：http://yo.huixiangedu.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hf.shxzukj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://on.shxzukj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://mc.hahajie.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tf.521024.cn

Ruby: File.read("a.txt")
来源：http://rx.newstarts.cn

C#:   File.ReadAllText("a.txt");
来源：http://wu.hahajie.cn

[F02] 逐行读取文件
来源：http://od.nicolike.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gi.chemitech.net.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pl.nszjky.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cd.huixinmuqiang.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wo.shxzskj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wm.yuexingan06.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hr.yuexingan06.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wq.nicolike.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://eh.panjiajie.cn

[F03] 写入文件（覆盖）
来源：http://ae.haigaiapp.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bh.9csxet.cn


<!-- 参考信息 -->