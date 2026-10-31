代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://ro.panjiajie.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hb.szxytkj.cn

TS:   Math.max(...arr);
来源：http://yi.szsharing.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://oz.shxzskj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://kz.hnjuh.cn

Ruby: arr.max;  arr.min
来源：http://yy.bjjhwx.cn

C#:   list.Max();  list.Min()
来源：http://gr.huanxung.cn

[D18] 扁平化嵌套数组
来源：http://rs.shxzukj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pj.9csxet.cn

PHP:  array_merge(...$nested);
来源：http://zn.colortex.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pi.haigaiapp.cn

TS:   nested.flat();
来源：http://wq.huixiangedu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dq.gzmigu.cn

Go:   // 手写双层循环
来源：http://oq.9csxet.cn

Ruby: nested.flatten
来源：http://zf.jianghongdianzi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://xc.asd995.cn

[D19] 按字段分组
来源：http://zk.muxihuayi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://li.chemitech.net.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ab.jctech888.com.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mg.huixiangedu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://lf.nszjky.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vp.shxzukj.cn

Go:   // 手写 map[string][]T
来源：http://dr.lnxyls.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://wb.szsharing.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lu.nszjky.cn

[D20] 统计每个元素出现次数
来源：http://le.bjjhwx.cn

Py:   Counter(arr)
来源：http://os.gzmigu.cn

PHP:  array_count_values($arr);
来源：http://gh.jianghongdianzi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fh.colortex.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gw.9csxet.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ij.panjiajie.cn

Go:   // 手写 map[T]int
来源：http://wv.gzmigu.cn

Ruby: arr.tally
来源：http://pk.colortex.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fl.521024.cn

[D21] 判断是否包含某元素
来源：http://mm.haigaiapp.cn

Py:   x in arr
来源：http://uf.521024.cn

PHP:  in_array($x, $arr, true);
来源：http://tg.nszjky.cn

JS:   arr.includes(x)
来源：http://ee.huanxung.cn

TS:   arr.includes(x)
来源：http://tt.huixiangedu.cn

Java: list.contains(x)
来源：http://cx.chemitech.net.cn

Go:   slices.Contains(arr, x)
来源：http://wi.nicolike.cn

Ruby: arr.include?(x)
来源：http://hf.hnjuh.cn

C#:   list.Contains(x)
来源：http://rc.huixinmuqiang.cn

[D22] 复制数组（避免共享引用）
来源：http://lv.521024.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ep.asd995.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hr.asd995.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://va.colortex.cn

TS:   [...arr];
来源：http://pz.newstarts.cn

Java: new ArrayList<>(list);
来源：http://as.huixinmuqiang.cn

Go:   copied := append([]int(nil), arr...)
来源：http://yf.jianghongdianzi.cn

Ruby: arr.dup;  arr.clone
来源：http://zn.huixinmuqiang.cn

C#:   new List<int>(list);
来源：http://fz.bookmarksfly.cn

[D23] reduce 累积计算
来源：http://vy.colortex.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bt.shtwfgs.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cy.chemitech.net.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sj.lnxyls.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://om.muxihuayi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://dc.shxzukj.cn

Go:   // 手写循环
来源：http://hk.bjjhwx.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://yt.hnjuh.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://yj.521024.cn

[D24] 字典 / Map 基本操作
来源：http://yh.asd995.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://eq.gzmigu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kk.huanxung.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://pc.muxihuayi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://sv.szsharing.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://us.panjiajie.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bs.huanxung.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lp.huixiangedu.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ik.asd995.cn

[D25] Set 集合去重与交并差
来源：http://pv.szsharing.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ne.lnxyls.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://oq.nszjky.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://st.lnxyls.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wb.szsharing.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ds.jianghongdianzi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://iy.panjiajie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://df.huixinmuqiang.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jz.yuexingan06.cn

[D26] 数组转字符串
来源：http://ni.haigaiapp.cn

Py:   ", ".join(map(str, arr))
来源：http://jr.haigaiapp.cn

PHP:  implode(", ", $arr);
来源：http://or.huanxung.cn

JS:   arr.join(", ")
来源：http://ow.bookmarksfly.cn

TS:   arr.join(", ")
来源：http://gf.colortex.cn

Java: String.join(", ", list)
来源：http://ca.nicolike.cn

Go:   strings.Join(strs, ", ")
来源：http://cb.jctech888.com.cn

Ruby: arr.join(", ")
来源：http://wa.haigaiapp.cn

C#:   string.Join(", ", list)
来源：http://vu.shtwfgs.cn

================================================================================
来源：http://mn.muxihuayi.cn

E. 字符串处理
来源：http://df.521024.cn

================================================================================
来源：http://jj.nicolike.cn

[E01] 拼接字符串
来源：http://im.szsharing.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://so.colortex.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://od.shxzskj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ek.bookmarksfly.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xf.nicolike.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rh.jctech888.com.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ar.hnjuh.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ka.bookmarksfly.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fx.bookmarksfly.cn

[E02] 重复字符串
来源：http://kq.lnxyls.cn

