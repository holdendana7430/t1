代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xn.muxihuayi.cn

JS:   arr.filter(x => x > 3)
来源：http://jj.hahajie.cn

TS:   arr.filter(x => x > 3)
来源：http://rr.colortex.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wf.9csxet.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ld.9csxet.cn

Ruby: arr.select { |x| x > 3 }
来源：http://hq.szxytkj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://hd.haigaiapp.cn

[D14] 映射转换（每个元素变形）
来源：http://jw.asd995.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://sw.wgjwhj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gr.chemitech.net.cn

JS:   arr.map(x => x * 2)
来源：http://yn.huanxung.cn

TS:   arr.map(x => x * 2)
来源：http://df.bjjhwx.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ur.huanxung.cn

Go:   // 手写循环
来源：http://hr.yuexingan06.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ca.wgjwhj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://yr.colortex.cn

[D15] 去重
来源：http://sv.521024.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bm.hahajie.cn

PHP:  array_unique($arr);
来源：http://rx.szsharing.cn

JS:   [...new Set(arr)]
来源：http://dr.yuntaijiaju.cn

TS:   [...new Set(arr)]
来源：http://ei.9csxet.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dv.muxihuayi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://op.muxihuayi.cn

Ruby: arr.uniq
来源：http://en.panjiajie.cn

C#:   list.Distinct().ToList()
来源：http://nz.nicolike.cn

[D16] 求和与平均值
来源：http://qh.wgjwhj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mx.bookmarksfly.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ip.szxytkj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rl.jianghongdianzi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://sb.wgjwhj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://sp.hahajie.cn

Go:   // 手写循环累加
来源：http://td.hahajie.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ah.szsharing.cn

C#:   list.Sum();  list.Average()
来源：http://yb.yuntaijiaju.cn

[D17] 最大值与最小值
来源：http://sw.shxzskj.cn

Py:   max(arr);  min(arr)
来源：http://sk.newstarts.cn

PHP:  max($arr);  min($arr);
来源：http://og.huixinmuqiang.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ug.jianghongdianzi.cn

TS:   Math.max(...arr);
来源：http://ss.shtwfgs.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ch.szsharing.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jz.colortex.cn

Ruby: arr.max;  arr.min
来源：http://cj.gzmigu.cn

C#:   list.Max();  list.Min()
来源：http://zo.shxzskj.cn

[D18] 扁平化嵌套数组
来源：http://ey.muxihuayi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fa.asd995.cn

PHP:  array_merge(...$nested);
来源：http://ul.hahajie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zt.gzmigu.cn

TS:   nested.flat();
来源：http://ky.jctech888.com.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cj.jianghongdianzi.cn

Go:   // 手写双层循环
来源：http://fw.shtwfgs.cn

Ruby: nested.flatten
来源：http://ex.shtwfgs.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://bb.bjjhwx.cn

[D19] 按字段分组
来源：http://ey.521024.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://bl.jianghongdianzi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wu.haigaiapp.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wm.haigaiapp.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://fi.wgjwhj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://cd.jctech888.com.cn

Go:   // 手写 map[string][]T
来源：http://uz.asd995.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://cu.521024.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://co.colortex.cn

[D20] 统计每个元素出现次数
来源：http://lg.asd995.cn

Py:   Counter(arr)
来源：http://ux.muxihuayi.cn

PHP:  array_count_values($arr);
来源：http://sp.szsharing.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kg.huixiangedu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bm.haigaiapp.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gn.chemitech.net.cn

Go:   // 手写 map[T]int
来源：http://aa.colortex.cn

Ruby: arr.tally
来源：http://nd.bookmarksfly.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wd.wgjwhj.cn

[D21] 判断是否包含某元素
来源：http://bw.shtwfgs.cn

Py:   x in arr
来源：http://ma.521024.cn

PHP:  in_array($x, $arr, true);
来源：http://ab.huanxung.cn

