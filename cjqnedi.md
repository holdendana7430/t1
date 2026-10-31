代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vg.haigaiapp.cn

JS:   arr.filter(x => x > 3)
来源：http://tf.muxihuayi.cn

TS:   arr.filter(x => x > 3)
来源：http://qr.haigaiapp.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vi.huixinmuqiang.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ap.shtwfgs.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ed.521024.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://fs.hnjuh.cn

[D14] 映射转换（每个元素变形）
来源：http://ib.shxzukj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://px.521024.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hh.yuntaijiaju.cn

JS:   arr.map(x => x * 2)
来源：http://ze.521024.cn

TS:   arr.map(x => x * 2)
来源：http://wm.yuexingan06.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://oo.muxihuayi.cn

Go:   // 手写循环
来源：http://fv.9csxet.cn

Ruby: arr.map { |x| x * 2 }
来源：http://wf.yuexingan06.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://kc.wgjwhj.cn

[D15] 去重
来源：http://wl.shxzskj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ku.szsharing.cn

PHP:  array_unique($arr);
来源：http://rq.nicolike.cn

JS:   [...new Set(arr)]
来源：http://fp.huixinmuqiang.cn

TS:   [...new Set(arr)]
来源：http://cu.hnjuh.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://po.shxzskj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://qx.huixiangedu.cn

Ruby: arr.uniq
来源：http://ml.nicolike.cn

C#:   list.Distinct().ToList()
来源：http://gb.shxzukj.cn

[D16] 求和与平均值
来源：http://iz.bjjhwx.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://as.huanxung.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nf.haigaiapp.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://pe.nicolike.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xu.bjjhwx.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://it.huixinmuqiang.cn

Go:   // 手写循环累加
来源：http://on.9csxet.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://eg.szxytkj.cn

C#:   list.Sum();  list.Average()
来源：http://my.chemitech.net.cn

[D17] 最大值与最小值
来源：http://sn.panjiajie.cn

Py:   max(arr);  min(arr)
来源：http://fr.haigaiapp.cn

PHP:  max($arr);  min($arr);
来源：http://qz.9csxet.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fo.shxzukj.cn

TS:   Math.max(...arr);
来源：http://ip.newstarts.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://mn.gzmigu.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vr.bjjhwx.cn

Ruby: arr.max;  arr.min
来源：http://ga.bookmarksfly.cn

C#:   list.Max();  list.Min()
来源：http://fu.yuntaijiaju.cn

[D18] 扁平化嵌套数组
来源：http://ls.newstarts.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mc.9csxet.cn

PHP:  array_merge(...$nested);
来源：http://ep.hnjuh.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jk.szxytkj.cn

TS:   nested.flat();
来源：http://wq.chemitech.net.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ko.lnxyls.cn

Go:   // 手写双层循环
来源：http://el.shxzskj.cn

Ruby: nested.flatten
来源：http://jt.shxzskj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://sn.huixiangedu.cn

[D19] 按字段分组
来源：http://zq.hahajie.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wi.yuexingan06.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mv.9csxet.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://iw.jctech888.com.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://je.muxihuayi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://et.panjiajie.cn

Go:   // 手写 map[string][]T
来源：http://zl.yuexingan06.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://on.muxihuayi.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ry.szxytkj.cn

[D20] 统计每个元素出现次数
来源：http://zm.hahajie.cn

Py:   Counter(arr)
来源：http://xp.9csxet.cn

PHP:  array_count_values($arr);
来源：http://vd.521024.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ov.wgjwhj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ot.shxzukj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rg.nicolike.cn

Go:   // 手写 map[T]int
来源：http://ur.shxzskj.cn

Ruby: arr.tally
来源：http://mq.nszjky.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mm.yuntaijiaju.cn

[D21] 判断是否包含某元素
来源：http://ey.yuexingan06.cn

Py:   x in arr
来源：http://sr.szxytkj.cn

PHP:  in_array($x, $arr, true);
来源：http://cw.colortex.cn