Py:   "ab" * 3
来源：http://uu.colortex.cn

PHP:  str_repeat("ab", 3);
来源：http://hr.haigaiapp.cn

JS:   "ab".repeat(3)
来源：http://sm.jianghongdianzi.cn

TS:   "ab".repeat(3)
来源：http://qy.nicolike.cn

Java: "ab".repeat(3)
来源：http://hd.shxzskj.cn

Go:   strings.Repeat("ab", 3)
来源：http://vb.huanxung.cn

Ruby: "ab" * 3
来源：http://yb.jctech888.com.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qr.bjjhwx.cn

[E03] 截取子串
来源：http://zo.jianghongdianzi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ir.shxzukj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://an.bookmarksfly.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://eu.hahajie.cn

TS:   s.slice(1, 4)
来源：http://cf.gzmigu.cn

Java: s.substring(1, 4)
来源：http://of.shtwfgs.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hu.chemitech.net.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ef.hnjuh.cn

C#:   s.Substring(1, 3)
来源：http://wk.wgjwhj.cn

[E04] 查找子串位置
来源：http://jb.gzmigu.cn

Py:   s.find("x");  s.index("x")
来源：http://fl.hahajie.cn

PHP:  strpos($s, "x");
来源：http://tf.9csxet.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://cq.huanxung.cn

TS:   s.indexOf("x")
来源：http://yj.shxzskj.cn

Java: s.indexOf("x")
来源：http://qv.lnxyls.cn

Go:   strings.Index(s, "x")
来源：http://sh.nszjky.cn

Ruby: s.index("x")
来源：http://ob.gzmigu.cn

C#:   s.IndexOf("x")
来源：http://sa.szsharing.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://cc.colortex.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jp.colortex.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bi.521024.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://na.bjjhwx.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ge.colortex.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jz.yuexingan06.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qh.huanxung.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pn.nicolike.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jb.hahajie.cn

[E06] 替换子串
来源：http://jf.gzmigu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ya.yuexingan06.cn

PHP:  str_replace("a", "b", $s);
来源：http://ya.huanxung.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zu.gzmigu.cn

TS:   s.replaceAll("a", "b")
来源：http://gd.yuntaijiaju.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rk.jianghongdianzi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://uu.hahajie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://sw.colortex.cn

C#:   s.Replace("a", "b")
来源：http://zy.nszjky.cn

[E07] 按分隔符拆分
来源：http://mg.huanxung.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lb.9csxet.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://du.yuntaijiaju.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://dw.hnjuh.cn

TS:   s.split(",")
来源：http://ux.newstarts.cn

Java: s.split(",");  s.split("\\s+")
来源：http://gs.szxytkj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://sc.hahajie.cn

Ruby: s.split(",");  s.split
来源：http://hw.huanxung.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hb.yuntaijiaju.cn

[E08] 数组按分隔符合并
来源：http://bv.muxihuayi.cn

Py:   ",".join(items)
来源：http://id.jianghongdianzi.cn

PHP:  implode(",", $items);
来源：http://sx.colortex.cn

JS:   items.join(",")
来源：http://kr.huixiangedu.cn

TS:   items.join(",")
来源：http://um.muxihuayi.cn

Java: String.join(",", items)
来源：http://zr.bjjhwx.cn

Go:   strings.Join(items, ",")
来源：http://si.nszjky.cn

Ruby: items.join(",")
来源：http://in.bjjhwx.cn

C#:   string.Join(",", items)
来源：http://qt.nszjky.cn

[E09] 去除所有空白字符
来源：http://ks.nicolike.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xv.shxzskj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://yk.szsharing.cn

JS:   s.replace(/\s+/g, "")
来源：http://nv.huixinmuqiang.cn

TS:   s.replace(/\s+/g, "")
来源：http://pb.szxytkj.cn

Java: s.replaceAll("\\s+", "")
来源：http://gu.huixiangedu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ck.521024.cn

Ruby: s.gsub(/\s+/, "")
来源：http://su.bjjhwx.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://yh.jctech888.com.cn

[E10] 左侧补零 / 定长填充
来源：http://gg.yuntaijiaju.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zv.nszjky.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://lj.colortex.cn

JS:   "7".padStart(3, "0")
来源：http://xn.521024.cn

TS:   "7".padStart(3, "0")
来源：http://ni.muxihuayi.cn

Java: String.format("%03d", 7)
来源：http://xq.yuexingan06.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://yq.szsharing.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://is.hnjuh.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qv.huixiangedu.cn

[E11] 反转字符串
来源：http://ze.newstarts.cn

Py:   s[::-1]
来源：http://zh.bjjhwx.cn

PHP:  strrev($s);
来源：http://zj.shxzskj.cn

JS:   [...s].reverse().join("")
来源：http://mf.9csxet.cn

TS:   [...s].reverse().join("")
来源：http://ba.hnjuh.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://wz.bookmarksfly.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://pd.wgjwhj.cn

Ruby: s.reverse
来源：http://ki.bjjhwx.cn

C#:   new string(s.Reverse().ToArray())
来源：http://we.huixiangedu.cn

