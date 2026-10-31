代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://aa.hahajie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fe.9csxet.cn

JS:   arr.map(x => x * 2)
来源：http://do.jianghongdianzi.cn

TS:   arr.map(x => x * 2)
来源：http://sf.nszjky.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://tn.nszjky.cn

Go:   // 手写循环
来源：http://fs.yuexingan06.cn

Ruby: arr.map { |x| x * 2 }
来源：http://xy.jctech888.com.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ao.asd995.cn

[D15] 去重
来源：http://iv.shxzukj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ar.jianghongdianzi.cn

PHP:  array_unique($arr);
来源：http://gn.newstarts.cn

JS:   [...new Set(arr)]
来源：http://yr.hahajie.cn

TS:   [...new Set(arr)]
来源：http://uo.huixinmuqiang.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dl.nszjky.cn

Go:   // 用 map[T]struct{} 手写
来源：http://iv.lnxyls.cn

Ruby: arr.uniq
来源：http://zr.haigaiapp.cn

C#:   list.Distinct().ToList()
来源：http://av.colortex.cn

[D16] 求和与平均值
来源：http://gy.yuexingan06.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://en.shxzukj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fg.shtwfgs.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xq.shxzukj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jl.bookmarksfly.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://pj.shxzukj.cn

Go:   // 手写循环累加
来源：http://uw.lnxyls.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hj.shxzskj.cn

C#:   list.Sum();  list.Average()
来源：http://ms.9csxet.cn

[D17] 最大值与最小值
来源：http://es.shxzskj.cn

Py:   max(arr);  min(arr)
来源：http://mp.asd995.cn

PHP:  max($arr);  min($arr);
来源：http://zr.hahajie.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ue.hnjuh.cn

TS:   Math.max(...arr);
来源：http://fe.hnjuh.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://cw.hahajie.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dp.shxzskj.cn

Ruby: arr.max;  arr.min
来源：http://ll.haigaiapp.cn

C#:   list.Max();  list.Min()
来源：http://fd.shxzskj.cn

[D18] 扁平化嵌套数组
来源：http://sg.bookmarksfly.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://gi.hnjuh.cn

PHP:  array_merge(...$nested);
来源：http://tj.wgjwhj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://en.521024.cn

TS:   nested.flat();
来源：http://se.jianghongdianzi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://iu.shxzukj.cn

Go:   // 手写双层循环
来源：http://os.521024.cn

Ruby: nested.flatten
来源：http://xm.shxzskj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://fh.521024.cn

[D19] 按字段分组
来源：http://ul.hnjuh.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://oi.yuexingan06.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ci.9csxet.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://td.jctech888.com.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://sf.jianghongdianzi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fy.jctech888.com.cn

Go:   // 手写 map[string][]T
来源：http://fx.shxzskj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://zt.huixinmuqiang.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qn.colortex.cn

[D20] 统计每个元素出现次数
来源：http://qz.asd995.cn

Py:   Counter(arr)
来源：http://eu.9csxet.cn

PHP:  array_count_values($arr);
来源：http://js.szsharing.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dl.yuntaijiaju.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uu.panjiajie.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ah.szxytkj.cn

Go:   // 手写 map[T]int
来源：http://ky.bjjhwx.cn

Ruby: arr.tally
来源：http://de.gzmigu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ot.bjjhwx.cn

[D21] 判断是否包含某元素
来源：http://bm.huixinmuqiang.cn

Py:   x in arr
来源：http://tt.colortex.cn

PHP:  in_array($x, $arr, true);
来源：http://ms.szsharing.cn

JS:   arr.includes(x)
来源：http://qo.huixiangedu.cn

TS:   arr.includes(x)
来源：http://ou.521024.cn

Java: list.contains(x)
来源：http://nq.shxzskj.cn

Go:   slices.Contains(arr, x)
来源：http://tc.521024.cn

Ruby: arr.include?(x)
来源：http://qq.szxytkj.cn

