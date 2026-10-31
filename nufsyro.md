代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ti.muxihuayi.cn

Go:   // 手写双层循环
来源：http://qm.nszjky.cn

Ruby: nested.flatten
来源：http://ts.521024.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://fw.shtwfgs.cn

[D19] 按字段分组
来源：http://lu.szsharing.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xk.szxytkj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://iu.hnjuh.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://cm.huixiangedu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ug.newstarts.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hr.hahajie.cn

Go:   // 手写 map[string][]T
来源：http://bt.jctech888.com.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://gb.colortex.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ed.wgjwhj.cn

[D20] 统计每个元素出现次数
来源：http://pi.haigaiapp.cn

Py:   Counter(arr)
来源：http://qf.lnxyls.cn

PHP:  array_count_values($arr);
来源：http://jy.nszjky.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jl.yuntaijiaju.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vr.huixiangedu.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://yc.newstarts.cn

Go:   // 手写 map[T]int
来源：http://kl.shxzskj.cn

Ruby: arr.tally
来源：http://zc.521024.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kc.huixiangedu.cn

[D21] 判断是否包含某元素
来源：http://yq.wgjwhj.cn

Py:   x in arr
来源：http://ym.haigaiapp.cn

PHP:  in_array($x, $arr, true);
来源：http://wv.shxzskj.cn

JS:   arr.includes(x)
来源：http://tv.hahajie.cn

TS:   arr.includes(x)
来源：http://vw.szxytkj.cn

Java: list.contains(x)
来源：http://cm.jctech888.com.cn

Go:   slices.Contains(arr, x)
来源：http://pb.gzmigu.cn

Ruby: arr.include?(x)
来源：http://xf.newstarts.cn

C#:   list.Contains(x)
来源：http://tv.yuexingan06.cn

[D22] 复制数组（避免共享引用）
来源：http://be.colortex.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://re.chemitech.net.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zx.bookmarksfly.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://cd.bookmarksfly.cn

TS:   [...arr];
来源：http://fi.chemitech.net.cn

Java: new ArrayList<>(list);
来源：http://pq.nicolike.cn

Go:   copied := append([]int(nil), arr...)
来源：http://zl.bjjhwx.cn

Ruby: arr.dup;  arr.clone
来源：http://kz.yuexingan06.cn

C#:   new List<int>(list);
来源：http://lg.lnxyls.cn

[D23] reduce 累积计算
来源：http://xt.shtwfgs.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zu.nszjky.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rr.jctech888.com.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gj.bjjhwx.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lq.hnjuh.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://bt.hnjuh.cn

Go:   // 手写循环
来源：http://kn.szsharing.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ri.asd995.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://fy.nicolike.cn

[D24] 字典 / Map 基本操作
来源：http://vq.chemitech.net.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://tt.szsharing.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hp.9csxet.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xv.nszjky.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://kk.gzmigu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://uy.shxzskj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://kw.shxzukj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kx.hahajie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ho.shtwfgs.cn

[D25] Set 集合去重与交并差
来源：http://lv.jctech888.com.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://uw.yuntaijiaju.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://kn.yuntaijiaju.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ss.lnxyls.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ah.chemitech.net.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://yu.gzmigu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://dg.shxzukj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://sr.9csxet.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://kg.asd995.cn

[D26] 数组转字符串
来源：http://xp.szxytkj.cn

Py:   ", ".join(map(str, arr))
来源：http://li.gzmigu.cn

PHP:  implode(", ", $arr);
来源：http://gh.bjjhwx.cn

JS:   arr.join(", ")
来源：http://xf.shtwfgs.cn

TS:   arr.join(", ")
来源：http://ma.panjiajie.cn

Java: String.join(", ", list)
来源：http://hf.panjiajie.cn

Go:   strings.Join(strs, ", ")
来源：http://ga.colortex.cn

Ruby: arr.join(", ")
来源：http://wi.newstarts.cn

C#:   string.Join(", ", list)
来源：http://ri.chemitech.net.cn

================================================================================
来源：http://bd.szxytkj.cn

E. 字符串处理
来源：http://sw.lnxyls.cn

================================================================================
来源：http://tn.shxzskj.cn

[E01] 拼接字符串
来源：http://nh.colortex.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://eu.nicolike.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rf.shtwfgs.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fd.521024.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ar.jctech888.com.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fn.asd995.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xz.muxihuayi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ul.chemitech.net.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://df.9csxet.cn

[E02] 重复字符串
来源：http://rn.nicolike.cn

Py:   "ab" * 3
来源：http://bn.muxihuayi.cn

PHP:  str_repeat("ab", 3);
来源：http://zq.nicolike.cn

JS:   "ab".repeat(3)
来源：http://zq.asd995.cn

TS:   "ab".repeat(3)
来源：http://dk.lnxyls.cn

Java: "ab".repeat(3)
来源：http://gx.shtwfgs.cn

Go:   strings.Repeat("ab", 3)
来源：http://jt.9csxet.cn

Ruby: "ab" * 3
来源：http://ux.bookmarksfly.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fa.huixinmuqiang.cn

