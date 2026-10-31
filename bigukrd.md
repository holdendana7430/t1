代发 wailian999

[D19] 按字段分组
来源：http://ip.shxzskj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vk.nicolike.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vl.haigaiapp.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://se.huixiangedu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://kx.nszjky.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://oa.shxzskj.cn

Go:   // 手写 map[string][]T
来源：http://ps.nicolike.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://it.huanxung.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ls.colortex.cn

[D20] 统计每个元素出现次数
来源：http://fc.shxzukj.cn

Py:   Counter(arr)
来源：http://ng.yuntaijiaju.cn

PHP:  array_count_values($arr);
来源：http://nw.newstarts.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cz.huanxung.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oz.newstarts.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ka.asd995.cn

Go:   // 手写 map[T]int
来源：http://bt.yuexingan06.cn

Ruby: arr.tally
来源：http://oa.bookmarksfly.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cp.lnxyls.cn

[D21] 判断是否包含某元素
来源：http://co.panjiajie.cn

Py:   x in arr
来源：http://gz.chemitech.net.cn

PHP:  in_array($x, $arr, true);
来源：http://hg.nszjky.cn

JS:   arr.includes(x)
来源：http://qh.gzmigu.cn

TS:   arr.includes(x)
来源：http://vw.panjiajie.cn

Java: list.contains(x)
来源：http://em.bookmarksfly.cn

Go:   slices.Contains(arr, x)
来源：http://mj.szsharing.cn

Ruby: arr.include?(x)
来源：http://ty.jianghongdianzi.cn

C#:   list.Contains(x)
来源：http://on.nszjky.cn

[D22] 复制数组（避免共享引用）
来源：http://va.wgjwhj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://em.chemitech.net.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ai.huanxung.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wv.szxytkj.cn

TS:   [...arr];
来源：http://uq.asd995.cn

Java: new ArrayList<>(list);
来源：http://fr.muxihuayi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://vi.asd995.cn

Ruby: arr.dup;  arr.clone
来源：http://rd.shtwfgs.cn

C#:   new List<int>(list);
来源：http://cx.shxzskj.cn

[D23] reduce 累积计算
来源：http://hk.jianghongdianzi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://js.huixiangedu.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://aa.asd995.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wv.yuexingan06.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://eh.huixiangedu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://yi.panjiajie.cn

Go:   // 手写循环
来源：http://lg.chemitech.net.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mm.szsharing.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gz.asd995.cn

[D24] 字典 / Map 基本操作
来源：http://ks.huanxung.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qe.bjjhwx.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vq.wgjwhj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ps.chemitech.net.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dt.szsharing.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://pk.colortex.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ff.haigaiapp.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ki.muxihuayi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wv.yuntaijiaju.cn

[D25] Set 集合去重与交并差
来源：http://af.bjjhwx.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ua.szsharing.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qt.colortex.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qq.hahajie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jf.muxihuayi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qa.lnxyls.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://yo.nicolike.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://us.huixinmuqiang.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://op.szxytkj.cn

[D26] 数组转字符串
来源：http://sv.bjjhwx.cn

Py:   ", ".join(map(str, arr))
来源：http://uc.lnxyls.cn

PHP:  implode(", ", $arr);
来源：http://wn.asd995.cn

JS:   arr.join(", ")
来源：http://xd.huixinmuqiang.cn

TS:   arr.join(", ")
来源：http://zo.hahajie.cn

Java: String.join(", ", list)
来源：http://ud.newstarts.cn

Go:   strings.Join(strs, ", ")
来源：http://yo.shxzskj.cn

Ruby: arr.join(", ")
来源：http://xe.panjiajie.cn

C#:   string.Join(", ", list)
来源：http://fd.jctech888.com.cn

================================================================================
来源：http://ue.yuexingan06.cn

E. 字符串处理
来源：http://ng.hahajie.cn

================================================================================
来源：http://mp.huanxung.cn

[E01] 拼接字符串
来源：http://vx.yuexingan06.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://uo.newstarts.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://gm.shxzskj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lj.gzmigu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wh.bjjhwx.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://kg.newstarts.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wn.panjiajie.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xb.lnxyls.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qc.jianghongdianzi.cn

[E02] 重复字符串
来源：http://um.huixinmuqiang.cn

Py:   "ab" * 3
来源：http://iv.shxzskj.cn

PHP:  str_repeat("ab", 3);
来源：http://vo.jctech888.com.cn

JS:   "ab".repeat(3)
来源：http://ri.asd995.cn

TS:   "ab".repeat(3)
来源：http://vy.nicolike.cn

Java: "ab".repeat(3)
来源：http://xw.wgjwhj.cn

Go:   strings.Repeat("ab", 3)
来源：http://ue.jianghongdianzi.cn

Ruby: "ab" * 3
来源：http://fy.521024.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rn.panjiajie.cn

[E03] 截取子串
来源：http://sv.nicolike.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xt.szsharing.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://zm.huixinmuqiang.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lv.yuexingan06.cn

