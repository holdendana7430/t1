代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://tq.jianghongdianzi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kc.newstarts.cn

JS:   arr.map(x => x * 2)
来源：http://ka.muxihuayi.cn

TS:   arr.map(x => x * 2)
来源：http://hp.asd995.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://qb.gzmigu.cn

Go:   // 手写循环
来源：http://nt.bjjhwx.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ln.hnjuh.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://dl.chemitech.net.cn

[D15] 去重
来源：http://ei.bookmarksfly.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tm.lnxyls.cn

PHP:  array_unique($arr);
来源：http://ml.yuexingan06.cn

JS:   [...new Set(arr)]
来源：http://rj.bookmarksfly.cn

TS:   [...new Set(arr)]
来源：http://yq.521024.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bu.colortex.cn

Go:   // 用 map[T]struct{} 手写
来源：http://af.nszjky.cn

Ruby: arr.uniq
来源：http://dh.szxytkj.cn

C#:   list.Distinct().ToList()
来源：http://gg.gzmigu.cn

[D16] 求和与平均值
来源：http://wr.shxzskj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://yr.jianghongdianzi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://om.jianghongdianzi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://sl.jianghongdianzi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lg.gzmigu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wl.nicolike.cn

Go:   // 手写循环累加
来源：http://fm.chemitech.net.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qg.asd995.cn

C#:   list.Sum();  list.Average()
来源：http://xr.muxihuayi.cn

[D17] 最大值与最小值
来源：http://ie.chemitech.net.cn

Py:   max(arr);  min(arr)
来源：http://io.jctech888.com.cn

PHP:  max($arr);  min($arr);
来源：http://ng.huixiangedu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dh.huixinmuqiang.cn

TS:   Math.max(...arr);
来源：http://or.huanxung.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://rn.haigaiapp.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ao.huanxung.cn

Ruby: arr.max;  arr.min
来源：http://ps.bookmarksfly.cn

C#:   list.Max();  list.Min()
来源：http://tj.szxytkj.cn

[D18] 扁平化嵌套数组
来源：http://zc.muxihuayi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mz.chemitech.net.cn

PHP:  array_merge(...$nested);
来源：http://nj.hnjuh.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://eg.chemitech.net.cn

TS:   nested.flat();
来源：http://ex.asd995.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://lx.muxihuayi.cn

Go:   // 手写双层循环
来源：http://cm.jctech888.com.cn

Ruby: nested.flatten
来源：http://xe.shxzskj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://br.shxzskj.cn

[D19] 按字段分组
来源：http://ue.shtwfgs.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://cp.yuexingan06.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wa.huanxung.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://eq.szxytkj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://rq.szxytkj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://lc.nszjky.cn

Go:   // 手写 map[string][]T
来源：http://fp.szxytkj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://bm.nszjky.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://np.chemitech.net.cn

[D20] 统计每个元素出现次数
来源：http://sy.9csxet.cn

Py:   Counter(arr)
来源：http://bm.bookmarksfly.cn

PHP:  array_count_values($arr);
来源：http://yf.yuntaijiaju.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ux.huanxung.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fc.9csxet.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bd.hnjuh.cn

Go:   // 手写 map[T]int
来源：http://mx.szsharing.cn

Ruby: arr.tally
来源：http://eu.asd995.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://nk.yuexingan06.cn

[D21] 判断是否包含某元素
来源：http://wt.asd995.cn

Py:   x in arr
来源：http://hr.hnjuh.cn

PHP:  in_array($x, $arr, true);
来源：http://lp.hahajie.cn

JS:   arr.includes(x)
来源：http://sz.haigaiapp.cn

TS:   arr.includes(x)
来源：http://ec.bookmarksfly.cn

Java: list.contains(x)
来源：http://bq.chemitech.net.cn

Go:   slices.Contains(arr, x)
来源：http://pr.muxihuayi.cn

Ruby: arr.include?(x)
来源：http://rl.shxzskj.cn

