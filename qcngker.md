代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://pt.shtwfgs.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://he.huanxung.cn

TS:   Math.max(...arr);
来源：http://so.yuntaijiaju.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://vl.muxihuayi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ki.yuexingan06.cn

Ruby: arr.max;  arr.min
来源：http://as.bjjhwx.cn

C#:   list.Max();  list.Min()
来源：http://px.yuexingan06.cn

[D18] 扁平化嵌套数组
来源：http://qp.haigaiapp.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://sc.yuntaijiaju.cn

PHP:  array_merge(...$nested);
来源：http://sn.muxihuayi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://nd.hahajie.cn

TS:   nested.flat();
来源：http://se.bookmarksfly.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gh.hahajie.cn

Go:   // 手写双层循环
来源：http://lw.nszjky.cn

Ruby: nested.flatten
来源：http://ev.huixiangedu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://zl.colortex.cn

[D19] 按字段分组
来源：http://iz.jianghongdianzi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kq.huanxung.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mz.shxzskj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gh.wgjwhj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ga.haigaiapp.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vg.hahajie.cn

Go:   // 手写 map[string][]T
来源：http://ga.yuntaijiaju.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://zu.521024.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xl.jianghongdianzi.cn

[D20] 统计每个元素出现次数
来源：http://ds.nszjky.cn

Py:   Counter(arr)
来源：http://ru.shxzskj.cn

PHP:  array_count_values($arr);
来源：http://rb.huixiangedu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ne.nszjky.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dp.szsharing.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ls.nszjky.cn

Go:   // 手写 map[T]int
来源：http://hg.wgjwhj.cn

Ruby: arr.tally
来源：http://jg.huanxung.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rg.haigaiapp.cn

[D21] 判断是否包含某元素
来源：http://yn.yuntaijiaju.cn

Py:   x in arr
来源：http://sj.panjiajie.cn

PHP:  in_array($x, $arr, true);
来源：http://bl.hahajie.cn

JS:   arr.includes(x)
来源：http://dq.muxihuayi.cn

TS:   arr.includes(x)
来源：http://pm.panjiajie.cn

Java: list.contains(x)
来源：http://tk.muxihuayi.cn

Go:   slices.Contains(arr, x)
来源：http://pj.szsharing.cn

Ruby: arr.include?(x)
来源：http://se.huanxung.cn

C#:   list.Contains(x)
来源：http://ky.newstarts.cn

[D22] 复制数组（避免共享引用）
来源：http://th.huixinmuqiang.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mt.shxzskj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zf.szxytkj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hv.szsharing.cn

TS:   [...arr];
来源：http://qd.haigaiapp.cn

Java: new ArrayList<>(list);
来源：http://gb.huixinmuqiang.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ld.shtwfgs.cn

Ruby: arr.dup;  arr.clone
来源：http://vo.lnxyls.cn

C#:   new List<int>(list);
来源：http://uf.muxihuayi.cn

[D23] reduce 累积计算
来源：http://sc.bjjhwx.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rb.9csxet.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jh.bookmarksfly.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ai.asd995.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zj.lnxyls.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://wk.huixiangedu.cn

Go:   // 手写循环
来源：http://ll.wgjwhj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://uc.nicolike.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ya.chemitech.net.cn

[D24] 字典 / Map 基本操作
来源：http://cd.bjjhwx.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pw.newstarts.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mm.huixinmuqiang.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://km.chemitech.net.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bo.hahajie.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ci.jctech888.com.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xo.chemitech.net.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zj.9csxet.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://nn.yuntaijiaju.cn

[D25] Set 集合去重与交并差
来源：http://zi.hahajie.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://so.newstarts.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://id.nszjky.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://us.shxzskj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://uc.9csxet.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://la.newstarts.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qe.huixinmuqiang.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://fr.colortex.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://oc.huixinmuqiang.cn

[D26] 数组转字符串
来源：http://sk.huixinmuqiang.cn

Py:   ", ".join(map(str, arr))
来源：http://mt.jctech888.com.cn

PHP:  implode(", ", $arr);
来源：http://pd.huixinmuqiang.cn

JS:   arr.join(", ")
来源：http://ib.hahajie.cn

TS:   arr.join(", ")
来源：http://uw.shxzskj.cn

Java: String.join(", ", list)
来源：http://qv.jctech888.com.cn

Go:   strings.Join(strs, ", ")
来源：http://og.asd995.cn

Ruby: arr.join(", ")
来源：http://hr.bookmarksfly.cn

C#:   string.Join(", ", list)
来源：http://zq.nszjky.cn

================================================================================
来源：http://nr.jctech888.com.cn

E. 字符串处理
来源：http://pj.huixinmuqiang.cn

================================================================================
来源：http://rp.wgjwhj.cn

[E01] 拼接字符串
来源：http://rd.jctech888.com.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qq.lnxyls.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ia.gzmigu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xm.jianghongdianzi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://kf.yuntaijiaju.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lm.huanxung.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dp.szxytkj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.521024.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ed.gzmigu.cn

[E02] 重复字符串
来源：http://ve.huixinmuqiang.cn

