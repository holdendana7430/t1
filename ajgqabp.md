代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wx.hnjuh.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mn.colortex.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fe.huixinmuqiang.cn

Go:   // 手写循环累加
来源：http://wx.jianghongdianzi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zy.bookmarksfly.cn

C#:   list.Sum();  list.Average()
来源：http://iz.hahajie.cn

[D17] 最大值与最小值
来源：http://bn.yuntaijiaju.cn

Py:   max(arr);  min(arr)
来源：http://wj.shtwfgs.cn

PHP:  max($arr);  min($arr);
来源：http://xm.newstarts.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xy.huanxung.cn

TS:   Math.max(...arr);
来源：http://ea.shxzskj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://wa.panjiajie.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ze.szsharing.cn

Ruby: arr.max;  arr.min
来源：http://gj.jianghongdianzi.cn

C#:   list.Max();  list.Min()
来源：http://uc.yuntaijiaju.cn

[D18] 扁平化嵌套数组
来源：http://yu.shxzskj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rw.huixinmuqiang.cn

PHP:  array_merge(...$nested);
来源：http://kd.huanxung.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ej.9csxet.cn

TS:   nested.flat();
来源：http://mn.hnjuh.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rv.nszjky.cn

Go:   // 手写双层循环
来源：http://qx.bookmarksfly.cn

Ruby: nested.flatten
来源：http://ka.asd995.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://zi.colortex.cn

[D19] 按字段分组
来源：http://fm.szsharing.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://sr.hnjuh.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xh.colortex.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ev.muxihuayi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://qw.wgjwhj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vx.bjjhwx.cn

Go:   // 手写 map[string][]T
来源：http://tv.gzmigu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://tt.bjjhwx.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ur.521024.cn

[D20] 统计每个元素出现次数
来源：http://mx.shtwfgs.cn

Py:   Counter(arr)
来源：http://ga.jctech888.com.cn

PHP:  array_count_values($arr);
来源：http://jg.bookmarksfly.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ze.9csxet.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kl.huixinmuqiang.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jw.muxihuayi.cn

Go:   // 手写 map[T]int
来源：http://qi.yuntaijiaju.cn

Ruby: arr.tally
来源：http://gj.newstarts.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vr.nszjky.cn

[D21] 判断是否包含某元素
来源：http://mi.huanxung.cn

Py:   x in arr
来源：http://wq.lnxyls.cn

PHP:  in_array($x, $arr, true);
来源：http://au.jianghongdianzi.cn

JS:   arr.includes(x)
来源：http://ku.muxihuayi.cn

TS:   arr.includes(x)
来源：http://un.bjjhwx.cn

Java: list.contains(x)
来源：http://zu.shtwfgs.cn

Go:   slices.Contains(arr, x)
来源：http://pc.bookmarksfly.cn

Ruby: arr.include?(x)
来源：http://em.521024.cn

C#:   list.Contains(x)
来源：http://pz.shtwfgs.cn

[D22] 复制数组（避免共享引用）
来源：http://af.muxihuayi.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vm.521024.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vi.yuexingan06.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://uj.jianghongdianzi.cn

TS:   [...arr];
来源：http://cu.huixinmuqiang.cn

Java: new ArrayList<>(list);
来源：http://th.yuexingan06.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ff.nszjky.cn

Ruby: arr.dup;  arr.clone
来源：http://vh.yuntaijiaju.cn

C#:   new List<int>(list);
来源：http://lx.panjiajie.cn

[D23] reduce 累积计算
来源：http://kr.szsharing.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xj.lnxyls.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pm.asd995.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ud.gzmigu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yv.chemitech.net.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://bx.shxzukj.cn

Go:   // 手写循环
来源：http://rd.szxytkj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ru.nszjky.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://en.shxzukj.cn

[D24] 字典 / Map 基本操作
来源：http://sy.hnjuh.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://nq.bjjhwx.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kt.szxytkj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hu.wgjwhj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vp.hahajie.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fa.bjjhwx.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wq.hahajie.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xe.asd995.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dv.newstarts.cn

[D25] Set 集合去重与交并差
来源：http://yy.colortex.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://gj.hahajie.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fw.bookmarksfly.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ba.bookmarksfly.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bi.haigaiapp.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hm.hnjuh.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://si.bjjhwx.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://cn.panjiajie.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mj.huixinmuqiang.cn

[D26] 数组转字符串
来源：http://jb.huixinmuqiang.cn

Py:   ", ".join(map(str, arr))
来源：http://cs.lnxyls.cn

PHP:  implode(", ", $arr);
来源：http://bl.shtwfgs.cn

JS:   arr.join(", ")
来源：http://sl.haigaiapp.cn

TS:   arr.join(", ")
来源：http://zk.bookmarksfly.cn

Java: String.join(", ", list)
来源：http://tl.lnxyls.cn

Go:   strings.Join(strs, ", ")
来源：http://dc.yuexingan06.cn

Ruby: arr.join(", ")
来源：http://cp.gzmigu.cn

C#:   string.Join(", ", list)
来源：http://ms.bjjhwx.cn

================================================================================
来源：http://xm.nszjky.cn