TS:   s.slice(1, 4)
来源：http://zm.gzmigu.cn

Java: s.substring(1, 4)
来源：http://jg.shxzskj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fj.muxihuayi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://im.yuntaijiaju.cn

C#:   s.Substring(1, 3)
来源：http://xi.szxytkj.cn

[E04] 查找子串位置
来源：http://vs.huanxung.cn

Py:   s.find("x");  s.index("x")
来源：http://lb.newstarts.cn

PHP:  strpos($s, "x");
来源：http://gd.wgjwhj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wz.jianghongdianzi.cn

TS:   s.indexOf("x")
来源：http://rv.huixinmuqiang.cn

Java: s.indexOf("x")
来源：http://bj.hnjuh.cn

Go:   strings.Index(s, "x")
来源：http://js.jianghongdianzi.cn

Ruby: s.index("x")
来源：http://hl.shxzukj.cn

C#:   s.IndexOf("x")
来源：http://nd.yuntaijiaju.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://je.bookmarksfly.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ly.nszjky.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://tk.yuntaijiaju.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qa.hnjuh.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://it.jctech888.com.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cg.521024.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ew.hnjuh.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://yp.huixinmuqiang.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://be.szsharing.cn

[E06] 替换子串
来源：http://kw.newstarts.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rm.nszjky.cn

PHP:  str_replace("a", "b", $s);
来源：http://ls.colortex.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kq.muxihuayi.cn

TS:   s.replaceAll("a", "b")
来源：http://uy.nszjky.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dl.yuexingan06.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://np.shxzskj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ub.huanxung.cn

C#:   s.Replace("a", "b")
来源：http://ef.gzmigu.cn

[E07] 按分隔符拆分
来源：http://nw.haigaiapp.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ut.shxzukj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fv.huixiangedu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://pn.asd995.cn

TS:   s.split(",")
来源：http://vl.yuexingan06.cn

Java: s.split(",");  s.split("\\s+")
来源：http://tg.wgjwhj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://oi.colortex.cn

Ruby: s.split(",");  s.split
来源：http://as.newstarts.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wd.bookmarksfly.cn

[E08] 数组按分隔符合并
来源：http://kp.shtwfgs.cn

Py:   ",".join(items)
来源：http://ys.colortex.cn

PHP:  implode(",", $items);
来源：http://cq.haigaiapp.cn

JS:   items.join(",")
来源：http://qx.bookmarksfly.cn

TS:   items.join(",")
来源：http://ud.huanxung.cn

Java: String.join(",", items)
来源：http://ud.panjiajie.cn

Go:   strings.Join(items, ",")
来源：http://el.panjiajie.cn

Ruby: items.join(",")
来源：http://vw.nszjky.cn

C#:   string.Join(",", items)
来源：http://st.nicolike.cn

[E09] 去除所有空白字符
来源：http://in.hahajie.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xq.colortex.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://yu.asd995.cn

JS:   s.replace(/\s+/g, "")
来源：http://ww.shxzukj.cn

TS:   s.replace(/\s+/g, "")
来源：http://ru.jianghongdianzi.cn

Java: s.replaceAll("\\s+", "")
来源：http://ju.wgjwhj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://lb.shxzskj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://tq.huixinmuqiang.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rs.shtwfgs.cn

[E10] 左侧补零 / 定长填充
来源：http://bh.muxihuayi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://rh.huixinmuqiang.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zk.jianghongdianzi.cn

JS:   "7".padStart(3, "0")
来源：http://ec.wgjwhj.cn

TS:   "7".padStart(3, "0")
来源：http://ix.muxihuayi.cn

Java: String.format("%03d", 7)
来源：http://km.shxzskj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://et.huixinmuqiang.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://yt.jianghongdianzi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://gf.lnxyls.cn

[E11] 反转字符串
来源：http://sc.szxytkj.cn

Py:   s[::-1]
来源：http://sm.muxihuayi.cn

PHP:  strrev($s);
来源：http://ot.jianghongdianzi.cn

JS:   [...s].reverse().join("")
来源：http://ir.gzmigu.cn

TS:   [...s].reverse().join("")
来源：http://mt.panjiajie.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://nu.haigaiapp.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://qy.szxytkj.cn

Ruby: s.reverse
来源：http://ef.hnjuh.cn

C#:   new string(s.Reverse().ToArray())
来源：http://qp.hnjuh.cn

[E12] 统计某字符出现次数
来源：http://qn.shxzukj.cn

Py:   s.count("a")
来源：http://di.shtwfgs.cn

PHP:  substr_count($s, "a");
来源：http://oo.szsharing.cn

JS:   s.split("a").length - 1
来源：http://wo.huanxung.cn

TS:   s.split("a").length - 1
来源：http://bw.gzmigu.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://er.muxihuayi.cn

Go:   strings.Count(s, "a")
来源：http://wf.panjiajie.cn

Ruby: s.count("a")
来源：http://bh.lnxyls.cn

C#:   s.Count(c => c == 'a')
来源：http://ev.nicolike.cn

