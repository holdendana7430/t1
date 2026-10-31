代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://xy.hnjuh.cn

Go:   // 手写循环
来源：http://ha.hnjuh.cn

Ruby: arr.map { |x| x * 2 }
来源：http://by.lnxyls.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ab.chemitech.net.cn

[D15] 去重
来源：http://id.jctech888.com.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ro.yuexingan06.cn

PHP:  array_unique($arr);
来源：http://mt.yuexingan06.cn

JS:   [...new Set(arr)]
来源：http://nb.hnjuh.cn

TS:   [...new Set(arr)]
来源：http://ws.shxzukj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ho.szxytkj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://hr.muxihuayi.cn

Ruby: arr.uniq
来源：http://ud.shxzukj.cn

C#:   list.Distinct().ToList()
来源：http://fn.jianghongdianzi.cn

[D16] 求和与平均值
来源：http://ua.huixinmuqiang.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://em.newstarts.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fg.shtwfgs.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qy.lnxyls.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://js.huixiangedu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://kt.bjjhwx.cn

Go:   // 手写循环累加
来源：http://pj.asd995.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vc.szxytkj.cn

C#:   list.Sum();  list.Average()
来源：http://xd.lnxyls.cn

[D17] 最大值与最小值
来源：http://uj.colortex.cn

Py:   max(arr);  min(arr)
来源：http://mr.muxihuayi.cn

PHP:  max($arr);  min($arr);
来源：http://uh.521024.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://yy.newstarts.cn

TS:   Math.max(...arr);
来源：http://mi.jianghongdianzi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://oj.yuexingan06.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ne.jianghongdianzi.cn

Ruby: arr.max;  arr.min
来源：http://yf.hahajie.cn

C#:   list.Max();  list.Min()
来源：http://nd.yuntaijiaju.cn

[D18] 扁平化嵌套数组
来源：http://pl.shtwfgs.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://cl.bookmarksfly.cn

PHP:  array_merge(...$nested);
来源：http://am.nszjky.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ls.chemitech.net.cn

TS:   nested.flat();
来源：http://ca.asd995.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zu.shxzskj.cn

Go:   // 手写双层循环
来源：http://vm.huixiangedu.cn

Ruby: nested.flatten
来源：http://fb.jianghongdianzi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ow.szxytkj.cn

[D19] 按字段分组
来源：http://ay.muxihuayi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jv.hahajie.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xl.huixinmuqiang.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lk.asd995.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://sj.bookmarksfly.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wi.szxytkj.cn

Go:   // 手写 map[string][]T
来源：http://sv.szxytkj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://mh.szxytkj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dj.jctech888.com.cn

[D20] 统计每个元素出现次数
来源：http://te.szsharing.cn

Py:   Counter(arr)
来源：http://yb.szxytkj.cn

PHP:  array_count_values($arr);
来源：http://zl.nicolike.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zd.hnjuh.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://st.panjiajie.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bi.bookmarksfly.cn

Go:   // 手写 map[T]int
来源：http://ii.shxzukj.cn

Ruby: arr.tally
来源：http://tv.bookmarksfly.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ru.bookmarksfly.cn

[D21] 判断是否包含某元素
来源：http://zt.yuntaijiaju.cn

Py:   x in arr
来源：http://fp.panjiajie.cn

PHP:  in_array($x, $arr, true);
来源：http://os.hahajie.cn

JS:   arr.includes(x)
来源：http://os.yuexingan06.cn

TS:   arr.includes(x)
来源：http://oa.gzmigu.cn

Java: list.contains(x)
来源：http://ls.yuexingan06.cn

Go:   slices.Contains(arr, x)
来源：http://le.hahajie.cn

Ruby: arr.include?(x)
来源：http://ol.colortex.cn

C#:   list.Contains(x)
来源：http://hb.9csxet.cn

[D22] 复制数组（避免共享引用）
来源：http://dw.asd995.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mm.asd995.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cv.muxihuayi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://uc.shxzukj.cn

