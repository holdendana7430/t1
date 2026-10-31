代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xy.yuntaijiaju.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rw.hahajie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rc.hnjuh.cn

Go:   // 手写循环累加
来源：http://qq.521024.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ma.yuexingan06.cn

C#:   list.Sum();  list.Average()
来源：http://xc.shtwfgs.cn

[D17] 最大值与最小值
来源：http://am.szsharing.cn

Py:   max(arr);  min(arr)
来源：http://nk.jctech888.com.cn

PHP:  max($arr);  min($arr);
来源：http://pl.yuntaijiaju.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xb.huixiangedu.cn

TS:   Math.max(...arr);
来源：http://dl.huanxung.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://vk.chemitech.net.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yn.hahajie.cn

Ruby: arr.max;  arr.min
来源：http://fd.colortex.cn

C#:   list.Max();  list.Min()
来源：http://qf.gzmigu.cn

[D18] 扁平化嵌套数组
来源：http://ea.haigaiapp.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://eo.jianghongdianzi.cn

PHP:  array_merge(...$nested);
来源：http://qg.bookmarksfly.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hg.newstarts.cn

TS:   nested.flat();
来源：http://uv.yuexingan06.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dw.shtwfgs.cn

Go:   // 手写双层循环
来源：http://qx.panjiajie.cn

Ruby: nested.flatten
来源：http://pi.bjjhwx.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://sg.hahajie.cn

[D19] 按字段分组
来源：http://ya.wgjwhj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://lr.huixinmuqiang.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ow.chemitech.net.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://zd.shtwfgs.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://zm.yuntaijiaju.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://oz.szsharing.cn

Go:   // 手写 map[string][]T
来源：http://sc.bookmarksfly.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ip.shxzskj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yq.521024.cn

[D20] 统计每个元素出现次数
来源：http://kk.bookmarksfly.cn

Py:   Counter(arr)
来源：http://nu.521024.cn

PHP:  array_count_values($arr);
来源：http://ur.gzmigu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zm.yuntaijiaju.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gi.yuntaijiaju.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ay.jianghongdianzi.cn

Go:   // 手写 map[T]int
来源：http://ec.jianghongdianzi.cn

Ruby: arr.tally
来源：http://ae.szsharing.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://aw.jianghongdianzi.cn

[D21] 判断是否包含某元素
来源：http://no.bjjhwx.cn

Py:   x in arr
来源：http://um.nszjky.cn

PHP:  in_array($x, $arr, true);
来源：http://sr.newstarts.cn

JS:   arr.includes(x)
来源：http://gg.hnjuh.cn

TS:   arr.includes(x)
来源：http://ma.hnjuh.cn

Java: list.contains(x)
来源：http://kx.9csxet.cn

Go:   slices.Contains(arr, x)
来源：http://co.hnjuh.cn

Ruby: arr.include?(x)
来源：http://db.bjjhwx.cn

C#:   list.Contains(x)
来源：http://nl.haigaiapp.cn

[D22] 复制数组（避免共享引用）
来源：http://jn.muxihuayi.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zi.newstarts.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ds.wgjwhj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ym.jianghongdianzi.cn

TS:   [...arr];
来源：http://jy.chemitech.net.cn

Java: new ArrayList<>(list);
来源：http://nx.jianghongdianzi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://mt.huanxung.cn

Ruby: arr.dup;  arr.clone
来源：http://tr.shtwfgs.cn

C#:   new List<int>(list);
来源：http://kj.9csxet.cn

[D23] reduce 累积计算
来源：http://zh.hnjuh.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://sa.nszjky.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zd.huixiangedu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tb.asd995.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sk.haigaiapp.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://qc.colortex.cn

Go:   // 手写循环
来源：http://cs.jianghongdianzi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://au.jianghongdianzi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pz.shxzskj.cn

[D24] 字典 / Map 基本操作
来源：http://jb.szxytkj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://uf.gzmigu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ev.nszjky.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ox.521024.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://tf.jianghongdianzi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://yl.jctech888.com.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xg.haigaiapp.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pa.panjiajie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jn.szxytkj.cn

[D25] Set 集合去重与交并差
来源：http://di.colortex.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://sv.hnjuh.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://uq.chemitech.net.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://pv.bookmarksfly.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gj.huixinmuqiang.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hf.wgjwhj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://sf.shtwfgs.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nr.jctech888.com.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fr.newstarts.cn

[D26] 数组转字符串
来源：http://qf.chemitech.net.cn

Py:   ", ".join(map(str, arr))
来源：http://jn.yuntaijiaju.cn

PHP:  implode(", ", $arr);
来源：http://au.wgjwhj.cn

JS:   arr.join(", ")
来源：http://eq.jianghongdianzi.cn

TS:   arr.join(", ")
来源：http://kn.szsharing.cn

Java: String.join(", ", list)
来源：http://vr.bjjhwx.cn

Go:   strings.Join(strs, ", ")
来源：http://zm.shtwfgs.cn

Ruby: arr.join(", ")
来源：http://uc.huixinmuqiang.cn

C#:   string.Join(", ", list)
来源：http://qz.szsharing.cn