JS:   arr.includes(x)
来源：http://bu.9csxet.cn

TS:   arr.includes(x)
来源：http://yo.haigaiapp.cn

Java: list.contains(x)
来源：http://ft.shxzskj.cn

Go:   slices.Contains(arr, x)
来源：http://ia.huanxung.cn

Ruby: arr.include?(x)
来源：http://hs.9csxet.cn

C#:   list.Contains(x)
来源：http://cd.huanxung.cn

[D22] 复制数组（避免共享引用）
来源：http://ip.lnxyls.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lc.chemitech.net.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://pj.muxihuayi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xf.shtwfgs.cn

TS:   [...arr];
来源：http://lj.jianghongdianzi.cn

Java: new ArrayList<>(list);
来源：http://vh.hnjuh.cn

Go:   copied := append([]int(nil), arr...)
来源：http://fe.huanxung.cn

Ruby: arr.dup;  arr.clone
来源：http://db.huixinmuqiang.cn

C#:   new List<int>(list);
来源：http://pz.asd995.cn

[D23] reduce 累积计算
来源：http://ws.haigaiapp.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ku.huixinmuqiang.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kd.bookmarksfly.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pl.yuntaijiaju.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qu.szsharing.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://uo.huixinmuqiang.cn

Go:   // 手写循环
来源：http://pu.huixinmuqiang.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ao.szxytkj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jm.yuntaijiaju.cn

[D24] 字典 / Map 基本操作
来源：http://fd.asd995.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ek.chemitech.net.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://cg.asd995.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gx.shtwfgs.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ih.colortex.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gu.szsharing.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fq.jctech888.com.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qm.bookmarksfly.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wc.huanxung.cn

[D25] Set 集合去重与交并差
来源：http://ta.gzmigu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xr.newstarts.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gc.bookmarksfly.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rq.haigaiapp.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qn.nszjky.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mg.chemitech.net.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ej.jctech888.com.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://eo.yuntaijiaju.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ai.yuexingan06.cn

[D26] 数组转字符串
来源：http://ar.hahajie.cn

Py:   ", ".join(map(str, arr))
来源：http://hq.9csxet.cn

PHP:  implode(", ", $arr);
来源：http://oa.chemitech.net.cn

JS:   arr.join(", ")
来源：http://ds.hnjuh.cn

TS:   arr.join(", ")
来源：http://md.huixiangedu.cn

Java: String.join(", ", list)
来源：http://xp.szxytkj.cn

Go:   strings.Join(strs, ", ")
来源：http://lm.yuntaijiaju.cn

Ruby: arr.join(", ")
来源：http://mx.chemitech.net.cn

C#:   string.Join(", ", list)
来源：http://ve.jianghongdianzi.cn

================================================================================
来源：http://ex.szsharing.cn

E. 字符串处理
来源：http://ne.9csxet.cn

================================================================================
来源：http://xl.panjiajie.cn

[E01] 拼接字符串
来源：http://si.colortex.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lq.gzmigu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ag.yuntaijiaju.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ia.muxihuayi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hm.panjiajie.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://af.szsharing.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zm.9csxet.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://nc.bookmarksfly.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://go.hahajie.cn

[E02] 重复字符串
来源：http://sy.yuexingan06.cn

Py:   "ab" * 3
来源：http://sz.asd995.cn

PHP:  str_repeat("ab", 3);
来源：http://ev.hnjuh.cn

JS:   "ab".repeat(3)
来源：http://ne.shxzukj.cn

TS:   "ab".repeat(3)
来源：http://ag.jctech888.com.cn

Java: "ab".repeat(3)
来源：http://eu.huanxung.cn

Go:   strings.Repeat("ab", 3)
来源：http://aa.newstarts.cn

Ruby: "ab" * 3
来源：http://sh.chemitech.net.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://in.9csxet.cn

[E03] 截取子串
来源：http://xr.hahajie.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hc.521024.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bs.hahajie.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ne.szsharing.cn