[E03] 截取子串
来源：http://os.huixiangedu.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://at.newstarts.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://so.muxihuayi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xw.huanxung.cn

TS:   s.slice(1, 4)
来源：http://pp.yuexingan06.cn

Java: s.substring(1, 4)
来源：http://kb.colortex.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://uf.colortex.cn

Ruby: s[1, 3];  s[1..3]
来源：http://th.chemitech.net.cn

C#:   s.Substring(1, 3)
来源：http://ez.szsharing.cn

[E04] 查找子串位置
来源：http://wq.muxihuayi.cn

Py:   s.find("x");  s.index("x")
来源：http://fg.huanxung.cn

PHP:  strpos($s, "x");
来源：http://ia.9csxet.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vm.shxzukj.cn

TS:   s.indexOf("x")
来源：http://ej.newstarts.cn

Java: s.indexOf("x")
来源：http://by.szxytkj.cn

Go:   strings.Index(s, "x")
来源：http://nz.jianghongdianzi.cn

Ruby: s.index("x")
来源：http://zt.jianghongdianzi.cn

C#:   s.IndexOf("x")
来源：http://sg.shtwfgs.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://dv.yuntaijiaju.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jb.shxzukj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://za.yuexingan06.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://va.hahajie.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ok.huanxung.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yc.nszjky.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ie.asd995.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://sk.panjiajie.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ea.haigaiapp.cn

[E06] 替换子串
来源：http://rx.wgjwhj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ru.yuntaijiaju.cn

PHP:  str_replace("a", "b", $s);
来源：http://up.asd995.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xt.huanxung.cn

TS:   s.replaceAll("a", "b")
来源：http://re.hnjuh.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bq.panjiajie.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qq.szxytkj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://uw.huixinmuqiang.cn

C#:   s.Replace("a", "b")
来源：http://ix.newstarts.cn

[E07] 按分隔符拆分
来源：http://mg.muxihuayi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pb.hnjuh.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://lv.huixiangedu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://rk.bjjhwx.cn

TS:   s.split(",")
来源：http://xd.asd995.cn

Java: s.split(",");  s.split("\\s+")
来源：http://eh.szsharing.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zt.huixinmuqiang.cn

Ruby: s.split(",");  s.split
来源：http://eo.yuexingan06.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lm.newstarts.cn

[E08] 数组按分隔符合并
来源：http://xp.haigaiapp.cn

Py:   ",".join(items)
来源：http://we.yuntaijiaju.cn

PHP:  implode(",", $items);
来源：http://vt.hnjuh.cn

JS:   items.join(",")
来源：http://qh.huanxung.cn

TS:   items.join(",")
来源：http://fu.yuntaijiaju.cn

Java: String.join(",", items)
来源：http://nl.newstarts.cn

Go:   strings.Join(items, ",")
来源：http://vy.jianghongdianzi.cn

Ruby: items.join(",")
来源：http://af.lnxyls.cn

C#:   string.Join(",", items)
来源：http://de.521024.cn

[E09] 去除所有空白字符
来源：http://da.gzmigu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://uw.jctech888.com.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://pu.newstarts.cn

JS:   s.replace(/\s+/g, "")
来源：http://dr.colortex.cn

TS:   s.replace(/\s+/g, "")
来源：http://ze.hnjuh.cn

Java: s.replaceAll("\\s+", "")
来源：http://bx.colortex.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://tc.haigaiapp.cn

Ruby: s.gsub(/\s+/, "")
来源：http://xh.hahajie.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zr.chemitech.net.cn

[E10] 左侧补零 / 定长填充
来源：http://wf.9csxet.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://oi.shxzskj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://pi.haigaiapp.cn

JS:   "7".padStart(3, "0")
来源：http://rm.nicolike.cn

TS:   "7".padStart(3, "0")
来源：http://dy.jctech888.com.cn

Java: String.format("%03d", 7)
来源：http://er.huixiangedu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://so.wgjwhj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vu.shxzskj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qv.yuexingan06.cn

[E11] 反转字符串
来源：http://cl.nicolike.cn

Py:   s[::-1]
来源：http://dr.nszjky.cn

PHP:  strrev($s);
来源：http://xp.huanxung.cn

JS:   [...s].reverse().join("")
来源：http://hj.hahajie.cn

TS:   [...s].reverse().join("")
来源：http://ad.lnxyls.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ng.colortex.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://kk.shxzukj.cn

Ruby: s.reverse
来源：http://ub.colortex.cn

C#:   new string(s.Reverse().ToArray())
来源：http://yh.colortex.cn

[E12] 统计某字符出现次数
来源：http://zj.lnxyls.cn

Py:   s.count("a")
来源：http://ux.newstarts.cn

PHP:  substr_count($s, "a");
来源：http://yo.yuexingan06.cn

JS:   s.split("a").length - 1
来源：http://kg.yuntaijiaju.cn

TS:   s.split("a").length - 1
来源：http://vx.jianghongdianzi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ey.hahajie.cn

Go:   strings.Count(s, "a")
来源：http://fp.shxzukj.cn