TS:   [...arr];
来源：http://so.521024.cn

Java: new ArrayList<>(list);
来源：http://wo.panjiajie.cn

Go:   copied := append([]int(nil), arr...)
来源：http://mm.muxihuayi.cn

Ruby: arr.dup;  arr.clone
来源：http://ac.shxzskj.cn

C#:   new List<int>(list);
来源：http://ez.lnxyls.cn

[D23] reduce 累积计算
来源：http://jb.szxytkj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gh.hnjuh.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://yt.colortex.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mv.huixinmuqiang.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pw.huanxung.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://st.521024.cn

Go:   // 手写循环
来源：http://vz.9csxet.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ru.huixiangedu.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://fw.huanxung.cn

[D24] 字典 / Map 基本操作
来源：http://kd.yuexingan06.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qy.wgjwhj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zf.nszjky.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fm.9csxet.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://yj.gzmigu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gu.wgjwhj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ox.panjiajie.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ca.shxzukj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rf.colortex.cn

[D25] Set 集合去重与交并差
来源：http://dq.szxytkj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zj.wgjwhj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://sj.shxzskj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qn.huanxung.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qe.haigaiapp.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ne.yuntaijiaju.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rm.muxihuayi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ld.wgjwhj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wg.szsharing.cn

[D26] 数组转字符串
来源：http://xh.muxihuayi.cn

Py:   ", ".join(map(str, arr))
来源：http://eb.muxihuayi.cn

PHP:  implode(", ", $arr);
来源：http://bx.hnjuh.cn

JS:   arr.join(", ")
来源：http://iw.huanxung.cn

TS:   arr.join(", ")
来源：http://xc.huixinmuqiang.cn

Java: String.join(", ", list)
来源：http://ez.huixiangedu.cn

Go:   strings.Join(strs, ", ")
来源：http://vt.nszjky.cn

Ruby: arr.join(", ")
来源：http://as.asd995.cn

C#:   string.Join(", ", list)
来源：http://mv.bjjhwx.cn

================================================================================
来源：http://al.huixiangedu.cn

E. 字符串处理
来源：http://zj.gzmigu.cn

================================================================================
来源：http://oa.huixiangedu.cn

[E01] 拼接字符串
来源：http://qp.asd995.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://nv.nszjky.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://da.shtwfgs.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://pl.bjjhwx.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://sc.muxihuayi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wh.bjjhwx.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hc.szsharing.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rv.shtwfgs.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ej.muxihuayi.cn

[E02] 重复字符串
来源：http://ls.bookmarksfly.cn

Py:   "ab" * 3
来源：http://ch.chemitech.net.cn

PHP:  str_repeat("ab", 3);
来源：http://tq.haigaiapp.cn

JS:   "ab".repeat(3)
来源：http://jt.nicolike.cn

TS:   "ab".repeat(3)
来源：http://vp.huixinmuqiang.cn

Java: "ab".repeat(3)
来源：http://ub.jianghongdianzi.cn

Go:   strings.Repeat("ab", 3)
来源：http://dt.wgjwhj.cn

Ruby: "ab" * 3
来源：http://jy.szxytkj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ze.9csxet.cn

[E03] 截取子串
来源：http://ly.shxzukj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vs.szsharing.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hl.bookmarksfly.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lg.jianghongdianzi.cn

TS:   s.slice(1, 4)
来源：http://ri.newstarts.cn

Java: s.substring(1, 4)
来源：http://bk.muxihuayi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://td.yuexingan06.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ej.wgjwhj.cn

C#:   s.Substring(1, 3)
来源：http://nt.muxihuayi.cn

[E04] 查找子串位置
来源：http://jc.colortex.cn

Py:   s.find("x");  s.index("x")
来源：http://ym.521024.cn

PHP:  strpos($s, "x");
来源：http://td.huanxung.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kb.szxytkj.cn