C#:   list.Contains(x)
来源：http://in.chemitech.net.cn

[D22] 复制数组（避免共享引用）
来源：http://fe.huixiangedu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ia.huanxung.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://re.hahajie.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bd.lnxyls.cn

TS:   [...arr];
来源：http://db.jianghongdianzi.cn

Java: new ArrayList<>(list);
来源：http://cv.jctech888.com.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ix.shtwfgs.cn

Ruby: arr.dup;  arr.clone
来源：http://hj.chemitech.net.cn

C#:   new List<int>(list);
来源：http://gi.9csxet.cn

[D23] reduce 累积计算
来源：http://lo.newstarts.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://sp.colortex.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://il.szsharing.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jq.jctech888.com.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://av.shtwfgs.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://wa.szxytkj.cn

Go:   // 手写循环
来源：http://gp.szxytkj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ot.hahajie.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://sm.jctech888.com.cn

[D24] 字典 / Map 基本操作
来源：http://px.asd995.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bn.nicolike.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://br.bjjhwx.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://az.szxytkj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bs.panjiajie.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ei.shxzukj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xa.jianghongdianzi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hh.jctech888.com.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rz.hahajie.cn

[D25] Set 集合去重与交并差
来源：http://dc.huixiangedu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nb.asd995.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://kw.szxytkj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mk.hnjuh.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dp.hahajie.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ef.521024.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nr.chemitech.net.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ke.panjiajie.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://uo.gzmigu.cn

[D26] 数组转字符串
来源：http://xh.yuntaijiaju.cn

Py:   ", ".join(map(str, arr))
来源：http://ck.wgjwhj.cn

PHP:  implode(", ", $arr);
来源：http://eg.yuexingan06.cn

JS:   arr.join(", ")
来源：http://ut.asd995.cn

TS:   arr.join(", ")
来源：http://wa.hahajie.cn

Java: String.join(", ", list)
来源：http://uv.wgjwhj.cn

Go:   strings.Join(strs, ", ")
来源：http://rl.newstarts.cn

Ruby: arr.join(", ")
来源：http://sm.yuntaijiaju.cn

C#:   string.Join(", ", list)
来源：http://yv.hnjuh.cn

================================================================================
来源：http://hz.hahajie.cn

E. 字符串处理
来源：http://dl.lnxyls.cn

================================================================================
来源：http://vj.shtwfgs.cn

[E01] 拼接字符串
来源：http://vx.newstarts.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mm.hnjuh.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://aa.hahajie.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nb.yuexingan06.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xo.yuntaijiaju.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://eb.jctech888.com.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ib.nicolike.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ge.haigaiapp.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zs.muxihuayi.cn

[E02] 重复字符串
来源：http://lz.lnxyls.cn

Py:   "ab" * 3
来源：http://iv.nicolike.cn

PHP:  str_repeat("ab", 3);
来源：http://ac.lnxyls.cn

JS:   "ab".repeat(3)
来源：http://ti.haigaiapp.cn

TS:   "ab".repeat(3)
来源：http://kj.lnxyls.cn

Java: "ab".repeat(3)
来源：http://pr.yuexingan06.cn

Go:   strings.Repeat("ab", 3)
来源：http://nv.shxzukj.cn

Ruby: "ab" * 3
来源：http://et.panjiajie.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ba.szsharing.cn

[E03] 截取子串
来源：http://mf.szsharing.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rd.wgjwhj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://oa.huixinmuqiang.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://um.bjjhwx.cn

TS:   s.slice(1, 4)
来源：http://am.szxytkj.cn

Java: s.substring(1, 4)
来源：http://gw.colortex.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://pi.9csxet.cn

Ruby: s[1, 3];  s[1..3]
来源：http://co.muxihuayi.cn

C#:   s.Substring(1, 3)
来源：http://nr.9csxet.cn

[E04] 查找子串位置
来源：http://aa.jianghongdianzi.cn