Ruby: s.count("a")
来源：http://we.bookmarksfly.cn

C#:   s.Count(c => c == 'a')
来源：http://ax.newstarts.cn

[E13] 逐字符遍历
来源：http://cg.wgjwhj.cn

Py:   for ch in s: print(ch)
来源：http://fw.521024.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qk.szxytkj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://fh.jctech888.com.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://jm.huixiangedu.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://lx.muxihuayi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mv.colortex.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://mz.hahajie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://tu.bjjhwx.cn

[E14] URL 编码与 Base64
来源：http://oh.shxzskj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://sf.bjjhwx.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://iw.panjiajie.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://nr.521024.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://eb.yuexingan06.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bo.szxytkj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://st.lnxyls.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tf.shxzskj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fk.huixinmuqiang.cn

[E15] HTML 转义 / 反转义
来源：http://jk.bookmarksfly.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://py.wgjwhj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xu.colortex.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lk.szxytkj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://rf.huanxung.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kl.asd995.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://za.asd995.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cf.shxzukj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://rj.newstarts.cn

[E16] 数字千分位
来源：http://cz.hnjuh.cn

Py:   f"{1234567:,}"
来源：http://jr.chemitech.net.cn

PHP:  number_format(1234567);
来源：http://pr.shtwfgs.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ee.lnxyls.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://la.hahajie.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ob.shxzskj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hw.muxihuayi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://jl.yuntaijiaju.cn

C#:   1234567.ToString("N0")
来源：http://nt.jianghongdianzi.cn

[E17] 首字母大写
来源：http://ru.colortex.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://jd.nicolike.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://yw.hahajie.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kw.huixinmuqiang.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zt.shtwfgs.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kg.nszjky.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://dt.9csxet.cn

Ruby: s.capitalize
来源：http://uv.huixinmuqiang.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rb.panjiajie.cn

[E18] 模板占位符替换
来源：http://ah.chemitech.net.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://iv.huixinmuqiang.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bz.szxytkj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://bo.9csxet.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://pr.hahajie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ws.hnjuh.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ow.chemitech.net.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://pr.nicolike.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gp.huixiangedu.cn

[E19] 多行文本按行拆分
来源：http://hh.muxihuayi.cn

Py:   s.splitlines()
来源：http://ua.9csxet.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://un.bookmarksfly.cn

JS:   s.split(/\r?\n/)
来源：http://ax.newstarts.cn

TS:   s.split(/\r?\n/)
来源：http://ig.szsharing.cn

Java: s.lines().toList()
来源：http://nh.shtwfgs.cn

Go:   strings.Split(s, "\n")
来源：http://jr.nicolike.cn

Ruby: s.lines
来源：http://yg.jianghongdianzi.cn

C#:   s.Split('\n')
来源：http://rf.shxzukj.cn

[E20] 判断字符串是否为空
来源：http://sx.shxzskj.cn

Py:   if not s:
来源：http://ov.hahajie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://re.yuntaijiaju.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lp.lnxyls.cn

TS:   if (s === "") {}
来源：http://kg.9csxet.cn

Java: if (s.isEmpty()) {}
来源：http://yj.lnxyls.cn

Go:   if s == "" {}
来源：http://wu.muxihuayi.cn

Ruby: if s.empty?
来源：http://od.huixiangedu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ae.colortex.cn

[E21] 超长截断加省略号
来源：http://mj.shtwfgs.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://uj.colortex.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wp.521024.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cc.shxzukj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wr.bookmarksfly.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://sw.bookmarksfly.cn

Go:   // 按 rune 判断长度后截断
来源：http://ct.huixiangedu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dd.521024.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://md.newstarts.cn

[E22] 字节长度与字符长度
来源：http://on.hnjuh.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://lj.haigaiapp.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mn.huanxung.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wg.lnxyls.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ms.huixinmuqiang.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://oe.nszjky.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://iu.colortex.cn

Ruby: s.bytesize;  s.length
来源：http://fl.szsharing.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://sf.521024.cn

================================================================================
来源：http://ln.bjjhwx.cn

F. 文件与目录
来源：http://nq.nicolike.cn

================================================================================
来源：http://zx.shtwfgs.cn

[F01] 读取整个文件
来源：http://py.bookmarksfly.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://md.shxzskj.cn

PHP:  file_get_contents("a.txt");
来源：http://wh.shtwfgs.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ru.jctech888.com.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ps.huanxung.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://bx.huixinmuqiang.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hn.yuexingan06.cn

Ruby: File.read("a.txt")
来源：http://kl.521024.cn

C#:   File.ReadAllText("a.txt");
来源：http://ot.521024.cn

[F02] 逐行读取文件
来源：http://mo.colortex.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pm.yuexingan06.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wx.shtwfgs.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xk.panjiajie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jc.shxzskj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ek.szxytkj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gt.hnjuh.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vo.bookmarksfly.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://uy.szsharing.cn

[F03] 写入文件（覆盖）
来源：http://pu.huixiangedu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://tj.asd995.cn


<!-- 参考信息 -->