TS:   s.indexOf("x")
来源：http://tw.yuntaijiaju.cn

Java: s.indexOf("x")
来源：http://kl.szxytkj.cn

Go:   strings.Index(s, "x")
来源：http://uq.colortex.cn

Ruby: s.index("x")
来源：http://ht.yuexingan06.cn

C#:   s.IndexOf("x")
来源：http://qp.yuntaijiaju.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://bs.asd995.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ip.colortex.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ru.shxzskj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ny.shxzukj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ll.jianghongdianzi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://da.colortex.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://yb.asd995.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://py.nszjky.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ym.huixiangedu.cn

[E06] 替换子串
来源：http://uh.521024.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zf.chemitech.net.cn

PHP:  str_replace("a", "b", $s);
来源：http://pq.jctech888.com.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://js.jctech888.com.cn

TS:   s.replaceAll("a", "b")
来源：http://bh.jctech888.com.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bx.colortex.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bo.muxihuayi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://tx.521024.cn

C#:   s.Replace("a", "b")
来源：http://sc.haigaiapp.cn

[E07] 按分隔符拆分
来源：http://ti.colortex.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zh.9csxet.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bm.shtwfgs.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://yd.wgjwhj.cn

TS:   s.split(",")
来源：http://cf.asd995.cn

Java: s.split(",");  s.split("\\s+")
来源：http://zy.gzmigu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://gp.huixinmuqiang.cn

Ruby: s.split(",");  s.split
来源：http://kj.huixinmuqiang.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kw.jctech888.com.cn

[E08] 数组按分隔符合并
来源：http://bh.szxytkj.cn

Py:   ",".join(items)
来源：http://bp.hnjuh.cn

PHP:  implode(",", $items);
来源：http://oo.hahajie.cn

JS:   items.join(",")
来源：http://yc.nicolike.cn

TS:   items.join(",")
来源：http://ie.newstarts.cn

Java: String.join(",", items)
来源：http://zk.asd995.cn

Go:   strings.Join(items, ",")
来源：http://vj.lnxyls.cn

Ruby: items.join(",")
来源：http://td.haigaiapp.cn

C#:   string.Join(",", items)
来源：http://eq.panjiajie.cn

[E09] 去除所有空白字符
来源：http://dg.yuntaijiaju.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vq.szsharing.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ne.lnxyls.cn

JS:   s.replace(/\s+/g, "")
来源：http://gg.shxzskj.cn

TS:   s.replace(/\s+/g, "")
来源：http://oj.chemitech.net.cn

Java: s.replaceAll("\\s+", "")
来源：http://df.9csxet.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://vt.bjjhwx.cn

Ruby: s.gsub(/\s+/, "")
来源：http://db.colortex.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qr.nszjky.cn

[E10] 左侧补零 / 定长填充
来源：http://si.shtwfgs.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://em.jctech888.com.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bk.gzmigu.cn

JS:   "7".padStart(3, "0")
来源：http://ly.hnjuh.cn

TS:   "7".padStart(3, "0")
来源：http://mq.gzmigu.cn

Java: String.format("%03d", 7)
来源：http://me.jctech888.com.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://zy.lnxyls.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ue.muxihuayi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rd.haigaiapp.cn

[E11] 反转字符串
来源：http://ri.huixiangedu.cn

Py:   s[::-1]
来源：http://pm.shxzukj.cn

PHP:  strrev($s);
来源：http://yw.huixiangedu.cn

JS:   [...s].reverse().join("")
来源：http://yh.hahajie.cn

TS:   [...s].reverse().join("")
来源：http://sq.huixiangedu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://mt.newstarts.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://rw.muxihuayi.cn

Ruby: s.reverse
来源：http://dl.panjiajie.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ct.panjiajie.cn

[E12] 统计某字符出现次数
来源：http://ey.chemitech.net.cn

Py:   s.count("a")
来源：http://em.hahajie.cn