TS:   s.slice(1, 4)
来源：http://zu.haigaiapp.cn

Java: s.substring(1, 4)
来源：http://ok.bookmarksfly.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wy.shtwfgs.cn

Ruby: s[1, 3];  s[1..3]
来源：http://rv.colortex.cn

C#:   s.Substring(1, 3)
来源：http://go.jianghongdianzi.cn

[E04] 查找子串位置
来源：http://lc.huanxung.cn

Py:   s.find("x");  s.index("x")
来源：http://my.9csxet.cn

PHP:  strpos($s, "x");
来源：http://do.huanxung.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fn.jianghongdianzi.cn

TS:   s.indexOf("x")
来源：http://xc.panjiajie.cn

Java: s.indexOf("x")
来源：http://zm.yuexingan06.cn

Go:   strings.Index(s, "x")
来源：http://bd.9csxet.cn

Ruby: s.index("x")
来源：http://ca.shtwfgs.cn

C#:   s.IndexOf("x")
来源：http://nl.521024.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://iz.nszjky.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://bz.huixiangedu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://so.jctech888.com.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yf.lnxyls.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://tn.huixiangedu.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hh.yuntaijiaju.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://me.yuexingan06.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://dj.yuntaijiaju.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fp.szsharing.cn

[E06] 替换子串
来源：http://af.bjjhwx.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ie.bookmarksfly.cn

PHP:  str_replace("a", "b", $s);
来源：http://ss.newstarts.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ke.shxzukj.cn

TS:   s.replaceAll("a", "b")
来源：http://nv.newstarts.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mk.lnxyls.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mi.jctech888.com.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zk.chemitech.net.cn

C#:   s.Replace("a", "b")
来源：http://yv.shtwfgs.cn

[E07] 按分隔符拆分
来源：http://dj.szsharing.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://kn.jianghongdianzi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kr.huixinmuqiang.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://el.colortex.cn

TS:   s.split(",")
来源：http://ms.yuntaijiaju.cn

Java: s.split(",");  s.split("\\s+")
来源：http://gd.shxzukj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://on.huixiangedu.cn

Ruby: s.split(",");  s.split
来源：http://fi.jianghongdianzi.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gq.panjiajie.cn

[E08] 数组按分隔符合并
来源：http://qf.huanxung.cn

Py:   ",".join(items)
来源：http://yo.newstarts.cn

PHP:  implode(",", $items);
来源：http://jz.chemitech.net.cn

JS:   items.join(",")
来源：http://mx.nszjky.cn

TS:   items.join(",")
来源：http://in.hahajie.cn

Java: String.join(",", items)
来源：http://qy.panjiajie.cn

Go:   strings.Join(items, ",")
来源：http://bg.jianghongdianzi.cn

Ruby: items.join(",")
来源：http://fa.newstarts.cn

C#:   string.Join(",", items)
来源：http://su.haigaiapp.cn

[E09] 去除所有空白字符
来源：http://qw.haigaiapp.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ga.panjiajie.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ib.huixiangedu.cn

JS:   s.replace(/\s+/g, "")
来源：http://ym.bookmarksfly.cn

TS:   s.replace(/\s+/g, "")
来源：http://jo.jianghongdianzi.cn

Java: s.replaceAll("\\s+", "")
来源：http://ni.hahajie.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://zl.huanxung.cn

Ruby: s.gsub(/\s+/, "")
来源：http://bk.shxzskj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fo.yuexingan06.cn

[E10] 左侧补零 / 定长填充
来源：http://av.hahajie.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jz.wgjwhj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qv.haigaiapp.cn

JS:   "7".padStart(3, "0")
来源：http://xk.panjiajie.cn

TS:   "7".padStart(3, "0")
来源：http://th.szsharing.cn

Java: String.format("%03d", 7)
来源：http://mx.szxytkj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://yt.szsharing.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://et.yuexingan06.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qf.szsharing.cn

[E11] 反转字符串
来源：http://xl.huixinmuqiang.cn