================================================================================
来源：http://te.huanxung.cn

E. 字符串处理
来源：http://xb.jctech888.com.cn

================================================================================
来源：http://jf.szxytkj.cn

[E01] 拼接字符串
来源：http://qt.colortex.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ds.bjjhwx.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ky.yuexingan06.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fw.szxytkj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://is.newstarts.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mi.shtwfgs.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://va.hahajie.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ax.shxzskj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qq.nszjky.cn

[E02] 重复字符串
来源：http://db.newstarts.cn

Py:   "ab" * 3
来源：http://pn.hahajie.cn

PHP:  str_repeat("ab", 3);
来源：http://on.nszjky.cn

JS:   "ab".repeat(3)
来源：http://qu.huixiangedu.cn

TS:   "ab".repeat(3)
来源：http://we.521024.cn

Java: "ab".repeat(3)
来源：http://ui.haigaiapp.cn

Go:   strings.Repeat("ab", 3)
来源：http://am.szsharing.cn

Ruby: "ab" * 3
来源：http://fq.nszjky.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://he.hahajie.cn

[E03] 截取子串
来源：http://yt.yuntaijiaju.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xa.wgjwhj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://kg.colortex.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qa.hahajie.cn

TS:   s.slice(1, 4)
来源：http://eq.newstarts.cn

Java: s.substring(1, 4)
来源：http://is.asd995.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://vf.bookmarksfly.cn

Ruby: s[1, 3];  s[1..3]
来源：http://hw.nicolike.cn

C#:   s.Substring(1, 3)
来源：http://ly.huixinmuqiang.cn

[E04] 查找子串位置
来源：http://xh.jianghongdianzi.cn

Py:   s.find("x");  s.index("x")
来源：http://zh.wgjwhj.cn

PHP:  strpos($s, "x");
来源：http://zg.jianghongdianzi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://bk.szxytkj.cn

TS:   s.indexOf("x")
来源：http://ve.muxihuayi.cn

Java: s.indexOf("x")
来源：http://sx.szxytkj.cn

Go:   strings.Index(s, "x")
来源：http://yk.nicolike.cn

Ruby: s.index("x")
来源：http://jd.shxzukj.cn

C#:   s.IndexOf("x")
来源：http://ur.muxihuayi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://zj.nicolike.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ov.521024.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://sy.lnxyls.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gu.huixiangedu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://re.huixiangedu.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yg.shxzukj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://oa.yuexingan06.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rs.panjiajie.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rj.szsharing.cn

[E06] 替换子串
来源：http://tu.hnjuh.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://cc.haigaiapp.cn

PHP:  str_replace("a", "b", $s);
来源：http://lr.haigaiapp.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://eq.newstarts.cn

TS:   s.replaceAll("a", "b")
来源：http://bd.bookmarksfly.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cn.nicolike.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fh.muxihuayi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jd.huixiangedu.cn

C#:   s.Replace("a", "b")
来源：http://ca.shtwfgs.cn

[E07] 按分隔符拆分
来源：http://ru.yuntaijiaju.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fh.huixinmuqiang.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://sd.haigaiapp.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://kr.szsharing.cn

TS:   s.split(",")
来源：http://oj.asd995.cn

Java: s.split(",");  s.split("\\s+")
来源：http://fh.521024.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pe.521024.cn

Ruby: s.split(",");  s.split
来源：http://mv.hahajie.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://en.hahajie.cn

[E08] 数组按分隔符合并
来源：http://lo.nicolike.cn

Py:   ",".join(items)
来源：http://he.colortex.cn

PHP:  implode(",", $items);
来源：http://gn.huanxung.cn

JS:   items.join(",")
来源：http://qc.shtwfgs.cn

TS:   items.join(",")
来源：http://ud.521024.cn

Java: String.join(",", items)
来源：http://ux.9csxet.cn

Go:   strings.Join(items, ",")
来源：http://nc.huixinmuqiang.cn

Ruby: items.join(",")
来源：http://gu.haigaiapp.cn

C#:   string.Join(",", items)
来源：http://jb.jianghongdianzi.cn

[E09] 去除所有空白字符
来源：http://tg.gzmigu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://gv.gzmigu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ab.lnxyls.cn

JS:   s.replace(/\s+/g, "")
来源：http://qy.huixiangedu.cn

TS:   s.replace(/\s+/g, "")
来源：http://tf.huixiangedu.cn

Java: s.replaceAll("\\s+", "")
来源：http://an.bookmarksfly.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://hp.hnjuh.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ki.lnxyls.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://az.lnxyls.cn

[E10] 左侧补零 / 定长填充
来源：http://sz.yuntaijiaju.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fh.shtwfgs.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qj.nszjky.cn

JS:   "7".padStart(3, "0")
来源：http://mh.shxzskj.cn

TS:   "7".padStart(3, "0")
来源：http://lf.shxzskj.cn

Java: String.format("%03d", 7)
来源：http://qu.szsharing.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://zx.bookmarksfly.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pb.nicolike.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zf.panjiajie.cn

[E11] 反转字符串
来源：http://af.shxzukj.cn

Py:   s[::-1]
来源：http://wx.szxytkj.cn

