代发 wailian999

[D15] 去重
来源：http://nl.9csxet.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://av.haigaiapp.cn

PHP:  array_unique($arr);
来源：http://un.wgjwhj.cn

JS:   [...new Set(arr)]
来源：http://dg.newstarts.cn

TS:   [...new Set(arr)]
来源：http://dt.yuntaijiaju.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kx.muxihuayi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://av.nicolike.cn

Ruby: arr.uniq
来源：http://co.lnxyls.cn

C#:   list.Distinct().ToList()
来源：http://js.jctech888.com.cn

[D16] 求和与平均值
来源：http://yn.9csxet.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bd.hnjuh.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bj.hnjuh.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://cy.bookmarksfly.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hl.bookmarksfly.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://su.huixinmuqiang.cn

Go:   // 手写循环累加
来源：http://iw.haigaiapp.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xh.huanxung.cn

C#:   list.Sum();  list.Average()
来源：http://nq.asd995.cn

[D17] 最大值与最小值
来源：http://dg.jctech888.com.cn

Py:   max(arr);  min(arr)
来源：http://fa.nicolike.cn

PHP:  max($arr);  min($arr);
来源：http://sx.bookmarksfly.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hy.huanxung.cn

TS:   Math.max(...arr);
来源：http://fd.jctech888.com.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ea.9csxet.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xf.hahajie.cn

Ruby: arr.max;  arr.min
来源：http://pn.shtwfgs.cn

C#:   list.Max();  list.Min()
来源：http://ou.nicolike.cn

[D18] 扁平化嵌套数组
来源：http://sj.yuexingan06.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://yr.shxzukj.cn

PHP:  array_merge(...$nested);
来源：http://uj.bookmarksfly.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://lm.szsharing.cn

TS:   nested.flat();
来源：http://is.szxytkj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hn.9csxet.cn

Go:   // 手写双层循环
来源：http://xg.huanxung.cn

Ruby: nested.flatten
来源：http://uf.colortex.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://kp.nicolike.cn

[D19] 按字段分组
来源：http://gz.muxihuayi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rc.shxzskj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wp.shxzskj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://zu.nicolike.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://qw.shtwfgs.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gs.wgjwhj.cn

Go:   // 手写 map[string][]T
来源：http://ql.shxzskj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://iu.9csxet.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gv.nicolike.cn

[D20] 统计每个元素出现次数
来源：http://ui.haigaiapp.cn

Py:   Counter(arr)
来源：http://ly.yuntaijiaju.cn

PHP:  array_count_values($arr);
来源：http://lm.panjiajie.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cc.bjjhwx.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://em.shxzukj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ke.szsharing.cn

Go:   // 手写 map[T]int
来源：http://ka.521024.cn

Ruby: arr.tally
来源：http://lq.9csxet.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tn.gzmigu.cn

[D21] 判断是否包含某元素
来源：http://hv.newstarts.cn

Py:   x in arr
来源：http://xe.hahajie.cn

PHP:  in_array($x, $arr, true);
来源：http://hp.lnxyls.cn

JS:   arr.includes(x)
来源：http://zk.hnjuh.cn

TS:   arr.includes(x)
来源：http://yr.shxzukj.cn

Java: list.contains(x)
来源：http://sy.chemitech.net.cn

Go:   slices.Contains(arr, x)
来源：http://lq.shxzukj.cn

Ruby: arr.include?(x)
来源：http://wj.yuexingan06.cn

C#:   list.Contains(x)
来源：http://bj.bookmarksfly.cn

[D22] 复制数组（避免共享引用）
来源：http://sk.huixiangedu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pu.chemitech.net.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ax.nszjky.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://oc.huanxung.cn

TS:   [...arr];
来源：http://tv.wgjwhj.cn

Java: new ArrayList<>(list);
来源：http://cn.muxihuayi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://rq.yuntaijiaju.cn

Ruby: arr.dup;  arr.clone
来源：http://yc.lnxyls.cn

C#:   new List<int>(list);
来源：http://oi.huixinmuqiang.cn

[D23] reduce 累积计算
来源：http://sy.shxzskj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vz.bjjhwx.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://oo.yuexingan06.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lb.panjiajie.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sm.nicolike.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://uv.newstarts.cn

Go:   // 手写循环
来源：http://tb.huixiangedu.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://il.szxytkj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mf.panjiajie.cn

[D24] 字典 / Map 基本操作
来源：http://wx.9csxet.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://lk.bookmarksfly.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ru.huixiangedu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://iz.gzmigu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://uq.yuntaijiaju.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rr.panjiajie.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://iq.asd995.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://oz.nszjky.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gm.521024.cn

[D25] Set 集合去重与交并差
来源：http://xg.jianghongdianzi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ez.nszjky.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fp.jianghongdianzi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://sq.lnxyls.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ou.nicolike.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hj.muxihuayi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ba.wgjwhj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pe.gzmigu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://sj.shtwfgs.cn

[D26] 数组转字符串
来源：http://gy.muxihuayi.cn

Py:   ", ".join(map(str, arr))
来源：http://vq.shxzskj.cn

PHP:  implode(", ", $arr);
来源：http://dc.jctech888.com.cn

