代发 wailian999

C#:   list.Distinct().ToList()
来源：http://jw.jctech888.com.cn

[D16] 求和与平均值
来源：http://yy.shxzskj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mr.wgjwhj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://st.yuntaijiaju.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hl.bjjhwx.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zl.shtwfgs.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://es.lnxyls.cn

Go:   // 手写循环累加
来源：http://ea.shxzukj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wf.chemitech.net.cn

C#:   list.Sum();  list.Average()
来源：http://hm.gzmigu.cn

[D17] 最大值与最小值
来源：http://yl.panjiajie.cn

Py:   max(arr);  min(arr)
来源：http://uq.newstarts.cn

PHP:  max($arr);  min($arr);
来源：http://ui.yuexingan06.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://tj.chemitech.net.cn

TS:   Math.max(...arr);
来源：http://sa.nicolike.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://qa.jctech888.com.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vi.hnjuh.cn

Ruby: arr.max;  arr.min
来源：http://xn.shxzukj.cn

C#:   list.Max();  list.Min()
来源：http://ko.yuntaijiaju.cn

[D18] 扁平化嵌套数组
来源：http://aa.yuexingan06.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jo.gzmigu.cn

PHP:  array_merge(...$nested);
来源：http://rh.szxytkj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://cf.panjiajie.cn

TS:   nested.flat();
来源：http://ye.shxzskj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://za.shxzskj.cn

Go:   // 手写双层循环
来源：http://xc.huixinmuqiang.cn

Ruby: nested.flatten
来源：http://kg.szxytkj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://be.huixiangedu.cn

[D19] 按字段分组
来源：http://fs.shtwfgs.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://aq.bjjhwx.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qt.huixiangedu.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nj.bookmarksfly.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ye.9csxet.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rn.muxihuayi.cn

Go:   // 手写 map[string][]T
来源：http://cf.colortex.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://yh.haigaiapp.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fa.huanxung.cn

[D20] 统计每个元素出现次数
来源：http://sb.szsharing.cn

Py:   Counter(arr)
来源：http://lh.bjjhwx.cn

PHP:  array_count_values($arr);
来源：http://dd.jctech888.com.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hh.yuexingan06.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lb.huixiangedu.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qb.bookmarksfly.cn

Go:   // 手写 map[T]int
来源：http://kn.nicolike.cn

Ruby: arr.tally
来源：http://ee.muxihuayi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://as.gzmigu.cn

[D21] 判断是否包含某元素
来源：http://ru.hahajie.cn

Py:   x in arr
来源：http://ss.huanxung.cn

PHP:  in_array($x, $arr, true);
来源：http://nd.haigaiapp.cn

JS:   arr.includes(x)
来源：http://qv.gzmigu.cn

TS:   arr.includes(x)
来源：http://go.hnjuh.cn

Java: list.contains(x)
来源：http://yt.szsharing.cn

Go:   slices.Contains(arr, x)
来源：http://qk.huanxung.cn

Ruby: arr.include?(x)
来源：http://nd.bjjhwx.cn

C#:   list.Contains(x)
来源：http://hq.shxzukj.cn

[D22] 复制数组（避免共享引用）
来源：http://wx.shxzskj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hs.shxzskj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://eb.colortex.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qx.wgjwhj.cn

TS:   [...arr];
来源：http://by.yuexingan06.cn

Java: new ArrayList<>(list);
来源：http://ie.muxihuayi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://qo.jctech888.com.cn

Ruby: arr.dup;  arr.clone
来源：http://uh.9csxet.cn

C#:   new List<int>(list);
来源：http://qf.hahajie.cn

[D23] reduce 累积计算
来源：http://km.jctech888.com.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zp.yuexingan06.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gt.chemitech.net.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tg.huixiangedu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mj.huixinmuqiang.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://at.newstarts.cn

Go:   // 手写循环
来源：http://cq.nicolike.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wy.9csxet.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ev.huanxung.cn

[D24] 字典 / Map 基本操作
来源：http://uc.yuntaijiaju.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qn.hahajie.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xt.jianghongdianzi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fn.chemitech.net.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://yl.muxihuayi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://px.szsharing.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rj.huixiangedu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rx.jctech888.com.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ah.huanxung.cn

[D25] Set 集合去重与交并差
来源：http://hd.yuntaijiaju.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fw.shtwfgs.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mn.huixinmuqiang.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://aj.chemitech.net.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bk.shxzukj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hy.hnjuh.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://fc.jctech888.com.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://fj.huixinmuqiang.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://us.521024.cn

[D26] 数组转字符串
来源：http://nw.hnjuh.cn

Py:   ", ".join(map(str, arr))
来源：http://na.lnxyls.cn

PHP:  implode(", ", $arr);
来源：http://sk.yuntaijiaju.cn

JS:   arr.join(", ")
来源：http://lx.shxzukj.cn

TS:   arr.join(", ")
来源：http://vz.hahajie.cn

Java: String.join(", ", list)
来源：http://hb.szsharing.cn

Go:   strings.Join(strs, ", ")
来源：http://mn.szxytkj.cn