Py:   s.find("x");  s.index("x")
来源：http://cr.wgjwhj.cn

PHP:  strpos($s, "x");
来源：http://xw.colortex.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://sf.huixinmuqiang.cn

TS:   s.indexOf("x")
来源：http://gd.huanxung.cn

Java: s.indexOf("x")
来源：http://cq.huanxung.cn

Go:   strings.Index(s, "x")
来源：http://jf.asd995.cn

Ruby: s.index("x")
来源：http://gr.huixinmuqiang.cn

C#:   s.IndexOf("x")
来源：http://av.colortex.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://tl.muxihuayi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://nr.colortex.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://tu.szxytkj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qc.shxzukj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://zw.hnjuh.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uc.colortex.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bo.huixiangedu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jz.521024.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mh.huanxung.cn

[E06] 替换子串
来源：http://st.huixinmuqiang.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hb.chemitech.net.cn

PHP:  str_replace("a", "b", $s);
来源：http://in.bookmarksfly.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xn.szsharing.cn

TS:   s.replaceAll("a", "b")
来源：http://wb.nicolike.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lo.szsharing.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bu.hnjuh.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vq.gzmigu.cn

C#:   s.Replace("a", "b")
来源：http://ef.chemitech.net.cn

[E07] 按分隔符拆分
来源：http://gu.lnxyls.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gc.shtwfgs.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qw.bjjhwx.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ab.shxzukj.cn

TS:   s.split(",")
来源：http://zb.chemitech.net.cn

Java: s.split(",");  s.split("\\s+")
来源：http://bo.huanxung.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jh.nicolike.cn

Ruby: s.split(",");  s.split
来源：http://im.521024.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ny.jianghongdianzi.cn

[E08] 数组按分隔符合并
来源：http://mb.9csxet.cn

Py:   ",".join(items)
来源：http://oi.shxzskj.cn

PHP:  implode(",", $items);
来源：http://vk.szxytkj.cn

JS:   items.join(",")
来源：http://cu.huanxung.cn

TS:   items.join(",")
来源：http://nj.newstarts.cn

Java: String.join(",", items)
来源：http://am.yuexingan06.cn

Go:   strings.Join(items, ",")
来源：http://iy.huixinmuqiang.cn

Ruby: items.join(",")
来源：http://hz.yuntaijiaju.cn

C#:   string.Join(",", items)
来源：http://ie.nszjky.cn

[E09] 去除所有空白字符
来源：http://fk.yuntaijiaju.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zz.nszjky.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://gd.nszjky.cn

JS:   s.replace(/\s+/g, "")
来源：http://gp.panjiajie.cn

TS:   s.replace(/\s+/g, "")
来源：http://bv.nicolike.cn

Java: s.replaceAll("\\s+", "")
来源：http://jw.asd995.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ba.shxzukj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://an.bjjhwx.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vx.hahajie.cn

[E10] 左侧补零 / 定长填充
来源：http://xw.bookmarksfly.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bs.yuexingan06.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://kf.yuntaijiaju.cn

JS:   "7".padStart(3, "0")
来源：http://ui.jianghongdianzi.cn

TS:   "7".padStart(3, "0")
来源：http://ez.nicolike.cn

Java: String.format("%03d", 7)
来源：http://lh.asd995.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://zj.lnxyls.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mn.hnjuh.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hv.newstarts.cn

[E11] 反转字符串
来源：http://zs.jianghongdianzi.cn

Py:   s[::-1]
来源：http://mf.asd995.cn

PHP:  strrev($s);
来源：http://sy.haigaiapp.cn

JS:   [...s].reverse().join("")
来源：http://ug.lnxyls.cn

TS:   [...s].reverse().join("")
来源：http://kc.szxytkj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://fa.colortex.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://bo.colortex.cn

Ruby: s.reverse
来源：http://aj.muxihuayi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://cb.nszjky.cn