E. 字符串处理
来源：http://pj.huixinmuqiang.cn

================================================================================
来源：http://ae.huixiangedu.cn

[E01] 拼接字符串
来源：http://sl.asd995.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ok.bookmarksfly.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://nc.huixinmuqiang.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tj.9csxet.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://le.yuntaijiaju.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://kw.bookmarksfly.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tg.lnxyls.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vi.colortex.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xg.bjjhwx.cn

[E02] 重复字符串
来源：http://we.hahajie.cn

Py:   "ab" * 3
来源：http://id.asd995.cn

PHP:  str_repeat("ab", 3);
来源：http://vz.shxzukj.cn

JS:   "ab".repeat(3)
来源：http://co.shxzskj.cn

TS:   "ab".repeat(3)
来源：http://hq.lnxyls.cn

Java: "ab".repeat(3)
来源：http://kf.szxytkj.cn

Go:   strings.Repeat("ab", 3)
来源：http://tx.521024.cn

Ruby: "ab" * 3
来源：http://mv.hahajie.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wt.szxytkj.cn

[E03] 截取子串
来源：http://jh.gzmigu.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ax.nicolike.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://rp.szxytkj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jb.521024.cn

TS:   s.slice(1, 4)
来源：http://iy.panjiajie.cn

Java: s.substring(1, 4)
来源：http://cu.shxzskj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ui.yuexingan06.cn

Ruby: s[1, 3];  s[1..3]
来源：http://mj.shxzskj.cn

C#:   s.Substring(1, 3)
来源：http://ek.haigaiapp.cn

[E04] 查找子串位置
来源：http://tj.colortex.cn

Py:   s.find("x");  s.index("x")
来源：http://oz.huanxung.cn

PHP:  strpos($s, "x");
来源：http://vy.szsharing.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jw.bookmarksfly.cn

TS:   s.indexOf("x")
来源：http://ug.bookmarksfly.cn

Java: s.indexOf("x")
来源：http://ov.jianghongdianzi.cn

Go:   strings.Index(s, "x")
来源：http://au.9csxet.cn

Ruby: s.index("x")
来源：http://sy.bjjhwx.cn

C#:   s.IndexOf("x")
来源：http://ri.szsharing.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://zm.9csxet.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://sr.yuntaijiaju.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jl.hnjuh.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xv.wgjwhj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://xs.yuexingan06.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qm.hahajie.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ky.szxytkj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rw.chemitech.net.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mv.lnxyls.cn

[E06] 替换子串
来源：http://dj.chemitech.net.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zo.nicolike.cn

PHP:  str_replace("a", "b", $s);
来源：http://vi.521024.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vp.shxzskj.cn

TS:   s.replaceAll("a", "b")
来源：http://qj.shxzskj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zm.huanxung.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ma.muxihuayi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wc.jctech888.com.cn

C#:   s.Replace("a", "b")
来源：http://qq.jianghongdianzi.cn

[E07] 按分隔符拆分
来源：http://kk.jctech888.com.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://kp.jianghongdianzi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://uv.colortex.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://at.panjiajie.cn

TS:   s.split(",")
来源：http://xi.muxihuayi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://gc.huixiangedu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hf.shtwfgs.cn

Ruby: s.split(",");  s.split
来源：http://fr.jianghongdianzi.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rz.shtwfgs.cn

[E08] 数组按分隔符合并
来源：http://cj.colortex.cn

Py:   ",".join(items)
来源：http://oc.colortex.cn

PHP:  implode(",", $items);
来源：http://wi.yuntaijiaju.cn

JS:   items.join(",")
来源：http://th.muxihuayi.cn

TS:   items.join(",")
来源：http://nv.shxzukj.cn

Java: String.join(",", items)
来源：http://bl.nicolike.cn

Go:   strings.Join(items, ",")
来源：http://jx.nszjky.cn

Ruby: items.join(",")
来源：http://kr.9csxet.cn

C#:   string.Join(",", items)
来源：http://ua.nszjky.cn

[E09] 去除所有空白字符
来源：http://up.szxytkj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lj.haigaiapp.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ch.szxytkj.cn

JS:   s.replace(/\s+/g, "")
来源：http://oz.huixinmuqiang.cn

TS:   s.replace(/\s+/g, "")
来源：http://oe.colortex.cn

Java: s.replaceAll("\\s+", "")
来源：http://dh.szxytkj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ks.shxzskj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://qh.nszjky.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gr.jianghongdianzi.cn

[E10] 左侧补零 / 定长填充
来源：http://kf.huixiangedu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ik.nszjky.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qq.muxihuayi.cn

JS:   "7".padStart(3, "0")
来源：http://ss.panjiajie.cn

TS:   "7".padStart(3, "0")
来源：http://az.bjjhwx.cn

Java: String.format("%03d", 7)
来源：http://vd.hnjuh.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ry.bookmarksfly.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://js.shxzskj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vj.521024.cn

[E11] 反转字符串
来源：http://jd.shxzskj.cn

Py:   s[::-1]
来源：http://pw.nicolike.cn

PHP:  strrev($s);
来源：http://xn.chemitech.net.cn