C#:   list.Contains(x)
来源：http://lh.huixinmuqiang.cn

[D22] 复制数组（避免共享引用）
来源：http://xr.hahajie.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gl.shtwfgs.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mk.szsharing.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://kb.chemitech.net.cn

TS:   [...arr];
来源：http://um.nicolike.cn

Java: new ArrayList<>(list);
来源：http://qa.521024.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ti.gzmigu.cn

Ruby: arr.dup;  arr.clone
来源：http://te.huixiangedu.cn

C#:   new List<int>(list);
来源：http://oz.shtwfgs.cn

[D23] reduce 累积计算
来源：http://ov.lnxyls.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jx.shtwfgs.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://yk.bookmarksfly.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wj.yuexingan06.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ht.gzmigu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://sy.huanxung.cn

Go:   // 手写循环
来源：http://mj.jctech888.com.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pp.wgjwhj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qi.gzmigu.cn

[D24] 字典 / Map 基本操作
来源：http://iz.nicolike.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://oq.newstarts.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pa.huixiangedu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ph.yuexingan06.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://pq.yuntaijiaju.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://pp.wgjwhj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://nz.yuexingan06.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ga.huanxung.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kh.hahajie.cn

[D25] Set 集合去重与交并差
来源：http://rj.huixiangedu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bn.colortex.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://no.newstarts.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://eh.newstarts.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zv.newstarts.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hp.shtwfgs.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://id.wgjwhj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ba.asd995.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lk.nicolike.cn

[D26] 数组转字符串
来源：http://it.wgjwhj.cn

Py:   ", ".join(map(str, arr))
来源：http://db.huanxung.cn

PHP:  implode(", ", $arr);
来源：http://sg.newstarts.cn

JS:   arr.join(", ")
来源：http://kx.hnjuh.cn

TS:   arr.join(", ")
来源：http://vd.yuntaijiaju.cn

Java: String.join(", ", list)
来源：http://gg.asd995.cn

Go:   strings.Join(strs, ", ")
来源：http://vf.lnxyls.cn

Ruby: arr.join(", ")
来源：http://az.jctech888.com.cn

C#:   string.Join(", ", list)
来源：http://qs.nszjky.cn

================================================================================
来源：http://dc.nicolike.cn

E. 字符串处理
来源：http://ff.gzmigu.cn

================================================================================
来源：http://yh.nicolike.cn

[E01] 拼接字符串
来源：http://xo.huixinmuqiang.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://id.asd995.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dn.shxzukj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://el.huixinmuqiang.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tt.hahajie.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://cp.jctech888.com.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gf.wgjwhj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ao.chemitech.net.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jb.hahajie.cn

[E02] 重复字符串
来源：http://mw.shtwfgs.cn

Py:   "ab" * 3
来源：http://am.bookmarksfly.cn

PHP:  str_repeat("ab", 3);
来源：http://xu.szsharing.cn

JS:   "ab".repeat(3)
来源：http://cj.asd995.cn

TS:   "ab".repeat(3)
来源：http://fc.huanxung.cn

Java: "ab".repeat(3)
来源：http://oy.asd995.cn

Go:   strings.Repeat("ab", 3)
来源：http://kw.shxzukj.cn

Ruby: "ab" * 3
来源：http://pa.newstarts.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ca.nicolike.cn

[E03] 截取子串
来源：http://wf.lnxyls.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ew.colortex.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://yr.wgjwhj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fm.huixinmuqiang.cn

TS:   s.slice(1, 4)
来源：http://lq.hnjuh.cn

Java: s.substring(1, 4)
来源：http://vl.newstarts.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kk.yuntaijiaju.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ic.yuexingan06.cn

C#:   s.Substring(1, 3)
来源：http://fj.huanxung.cn

[E04] 查找子串位置
来源：http://gs.chemitech.net.cn

Py:   s.find("x");  s.index("x")
来源：http://lh.jctech888.com.cn