Ruby: arr.join(", ")
来源：http://vh.gzmigu.cn

C#:   string.Join(", ", list)
来源：http://cg.lnxyls.cn

================================================================================
来源：http://py.nszjky.cn

E. 字符串处理
来源：http://ur.jianghongdianzi.cn

================================================================================
来源：http://af.bookmarksfly.cn

[E01] 拼接字符串
来源：http://sd.shxzskj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hm.jianghongdianzi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://cl.nszjky.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://cc.shxzskj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://lr.muxihuayi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://dz.shxzukj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dr.newstarts.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vv.huixiangedu.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://co.bookmarksfly.cn

[E02] 重复字符串
来源：http://bt.bjjhwx.cn

Py:   "ab" * 3
来源：http://gw.shtwfgs.cn

PHP:  str_repeat("ab", 3);
来源：http://aa.muxihuayi.cn

JS:   "ab".repeat(3)
来源：http://zv.szxytkj.cn

TS:   "ab".repeat(3)
来源：http://rt.huanxung.cn

Java: "ab".repeat(3)
来源：http://dx.yuntaijiaju.cn

Go:   strings.Repeat("ab", 3)
来源：http://zr.huixinmuqiang.cn

Ruby: "ab" * 3
来源：http://de.shxzskj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xz.szsharing.cn

[E03] 截取子串
来源：http://kd.shxzskj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rz.yuexingan06.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wq.panjiajie.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ox.colortex.cn

TS:   s.slice(1, 4)
来源：http://fa.bookmarksfly.cn

Java: s.substring(1, 4)
来源：http://dv.wgjwhj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rs.szsharing.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ic.szsharing.cn

C#:   s.Substring(1, 3)
来源：http://mr.szxytkj.cn

[E04] 查找子串位置
来源：http://gj.521024.cn

Py:   s.find("x");  s.index("x")
来源：http://gy.asd995.cn

PHP:  strpos($s, "x");
来源：http://gy.huixiangedu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://lf.muxihuayi.cn

TS:   s.indexOf("x")
来源：http://bk.gzmigu.cn

Java: s.indexOf("x")
来源：http://ix.jianghongdianzi.cn

Go:   strings.Index(s, "x")
来源：http://el.huixiangedu.cn

Ruby: s.index("x")
来源：http://an.muxihuayi.cn

C#:   s.IndexOf("x")
来源：http://jk.hahajie.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://tm.szsharing.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dt.asd995.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://en.gzmigu.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ow.gzmigu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://uo.nszjky.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cg.haigaiapp.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://oi.szxytkj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hw.yuexingan06.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://cd.lnxyls.cn

[E06] 替换子串
来源：http://az.huanxung.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ae.wgjwhj.cn

PHP:  str_replace("a", "b", $s);
来源：http://uq.9csxet.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qw.lnxyls.cn

TS:   s.replaceAll("a", "b")
来源：http://tg.huanxung.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://an.521024.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zy.lnxyls.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wm.newstarts.cn

C#:   s.Replace("a", "b")
来源：http://td.bookmarksfly.cn

[E07] 按分隔符拆分
来源：http://an.wgjwhj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fw.shxzskj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ya.panjiajie.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://zj.521024.cn

TS:   s.split(",")
来源：http://ap.bjjhwx.cn

Java: s.split(",");  s.split("\\s+")
来源：http://zh.chemitech.net.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fj.yuexingan06.cn

Ruby: s.split(",");  s.split
来源：http://om.huixiangedu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rf.hnjuh.cn

[E08] 数组按分隔符合并
来源：http://pj.panjiajie.cn

Py:   ",".join(items)
来源：http://tl.nszjky.cn

PHP:  implode(",", $items);
来源：http://ym.panjiajie.cn

JS:   items.join(",")
来源：http://ew.hnjuh.cn

TS:   items.join(",")
来源：http://cb.muxihuayi.cn

Java: String.join(",", items)
来源：http://aa.szsharing.cn

Go:   strings.Join(items, ",")
来源：http://vj.hnjuh.cn

Ruby: items.join(",")
来源：http://jw.lnxyls.cn

C#:   string.Join(",", items)
来源：http://en.newstarts.cn

[E09] 去除所有空白字符
来源：http://yi.bookmarksfly.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://yr.hahajie.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rm.muxihuayi.cn

JS:   s.replace(/\s+/g, "")
来源：http://gu.jctech888.com.cn

TS:   s.replace(/\s+/g, "")
来源：http://wz.yuexingan06.cn

Java: s.replaceAll("\\s+", "")
来源：http://wh.shxzskj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://tg.lnxyls.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ow.hahajie.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://iv.shxzskj.cn

[E10] 左侧补零 / 定长填充
来源：http://mq.huixinmuqiang.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ak.haigaiapp.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://nx.asd995.cn

JS:   "7".padStart(3, "0")
来源：http://ex.bjjhwx.cn

TS:   "7".padStart(3, "0")
来源：http://op.nicolike.cn

Java: String.format("%03d", 7)
来源：http://up.bjjhwx.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://by.521024.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://na.huixiangedu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hi.haigaiapp.cn

