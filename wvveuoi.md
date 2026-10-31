代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pk.nszjky.cn

Go:   // 手写双层循环
来源：http://fv.shtwfgs.cn

Ruby: nested.flatten
来源：http://qa.panjiajie.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ki.szsharing.cn

[D19] 按字段分组
来源：http://oc.hnjuh.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xv.asd995.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://sl.hnjuh.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tr.huanxung.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://dl.wgjwhj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mz.wgjwhj.cn

Go:   // 手写 map[string][]T
来源：http://da.lnxyls.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://dk.newstarts.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kd.jctech888.com.cn

[D20] 统计每个元素出现次数
来源：http://dw.szxytkj.cn

Py:   Counter(arr)
来源：http://mh.hnjuh.cn

PHP:  array_count_values($arr);
来源：http://wq.yuexingan06.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ie.bookmarksfly.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qq.huanxung.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://yu.asd995.cn

Go:   // 手写 map[T]int
来源：http://cb.huixiangedu.cn

Ruby: arr.tally
来源：http://lb.panjiajie.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://nu.gzmigu.cn

[D21] 判断是否包含某元素
来源：http://xl.huixiangedu.cn

Py:   x in arr
来源：http://bq.asd995.cn

PHP:  in_array($x, $arr, true);
来源：http://mm.muxihuayi.cn

JS:   arr.includes(x)
来源：http://ti.nicolike.cn

TS:   arr.includes(x)
来源：http://gk.jctech888.com.cn

Java: list.contains(x)
来源：http://bv.asd995.cn

Go:   slices.Contains(arr, x)
来源：http://pa.yuexingan06.cn

Ruby: arr.include?(x)
来源：http://au.hnjuh.cn

C#:   list.Contains(x)
来源：http://wq.asd995.cn

[D22] 复制数组（避免共享引用）
来源：http://cx.yuntaijiaju.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://bj.shtwfgs.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jd.yuntaijiaju.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bg.9csxet.cn

TS:   [...arr];
来源：http://qe.asd995.cn

Java: new ArrayList<>(list);
来源：http://da.hahajie.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ir.newstarts.cn

Ruby: arr.dup;  arr.clone
来源：http://pd.bjjhwx.cn

C#:   new List<int>(list);
来源：http://bo.huanxung.cn

[D23] reduce 累积计算
来源：http://ij.newstarts.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qg.colortex.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jm.bookmarksfly.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qo.huanxung.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ni.bjjhwx.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://rx.muxihuayi.cn

Go:   // 手写循环
来源：http://fm.jctech888.com.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bw.bookmarksfly.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ka.szxytkj.cn

[D24] 字典 / Map 基本操作
来源：http://ha.szxytkj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://oy.szsharing.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xf.chemitech.net.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ki.szxytkj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://uy.huanxung.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ug.newstarts.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://cl.jianghongdianzi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://oz.szsharing.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ll.panjiajie.cn

[D25] Set 集合去重与交并差
来源：http://zs.hnjuh.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fu.szxytkj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://lg.huanxung.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://cn.shtwfgs.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kg.lnxyls.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zw.jctech888.com.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xi.hnjuh.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mt.bjjhwx.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qa.szsharing.cn

[D26] 数组转字符串
来源：http://su.yuexingan06.cn

Py:   ", ".join(map(str, arr))
来源：http://gi.szxytkj.cn

PHP:  implode(", ", $arr);
来源：http://fq.huanxung.cn

JS:   arr.join(", ")
来源：http://wu.huixinmuqiang.cn

TS:   arr.join(", ")
来源：http://ar.huixiangedu.cn

Java: String.join(", ", list)
来源：http://yc.chemitech.net.cn

Go:   strings.Join(strs, ", ")
来源：http://nz.asd995.cn

Ruby: arr.join(", ")
来源：http://jb.haigaiapp.cn

C#:   string.Join(", ", list)
来源：http://go.nicolike.cn

================================================================================
来源：http://oq.haigaiapp.cn

E. 字符串处理
来源：http://em.asd995.cn

================================================================================
来源：http://mn.lnxyls.cn

[E01] 拼接字符串
来源：http://xr.wgjwhj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zb.hahajie.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mf.shxzskj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ma.bookmarksfly.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://yx.huanxung.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://oo.lnxyls.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://no.asd995.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://oc.shtwfgs.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gl.huixinmuqiang.cn

[E02] 重复字符串
来源：http://ji.panjiajie.cn

Py:   "ab" * 3
来源：http://it.9csxet.cn

PHP:  str_repeat("ab", 3);
来源：http://bn.huixinmuqiang.cn

JS:   "ab".repeat(3)
来源：http://it.hahajie.cn

TS:   "ab".repeat(3)
来源：http://ub.haigaiapp.cn

Java: "ab".repeat(3)
来源：http://pa.huixiangedu.cn

Go:   strings.Repeat("ab", 3)
来源：http://lx.9csxet.cn

Ruby: "ab" * 3
来源：http://of.newstarts.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rv.yuntaijiaju.cn