PHP:  substr_count($s, "a");
来源：http://je.shxzukj.cn

JS:   s.split("a").length - 1
来源：http://am.panjiajie.cn

TS:   s.split("a").length - 1
来源：http://uq.nszjky.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ml.yuntaijiaju.cn

Go:   strings.Count(s, "a")
来源：http://ti.huixiangedu.cn

Ruby: s.count("a")
来源：http://ns.colortex.cn

C#:   s.Count(c => c == 'a')
来源：http://iq.muxihuayi.cn

[E13] 逐字符遍历
来源：http://hy.colortex.cn

Py:   for ch in s: print(ch)
来源：http://pw.nszjky.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bz.huixinmuqiang.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://lz.9csxet.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://of.asd995.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ga.yuntaijiaju.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ip.jianghongdianzi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://uz.yuntaijiaju.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qz.9csxet.cn

[E14] URL 编码与 Base64
来源：http://mq.hnjuh.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://if.lnxyls.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://zl.panjiajie.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://am.huixinmuqiang.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ft.newstarts.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rj.bookmarksfly.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://du.haigaiapp.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://lp.szsharing.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zx.hnjuh.cn

[E15] HTML 转义 / 反转义
来源：http://qv.nicolike.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://va.asd995.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://yn.yuntaijiaju.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pq.muxihuayi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://mz.521024.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zb.wgjwhj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://yb.wgjwhj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://kl.jctech888.com.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://dq.chemitech.net.cn

[E16] 数字千分位
来源：http://tf.jianghongdianzi.cn

Py:   f"{1234567:,}"
来源：http://lh.muxihuayi.cn

PHP:  number_format(1234567);
来源：http://tt.newstarts.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://yc.yuntaijiaju.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://dw.shxzukj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ci.shxzukj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xg.colortex.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vq.chemitech.net.cn

C#:   1234567.ToString("N0")
来源：http://tx.shxzskj.cn

[E17] 首字母大写
来源：http://be.asd995.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://go.huanxung.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://xw.lnxyls.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xt.521024.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kh.haigaiapp.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://re.panjiajie.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qn.huanxung.cn

Ruby: s.capitalize
来源：http://xd.gzmigu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://yz.shxzukj.cn

[E18] 模板占位符替换
来源：http://sk.szxytkj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wi.9csxet.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://di.panjiajie.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://be.shxzskj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://lq.yuntaijiaju.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mk.bjjhwx.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://eu.huixinmuqiang.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://lj.bjjhwx.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vx.shxzskj.cn

[E19] 多行文本按行拆分
来源：http://ri.gzmigu.cn

Py:   s.splitlines()
来源：http://ba.nszjky.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://oe.lnxyls.cn

JS:   s.split(/\r?\n/)
来源：http://tu.haigaiapp.cn

TS:   s.split(/\r?\n/)
来源：http://nw.yuexingan06.cn

Java: s.lines().toList()
来源：http://vz.asd995.cn

Go:   strings.Split(s, "\n")
来源：http://mz.huanxung.cn

Ruby: s.lines
来源：http://ct.yuexingan06.cn

C#:   s.Split('\n')
来源：http://ty.huixiangedu.cn

[E20] 判断字符串是否为空
来源：http://on.lnxyls.cn

Py:   if not s:
来源：http://be.haigaiapp.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://za.huixiangedu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://cf.521024.cn

TS:   if (s === "") {}
来源：http://fh.yuexingan06.cn

Java: if (s.isEmpty()) {}
来源：http://ah.yuntaijiaju.cn

Go:   if s == "" {}
来源：http://mq.shxzskj.cn

Ruby: if s.empty?
来源：http://nf.haigaiapp.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://up.muxihuayi.cn

[E21] 超长截断加省略号
来源：http://qo.gzmigu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rt.hahajie.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xb.asd995.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ng.huixiangedu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nm.shtwfgs.cn


<!-- 参考信息 -->