JS:   arr.join(", ")
来源：http://zt.shtwfgs.cn

TS:   arr.join(", ")
来源：http://xo.bjjhwx.cn

Java: String.join(", ", list)
来源：http://sm.panjiajie.cn

Go:   strings.Join(strs, ", ")
来源：http://mo.9csxet.cn

Ruby: arr.join(", ")
来源：http://ge.asd995.cn

C#:   string.Join(", ", list)
来源：http://dq.hnjuh.cn

================================================================================
来源：http://jk.shtwfgs.cn

E. 字符串处理
来源：http://vm.huanxung.cn

================================================================================
来源：http://aj.521024.cn

[E01] 拼接字符串
来源：http://yw.nicolike.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://it.nszjky.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rz.panjiajie.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://pm.jctech888.com.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://lv.nicolike.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ex.bjjhwx.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vl.shxzskj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hh.shxzukj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ws.lnxyls.cn

[E02] 重复字符串
来源：http://fc.bjjhwx.cn

Py:   "ab" * 3
来源：http://rx.asd995.cn

PHP:  str_repeat("ab", 3);
来源：http://en.yuntaijiaju.cn

JS:   "ab".repeat(3)
来源：http://dm.huanxung.cn

TS:   "ab".repeat(3)
来源：http://mb.yuexingan06.cn

Java: "ab".repeat(3)
来源：http://qf.yuexingan06.cn

Go:   strings.Repeat("ab", 3)
来源：http://wg.haigaiapp.cn

Ruby: "ab" * 3
来源：http://hd.asd995.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ea.bookmarksfly.cn

[E03] 截取子串
来源：http://my.hnjuh.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rp.jianghongdianzi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ns.jianghongdianzi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://se.panjiajie.cn

TS:   s.slice(1, 4)
来源：http://ys.521024.cn

Java: s.substring(1, 4)
来源：http://wf.521024.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://cl.bookmarksfly.cn

Ruby: s[1, 3];  s[1..3]
来源：http://cc.newstarts.cn

C#:   s.Substring(1, 3)
来源：http://cx.jctech888.com.cn

[E04] 查找子串位置
来源：http://zy.yuexingan06.cn

Py:   s.find("x");  s.index("x")
来源：http://ae.colortex.cn

PHP:  strpos($s, "x");
来源：http://gz.haigaiapp.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://su.bjjhwx.cn

TS:   s.indexOf("x")
来源：http://ep.szxytkj.cn

Java: s.indexOf("x")
来源：http://nf.bookmarksfly.cn

Go:   strings.Index(s, "x")
来源：http://ph.jctech888.com.cn

Ruby: s.index("x")
来源：http://lo.hahajie.cn

C#:   s.IndexOf("x")
来源：http://bz.newstarts.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://bm.shxzskj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://bw.521024.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qt.bjjhwx.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bu.yuntaijiaju.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://zg.asd995.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ii.9csxet.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fk.bookmarksfly.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://kh.shtwfgs.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ty.nicolike.cn

[E06] 替换子串
来源：http://ge.haigaiapp.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xn.szsharing.cn

PHP:  str_replace("a", "b", $s);
来源：http://lb.9csxet.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yj.bookmarksfly.cn

TS:   s.replaceAll("a", "b")
来源：http://pd.asd995.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qr.muxihuayi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mj.chemitech.net.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xi.yuntaijiaju.cn

C#:   s.Replace("a", "b")
来源：http://hp.szsharing.cn

[E07] 按分隔符拆分
来源：http://wb.bookmarksfly.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xx.521024.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ky.panjiajie.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://bb.shtwfgs.cn

TS:   s.split(",")
来源：http://wh.colortex.cn

Java: s.split(",");  s.split("\\s+")
来源：http://tw.huixiangedu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tk.asd995.cn

Ruby: s.split(",");  s.split
来源：http://yt.bjjhwx.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yf.jianghongdianzi.cn

[E08] 数组按分隔符合并
来源：http://li.huixiangedu.cn

Py:   ",".join(items)
来源：http://uw.haigaiapp.cn

PHP:  implode(",", $items);
来源：http://eb.bookmarksfly.cn

JS:   items.join(",")
来源：http://ws.yuexingan06.cn

TS:   items.join(",")
来源：http://bo.9csxet.cn

Java: String.join(",", items)
来源：http://ep.nszjky.cn

Go:   strings.Join(items, ",")
来源：http://vz.bjjhwx.cn

Ruby: items.join(",")
来源：http://kk.9csxet.cn

C#:   string.Join(",", items)
来源：http://kk.lnxyls.cn

[E09] 去除所有空白字符
来源：http://on.lnxyls.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ph.lnxyls.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qo.521024.cn

JS:   s.replace(/\s+/g, "")
来源：http://vu.szxytkj.cn

TS:   s.replace(/\s+/g, "")
来源：http://zx.asd995.cn

Java: s.replaceAll("\\s+", "")
来源：http://gy.hahajie.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ci.jctech888.com.cn

Ruby: s.gsub(/\s+/, "")
来源：http://xx.shxzskj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://nh.9csxet.cn

