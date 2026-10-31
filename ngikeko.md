代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ze.bjjhwx.cn

JS:   arr.filter(x => x > 3)
来源：http://af.muxihuayi.cn

TS:   arr.filter(x => x > 3)
来源：http://hp.huixiangedu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://no.shxzukj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wi.haigaiapp.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ck.gzmigu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://nd.lnxyls.cn

[D14] 映射转换（每个元素变形）
来源：http://ba.jianghongdianzi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qr.panjiajie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ab.muxihuayi.cn

JS:   arr.map(x => x * 2)
来源：http://ga.szxytkj.cn

TS:   arr.map(x => x * 2)
来源：http://de.huixiangedu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://qb.yuexingan06.cn

Go:   // 手写循环
来源：http://kq.chemitech.net.cn

Ruby: arr.map { |x| x * 2 }
来源：http://dg.yuntaijiaju.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://pa.yuexingan06.cn

[D15] 去重
来源：http://nu.szxytkj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xd.jianghongdianzi.cn

PHP:  array_unique($arr);
来源：http://on.huixiangedu.cn

JS:   [...new Set(arr)]
来源：http://bd.hahajie.cn

TS:   [...new Set(arr)]
来源：http://om.muxihuayi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qa.shtwfgs.cn

Go:   // 用 map[T]struct{} 手写
来源：http://xc.nicolike.cn

Ruby: arr.uniq
来源：http://sp.yuexingan06.cn

C#:   list.Distinct().ToList()
来源：http://oz.huixiangedu.cn

[D16] 求和与平均值
来源：http://mf.newstarts.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zy.huanxung.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hv.shxzukj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wm.huanxung.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ha.newstarts.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qg.szsharing.cn

Go:   // 手写循环累加
来源：http://xe.nicolike.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zx.chemitech.net.cn

C#:   list.Sum();  list.Average()
来源：http://su.yuntaijiaju.cn

[D17] 最大值与最小值
来源：http://vz.yuntaijiaju.cn

Py:   max(arr);  min(arr)
来源：http://ln.bjjhwx.cn

PHP:  max($arr);  min($arr);
来源：http://is.9csxet.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jv.panjiajie.cn

TS:   Math.max(...arr);
来源：http://nn.nicolike.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://mw.huixinmuqiang.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zh.muxihuayi.cn

Ruby: arr.max;  arr.min
来源：http://li.yuntaijiaju.cn

C#:   list.Max();  list.Min()
来源：http://yk.9csxet.cn

[D18] 扁平化嵌套数组
来源：http://lg.bookmarksfly.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://gz.huixiangedu.cn

PHP:  array_merge(...$nested);
来源：http://mt.yuntaijiaju.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wc.huixinmuqiang.cn

TS:   nested.flat();
来源：http://qv.nicolike.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ig.panjiajie.cn

Go:   // 手写双层循环
来源：http://tu.haigaiapp.cn

Ruby: nested.flatten
来源：http://vr.chemitech.net.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://rw.9csxet.cn

[D19] 按字段分组
来源：http://ow.yuexingan06.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ca.shtwfgs.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://uj.hahajie.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://uj.hahajie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ki.bjjhwx.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qr.wgjwhj.cn

Go:   // 手写 map[string][]T
来源：http://yd.hnjuh.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://di.jctech888.com.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://iq.jctech888.com.cn

[D20] 统计每个元素出现次数
来源：http://cl.yuntaijiaju.cn

Py:   Counter(arr)
来源：http://bn.bookmarksfly.cn

PHP:  array_count_values($arr);
来源：http://bm.shxzskj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fu.chemitech.net.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sk.jianghongdianzi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xx.nszjky.cn

Go:   // 手写 map[T]int
来源：http://io.bookmarksfly.cn

Ruby: arr.tally
来源：http://yl.haigaiapp.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://sy.hnjuh.cn

[D21] 判断是否包含某元素
来源：http://og.chemitech.net.cn