JS:   arr.includes(x)
来源：http://af.muxihuayi.cn

TS:   arr.includes(x)
来源：http://bu.huanxung.cn

Java: list.contains(x)
来源：http://zx.huixiangedu.cn

Go:   slices.Contains(arr, x)
来源：http://gs.huixinmuqiang.cn

Ruby: arr.include?(x)
来源：http://dz.9csxet.cn

C#:   list.Contains(x)
来源：http://zy.chemitech.net.cn

[D22] 复制数组（避免共享引用）
来源：http://ut.wgjwhj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qp.huixinmuqiang.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://sd.jctech888.com.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://pk.muxihuayi.cn

TS:   [...arr];
来源：http://kk.huanxung.cn

Java: new ArrayList<>(list);
来源：http://em.shxzukj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://hg.bookmarksfly.cn

Ruby: arr.dup;  arr.clone
来源：http://rs.newstarts.cn

C#:   new List<int>(list);
来源：http://wz.panjiajie.cn

[D23] reduce 累积计算
来源：http://hb.muxihuayi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ja.szsharing.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qh.yuntaijiaju.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fp.bjjhwx.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hu.huanxung.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://nl.jctech888.com.cn

Go:   // 手写循环
来源：http://ki.shxzskj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://nb.bjjhwx.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://uh.9csxet.cn

[D24] 字典 / Map 基本操作
来源：http://wh.jctech888.com.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kw.521024.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ow.bjjhwx.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wk.bookmarksfly.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vn.yuntaijiaju.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qn.yuexingan06.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fl.huixinmuqiang.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bi.huixinmuqiang.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rl.shxzskj.cn

[D25] Set 集合去重与交并差
来源：http://wo.jianghongdianzi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vt.9csxet.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://yt.gzmigu.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://dh.hnjuh.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ms.jctech888.com.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://te.shtwfgs.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zo.jctech888.com.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://yn.yuexingan06.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://co.gzmigu.cn

[D26] 数组转字符串
来源：http://yw.yuntaijiaju.cn

Py:   ", ".join(map(str, arr))
来源：http://km.colortex.cn

PHP:  implode(", ", $arr);
来源：http://mq.yuexingan06.cn

JS:   arr.join(", ")
来源：http://jo.muxihuayi.cn

TS:   arr.join(", ")
来源：http://fp.huixinmuqiang.cn

Java: String.join(", ", list)
来源：http://ty.yuexingan06.cn

Go:   strings.Join(strs, ", ")
来源：http://oh.shtwfgs.cn

Ruby: arr.join(", ")
来源：http://eo.asd995.cn

C#:   string.Join(", ", list)
来源：http://qw.hnjuh.cn

================================================================================
来源：http://th.lnxyls.cn

E. 字符串处理
来源：http://qj.lnxyls.cn

================================================================================
来源：http://vk.shxzskj.cn

[E01] 拼接字符串
来源：http://nk.huixiangedu.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ev.asd995.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zw.gzmigu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tv.chemitech.net.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tl.bookmarksfly.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pc.szxytkj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://oq.szxytkj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jz.jctech888.com.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xv.yuexingan06.cn

[E02] 重复字符串
来源：http://mb.huixinmuqiang.cn

Py:   "ab" * 3
来源：http://oj.colortex.cn

PHP:  str_repeat("ab", 3);
来源：http://pf.shxzskj.cn

JS:   "ab".repeat(3)
来源：http://ti.szxytkj.cn

TS:   "ab".repeat(3)
来源：http://km.yuntaijiaju.cn

Java: "ab".repeat(3)
来源：http://vw.bjjhwx.cn

Go:   strings.Repeat("ab", 3)
来源：http://sa.huanxung.cn

Ruby: "ab" * 3
来源：http://io.szxytkj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dx.bookmarksfly.cn

[E03] 截取子串
来源：http://vo.szxytkj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vh.jctech888.com.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xj.jctech888.com.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://uf.panjiajie.cn