[E10] 左侧补零 / 定长填充
来源：http://ms.shtwfgs.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://st.hahajie.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xr.521024.cn

JS:   "7".padStart(3, "0")
来源：http://xi.9csxet.cn

TS:   "7".padStart(3, "0")
来源：http://jo.haigaiapp.cn

Java: String.format("%03d", 7)
来源：http://gt.huixinmuqiang.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://nd.yuntaijiaju.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xe.521024.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://oy.lnxyls.cn

[E11] 反转字符串
来源：http://ez.bookmarksfly.cn

Py:   s[::-1]
来源：http://wd.huanxung.cn

PHP:  strrev($s);
来源：http://rz.huanxung.cn

JS:   [...s].reverse().join("")
来源：http://hr.521024.cn

TS:   [...s].reverse().join("")
来源：http://uf.muxihuayi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://yd.nszjky.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ds.nszjky.cn

Ruby: s.reverse
来源：http://ca.szxytkj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://he.521024.cn

[E12] 统计某字符出现次数
来源：http://pu.jianghongdianzi.cn

Py:   s.count("a")
来源：http://zd.szxytkj.cn

PHP:  substr_count($s, "a");
来源：http://rs.shxzskj.cn

JS:   s.split("a").length - 1
来源：http://qx.gzmigu.cn

TS:   s.split("a").length - 1
来源：http://km.asd995.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kv.hnjuh.cn

Go:   strings.Count(s, "a")
来源：http://sv.lnxyls.cn

Ruby: s.count("a")
来源：http://sv.haigaiapp.cn

C#:   s.Count(c => c == 'a')
来源：http://lo.521024.cn

[E13] 逐字符遍历
来源：http://ch.yuntaijiaju.cn

Py:   for ch in s: print(ch)
来源：http://eu.gzmigu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jg.huanxung.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://vl.yuexingan06.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://gh.panjiajie.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rq.huanxung.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://sb.szxytkj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://xj.9csxet.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gh.asd995.cn

[E14] URL 编码与 Base64
来源：http://ha.hnjuh.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://sz.hnjuh.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://uj.jianghongdianzi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ad.9csxet.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ot.haigaiapp.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kw.521024.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ue.jianghongdianzi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://pk.colortex.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vh.wgjwhj.cn

[E15] HTML 转义 / 反转义
来源：http://un.wgjwhj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://tx.521024.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gg.wgjwhj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rt.jctech888.com.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://pm.lnxyls.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://sn.huanxung.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rw.nszjky.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pl.shtwfgs.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://el.szsharing.cn

[E16] 数字千分位
来源：http://ub.hnjuh.cn

Py:   f"{1234567:,}"
来源：http://fr.szxytkj.cn

PHP:  number_format(1234567);
来源：http://cv.huixiangedu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://mx.bookmarksfly.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://tt.nszjky.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://oy.szxytkj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xh.huixiangedu.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dz.9csxet.cn

C#:   1234567.ToString("N0")
来源：http://ct.nszjky.cn

[E17] 首字母大写
来源：http://ao.lnxyls.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bm.panjiajie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ow.muxihuayi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mz.lnxyls.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wb.yuntaijiaju.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nu.muxihuayi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wm.lnxyls.cn

Ruby: s.capitalize
来源：http://js.newstarts.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://kt.jctech888.com.cn

[E18] 模板占位符替换
来源：http://an.jianghongdianzi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xk.newstarts.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ve.jctech888.com.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ht.muxihuayi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://bb.lnxyls.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wk.panjiajie.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hf.muxihuayi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kl.yuexingan06.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yx.shxzskj.cn

[E19] 多行文本按行拆分
来源：http://yz.bjjhwx.cn

Py:   s.splitlines()
来源：http://cd.shxzukj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qh.haigaiapp.cn

JS:   s.split(/\r?\n/)
来源：http://tb.panjiajie.cn

TS:   s.split(/\r?\n/)
来源：http://zj.panjiajie.cn

Java: s.lines().toList()
来源：http://hi.lnxyls.cn

Go:   strings.Split(s, "\n")
来源：http://vw.haigaiapp.cn

Ruby: s.lines
来源：http://mi.panjiajie.cn

C#:   s.Split('\n')
来源：http://mc.hnjuh.cn

[E20] 判断字符串是否为空
来源：http://mk.szsharing.cn

Py:   if not s:
来源：http://ob.9csxet.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bm.muxihuayi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fr.gzmigu.cn

TS:   if (s === "") {}
来源：http://os.bjjhwx.cn

Java: if (s.isEmpty()) {}
来源：http://vl.newstarts.cn

Go:   if s == "" {}
来源：http://zi.nicolike.cn

Ruby: if s.empty?
来源：http://nz.szxytkj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ij.huixiangedu.cn

[E21] 超长截断加省略号
来源：http://yd.hahajie.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hy.nicolike.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qc.asd995.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hu.nszjky.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sl.muxihuayi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rb.huixinmuqiang.cn

Go:   // 按 rune 判断长度后截断
来源：http://fc.jctech888.com.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lu.panjiajie.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://em.haigaiapp.cn


<!-- 参考信息 -->