Py:   "ab" * 3
来源：http://iw.asd995.cn

PHP:  str_repeat("ab", 3);
来源：http://vn.bjjhwx.cn

JS:   "ab".repeat(3)
来源：http://bq.lnxyls.cn

TS:   "ab".repeat(3)
来源：http://ad.shxzukj.cn

Java: "ab".repeat(3)
来源：http://dk.yuntaijiaju.cn

Go:   strings.Repeat("ab", 3)
来源：http://fg.shxzukj.cn

Ruby: "ab" * 3
来源：http://gj.shxzukj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rh.huixinmuqiang.cn

[E03] 截取子串
来源：http://pj.huixiangedu.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ey.colortex.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://if.shxzskj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://pb.huixinmuqiang.cn

TS:   s.slice(1, 4)
来源：http://ym.bjjhwx.cn

Java: s.substring(1, 4)
来源：http://ii.szsharing.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qt.nicolike.cn

Ruby: s[1, 3];  s[1..3]
来源：http://fm.shxzukj.cn

C#:   s.Substring(1, 3)
来源：http://wk.colortex.cn

[E04] 查找子串位置
来源：http://nk.chemitech.net.cn

Py:   s.find("x");  s.index("x")
来源：http://zd.haigaiapp.cn

PHP:  strpos($s, "x");
来源：http://xn.lnxyls.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fu.jctech888.com.cn

TS:   s.indexOf("x")
来源：http://wp.huanxung.cn

Java: s.indexOf("x")
来源：http://it.lnxyls.cn

Go:   strings.Index(s, "x")
来源：http://kc.hahajie.cn

Ruby: s.index("x")
来源：http://lp.bjjhwx.cn

C#:   s.IndexOf("x")
来源：http://wo.shxzskj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://zp.bookmarksfly.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wt.yuexingan06.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hd.shxzskj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sn.hahajie.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ty.haigaiapp.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bx.yuntaijiaju.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xg.gzmigu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hm.shxzskj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://cp.shxzskj.cn

[E06] 替换子串
来源：http://eo.9csxet.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ag.asd995.cn

PHP:  str_replace("a", "b", $s);
来源：http://al.chemitech.net.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ew.shxzukj.cn

TS:   s.replaceAll("a", "b")
来源：http://mb.colortex.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hj.muxihuayi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://yq.jctech888.com.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://rf.asd995.cn

C#:   s.Replace("a", "b")
来源：http://ai.newstarts.cn

[E07] 按分隔符拆分
来源：http://ld.wgjwhj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://sl.shxzukj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ef.panjiajie.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://hu.lnxyls.cn

TS:   s.split(",")
来源：http://qc.shxzukj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ou.yuntaijiaju.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wk.asd995.cn

Ruby: s.split(",");  s.split
来源：http://gc.bjjhwx.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kc.nszjky.cn

[E08] 数组按分隔符合并
来源：http://ig.lnxyls.cn

Py:   ",".join(items)
来源：http://rc.newstarts.cn

PHP:  implode(",", $items);
来源：http://lf.9csxet.cn

JS:   items.join(",")
来源：http://rq.muxihuayi.cn

TS:   items.join(",")
来源：http://bh.chemitech.net.cn

Java: String.join(",", items)
来源：http://cv.asd995.cn

Go:   strings.Join(items, ",")
来源：http://fa.9csxet.cn

Ruby: items.join(",")
来源：http://ge.szxytkj.cn

C#:   string.Join(",", items)
来源：http://wk.shxzukj.cn

[E09] 去除所有空白字符
来源：http://re.jianghongdianzi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://tv.yuntaijiaju.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://au.haigaiapp.cn

JS:   s.replace(/\s+/g, "")
来源：http://oq.haigaiapp.cn

TS:   s.replace(/\s+/g, "")
来源：http://zg.bjjhwx.cn

Java: s.replaceAll("\\s+", "")
来源：http://fj.nszjky.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://wm.hnjuh.cn

Ruby: s.gsub(/\s+/, "")
来源：http://og.yuntaijiaju.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ki.wgjwhj.cn

[E10] 左侧补零 / 定长填充
来源：http://zt.521024.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qr.yuexingan06.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://sr.huixinmuqiang.cn

JS:   "7".padStart(3, "0")
来源：http://oy.521024.cn

TS:   "7".padStart(3, "0")
来源：http://ql.szsharing.cn

Java: String.format("%03d", 7)
来源：http://om.panjiajie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ub.asd995.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qj.9csxet.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ld.9csxet.cn

[E11] 反转字符串
来源：http://qk.muxihuayi.cn

Py:   s[::-1]
来源：http://jj.lnxyls.cn

PHP:  strrev($s);
来源：http://ay.9csxet.cn

JS:   [...s].reverse().join("")
来源：http://mz.huixiangedu.cn

TS:   [...s].reverse().join("")
来源：http://gl.huanxung.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://uv.jianghongdianzi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://lk.nszjky.cn

Ruby: s.reverse
来源：http://aw.9csxet.cn

C#:   new string(s.Reverse().ToArray())
来源：http://vf.chemitech.net.cn