JS:   [...s].reverse().join("")
来源：http://ao.jianghongdianzi.cn

TS:   [...s].reverse().join("")
来源：http://ai.chemitech.net.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://la.bookmarksfly.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://vo.yuexingan06.cn

Ruby: s.reverse
来源：http://lk.huanxung.cn

C#:   new string(s.Reverse().ToArray())
来源：http://kf.huixiangedu.cn

[E12] 统计某字符出现次数
来源：http://ta.nicolike.cn

Py:   s.count("a")
来源：http://mc.521024.cn

PHP:  substr_count($s, "a");
来源：http://gd.wgjwhj.cn

JS:   s.split("a").length - 1
来源：http://vg.gzmigu.cn

TS:   s.split("a").length - 1
来源：http://du.bookmarksfly.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://tr.521024.cn

Go:   strings.Count(s, "a")
来源：http://hw.wgjwhj.cn

Ruby: s.count("a")
来源：http://ic.nicolike.cn

C#:   s.Count(c => c == 'a')
来源：http://be.szxytkj.cn

[E13] 逐字符遍历
来源：http://ec.panjiajie.cn

Py:   for ch in s: print(ch)
来源：http://ti.asd995.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://nl.nicolike.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://tb.huixiangedu.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://xl.huixiangedu.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ym.hnjuh.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://cq.muxihuayi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://nq.lnxyls.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vm.muxihuayi.cn

[E14] URL 编码与 Base64
来源：http://eq.hnjuh.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://yi.jctech888.com.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ij.shtwfgs.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kh.chemitech.net.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://su.jianghongdianzi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ie.huixiangedu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qi.wgjwhj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://do.shtwfgs.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qc.shxzskj.cn

[E15] HTML 转义 / 反转义
来源：http://jh.haigaiapp.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://tn.panjiajie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hk.wgjwhj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zy.asd995.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://pp.shtwfgs.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vc.huixiangedu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wd.9csxet.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://kn.lnxyls.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://tt.9csxet.cn

[E16] 数字千分位
来源：http://ao.jctech888.com.cn

Py:   f"{1234567:,}"
来源：http://wx.jianghongdianzi.cn

PHP:  number_format(1234567);
来源：http://kt.nicolike.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ur.9csxet.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://tk.szsharing.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://np.muxihuayi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://kc.huanxung.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://yy.wgjwhj.cn

C#:   1234567.ToString("N0")
来源：http://iu.gzmigu.cn

[E17] 首字母大写
来源：http://nj.nicolike.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cs.muxihuayi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://sa.szxytkj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ij.shxzukj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ix.lnxyls.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://eu.shtwfgs.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ex.colortex.cn

Ruby: s.capitalize
来源：http://kv.szxytkj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ks.shxzukj.cn

[E18] 模板占位符替换
来源：http://bq.szsharing.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xc.gzmigu.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://no.jianghongdianzi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://kh.yuexingan06.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://gd.huixinmuqiang.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mu.yuexingan06.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bj.gzmigu.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://or.lnxyls.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://oo.jianghongdianzi.cn

[E19] 多行文本按行拆分
来源：http://vr.haigaiapp.cn

Py:   s.splitlines()
来源：http://bb.huixiangedu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cs.hahajie.cn

JS:   s.split(/\r?\n/)
来源：http://ov.asd995.cn

TS:   s.split(/\r?\n/)
来源：http://ed.muxihuayi.cn

Java: s.lines().toList()
来源：http://th.panjiajie.cn

Go:   strings.Split(s, "\n")
来源：http://gw.yuntaijiaju.cn

Ruby: s.lines
来源：http://jb.szxytkj.cn

C#:   s.Split('\n')
来源：http://qi.yuexingan06.cn

[E20] 判断字符串是否为空
来源：http://uw.yuntaijiaju.cn

Py:   if not s:
来源：http://ha.9csxet.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ew.bjjhwx.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://bf.shxzskj.cn

TS:   if (s === "") {}
来源：http://tt.huanxung.cn

Java: if (s.isEmpty()) {}
来源：http://ac.chemitech.net.cn

Go:   if s == "" {}
来源：http://he.hahajie.cn

Ruby: if s.empty?
来源：http://rv.bjjhwx.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qg.huanxung.cn

[E21] 超长截断加省略号
来源：http://sc.colortex.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hu.asd995.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://nf.gzmigu.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mb.colortex.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zg.huixiangedu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pa.shxzukj.cn

Go:   // 按 rune 判断长度后截断
来源：http://au.chemitech.net.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dt.wgjwhj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xa.asd995.cn

[E22] 字节长度与字符长度
来源：http://vh.wgjwhj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://oe.szsharing.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sn.haigaiapp.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fb.colortex.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tw.panjiajie.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://eu.wgjwhj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kf.wgjwhj.cn

Ruby: s.bytesize;  s.length
来源：http://db.colortex.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fn.asd995.cn

================================================================================
来源：http://az.szsharing.cn

F. 文件与目录
来源：http://fv.jianghongdianzi.cn

================================================================================
来源：http://di.szsharing.cn


<!-- 参考信息 -->