[E11] 反转字符串
来源：http://vp.muxihuayi.cn

Py:   s[::-1]
来源：http://fn.huixinmuqiang.cn

PHP:  strrev($s);
来源：http://za.shtwfgs.cn

JS:   [...s].reverse().join("")
来源：http://lc.shxzskj.cn

TS:   [...s].reverse().join("")
来源：http://tv.9csxet.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://qm.asd995.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://zf.shtwfgs.cn

Ruby: s.reverse
来源：http://or.haigaiapp.cn

C#:   new string(s.Reverse().ToArray())
来源：http://qm.chemitech.net.cn

[E12] 统计某字符出现次数
来源：http://xz.yuexingan06.cn

Py:   s.count("a")
来源：http://ti.shxzukj.cn

PHP:  substr_count($s, "a");
来源：http://ex.huixiangedu.cn

JS:   s.split("a").length - 1
来源：http://nn.muxihuayi.cn

TS:   s.split("a").length - 1
来源：http://jv.hnjuh.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ac.9csxet.cn

Go:   strings.Count(s, "a")
来源：http://fj.521024.cn

Ruby: s.count("a")
来源：http://hm.bjjhwx.cn

C#:   s.Count(c => c == 'a')
来源：http://vo.9csxet.cn

[E13] 逐字符遍历
来源：http://va.muxihuayi.cn

Py:   for ch in s: print(ch)
来源：http://rv.huanxung.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gp.hahajie.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ue.lnxyls.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://it.newstarts.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://tr.9csxet.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vp.lnxyls.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://gr.jianghongdianzi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ai.shxzukj.cn

[E14] URL 编码与 Base64
来源：http://xq.asd995.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ku.nszjky.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://tq.jianghongdianzi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vt.nicolike.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ea.szxytkj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ey.panjiajie.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qx.newstarts.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rq.shtwfgs.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qo.shxzukj.cn

[E15] HTML 转义 / 反转义
来源：http://zw.shxzukj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://nr.lnxyls.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://in.shxzskj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jf.gzmigu.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://cv.hnjuh.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gn.jctech888.com.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://yd.wgjwhj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mx.szsharing.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vp.9csxet.cn

[E16] 数字千分位
来源：http://pv.haigaiapp.cn

Py:   f"{1234567:,}"
来源：http://km.newstarts.cn

PHP:  number_format(1234567);
来源：http://tj.szsharing.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://mt.colortex.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://jb.hahajie.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mq.muxihuayi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jo.szxytkj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pw.9csxet.cn

C#:   1234567.ToString("N0")
来源：http://xx.chemitech.net.cn

[E17] 首字母大写
来源：http://xg.muxihuayi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cb.huixinmuqiang.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://vm.yuexingan06.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qd.colortex.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wr.wgjwhj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zg.lnxyls.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qq.yuexingan06.cn

Ruby: s.capitalize
来源：http://hx.bookmarksfly.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gu.huixiangedu.cn

[E18] 模板占位符替换
来源：http://dr.haigaiapp.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://in.hnjuh.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wk.hahajie.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://gh.bjjhwx.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ag.huanxung.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jv.szxytkj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ha.szsharing.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://tb.jianghongdianzi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bo.newstarts.cn

[E19] 多行文本按行拆分
来源：http://fr.shtwfgs.cn

Py:   s.splitlines()
来源：http://yw.chemitech.net.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://yj.yuexingan06.cn

JS:   s.split(/\r?\n/)
来源：http://eo.asd995.cn

TS:   s.split(/\r?\n/)
来源：http://wb.gzmigu.cn

Java: s.lines().toList()
来源：http://zb.asd995.cn

Go:   strings.Split(s, "\n")
来源：http://ip.asd995.cn

Ruby: s.lines
来源：http://qm.szxytkj.cn

C#:   s.Split('\n')
来源：http://zq.huixiangedu.cn

[E20] 判断字符串是否为空
来源：http://ek.nszjky.cn

Py:   if not s:
来源：http://wr.yuntaijiaju.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://nh.jianghongdianzi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://iy.muxihuayi.cn

TS:   if (s === "") {}
来源：http://lz.colortex.cn

Java: if (s.isEmpty()) {}
来源：http://kv.hnjuh.cn

Go:   if s == "" {}
来源：http://ur.wgjwhj.cn

Ruby: if s.empty?
来源：http://ei.huixiangedu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xa.521024.cn

[E21] 超长截断加省略号
来源：http://dw.panjiajie.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://gu.wgjwhj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://re.szxytkj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gd.9csxet.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bd.huanxung.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://kt.yuexingan06.cn

Go:   // 按 rune 判断长度后截断
来源：http://ws.asd995.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://pm.shxzskj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tb.huixiangedu.cn

[E22] 字节长度与字符长度
来源：http://dk.panjiajie.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pe.szxytkj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://af.yuexingan06.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://uq.huixiangedu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zq.521024.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mt.newstarts.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://eg.nicolike.cn

Ruby: s.bytesize;  s.length
来源：http://ne.chemitech.net.cn


<!-- 参考信息 -->