[E03] 截取子串
来源：http://wd.haigaiapp.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jg.newstarts.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://je.bookmarksfly.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://pq.shxzukj.cn

TS:   s.slice(1, 4)
来源：http://jw.bookmarksfly.cn

Java: s.substring(1, 4)
来源：http://hq.huixinmuqiang.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ek.panjiajie.cn

Ruby: s[1, 3];  s[1..3]
来源：http://xu.chemitech.net.cn

C#:   s.Substring(1, 3)
来源：http://qv.szxytkj.cn

[E04] 查找子串位置
来源：http://kw.yuntaijiaju.cn

Py:   s.find("x");  s.index("x")
来源：http://rd.lnxyls.cn

PHP:  strpos($s, "x");
来源：http://cq.shtwfgs.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://dr.bjjhwx.cn

TS:   s.indexOf("x")
来源：http://ya.bjjhwx.cn

Java: s.indexOf("x")
来源：http://iu.shtwfgs.cn

Go:   strings.Index(s, "x")
来源：http://gc.chemitech.net.cn

Ruby: s.index("x")
来源：http://om.jianghongdianzi.cn

C#:   s.IndexOf("x")
来源：http://ki.521024.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://hj.shtwfgs.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dg.hnjuh.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jw.haigaiapp.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ns.shtwfgs.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://te.huanxung.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ha.panjiajie.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ua.haigaiapp.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qg.9csxet.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bc.huixiangedu.cn

[E06] 替换子串
来源：http://cd.nicolike.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ok.bookmarksfly.cn

PHP:  str_replace("a", "b", $s);
来源：http://fk.colortex.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xw.bookmarksfly.cn

TS:   s.replaceAll("a", "b")
来源：http://gj.bookmarksfly.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://oh.lnxyls.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ac.yuntaijiaju.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ky.nicolike.cn

C#:   s.Replace("a", "b")
来源：http://ng.lnxyls.cn

[E07] 按分隔符拆分
来源：http://jp.bookmarksfly.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pm.yuntaijiaju.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://oy.lnxyls.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ca.shtwfgs.cn

TS:   s.split(",")
来源：http://po.chemitech.net.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ey.nicolike.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kf.jctech888.com.cn

Ruby: s.split(",");  s.split
来源：http://pq.nicolike.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lu.haigaiapp.cn

[E08] 数组按分隔符合并
来源：http://fb.shxzskj.cn

Py:   ",".join(items)
来源：http://my.hnjuh.cn

PHP:  implode(",", $items);
来源：http://nz.chemitech.net.cn

JS:   items.join(",")
来源：http://sn.newstarts.cn

TS:   items.join(",")
来源：http://nn.yuexingan06.cn

Java: String.join(",", items)
来源：http://uw.huixiangedu.cn

Go:   strings.Join(items, ",")
来源：http://ze.jctech888.com.cn

Ruby: items.join(",")
来源：http://ko.asd995.cn

C#:   string.Join(",", items)
来源：http://jh.9csxet.cn

[E09] 去除所有空白字符
来源：http://kl.wgjwhj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vo.huixiangedu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fv.yuntaijiaju.cn

JS:   s.replace(/\s+/g, "")
来源：http://rg.huixiangedu.cn

TS:   s.replace(/\s+/g, "")
来源：http://nh.newstarts.cn

Java: s.replaceAll("\\s+", "")
来源：http://yw.shxzskj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://jd.szsharing.cn

Ruby: s.gsub(/\s+/, "")
来源：http://za.muxihuayi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rz.shtwfgs.cn

[E10] 左侧补零 / 定长填充
来源：http://tw.9csxet.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ac.lnxyls.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jw.bjjhwx.cn

JS:   "7".padStart(3, "0")
来源：http://nz.szsharing.cn

TS:   "7".padStart(3, "0")
来源：http://va.newstarts.cn

Java: String.format("%03d", 7)
来源：http://oy.panjiajie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://gi.haigaiapp.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://os.bookmarksfly.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ue.wgjwhj.cn

[E11] 反转字符串
来源：http://sr.szxytkj.cn

Py:   s[::-1]
来源：http://up.huixinmuqiang.cn

PHP:  strrev($s);
来源：http://vi.panjiajie.cn

JS:   [...s].reverse().join("")
来源：http://hu.chemitech.net.cn

TS:   [...s].reverse().join("")
来源：http://qn.lnxyls.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://iy.colortex.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://is.newstarts.cn

Ruby: s.reverse
来源：http://rj.asd995.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ng.chemitech.net.cn

[E12] 统计某字符出现次数
来源：http://zs.haigaiapp.cn

Py:   s.count("a")
来源：http://tq.521024.cn

PHP:  substr_count($s, "a");
来源：http://lx.lnxyls.cn

JS:   s.split("a").length - 1
来源：http://fo.huixiangedu.cn

TS:   s.split("a").length - 1
来源：http://eb.hahajie.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hg.gzmigu.cn

Go:   strings.Count(s, "a")
来源：http://hh.nszjky.cn

Ruby: s.count("a")
来源：http://wx.szxytkj.cn

