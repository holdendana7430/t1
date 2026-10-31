代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://vi.nszjky.cn

Go:   // 手写循环
来源：http://ns.panjiajie.cn

Ruby: arr.map { |x| x * 2 }
来源：http://aa.newstarts.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://pt.asd995.cn

[D15] 去重
来源：http://lj.haigaiapp.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nk.shtwfgs.cn

PHP:  array_unique($arr);
来源：http://ra.szxytkj.cn

JS:   [...new Set(arr)]
来源：http://gw.bookmarksfly.cn

TS:   [...new Set(arr)]
来源：http://yh.bookmarksfly.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jz.asd995.cn

Go:   // 用 map[T]struct{} 手写
来源：http://yu.shxzskj.cn

Ruby: arr.uniq
来源：http://gk.bjjhwx.cn

C#:   list.Distinct().ToList()
来源：http://to.muxihuayi.cn

[D16] 求和与平均值
来源：http://vn.huixiangedu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://on.shxzukj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jz.yuntaijiaju.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://pt.jctech888.com.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://cc.bookmarksfly.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://nl.chemitech.net.cn

Go:   // 手写循环累加
来源：http://xb.nicolike.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://go.nszjky.cn

C#:   list.Sum();  list.Average()
来源：http://wp.hnjuh.cn

[D17] 最大值与最小值
来源：http://it.shtwfgs.cn

Py:   max(arr);  min(arr)
来源：http://rk.yuntaijiaju.cn

PHP:  max($arr);  min($arr);
来源：http://xa.shxzskj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ko.szsharing.cn

TS:   Math.max(...arr);
来源：http://er.huanxung.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://op.shxzskj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hy.hnjuh.cn

Ruby: arr.max;  arr.min
来源：http://pe.bookmarksfly.cn

C#:   list.Max();  list.Min()
来源：http://pl.jctech888.com.cn

[D18] 扁平化嵌套数组
来源：http://ta.9csxet.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xv.hahajie.cn

PHP:  array_merge(...$nested);
来源：http://sk.shtwfgs.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://tl.bookmarksfly.cn

TS:   nested.flat();
来源：http://mx.9csxet.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rv.bookmarksfly.cn

Go:   // 手写双层循环
来源：http://bu.szsharing.cn

Ruby: nested.flatten
来源：http://bi.hahajie.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://hc.hnjuh.cn

[D19] 按字段分组
来源：http://mk.shxzukj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jp.yuexingan06.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wp.wgjwhj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ie.muxihuayi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ny.panjiajie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kx.lnxyls.cn

Go:   // 手写 map[string][]T
来源：http://qc.wgjwhj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://cb.jctech888.com.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nc.haigaiapp.cn

[D20] 统计每个元素出现次数
来源：http://vx.huanxung.cn

Py:   Counter(arr)
来源：http://ia.9csxet.cn

PHP:  array_count_values($arr);
来源：http://kn.nszjky.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ep.yuntaijiaju.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ru.newstarts.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://nd.521024.cn

Go:   // 手写 map[T]int
来源：http://eo.nicolike.cn

Ruby: arr.tally
来源：http://gb.lnxyls.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lo.newstarts.cn

[D21] 判断是否包含某元素
来源：http://od.shtwfgs.cn

Py:   x in arr
来源：http://yp.lnxyls.cn

PHP:  in_array($x, $arr, true);
来源：http://jz.jianghongdianzi.cn

JS:   arr.includes(x)
来源：http://fn.panjiajie.cn

TS:   arr.includes(x)
来源：http://dx.lnxyls.cn

Java: list.contains(x)
来源：http://fg.bjjhwx.cn

Go:   slices.Contains(arr, x)
来源：http://mk.huixinmuqiang.cn

Ruby: arr.include?(x)
来源：http://ia.nicolike.cn

C#:   list.Contains(x)
来源：http://uk.szsharing.cn