[E13] 逐字符遍历
来源：http://rz.szsharing.cn

Py:   for ch in s: print(ch)
来源：http://dx.muxihuayi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://sh.haigaiapp.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://qy.huanxung.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://qn.9csxet.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://cu.chemitech.net.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://yb.huanxung.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://nu.colortex.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://uy.nszjky.cn

[E14] URL 编码与 Base64
来源：http://pm.yuntaijiaju.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://bn.nszjky.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ln.huanxung.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ij.bookmarksfly.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.9csxet.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://sz.jctech888.com.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://uj.chemitech.net.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xr.newstarts.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fr.gzmigu.cn

[E15] HTML 转义 / 反转义
来源：http://wl.hnjuh.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ip.bjjhwx.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://yz.521024.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ty.yuntaijiaju.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://eu.521024.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://jg.jianghongdianzi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ou.shxzskj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fx.asd995.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://id.hahajie.cn

[E16] 数字千分位
来源：http://tb.lnxyls.cn

Py:   f"{1234567:,}"
来源：http://me.shxzukj.cn

PHP:  number_format(1234567);
来源：http://zr.panjiajie.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://xl.szxytkj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ms.lnxyls.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fp.wgjwhj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ak.nicolike.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://op.huanxung.cn

C#:   1234567.ToString("N0")
来源：http://us.521024.cn

[E17] 首字母大写
来源：http://wk.asd995.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cm.szsharing.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://hd.nicolike.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bo.bjjhwx.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://su.newstarts.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dr.shxzukj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://uo.shxzukj.cn

Ruby: s.capitalize
来源：http://ts.hnjuh.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ag.szxytkj.cn

[E18] 模板占位符替换
来源：http://ah.nicolike.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ei.bookmarksfly.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jw.asd995.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://hj.shxzukj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://cl.bookmarksfly.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rj.huixinmuqiang.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mf.gzmigu.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zv.wgjwhj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ey.chemitech.net.cn

[E19] 多行文本按行拆分
来源：http://bf.nszjky.cn

Py:   s.splitlines()
来源：http://gh.bjjhwx.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mu.wgjwhj.cn

JS:   s.split(/\r?\n/)
来源：http://qv.chemitech.net.cn

TS:   s.split(/\r?\n/)
来源：http://eo.huixinmuqiang.cn

Java: s.lines().toList()
来源：http://gz.bjjhwx.cn

Go:   strings.Split(s, "\n")
来源：http://df.muxihuayi.cn

Ruby: s.lines
来源：http://hf.yuexingan06.cn

C#:   s.Split('\n')
来源：http://kk.nszjky.cn

[E20] 判断字符串是否为空
来源：http://px.lnxyls.cn

Py:   if not s:
来源：http://yr.szsharing.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://th.muxihuayi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rb.wgjwhj.cn

TS:   if (s === "") {}
来源：http://ay.521024.cn

Java: if (s.isEmpty()) {}
来源：http://wi.wgjwhj.cn

Go:   if s == "" {}
来源：http://wh.jianghongdianzi.cn

Ruby: if s.empty?
来源：http://or.lnxyls.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ls.huixiangedu.cn

[E21] 超长截断加省略号
来源：http://wc.huixinmuqiang.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mz.huanxung.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zn.jianghongdianzi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zd.huixinmuqiang.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dr.hnjuh.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pc.huixinmuqiang.cn

Go:   // 按 rune 判断长度后截断
来源：http://pq.yuntaijiaju.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lm.gzmigu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wi.hahajie.cn

[E22] 字节长度与字符长度
来源：http://lf.gzmigu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://sb.huixiangedu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wy.muxihuayi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://eu.nicolike.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hd.bjjhwx.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://tk.bjjhwx.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tg.bjjhwx.cn

Ruby: s.bytesize;  s.length
来源：http://du.9csxet.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bu.bjjhwx.cn

================================================================================
来源：http://hq.lnxyls.cn

F. 文件与目录
来源：http://pf.szsharing.cn

================================================================================
来源：http://qs.jctech888.com.cn

[F01] 读取整个文件
来源：http://ez.shxzukj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ne.asd995.cn

PHP:  file_get_contents("a.txt");
来源：http://vp.yuntaijiaju.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gp.hahajie.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://gf.hahajie.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ow.shxzskj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nv.shtwfgs.cn

Ruby: File.read("a.txt")
来源：http://sf.huixinmuqiang.cn

C#:   File.ReadAllText("a.txt");
来源：http://ng.9csxet.cn

[F02] 逐行读取文件
来源：http://be.huixiangedu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ya.hahajie.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://lx.shxzukj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kj.chemitech.net.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yc.huixinmuqiang.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ix.newstarts.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fu.asd995.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gx.huanxung.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://sv.yuntaijiaju.cn

[F03] 写入文件（覆盖）
来源：http://tl.jctech888.com.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://sb.yuntaijiaju.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://je.hnjuh.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bg.bjjhwx.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nc.muxihuayi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://st.shxzukj.cn


<!-- 参考信息 -->