[E12] 统计某字符出现次数
来源：http://yl.huixinmuqiang.cn

Py:   s.count("a")
来源：http://ua.gzmigu.cn

PHP:  substr_count($s, "a");
来源：http://pl.szsharing.cn

JS:   s.split("a").length - 1
来源：http://gw.chemitech.net.cn

TS:   s.split("a").length - 1
来源：http://xo.hahajie.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wq.jianghongdianzi.cn

Go:   strings.Count(s, "a")
来源：http://xd.asd995.cn

Ruby: s.count("a")
来源：http://mv.chemitech.net.cn

C#:   s.Count(c => c == 'a')
来源：http://vz.muxihuayi.cn

[E13] 逐字符遍历
来源：http://ng.shxzukj.cn

Py:   for ch in s: print(ch)
来源：http://km.hnjuh.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ot.nszjky.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://qt.bjjhwx.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://jz.szxytkj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fg.wgjwhj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zk.jctech888.com.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://if.hnjuh.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://yj.shxzukj.cn

[E14] URL 编码与 Base64
来源：http://im.hnjuh.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lq.521024.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ih.shxzskj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gq.9csxet.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xz.huixiangedu.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xq.9csxet.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qn.yuexingan06.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ix.yuntaijiaju.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gp.gzmigu.cn

[E15] HTML 转义 / 反转义
来源：http://hn.shxzskj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://wb.9csxet.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://by.yuntaijiaju.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xr.jctech888.com.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://yq.hahajie.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ar.szxytkj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ga.bjjhwx.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://sk.wgjwhj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bt.huixinmuqiang.cn

[E16] 数字千分位
来源：http://kp.shxzukj.cn

Py:   f"{1234567:,}"
来源：http://au.jianghongdianzi.cn

PHP:  number_format(1234567);
来源：http://sv.nszjky.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://we.shtwfgs.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://jt.gzmigu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vp.huixiangedu.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://av.nicolike.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ej.nicolike.cn

C#:   1234567.ToString("N0")
来源：http://hu.huanxung.cn

[E17] 首字母大写
来源：http://oh.shxzskj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://tc.wgjwhj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://xj.nicolike.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fn.hahajie.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jb.yuntaijiaju.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://va.lnxyls.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ii.hahajie.cn

Ruby: s.capitalize
来源：http://qv.yuntaijiaju.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ae.asd995.cn

[E18] 模板占位符替换
来源：http://vo.newstarts.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gi.haigaiapp.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://eo.nszjky.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://cu.szsharing.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://vo.wgjwhj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ll.jctech888.com.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mw.muxihuayi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dm.huixiangedu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://cm.newstarts.cn

[E19] 多行文本按行拆分
来源：http://hh.hahajie.cn

Py:   s.splitlines()
来源：http://rz.chemitech.net.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jk.shtwfgs.cn

JS:   s.split(/\r?\n/)
来源：http://eo.huanxung.cn

TS:   s.split(/\r?\n/)
来源：http://yf.lnxyls.cn

Java: s.lines().toList()
来源：http://ct.jctech888.com.cn

Go:   strings.Split(s, "\n")
来源：http://fs.jctech888.com.cn

Ruby: s.lines
来源：http://zx.nszjky.cn

C#:   s.Split('\n')
来源：http://iy.muxihuayi.cn

[E20] 判断字符串是否为空
来源：http://gh.nicolike.cn

Py:   if not s:
来源：http://oy.shtwfgs.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ks.9csxet.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kw.bookmarksfly.cn

TS:   if (s === "") {}
来源：http://kk.bookmarksfly.cn

Java: if (s.isEmpty()) {}
来源：http://qy.nszjky.cn

Go:   if s == "" {}
来源：http://zt.szxytkj.cn

Ruby: if s.empty?
来源：http://sd.newstarts.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://kx.panjiajie.cn

[E21] 超长截断加省略号
来源：http://oi.muxihuayi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qd.gzmigu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jr.szxytkj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gk.nicolike.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xe.bookmarksfly.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wb.huanxung.cn

Go:   // 按 rune 判断长度后截断
来源：http://lw.wgjwhj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vl.gzmigu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xj.9csxet.cn

[E22] 字节长度与字符长度
来源：http://fh.shtwfgs.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ds.bookmarksfly.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lu.521024.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://om.shtwfgs.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qi.521024.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ed.wgjwhj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zj.hahajie.cn

Ruby: s.bytesize;  s.length
来源：http://sx.bookmarksfly.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ml.hnjuh.cn

================================================================================
来源：http://xy.521024.cn

F. 文件与目录
来源：http://nf.huixinmuqiang.cn

================================================================================
来源：http://io.yuntaijiaju.cn

[F01] 读取整个文件
来源：http://dv.9csxet.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hd.gzmigu.cn

PHP:  file_get_contents("a.txt");
来源：http://nr.lnxyls.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://tg.hahajie.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vt.9csxet.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://rc.9csxet.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fj.bjjhwx.cn

Ruby: File.read("a.txt")
来源：http://nn.shtwfgs.cn


<!-- 参考信息 -->