Py:   x in arr
来源：http://jp.yuntaijiaju.cn

PHP:  in_array($x, $arr, true);
来源：http://eo.shxzskj.cn

JS:   arr.includes(x)
来源：http://ct.bjjhwx.cn

TS:   arr.includes(x)
来源：http://hq.hnjuh.cn

Java: list.contains(x)
来源：http://mq.lnxyls.cn

Go:   slices.Contains(arr, x)
来源：http://vn.jianghongdianzi.cn

Ruby: arr.include?(x)
来源：http://sb.yuntaijiaju.cn

C#:   list.Contains(x)
来源：http://us.bjjhwx.cn

[D22] 复制数组（避免共享引用）
来源：http://wi.shxzskj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://rl.nszjky.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ns.jianghongdianzi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://sw.jctech888.com.cn

TS:   [...arr];
来源：http://js.szxytkj.cn

Java: new ArrayList<>(list);
来源：http://gv.panjiajie.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ic.hahajie.cn

Ruby: arr.dup;  arr.clone
来源：http://dn.shxzskj.cn

C#:   new List<int>(list);
来源：http://gy.newstarts.cn

[D23] reduce 累积计算
来源：http://gn.shxzskj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://dp.muxihuayi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ce.asd995.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rl.panjiajie.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://im.szxytkj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://jv.chemitech.net.cn

Go:   // 手写循环
来源：http://cj.shxzukj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://we.panjiajie.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ap.szxytkj.cn

[D24] 字典 / Map 基本操作
来源：http://yj.shxzskj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://dh.gzmigu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://sk.szxytkj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://nd.szsharing.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://pp.jianghongdianzi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hr.yuntaijiaju.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gj.huixinmuqiang.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vn.haigaiapp.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://op.hnjuh.cn

[D25] Set 集合去重与交并差
来源：http://bl.yuexingan06.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ij.yuexingan06.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pl.asd995.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://pt.chemitech.net.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hu.bjjhwx.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://yg.gzmigu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jm.9csxet.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://iz.nicolike.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jk.szxytkj.cn

[D26] 数组转字符串
来源：http://do.chemitech.net.cn

Py:   ", ".join(map(str, arr))
来源：http://ec.asd995.cn

PHP:  implode(", ", $arr);
来源：http://cp.yuntaijiaju.cn

JS:   arr.join(", ")
来源：http://hy.haigaiapp.cn

TS:   arr.join(", ")
来源：http://ov.huixiangedu.cn

Java: String.join(", ", list)
来源：http://zm.panjiajie.cn

Go:   strings.Join(strs, ", ")
来源：http://yc.szsharing.cn

Ruby: arr.join(", ")
来源：http://oe.huixiangedu.cn

C#:   string.Join(", ", list)
来源：http://wu.nszjky.cn

================================================================================
来源：http://mz.bookmarksfly.cn

E. 字符串处理
来源：http://uf.haigaiapp.cn

================================================================================
来源：http://bn.hnjuh.cn

[E01] 拼接字符串
来源：http://hp.bookmarksfly.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ki.colortex.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://er.panjiajie.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vm.nszjky.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zu.colortex.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rm.huixinmuqiang.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://kk.huixiangedu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://nn.lnxyls.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://te.jianghongdianzi.cn

[E02] 重复字符串
来源：http://et.shxzukj.cn

Py:   "ab" * 3
来源：http://kb.huanxung.cn

PHP:  str_repeat("ab", 3);
来源：http://yl.9csxet.cn

JS:   "ab".repeat(3)
来源：http://im.szsharing.cn

TS:   "ab".repeat(3)
来源：http://tn.haigaiapp.cn

Java: "ab".repeat(3)
来源：http://vl.huixinmuqiang.cn

Go:   strings.Repeat("ab", 3)
来源：http://fx.huixiangedu.cn

Ruby: "ab" * 3
来源：http://zu.huixiangedu.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ys.huanxung.cn