[E12] 统计某字符出现次数
来源：http://sf.9csxet.cn

Py:   s.count("a")
来源：http://eo.shtwfgs.cn

PHP:  substr_count($s, "a");
来源：http://li.521024.cn

JS:   s.split("a").length - 1
来源：http://jn.bookmarksfly.cn

TS:   s.split("a").length - 1
来源：http://ep.szsharing.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fc.muxihuayi.cn

Go:   strings.Count(s, "a")
来源：http://nr.jianghongdianzi.cn

Ruby: s.count("a")
来源：http://zn.shxzukj.cn

C#:   s.Count(c => c == 'a')
来源：http://re.panjiajie.cn

[E13] 逐字符遍历
来源：http://ro.nicolike.cn

Py:   for ch in s: print(ch)
来源：http://dd.wgjwhj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wm.szxytkj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://kv.gzmigu.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://zn.huanxung.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vb.wgjwhj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://cg.bookmarksfly.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://vx.wgjwhj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fk.asd995.cn

[E14] URL 编码与 Base64
来源：http://vl.9csxet.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://px.szxytkj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://rz.nszjky.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ku.shxzskj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ad.hnjuh.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://gp.huixiangedu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cg.asd995.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bu.wgjwhj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bl.huixinmuqiang.cn

[E15] HTML 转义 / 反转义
来源：http://gj.jctech888.com.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ib.huixinmuqiang.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://nc.huanxung.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ed.lnxyls.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://va.shtwfgs.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wn.bjjhwx.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://el.yuexingan06.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pz.wgjwhj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nw.shxzukj.cn

[E16] 数字千分位
来源：http://mj.chemitech.net.cn

Py:   f"{1234567:,}"
来源：http://tb.shxzukj.cn

PHP:  number_format(1234567);
来源：http://mn.gzmigu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://st.muxihuayi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://jt.bjjhwx.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://cw.shxzskj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://bi.gzmigu.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://de.521024.cn

C#:   1234567.ToString("N0")
来源：http://fh.gzmigu.cn

[E17] 首字母大写
来源：http://sv.newstarts.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dr.shxzskj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://dx.yuexingan06.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://da.huixinmuqiang.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uq.jianghongdianzi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://km.haigaiapp.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://px.jctech888.com.cn

Ruby: s.capitalize
来源：http://bs.jctech888.com.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://bb.huixinmuqiang.cn

[E18] 模板占位符替换
来源：http://gb.colortex.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://rg.lnxyls.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qq.wgjwhj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zs.huanxung.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ju.lnxyls.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rt.yuexingan06.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jk.yuntaijiaju.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://oe.yuexingan06.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://cw.muxihuayi.cn

[E19] 多行文本按行拆分
来源：http://gn.nszjky.cn

Py:   s.splitlines()
来源：http://jp.shtwfgs.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jm.szxytkj.cn

JS:   s.split(/\r?\n/)
来源：http://at.nicolike.cn

TS:   s.split(/\r?\n/)
来源：http://ug.yuexingan06.cn

Java: s.lines().toList()
来源：http://eq.muxihuayi.cn

Go:   strings.Split(s, "\n")
来源：http://jy.jctech888.com.cn

Ruby: s.lines
来源：http://fp.muxihuayi.cn

C#:   s.Split('\n')
来源：http://hs.muxihuayi.cn

[E20] 判断字符串是否为空
来源：http://iy.hahajie.cn

Py:   if not s:
来源：http://kl.nicolike.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qq.huixiangedu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mm.huanxung.cn

TS:   if (s === "") {}
来源：http://ny.szsharing.cn

Java: if (s.isEmpty()) {}
来源：http://jo.wgjwhj.cn

Go:   if s == "" {}
来源：http://za.colortex.cn

Ruby: if s.empty?
来源：http://kh.bjjhwx.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qv.shtwfgs.cn

[E21] 超长截断加省略号
来源：http://at.haigaiapp.cn


<!-- 参考信息 -->