Py:   s[::-1]
来源：http://wo.chemitech.net.cn

PHP:  strrev($s);
来源：http://px.panjiajie.cn

JS:   [...s].reverse().join("")
来源：http://jh.huixiangedu.cn

TS:   [...s].reverse().join("")
来源：http://kr.jianghongdianzi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://lu.shxzskj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://cu.haigaiapp.cn

Ruby: s.reverse
来源：http://ms.shxzskj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://rw.nszjky.cn

[E12] 统计某字符出现次数
来源：http://un.muxihuayi.cn

Py:   s.count("a")
来源：http://aw.lnxyls.cn

PHP:  substr_count($s, "a");
来源：http://bv.nicolike.cn

JS:   s.split("a").length - 1
来源：http://rq.panjiajie.cn

TS:   s.split("a").length - 1
来源：http://uw.bjjhwx.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://da.colortex.cn

Go:   strings.Count(s, "a")
来源：http://lw.haigaiapp.cn

Ruby: s.count("a")
来源：http://pu.jianghongdianzi.cn

C#:   s.Count(c => c == 'a')
来源：http://bj.bjjhwx.cn

[E13] 逐字符遍历
来源：http://vs.nszjky.cn

Py:   for ch in s: print(ch)
来源：http://wx.521024.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://na.szxytkj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ex.szxytkj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://jq.huanxung.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fg.newstarts.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://sh.bjjhwx.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://xr.szsharing.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mg.jctech888.com.cn

[E14] URL 编码与 Base64
来源：http://bb.9csxet.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gt.hnjuh.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://rs.yuexingan06.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://tp.521024.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://sl.hahajie.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ws.szsharing.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mn.szsharing.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mq.szxytkj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qx.lnxyls.cn

[E15] HTML 转义 / 反转义
来源：http://nt.jianghongdianzi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://fp.yuexingan06.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wn.nicolike.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pd.bookmarksfly.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ep.newstarts.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gt.shtwfgs.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wm.yuexingan06.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rl.panjiajie.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://tz.haigaiapp.cn

[E16] 数字千分位
来源：http://us.huixiangedu.cn

Py:   f"{1234567:,}"
来源：http://lw.shxzukj.cn

PHP:  number_format(1234567);
来源：http://ln.szsharing.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://sj.shxzukj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://wq.shtwfgs.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nf.yuntaijiaju.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ta.shxzukj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gn.jianghongdianzi.cn

C#:   1234567.ToString("N0")
来源：http://rw.wgjwhj.cn

[E17] 首字母大写
来源：http://vp.521024.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dx.wgjwhj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://vz.hahajie.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://by.huixiangedu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hn.asd995.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ls.szsharing.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://db.shxzukj.cn

Ruby: s.capitalize
来源：http://nd.huixiangedu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gc.jianghongdianzi.cn

[E18] 模板占位符替换
来源：http://qy.szxytkj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hk.haigaiapp.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ts.wgjwhj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://wr.muxihuayi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ty.haigaiapp.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qe.huixinmuqiang.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ah.nicolike.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vb.huixiangedu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://op.huanxung.cn

[E19] 多行文本按行拆分
来源：http://di.hnjuh.cn

Py:   s.splitlines()
来源：http://fi.szxytkj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ku.huanxung.cn

JS:   s.split(/\r?\n/)
来源：http://fp.newstarts.cn

TS:   s.split(/\r?\n/)
来源：http://it.szxytkj.cn

Java: s.lines().toList()
来源：http://fr.yuntaijiaju.cn

Go:   strings.Split(s, "\n")
来源：http://dk.nicolike.cn

Ruby: s.lines
来源：http://xs.lnxyls.cn

C#:   s.Split('\n')
来源：http://lt.bookmarksfly.cn

[E20] 判断字符串是否为空
来源：http://yu.haigaiapp.cn

Py:   if not s:
来源：http://dp.nszjky.cn


<!-- 参考信息 -->