[E03] 截取子串
来源：http://er.shxzskj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nd.colortex.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gg.newstarts.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mi.muxihuayi.cn

TS:   s.slice(1, 4)
来源：http://rh.panjiajie.cn

Java: s.substring(1, 4)
来源：http://qp.szsharing.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://no.jctech888.com.cn

Ruby: s[1, 3];  s[1..3]
来源：http://is.haigaiapp.cn

C#:   s.Substring(1, 3)
来源：http://ez.chemitech.net.cn

[E04] 查找子串位置
来源：http://nr.shtwfgs.cn

Py:   s.find("x");  s.index("x")
来源：http://cr.hnjuh.cn

PHP:  strpos($s, "x");
来源：http://gt.9csxet.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zv.huixiangedu.cn

TS:   s.indexOf("x")
来源：http://az.9csxet.cn

Java: s.indexOf("x")
来源：http://hv.bjjhwx.cn

Go:   strings.Index(s, "x")
来源：http://uo.9csxet.cn

Ruby: s.index("x")
来源：http://ao.panjiajie.cn

C#:   s.IndexOf("x")
来源：http://ny.hnjuh.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://tc.jctech888.com.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qt.szxytkj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://li.haigaiapp.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fn.bookmarksfly.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://yv.yuexingan06.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nw.huanxung.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ix.huanxung.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://io.jianghongdianzi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ig.muxihuayi.cn

[E06] 替换子串
来源：http://yk.nszjky.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gu.jianghongdianzi.cn

PHP:  str_replace("a", "b", $s);
来源：http://ib.szsharing.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ct.panjiajie.cn

TS:   s.replaceAll("a", "b")
来源：http://tp.shtwfgs.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ug.szsharing.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://pe.lnxyls.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jm.bjjhwx.cn

C#:   s.Replace("a", "b")
来源：http://mx.bjjhwx.cn

[E07] 按分隔符拆分
来源：http://yc.shtwfgs.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ne.szxytkj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://us.huixiangedu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://lj.hnjuh.cn

TS:   s.split(",")
来源：http://ua.nszjky.cn

Java: s.split(",");  s.split("\\s+")
来源：http://hm.shxzskj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://cb.shxzskj.cn

Ruby: s.split(",");  s.split
来源：http://fc.hahajie.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pi.521024.cn

[E08] 数组按分隔符合并
来源：http://tg.panjiajie.cn

Py:   ",".join(items)
来源：http://my.panjiajie.cn

PHP:  implode(",", $items);
来源：http://wz.panjiajie.cn

JS:   items.join(",")
来源：http://pt.asd995.cn

TS:   items.join(",")
来源：http://yl.shxzukj.cn

Java: String.join(",", items)
来源：http://we.wgjwhj.cn

Go:   strings.Join(items, ",")
来源：http://nn.bookmarksfly.cn

Ruby: items.join(",")
来源：http://dk.nszjky.cn

C#:   string.Join(",", items)
来源：http://bp.bookmarksfly.cn

[E09] 去除所有空白字符
来源：http://kw.newstarts.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qr.newstarts.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bw.521024.cn

JS:   s.replace(/\s+/g, "")
来源：http://gd.shtwfgs.cn

TS:   s.replace(/\s+/g, "")
来源：http://eh.9csxet.cn

Java: s.replaceAll("\\s+", "")
来源：http://kl.shtwfgs.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://xw.szxytkj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://lq.nszjky.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://dl.521024.cn

[E10] 左侧补零 / 定长填充
来源：http://gf.nicolike.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zu.lnxyls.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wd.haigaiapp.cn

JS:   "7".padStart(3, "0")
来源：http://lm.asd995.cn

TS:   "7".padStart(3, "0")
来源：http://cg.jctech888.com.cn

Java: String.format("%03d", 7)
来源：http://ve.muxihuayi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ty.shtwfgs.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://de.muxihuayi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ts.shxzskj.cn

[E11] 反转字符串
来源：http://yy.hahajie.cn