TS:   s.slice(1, 4)
来源：http://if.yuexingan06.cn

Java: s.substring(1, 4)
来源：http://iy.hahajie.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bv.gzmigu.cn

Ruby: s[1, 3];  s[1..3]
来源：http://la.jctech888.com.cn

C#:   s.Substring(1, 3)
来源：http://fa.jianghongdianzi.cn

[E04] 查找子串位置
来源：http://ug.hnjuh.cn

Py:   s.find("x");  s.index("x")
来源：http://cc.nicolike.cn

PHP:  strpos($s, "x");
来源：http://kr.nicolike.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mu.huanxung.cn

TS:   s.indexOf("x")
来源：http://md.521024.cn

Java: s.indexOf("x")
来源：http://xo.haigaiapp.cn

Go:   strings.Index(s, "x")
来源：http://gx.newstarts.cn

Ruby: s.index("x")
来源：http://oo.colortex.cn

C#:   s.IndexOf("x")
来源：http://hp.newstarts.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://da.nszjky.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wf.nicolike.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://si.huixiangedu.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cr.colortex.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://kf.newstarts.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yv.lnxyls.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://nv.shxzskj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ou.asd995.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wz.panjiajie.cn

[E06] 替换子串
来源：http://xs.9csxet.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ug.shxzskj.cn

PHP:  str_replace("a", "b", $s);
来源：http://jl.bookmarksfly.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vp.nszjky.cn

TS:   s.replaceAll("a", "b")
来源：http://ra.chemitech.net.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ne.newstarts.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://he.colortex.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://pj.521024.cn

C#:   s.Replace("a", "b")
来源：http://ct.haigaiapp.cn

[E07] 按分隔符拆分
来源：http://vw.yuexingan06.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ub.hnjuh.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://he.shxzukj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://kz.hahajie.cn

TS:   s.split(",")
来源：http://ob.szsharing.cn

Java: s.split(",");  s.split("\\s+")
来源：http://po.huixinmuqiang.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ld.bookmarksfly.cn

Ruby: s.split(",");  s.split
来源：http://zm.shxzukj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://by.jctech888.com.cn

[E08] 数组按分隔符合并
来源：http://ct.huanxung.cn

Py:   ",".join(items)
来源：http://vf.shxzskj.cn

PHP:  implode(",", $items);
来源：http://ig.colortex.cn

JS:   items.join(",")
来源：http://fy.muxihuayi.cn

TS:   items.join(",")
来源：http://lb.shxzukj.cn

Java: String.join(",", items)
来源：http://ya.hnjuh.cn

Go:   strings.Join(items, ",")
来源：http://lk.chemitech.net.cn

Ruby: items.join(",")
来源：http://vn.9csxet.cn

C#:   string.Join(",", items)
来源：http://oe.yuexingan06.cn

[E09] 去除所有空白字符
来源：http://ic.shtwfgs.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://yh.lnxyls.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qo.chemitech.net.cn

JS:   s.replace(/\s+/g, "")
来源：http://ew.nicolike.cn

TS:   s.replace(/\s+/g, "")
来源：http://ax.bjjhwx.cn

Java: s.replaceAll("\\s+", "")
来源：http://lz.yuntaijiaju.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://oy.huixinmuqiang.cn

Ruby: s.gsub(/\s+/, "")
来源：http://lo.hnjuh.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qt.shtwfgs.cn

[E10] 左侧补零 / 定长填充
来源：http://wm.shxzukj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ze.shxzukj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://up.chemitech.net.cn

JS:   "7".padStart(3, "0")
来源：http://ds.huanxung.cn

TS:   "7".padStart(3, "0")
来源：http://gi.hnjuh.cn

Java: String.format("%03d", 7)
来源：http://tw.colortex.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://qi.shxzskj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lq.hahajie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ft.shxzskj.cn

[E11] 反转字符串
来源：http://xl.muxihuayi.cn