[D22] 复制数组（避免共享引用）
来源：http://np.shxzukj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://uy.haigaiapp.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cy.chemitech.net.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gy.shxzskj.cn

TS:   [...arr];
来源：http://az.lnxyls.cn

Java: new ArrayList<>(list);
来源：http://re.jctech888.com.cn

Go:   copied := append([]int(nil), arr...)
来源：http://bo.bjjhwx.cn

Ruby: arr.dup;  arr.clone
来源：http://hh.nszjky.cn

C#:   new List<int>(list);
来源：http://qs.shxzukj.cn

[D23] reduce 累积计算
来源：http://hl.huixinmuqiang.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://do.muxihuayi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ov.nszjky.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yu.shtwfgs.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qp.asd995.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://xg.huanxung.cn

Go:   // 手写循环
来源：http://mf.huanxung.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://tv.lnxyls.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://as.haigaiapp.cn

[D24] 字典 / Map 基本操作
来源：http://gr.shxzskj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jx.shxzukj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hi.shxzukj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://nj.muxihuayi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://tl.haigaiapp.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wy.jianghongdianzi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xo.bjjhwx.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hb.panjiajie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://av.muxihuayi.cn

[D25] Set 集合去重与交并差
来源：http://lw.colortex.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zl.haigaiapp.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zk.huanxung.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://os.jctech888.com.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ml.bookmarksfly.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ue.asd995.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://cu.chemitech.net.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zw.colortex.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://al.lnxyls.cn

[D26] 数组转字符串
来源：http://yh.yuntaijiaju.cn

Py:   ", ".join(map(str, arr))
来源：http://st.huixinmuqiang.cn

PHP:  implode(", ", $arr);
来源：http://qa.nszjky.cn

JS:   arr.join(", ")
来源：http://rr.bjjhwx.cn

TS:   arr.join(", ")
来源：http://ww.521024.cn

Java: String.join(", ", list)
来源：http://zf.521024.cn

Go:   strings.Join(strs, ", ")
来源：http://aj.nszjky.cn

Ruby: arr.join(", ")
来源：http://gt.shxzukj.cn

C#:   string.Join(", ", list)
来源：http://tm.nszjky.cn

================================================================================
来源：http://pl.bjjhwx.cn

E. 字符串处理
来源：http://xb.nszjky.cn

================================================================================
来源：http://st.chemitech.net.cn

[E01] 拼接字符串
来源：http://so.chemitech.net.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mv.szsharing.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dw.yuexingan06.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://pr.huanxung.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wq.panjiajie.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wd.shxzskj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://cp.jctech888.com.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ro.newstarts.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ep.jianghongdianzi.cn

[E02] 重复字符串
来源：http://kq.szxytkj.cn

Py:   "ab" * 3
来源：http://wr.yuntaijiaju.cn

PHP:  str_repeat("ab", 3);
来源：http://ej.asd995.cn

JS:   "ab".repeat(3)
来源：http://rx.yuntaijiaju.cn

TS:   "ab".repeat(3)
来源：http://re.szxytkj.cn

Java: "ab".repeat(3)
来源：http://db.panjiajie.cn

Go:   strings.Repeat("ab", 3)
来源：http://lv.wgjwhj.cn

Ruby: "ab" * 3
来源：http://sb.szsharing.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://bp.chemitech.net.cn

[E03] 截取子串
来源：http://he.shxzskj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://se.asd995.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://oh.bjjhwx.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gh.szxytkj.cn

TS:   s.slice(1, 4)
来源：http://fd.asd995.cn

Java: s.substring(1, 4)
来源：http://mq.yuntaijiaju.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://do.panjiajie.cn

Ruby: s[1, 3];  s[1..3]
来源：http://tq.szsharing.cn

C#:   s.Substring(1, 3)
来源：http://cu.shxzskj.cn

[E04] 查找子串位置
来源：http://jw.chemitech.net.cn

Py:   s.find("x");  s.index("x")
来源：http://fj.hnjuh.cn