Py:   s[::-1]
来源：http://th.521024.cn

PHP:  strrev($s);
来源：http://my.shxzskj.cn

JS:   [...s].reverse().join("")
来源：http://us.haigaiapp.cn

TS:   [...s].reverse().join("")
来源：http://sv.yuntaijiaju.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://wl.huixiangedu.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://yd.shxzskj.cn

Ruby: s.reverse
来源：http://kk.gzmigu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://xs.hnjuh.cn

[E12] 统计某字符出现次数
来源：http://pv.jctech888.com.cn

Py:   s.count("a")
来源：http://qe.9csxet.cn

PHP:  substr_count($s, "a");
来源：http://gl.bjjhwx.cn

JS:   s.split("a").length - 1
来源：http://it.lnxyls.cn

TS:   s.split("a").length - 1
来源：http://ox.hahajie.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yi.lnxyls.cn

Go:   strings.Count(s, "a")
来源：http://ed.huanxung.cn

Ruby: s.count("a")
来源：http://pm.shxzskj.cn

C#:   s.Count(c => c == 'a')
来源：http://uy.521024.cn

[E13] 逐字符遍历
来源：http://ct.panjiajie.cn

Py:   for ch in s: print(ch)
来源：http://bm.wgjwhj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zm.bookmarksfly.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://zs.bjjhwx.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://wt.521024.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mp.huixinmuqiang.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://uj.wgjwhj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ql.wgjwhj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fq.szsharing.cn

[E14] URL 编码与 Base64
来源：http://ul.521024.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vy.szxytkj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://yv.wgjwhj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qz.huanxung.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://yp.521024.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zw.shtwfgs.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://we.bjjhwx.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://lc.yuexingan06.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bt.lnxyls.cn

[E15] HTML 转义 / 反转义
来源：http://ar.jianghongdianzi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://lw.colortex.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://yy.panjiajie.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lq.9csxet.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://qw.asd995.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://yr.hnjuh.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xl.nicolike.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pb.asd995.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ar.szsharing.cn

[E16] 数字千分位
来源：http://ll.yuntaijiaju.cn

Py:   f"{1234567:,}"
来源：http://fd.bjjhwx.cn

PHP:  number_format(1234567);
来源：http://zn.9csxet.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ud.wgjwhj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://sp.lnxyls.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://df.bjjhwx.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fy.szxytkj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zw.yuntaijiaju.cn

C#:   1234567.ToString("N0")
来源：http://kr.newstarts.cn

[E17] 首字母大写
来源：http://yb.shtwfgs.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mh.yuexingan06.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://uv.nicolike.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bb.bjjhwx.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sk.9csxet.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://az.colortex.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://cl.muxihuayi.cn

Ruby: s.capitalize
来源：http://zo.jianghongdianzi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://bv.yuntaijiaju.cn

[E18] 模板占位符替换
来源：http://fh.nszjky.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wm.haigaiapp.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://rp.panjiajie.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://bk.newstarts.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://xa.yuexingan06.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ji.haigaiapp.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://eg.panjiajie.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://tx.bookmarksfly.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ud.9csxet.cn

[E19] 多行文本按行拆分
来源：http://bw.hahajie.cn

Py:   s.splitlines()
来源：http://fv.haigaiapp.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vv.shtwfgs.cn

JS:   s.split(/\r?\n/)
来源：http://vh.jianghongdianzi.cn

TS:   s.split(/\r?\n/)
来源：http://kb.jctech888.com.cn

Java: s.lines().toList()
来源：http://qx.jianghongdianzi.cn

Go:   strings.Split(s, "\n")
来源：http://fv.gzmigu.cn

Ruby: s.lines
来源：http://na.hnjuh.cn

C#:   s.Split('\n')
来源：http://nw.yuntaijiaju.cn

[E20] 判断字符串是否为空
来源：http://ev.nicolike.cn

Py:   if not s:
来源：http://jp.shxzskj.cn


<!-- 参考信息 -->