Py:   s[::-1]
来源：http://dd.panjiajie.cn

PHP:  strrev($s);
来源：http://zx.jctech888.com.cn

JS:   [...s].reverse().join("")
来源：http://ef.jctech888.com.cn

TS:   [...s].reverse().join("")
来源：http://cw.colortex.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://mu.haigaiapp.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ps.szsharing.cn

Ruby: s.reverse
来源：http://fc.szsharing.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ts.yuexingan06.cn

[E12] 统计某字符出现次数
来源：http://kf.newstarts.cn

Py:   s.count("a")
来源：http://nd.shtwfgs.cn

PHP:  substr_count($s, "a");
来源：http://rr.shxzskj.cn

JS:   s.split("a").length - 1
来源：http://sm.huixiangedu.cn

TS:   s.split("a").length - 1
来源：http://yu.lnxyls.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dk.521024.cn

Go:   strings.Count(s, "a")
来源：http://yy.shxzukj.cn

Ruby: s.count("a")
来源：http://gj.huanxung.cn

C#:   s.Count(c => c == 'a')
来源：http://zw.huixiangedu.cn

[E13] 逐字符遍历
来源：http://gx.asd995.cn

Py:   for ch in s: print(ch)
来源：http://lx.shxzukj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bk.shxzskj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://lc.gzmigu.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://or.521024.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://za.jctech888.com.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://od.jianghongdianzi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://mu.huixiangedu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dg.yuexingan06.cn

[E14] URL 编码与 Base64
来源：http://mm.huixiangedu.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://yu.shtwfgs.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://yg.panjiajie.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://se.hahajie.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://uv.muxihuayi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mj.huixiangedu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://kt.521024.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bs.huixiangedu.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wy.muxihuayi.cn

[E15] HTML 转义 / 反转义
来源：http://ic.huixiangedu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://lc.szsharing.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zx.shxzukj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zf.lnxyls.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://jd.shxzskj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://cl.bjjhwx.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zq.wgjwhj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pf.huixiangedu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zn.jctech888.com.cn

[E16] 数字千分位
来源：http://zl.nicolike.cn

Py:   f"{1234567:,}"
来源：http://vh.nicolike.cn

PHP:  number_format(1234567);
来源：http://ov.wgjwhj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ka.szxytkj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://cw.chemitech.net.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://co.bookmarksfly.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://si.hahajie.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ig.wgjwhj.cn

C#:   1234567.ToString("N0")
来源：http://ho.hnjuh.cn

[E17] 首字母大写
来源：http://bb.yuntaijiaju.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://js.huanxung.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ub.huanxung.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ct.yuexingan06.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zf.9csxet.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ss.shtwfgs.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kh.huixiangedu.cn

Ruby: s.capitalize
来源：http://wp.chemitech.net.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://my.haigaiapp.cn

[E18] 模板占位符替换
来源：http://qi.newstarts.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://it.lnxyls.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bs.huanxung.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zk.chemitech.net.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ya.wgjwhj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rh.shxzukj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://eh.huixinmuqiang.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://tv.panjiajie.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gv.hnjuh.cn

[E19] 多行文本按行拆分
来源：http://qy.gzmigu.cn

Py:   s.splitlines()
来源：http://jw.asd995.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://op.nszjky.cn

JS:   s.split(/\r?\n/)
来源：http://bk.szsharing.cn

TS:   s.split(/\r?\n/)
来源：http://da.asd995.cn

Java: s.lines().toList()
来源：http://kt.huixiangedu.cn

Go:   strings.Split(s, "\n")
来源：http://vo.panjiajie.cn

Ruby: s.lines
来源：http://xg.yuntaijiaju.cn

C#:   s.Split('\n')
来源：http://at.colortex.cn

[E20] 判断字符串是否为空
来源：http://ji.wgjwhj.cn

Py:   if not s:
来源：http://te.haigaiapp.cn


<!-- 参考信息 -->