PHP:  strpos($s, "x");
来源：http://kh.chemitech.net.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qk.panjiajie.cn

TS:   s.indexOf("x")
来源：http://ya.asd995.cn

Java: s.indexOf("x")
来源：http://fm.shtwfgs.cn

Go:   strings.Index(s, "x")
来源：http://jq.nszjky.cn

Ruby: s.index("x")
来源：http://sf.chemitech.net.cn

C#:   s.IndexOf("x")
来源：http://ys.yuexingan06.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://in.gzmigu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ye.gzmigu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vk.jianghongdianzi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sr.9csxet.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ox.colortex.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://im.521024.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cu.colortex.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://un.huanxung.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://pm.lnxyls.cn

[E06] 替换子串
来源：http://zh.haigaiapp.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://aw.huixinmuqiang.cn

PHP:  str_replace("a", "b", $s);
来源：http://eg.nicolike.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fo.muxihuayi.cn

TS:   s.replaceAll("a", "b")
来源：http://tw.bjjhwx.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://us.chemitech.net.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mn.shtwfgs.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://os.nszjky.cn

C#:   s.Replace("a", "b")
来源：http://ix.nszjky.cn

[E07] 按分隔符拆分
来源：http://qi.hahajie.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pi.haigaiapp.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gj.panjiajie.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://pg.yuexingan06.cn

TS:   s.split(",")
来源：http://qd.gzmigu.cn

Java: s.split(",");  s.split("\\s+")
来源：http://bj.szsharing.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hm.9csxet.cn

Ruby: s.split(",");  s.split
来源：http://xv.bookmarksfly.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jk.jctech888.com.cn

[E08] 数组按分隔符合并
来源：http://tx.gzmigu.cn

Py:   ",".join(items)
来源：http://tc.521024.cn

PHP:  implode(",", $items);
来源：http://ex.gzmigu.cn

JS:   items.join(",")
来源：http://ok.shxzukj.cn

TS:   items.join(",")
来源：http://nl.panjiajie.cn

Java: String.join(",", items)
来源：http://kn.shxzukj.cn

Go:   strings.Join(items, ",")
来源：http://ba.jctech888.com.cn

Ruby: items.join(",")
来源：http://jd.colortex.cn

C#:   string.Join(",", items)
来源：http://wi.jctech888.com.cn

[E09] 去除所有空白字符
来源：http://uf.9csxet.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ae.jctech888.com.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ga.jctech888.com.cn

JS:   s.replace(/\s+/g, "")
来源：http://xj.shxzukj.cn

TS:   s.replace(/\s+/g, "")
来源：http://pl.nicolike.cn

Java: s.replaceAll("\\s+", "")
来源：http://ym.wgjwhj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ky.newstarts.cn

Ruby: s.gsub(/\s+/, "")
来源：http://nd.panjiajie.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://pl.9csxet.cn

[E10] 左侧补零 / 定长填充
来源：http://iu.huixinmuqiang.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mz.gzmigu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://nb.lnxyls.cn

JS:   "7".padStart(3, "0")
来源：http://uq.shtwfgs.cn

TS:   "7".padStart(3, "0")
来源：http://yj.newstarts.cn

Java: String.format("%03d", 7)
来源：http://ag.asd995.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://pd.shxzukj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://is.bookmarksfly.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://as.hahajie.cn

[E11] 反转字符串
来源：http://hc.huixiangedu.cn

Py:   s[::-1]
来源：http://vq.newstarts.cn

PHP:  strrev($s);
来源：http://jm.nicolike.cn

JS:   [...s].reverse().join("")
来源：http://tu.asd995.cn

TS:   [...s].reverse().join("")
来源：http://ud.hnjuh.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://zj.muxihuayi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://te.chemitech.net.cn

Ruby: s.reverse
来源：http://fi.asd995.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ts.nszjky.cn

[E12] 统计某字符出现次数
来源：http://pw.huixiangedu.cn