C#:   s.Count(c => c == 'a')
来源：http://bl.shtwfgs.cn

[E13] 逐字符遍历
来源：http://hj.521024.cn

Py:   for ch in s: print(ch)
来源：http://rl.lnxyls.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://cm.panjiajie.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://my.huixinmuqiang.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://au.colortex.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ru.nszjky.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://le.panjiajie.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://zh.gzmigu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ya.nszjky.cn

[E14] URL 编码与 Base64
来源：http://vb.bookmarksfly.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ss.colortex.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ly.huixinmuqiang.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://cg.shxzskj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://sz.hahajie.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://dx.wgjwhj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gj.yuexingan06.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dn.yuntaijiaju.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://kl.asd995.cn

[E15] HTML 转义 / 反转义
来源：http://ct.huixiangedu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://et.bjjhwx.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://iz.hahajie.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lj.chemitech.net.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ft.yuexingan06.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bd.shtwfgs.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rr.yuntaijiaju.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ux.lnxyls.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bu.hahajie.cn

[E16] 数字千分位
来源：http://ub.yuntaijiaju.cn

Py:   f"{1234567:,}"
来源：http://ma.shtwfgs.cn

PHP:  number_format(1234567);
来源：http://fu.wgjwhj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://il.bookmarksfly.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ib.shtwfgs.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wb.nicolike.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://in.bookmarksfly.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pi.jctech888.com.cn

C#:   1234567.ToString("N0")
来源：http://po.szsharing.cn

[E17] 首字母大写
来源：http://yp.szsharing.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cc.bjjhwx.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://pd.lnxyls.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nn.bjjhwx.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ct.9csxet.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://tr.yuexingan06.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://st.huixiangedu.cn

Ruby: s.capitalize
来源：http://ok.chemitech.net.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://oj.szsharing.cn

[E18] 模板占位符替换
来源：http://bc.gzmigu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vg.hahajie.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zz.jctech888.com.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://lo.shxzskj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://tf.panjiajie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ec.szxytkj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vz.haigaiapp.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rx.haigaiapp.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zh.yuntaijiaju.cn

[E19] 多行文本按行拆分
来源：http://ax.shxzukj.cn

Py:   s.splitlines()
来源：http://fl.huixiangedu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://af.newstarts.cn

JS:   s.split(/\r?\n/)
来源：http://ai.yuexingan06.cn

TS:   s.split(/\r?\n/)
来源：http://xf.gzmigu.cn

Java: s.lines().toList()
来源：http://fv.huixinmuqiang.cn

Go:   strings.Split(s, "\n")
来源：http://lb.panjiajie.cn

Ruby: s.lines
来源：http://dj.yuntaijiaju.cn

C#:   s.Split('\n')
来源：http://io.lnxyls.cn

[E20] 判断字符串是否为空
来源：http://sc.lnxyls.cn

Py:   if not s:
来源：http://rq.shtwfgs.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://om.shtwfgs.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yz.hnjuh.cn

TS:   if (s === "") {}
来源：http://rh.yuntaijiaju.cn

Java: if (s.isEmpty()) {}
来源：http://bi.shxzskj.cn

Go:   if s == "" {}
来源：http://dk.hnjuh.cn

Ruby: if s.empty?
来源：http://oj.asd995.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yq.jianghongdianzi.cn

[E21] 超长截断加省略号
来源：http://zi.bjjhwx.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kl.shxzskj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xc.shtwfgs.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pj.muxihuayi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://eu.muxihuayi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ho.shxzukj.cn

Go:   // 按 rune 判断长度后截断
来源：http://ep.bjjhwx.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ge.wgjwhj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gq.chemitech.net.cn

[E22] 字节长度与字符长度
来源：http://dw.huixiangedu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://nw.lnxyls.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vr.yuexingan06.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mg.wgjwhj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xw.wgjwhj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zq.lnxyls.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://af.shtwfgs.cn

Ruby: s.bytesize;  s.length
来源：http://mn.huixiangedu.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wl.huixiangedu.cn

================================================================================
来源：http://bc.hahajie.cn

F. 文件与目录
来源：http://hu.yuntaijiaju.cn

================================================================================
来源：http://ob.hahajie.cn

[F01] 读取整个文件
来源：http://xd.nszjky.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rl.yuexingan06.cn

PHP:  file_get_contents("a.txt");
来源：http://tq.jctech888.com.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://uz.szsharing.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mt.yuexingan06.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://lz.newstarts.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gh.yuntaijiaju.cn

Ruby: File.read("a.txt")
来源：http://ch.shxzskj.cn

C#:   File.ReadAllText("a.txt");
来源：http://ld.jianghongdianzi.cn

[F02] 逐行读取文件
来源：http://cm.jctech888.com.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lo.szxytkj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ub.huanxung.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sj.521024.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://an.lnxyls.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pr.hahajie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ic.wgjwhj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rm.newstarts.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qg.newstarts.cn

[F03] 写入文件（覆盖）
来源：http://rn.yuexingan06.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://yy.colortex.cn


<!-- 参考信息 -->