PHP:  strpos($s, "x");
来源：http://nl.panjiajie.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://pf.asd995.cn

TS:   s.indexOf("x")
来源：http://kd.bookmarksfly.cn

Java: s.indexOf("x")
来源：http://zz.shxzskj.cn

Go:   strings.Index(s, "x")
来源：http://ah.asd995.cn

Ruby: s.index("x")
来源：http://ad.newstarts.cn

C#:   s.IndexOf("x")
来源：http://bj.wgjwhj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://rh.szsharing.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://po.521024.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kn.bjjhwx.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zw.szsharing.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://mo.nicolike.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ir.9csxet.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ut.hnjuh.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tu.jianghongdianzi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://co.jianghongdianzi.cn

[E06] 替换子串
来源：http://zw.jctech888.com.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://tz.newstarts.cn

PHP:  str_replace("a", "b", $s);
来源：http://vl.shxzukj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://um.lnxyls.cn

TS:   s.replaceAll("a", "b")
来源：http://mf.gzmigu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xa.521024.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jb.yuexingan06.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kw.yuntaijiaju.cn

C#:   s.Replace("a", "b")
来源：http://up.bjjhwx.cn

[E07] 按分隔符拆分
来源：http://tg.szsharing.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zs.hahajie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zw.muxihuayi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://jg.wgjwhj.cn

TS:   s.split(",")
来源：http://wq.panjiajie.cn

Java: s.split(",");  s.split("\\s+")
来源：http://lj.shxzskj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://cq.szxytkj.cn

Ruby: s.split(",");  s.split
来源：http://ck.haigaiapp.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://oa.jctech888.com.cn

[E08] 数组按分隔符合并
来源：http://hc.hnjuh.cn

Py:   ",".join(items)
来源：http://lv.colortex.cn

PHP:  implode(",", $items);
来源：http://sj.huanxung.cn

JS:   items.join(",")
来源：http://ve.bookmarksfly.cn

TS:   items.join(",")
来源：http://rj.shxzskj.cn

Java: String.join(",", items)
来源：http://lw.jianghongdianzi.cn

Go:   strings.Join(items, ",")
来源：http://xo.gzmigu.cn

Ruby: items.join(",")
来源：http://ut.bjjhwx.cn

C#:   string.Join(",", items)
来源：http://at.nszjky.cn

[E09] 去除所有空白字符
来源：http://ew.nicolike.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ph.asd995.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ko.bjjhwx.cn

JS:   s.replace(/\s+/g, "")
来源：http://tv.panjiajie.cn

TS:   s.replace(/\s+/g, "")
来源：http://lm.panjiajie.cn

Java: s.replaceAll("\\s+", "")
来源：http://mw.hnjuh.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://dm.wgjwhj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://qd.yuntaijiaju.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xl.hahajie.cn

[E10] 左侧补零 / 定长填充
来源：http://fk.yuexingan06.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kw.asd995.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xn.muxihuayi.cn

JS:   "7".padStart(3, "0")
来源：http://hn.chemitech.net.cn

TS:   "7".padStart(3, "0")
来源：http://lz.bookmarksfly.cn

Java: String.format("%03d", 7)
来源：http://je.colortex.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ts.colortex.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://tm.bjjhwx.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bf.shxzukj.cn

[E11] 反转字符串
来源：http://tt.huixinmuqiang.cn

Py:   s[::-1]
来源：http://xh.521024.cn

PHP:  strrev($s);
来源：http://ee.yuexingan06.cn

JS:   [...s].reverse().join("")
来源：http://yz.colortex.cn

TS:   [...s].reverse().join("")
来源：http://zb.521024.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://pm.bjjhwx.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ip.bookmarksfly.cn

Ruby: s.reverse
来源：http://pr.521024.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ga.bookmarksfly.cn

[E12] 统计某字符出现次数
来源：http://sm.lnxyls.cn

Py:   s.count("a")
来源：http://ew.hahajie.cn