Py:   s.count("a")
来源：http://zp.szsharing.cn

PHP:  substr_count($s, "a");
来源：http://nu.jianghongdianzi.cn

JS:   s.split("a").length - 1
来源：http://kj.lnxyls.cn

TS:   s.split("a").length - 1
来源：http://ua.yuntaijiaju.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jl.nicolike.cn

Go:   strings.Count(s, "a")
来源：http://xy.haigaiapp.cn

Ruby: s.count("a")
来源：http://rm.szsharing.cn

C#:   s.Count(c => c == 'a')
来源：http://ff.huixinmuqiang.cn

[E13] 逐字符遍历
来源：http://rb.shtwfgs.cn

Py:   for ch in s: print(ch)
来源：http://vz.huixinmuqiang.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gb.hahajie.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ml.shxzskj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ox.asd995.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gy.yuntaijiaju.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://cb.muxihuayi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ka.panjiajie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hj.colortex.cn

[E14] URL 编码与 Base64
来源：http://gg.jctech888.com.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gz.yuntaijiaju.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://wi.hahajie.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ut.jctech888.com.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bj.nicolike.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ka.yuntaijiaju.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zf.shxzukj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://oe.colortex.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mn.chemitech.net.cn

[E15] HTML 转义 / 反转义
来源：http://ww.hnjuh.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://np.jianghongdianzi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://nn.shxzskj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gr.9csxet.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://mt.bjjhwx.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://oi.gzmigu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://az.bjjhwx.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jo.colortex.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nn.bookmarksfly.cn

[E16] 数字千分位
来源：http://pl.nszjky.cn

Py:   f"{1234567:,}"
来源：http://ka.yuntaijiaju.cn

PHP:  number_format(1234567);
来源：http://ny.jianghongdianzi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://jc.wgjwhj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://xv.nszjky.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ab.haigaiapp.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xr.asd995.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bq.wgjwhj.cn

C#:   1234567.ToString("N0")
来源：http://gc.jianghongdianzi.cn

[E17] 首字母大写
来源：http://oz.jctech888.com.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wp.nszjky.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://sp.huanxung.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fu.nicolike.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xq.yuexingan06.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bp.hnjuh.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vn.colortex.cn

Ruby: s.capitalize
来源：http://pv.9csxet.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ec.9csxet.cn

[E18] 模板占位符替换
来源：http://cl.yuexingan06.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://tu.bookmarksfly.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ye.bookmarksfly.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://co.huanxung.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://xu.jianghongdianzi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xm.lnxyls.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fm.szsharing.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vg.gzmigu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mi.yuexingan06.cn

[E19] 多行文本按行拆分
来源：http://jk.colortex.cn

Py:   s.splitlines()
来源：http://zw.lnxyls.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hb.huanxung.cn

JS:   s.split(/\r?\n/)
来源：http://ue.newstarts.cn

TS:   s.split(/\r?\n/)
来源：http://sl.9csxet.cn

Java: s.lines().toList()
来源：http://zn.lnxyls.cn

Go:   strings.Split(s, "\n")
来源：http://ve.szsharing.cn

Ruby: s.lines
来源：http://ig.muxihuayi.cn

C#:   s.Split('\n')
来源：http://sx.jctech888.com.cn

[E20] 判断字符串是否为空
来源：http://kf.wgjwhj.cn

Py:   if not s:
来源：http://fx.nszjky.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ya.9csxet.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://nw.shxzskj.cn

TS:   if (s === "") {}
来源：http://zl.jianghongdianzi.cn

Java: if (s.isEmpty()) {}
来源：http://en.chemitech.net.cn

Go:   if s == "" {}
来源：http://zv.shtwfgs.cn

Ruby: if s.empty?
来源：http://xu.bookmarksfly.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ay.9csxet.cn

[E21] 超长截断加省略号
来源：http://ja.9csxet.cn


<!-- 参考信息 -->