[E12] 统计某字符出现次数
来源：http://uo.shtwfgs.cn

Py:   s.count("a")
来源：http://gr.jianghongdianzi.cn

PHP:  substr_count($s, "a");
来源：http://bl.yuntaijiaju.cn

JS:   s.split("a").length - 1
来源：http://iu.521024.cn

TS:   s.split("a").length - 1
来源：http://so.lnxyls.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://me.bookmarksfly.cn

Go:   strings.Count(s, "a")
来源：http://vz.wgjwhj.cn

Ruby: s.count("a")
来源：http://il.shxzskj.cn

C#:   s.Count(c => c == 'a')
来源：http://az.muxihuayi.cn

[E13] 逐字符遍历
来源：http://hk.hahajie.cn

Py:   for ch in s: print(ch)
来源：http://qy.haigaiapp.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fh.bookmarksfly.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://cw.szsharing.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://gs.muxihuayi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://af.panjiajie.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zm.huixiangedu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://sp.nicolike.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://eg.szxytkj.cn

[E14] URL 编码与 Base64
来源：http://uf.huixiangedu.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://io.asd995.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://yx.bookmarksfly.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ln.haigaiapp.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://oj.szsharing.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ke.panjiajie.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://uf.chemitech.net.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://or.wgjwhj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bg.hnjuh.cn

[E15] HTML 转义 / 反转义
来源：http://lr.huanxung.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ce.jctech888.com.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fy.muxihuayi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fq.haigaiapp.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://wt.wgjwhj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ut.9csxet.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://kn.shtwfgs.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ve.szxytkj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://of.gzmigu.cn

[E16] 数字千分位
来源：http://qx.hnjuh.cn

Py:   f"{1234567:,}"
来源：http://ef.szsharing.cn

PHP:  number_format(1234567);
来源：http://jh.nszjky.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ak.shxzskj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://la.shxzskj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ct.yuntaijiaju.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jw.lnxyls.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hk.newstarts.cn

C#:   1234567.ToString("N0")
来源：http://kk.wgjwhj.cn

[E17] 首字母大写
来源：http://qr.muxihuayi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://kl.lnxyls.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ij.panjiajie.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sp.szsharing.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sn.jianghongdianzi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://iu.yuntaijiaju.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ra.bookmarksfly.cn

Ruby: s.capitalize
来源：http://tn.muxihuayi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qn.newstarts.cn

[E18] 模板占位符替换
来源：http://cf.haigaiapp.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zk.panjiajie.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://oh.521024.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://fb.szxytkj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://mz.panjiajie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://cs.lnxyls.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mk.yuexingan06.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zz.panjiajie.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mo.haigaiapp.cn

[E19] 多行文本按行拆分
来源：http://su.szsharing.cn

Py:   s.splitlines()
来源：http://pw.shtwfgs.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hx.asd995.cn

JS:   s.split(/\r?\n/)
来源：http://vs.haigaiapp.cn

TS:   s.split(/\r?\n/)
来源：http://fp.yuntaijiaju.cn

Java: s.lines().toList()
来源：http://nm.newstarts.cn

Go:   strings.Split(s, "\n")
来源：http://pa.huixinmuqiang.cn

Ruby: s.lines
来源：http://tn.bookmarksfly.cn

C#:   s.Split('\n')
来源：http://dp.newstarts.cn

[E20] 判断字符串是否为空
来源：http://tm.wgjwhj.cn

Py:   if not s:
来源：http://of.bookmarksfly.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vd.shtwfgs.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dp.panjiajie.cn

TS:   if (s === "") {}
来源：http://kl.hahajie.cn

Java: if (s.isEmpty()) {}
来源：http://yc.haigaiapp.cn

Go:   if s == "" {}
来源：http://xn.yuntaijiaju.cn

Ruby: if s.empty?
来源：http://vx.huixinmuqiang.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jq.shxzskj.cn

[E21] 超长截断加省略号
来源：http://se.nszjky.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ec.9csxet.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://aq.wgjwhj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kp.szxytkj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xh.bookmarksfly.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://lx.lnxyls.cn

Go:   // 按 rune 判断长度后截断
来源：http://fs.shxzskj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xw.521024.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fp.hahajie.cn

[E22] 字节长度与字符长度
来源：http://gh.hahajie.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ri.huanxung.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mv.szsharing.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fz.nicolike.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gy.yuntaijiaju.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://lz.huixinmuqiang.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rr.shxzukj.cn

Ruby: s.bytesize;  s.length
来源：http://fa.asd995.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://io.chemitech.net.cn

================================================================================
来源：http://sb.hahajie.cn

F. 文件与目录
来源：http://fl.wgjwhj.cn

================================================================================
来源：http://cl.jianghongdianzi.cn

[F01] 读取整个文件
来源：http://ww.9csxet.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vg.nicolike.cn

PHP:  file_get_contents("a.txt");
来源：http://jf.jctech888.com.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bd.yuexingan06.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ri.shxzskj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://nd.huanxung.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tz.521024.cn

Ruby: File.read("a.txt")
来源：http://lk.szxytkj.cn


<!-- 参考信息 -->