PHP:  substr_count($s, "a");
来源：http://hd.asd995.cn

JS:   s.split("a").length - 1
来源：http://cf.nicolike.cn

TS:   s.split("a").length - 1
来源：http://xl.huanxung.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rp.chemitech.net.cn

Go:   strings.Count(s, "a")
来源：http://uh.shxzukj.cn

Ruby: s.count("a")
来源：http://mo.chemitech.net.cn

C#:   s.Count(c => c == 'a')
来源：http://of.huixinmuqiang.cn

[E13] 逐字符遍历
来源：http://um.chemitech.net.cn

Py:   for ch in s: print(ch)
来源：http://yx.hahajie.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://iv.lnxyls.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://cf.szxytkj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://br.bookmarksfly.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://di.huixiangedu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fs.wgjwhj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://om.huanxung.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://nq.huixiangedu.cn

[E14] URL 编码与 Base64
来源：http://pm.9csxet.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kg.shtwfgs.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ws.yuntaijiaju.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kp.gzmigu.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://yn.jianghongdianzi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wv.jianghongdianzi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fv.panjiajie.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ie.panjiajie.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ni.yuexingan06.cn

[E15] HTML 转义 / 反转义
来源：http://fq.yuexingan06.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://lt.colortex.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ud.bookmarksfly.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hc.shxzukj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://kc.haigaiapp.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vc.huanxung.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ma.shxzukj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bd.huixiangedu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jl.521024.cn

[E16] 数字千分位
来源：http://dx.gzmigu.cn

Py:   f"{1234567:,}"
来源：http://vq.jctech888.com.cn

PHP:  number_format(1234567);
来源：http://bm.szsharing.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://rf.bookmarksfly.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://jd.nicolike.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://he.haigaiapp.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rp.muxihuayi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zt.panjiajie.cn

C#:   1234567.ToString("N0")
来源：http://xw.jianghongdianzi.cn

[E17] 首字母大写
来源：http://nt.wgjwhj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vs.hnjuh.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://wa.colortex.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rx.wgjwhj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xj.jianghongdianzi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kr.bookmarksfly.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://km.nszjky.cn

Ruby: s.capitalize
来源：http://gx.hnjuh.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zq.huanxung.cn

[E18] 模板占位符替换
来源：http://zo.bjjhwx.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kv.nicolike.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://sb.hnjuh.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://eq.shxzskj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://hf.nicolike.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://as.shxzukj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ka.yuntaijiaju.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://az.colortex.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wz.huixinmuqiang.cn

[E19] 多行文本按行拆分
来源：http://kv.gzmigu.cn

Py:   s.splitlines()
来源：http://ox.shtwfgs.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ae.haigaiapp.cn

JS:   s.split(/\r?\n/)
来源：http://my.huanxung.cn

TS:   s.split(/\r?\n/)
来源：http://va.panjiajie.cn

Java: s.lines().toList()
来源：http://kk.huanxung.cn

Go:   strings.Split(s, "\n")
来源：http://ta.nicolike.cn

Ruby: s.lines
来源：http://jy.asd995.cn

C#:   s.Split('\n')
来源：http://uc.newstarts.cn

[E20] 判断字符串是否为空
来源：http://xt.huixiangedu.cn

Py:   if not s:
来源：http://ru.muxihuayi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://kb.hahajie.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tw.yuexingan06.cn

TS:   if (s === "") {}
来源：http://up.chemitech.net.cn

Java: if (s.isEmpty()) {}
来源：http://zp.lnxyls.cn

Go:   if s == "" {}
来源：http://ju.panjiajie.cn

Ruby: if s.empty?
来源：http://xu.asd995.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://br.yuntaijiaju.cn

[E21] 超长截断加省略号
来源：http://dv.yuntaijiaju.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://al.yuntaijiaju.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://po.huixinmuqiang.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://no.yuntaijiaju.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yw.szsharing.cn


<!-- 参考信息 -->