PHP:  strrev($s);
来源：http://bz.hahajie.cn

JS:   [...s].reverse().join("")
来源：http://gw.hnjuh.cn

TS:   [...s].reverse().join("")
来源：http://ae.9csxet.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://of.9csxet.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://lj.521024.cn

Ruby: s.reverse
来源：http://qo.huixinmuqiang.cn

C#:   new string(s.Reverse().ToArray())
来源：http://wk.9csxet.cn

[E12] 统计某字符出现次数
来源：http://uh.szxytkj.cn

Py:   s.count("a")
来源：http://ot.521024.cn

PHP:  substr_count($s, "a");
来源：http://my.hnjuh.cn

JS:   s.split("a").length - 1
来源：http://rs.lnxyls.cn

TS:   s.split("a").length - 1
来源：http://wd.nicolike.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://iv.nszjky.cn

Go:   strings.Count(s, "a")
来源：http://zr.bookmarksfly.cn

Ruby: s.count("a")
来源：http://az.bjjhwx.cn

C#:   s.Count(c => c == 'a')
来源：http://re.shxzukj.cn

[E13] 逐字符遍历
来源：http://vi.nszjky.cn

Py:   for ch in s: print(ch)
来源：http://kr.yuntaijiaju.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zg.jianghongdianzi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://fo.bookmarksfly.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://fn.9csxet.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://br.shxzskj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://iu.wgjwhj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ln.shxzskj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://pr.panjiajie.cn

[E14] URL 编码与 Base64
来源：http://id.shxzskj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pz.nszjky.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://gv.panjiajie.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wd.bookmarksfly.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ui.jianghongdianzi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qf.asd995.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://kt.jctech888.com.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://js.shxzukj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ja.haigaiapp.cn

[E15] HTML 转义 / 反转义
来源：http://ui.asd995.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://mq.gzmigu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://cl.jctech888.com.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cs.colortex.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://pa.asd995.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wl.gzmigu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ul.nszjky.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://kr.chemitech.net.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://he.panjiajie.cn

[E16] 数字千分位
来源：http://lo.hahajie.cn

Py:   f"{1234567:,}"
来源：http://yv.shxzukj.cn

PHP:  number_format(1234567);
来源：http://lr.hnjuh.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://lg.nszjky.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://id.haigaiapp.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://kt.521024.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://kq.asd995.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://sn.huanxung.cn

C#:   1234567.ToString("N0")
来源：http://nv.haigaiapp.cn

[E17] 首字母大写
来源：http://oj.szsharing.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qr.gzmigu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://qq.asd995.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mo.jctech888.com.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gu.yuexingan06.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wh.shxzukj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ks.shtwfgs.cn

Ruby: s.capitalize
来源：http://au.haigaiapp.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ar.521024.cn

[E18] 模板占位符替换
来源：http://vh.jianghongdianzi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://dd.muxihuayi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ny.hahajie.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zj.jctech888.com.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ud.bookmarksfly.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zm.bookmarksfly.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qt.jianghongdianzi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ed.huixinmuqiang.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gs.huanxung.cn

[E19] 多行文本按行拆分
来源：http://eb.asd995.cn

Py:   s.splitlines()
来源：http://nh.nszjky.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://se.szsharing.cn

JS:   s.split(/\r?\n/)
来源：http://kz.nszjky.cn

TS:   s.split(/\r?\n/)
来源：http://fr.lnxyls.cn

Java: s.lines().toList()
来源：http://xj.huixinmuqiang.cn

Go:   strings.Split(s, "\n")
来源：http://wo.muxihuayi.cn

Ruby: s.lines
来源：http://xo.haigaiapp.cn

C#:   s.Split('\n')
来源：http://te.yuntaijiaju.cn

[E20] 判断字符串是否为空
来源：http://nm.huixinmuqiang.cn

Py:   if not s:
来源：http://yg.haigaiapp.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jw.asd995.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lh.colortex.cn

TS:   if (s === "") {}
来源：http://ii.521024.cn

Java: if (s.isEmpty()) {}
来源：http://on.muxihuayi.cn

Go:   if s == "" {}
来源：http://ma.shxzukj.cn

Ruby: if s.empty?
来源：http://wp.hahajie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fc.panjiajie.cn

[E21] 超长截断加省略号
来源：http://ab.bjjhwx.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vl.colortex.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vc.asd995.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rr.newstarts.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ck.nszjky.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://cw.bookmarksfly.cn

Go:   // 按 rune 判断长度后截断
来源：http://qm.szsharing.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dk.nicolike.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ku.nszjky.cn

[E22] 字节长度与字符长度
来源：http://ml.lnxyls.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kc.521024.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ix.huanxung.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://nn.wgjwhj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pa.szsharing.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zt.521024.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pu.haigaiapp.cn

Ruby: s.bytesize;  s.length
来源：http://ns.shxzskj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ig.wgjwhj.cn

================================================================================
来源：http://cu.lnxyls.cn

F. 文件与目录
来源：http://ye.gzmigu.cn

================================================================================
来源：http://in.hnjuh.cn


<!-- 参考信息 -->