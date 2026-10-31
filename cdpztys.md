代发 wailian999

C#:   list.Reverse();
来源：http://up.bjjhwx.cn

[D12] 查找元素下标
来源：http://vp.nszjky.cn

Py:   arr.index(x);  x in arr
来源：http://sw.gzmigu.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wt.asd995.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xv.chemitech.net.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wz.asd995.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qi.huanxung.cn

Go:   slices.Index(arr, x)
来源：http://bj.huixiangedu.cn

Ruby: arr.index(x)
来源：http://jy.jianghongdianzi.cn

C#:   list.IndexOf(x);
来源：http://yc.asd995.cn

[D13] 过滤（保留满足条件的）
来源：http://me.muxihuayi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ds.bookmarksfly.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ud.shxzskj.cn

JS:   arr.filter(x => x > 3)
来源：http://vh.huixiangedu.cn

TS:   arr.filter(x => x > 3)
来源：http://vv.bjjhwx.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qj.asd995.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://cg.bookmarksfly.cn

Ruby: arr.select { |x| x > 3 }
来源：http://mg.jianghongdianzi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ym.newstarts.cn

[D14] 映射转换（每个元素变形）
来源：http://zs.huixinmuqiang.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://pp.newstarts.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://uj.hnjuh.cn

JS:   arr.map(x => x * 2)
来源：http://ai.asd995.cn

TS:   arr.map(x => x * 2)
来源：http://tw.muxihuayi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://yd.shxzskj.cn

Go:   // 手写循环
来源：http://db.huixinmuqiang.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ed.gzmigu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://vr.newstarts.cn

[D15] 去重
来源：http://qe.shxzukj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yi.panjiajie.cn

PHP:  array_unique($arr);
来源：http://oi.haigaiapp.cn

JS:   [...new Set(arr)]
来源：http://ri.jctech888.com.cn

TS:   [...new Set(arr)]
来源：http://cy.9csxet.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qe.muxihuayi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ic.yuntaijiaju.cn

Ruby: arr.uniq
来源：http://uz.huixinmuqiang.cn

C#:   list.Distinct().ToList()
来源：http://re.nszjky.cn

[D16] 求和与平均值
来源：http://ks.huanxung.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dh.jctech888.com.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ik.wgjwhj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gi.shtwfgs.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://cn.bookmarksfly.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zk.colortex.cn

Go:   // 手写循环累加
来源：http://ee.bookmarksfly.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jj.521024.cn

C#:   list.Sum();  list.Average()
来源：http://zp.yuexingan06.cn

[D17] 最大值与最小值
来源：http://oz.szsharing.cn

Py:   max(arr);  min(arr)
来源：http://lv.newstarts.cn

PHP:  max($arr);  min($arr);
来源：http://jg.szxytkj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://lb.jianghongdianzi.cn

TS:   Math.max(...arr);
来源：http://ne.wgjwhj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://br.shxzskj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ce.huanxung.cn

Ruby: arr.max;  arr.min
来源：http://fj.lnxyls.cn

C#:   list.Max();  list.Min()
来源：http://lf.yuexingan06.cn

[D18] 扁平化嵌套数组
来源：http://ym.yuexingan06.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mx.521024.cn

PHP:  array_merge(...$nested);
来源：http://mj.jianghongdianzi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fv.muxihuayi.cn

TS:   nested.flat();
来源：http://rh.gzmigu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yv.newstarts.cn

Go:   // 手写双层循环
来源：http://ae.gzmigu.cn

Ruby: nested.flatten
来源：http://et.haigaiapp.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ff.nszjky.cn

[D19] 按字段分组
来源：http://lj.colortex.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fe.hnjuh.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xo.newstarts.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bt.huixinmuqiang.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://kp.hnjuh.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jm.panjiajie.cn

Go:   // 手写 map[string][]T
来源：http://ih.asd995.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://lm.gzmigu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ke.bjjhwx.cn

[D20] 统计每个元素出现次数
来源：http://xg.nicolike.cn

Py:   Counter(arr)
来源：http://cl.szsharing.cn

PHP:  array_count_values($arr);
来源：http://fl.yuexingan06.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kg.gzmigu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ag.shxzukj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://od.hahajie.cn

Go:   // 手写 map[T]int
来源：http://gz.nicolike.cn

Ruby: arr.tally
来源：http://lk.haigaiapp.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fg.szsharing.cn

[D21] 判断是否包含某元素
来源：http://tg.szsharing.cn

Py:   x in arr
来源：http://qt.szsharing.cn

PHP:  in_array($x, $arr, true);
来源：http://se.lnxyls.cn

JS:   arr.includes(x)
来源：http://zk.shtwfgs.cn

TS:   arr.includes(x)
来源：http://vp.gzmigu.cn

Java: list.contains(x)
来源：http://um.panjiajie.cn

Go:   slices.Contains(arr, x)
来源：http://jd.szxytkj.cn

Ruby: arr.include?(x)
来源：http://xk.szxytkj.cn

C#:   list.Contains(x)
来源：http://gb.wgjwhj.cn

[D22] 复制数组（避免共享引用）
来源：http://rp.bookmarksfly.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vv.jctech888.com.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://yw.hnjuh.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://az.asd995.cn

TS:   [...arr];
来源：http://uc.521024.cn

Java: new ArrayList<>(list);
来源：http://yo.szxytkj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ws.haigaiapp.cn

Ruby: arr.dup;  arr.clone
来源：http://pt.hnjuh.cn

C#:   new List<int>(list);
来源：http://bd.panjiajie.cn

[D23] reduce 累积计算
来源：http://kc.newstarts.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://nz.yuexingan06.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kd.shtwfgs.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sg.hnjuh.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wg.wgjwhj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ud.hahajie.cn

Go:   // 手写循环
来源：http://vt.panjiajie.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jr.lnxyls.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ce.nszjky.cn

[D24] 字典 / Map 基本操作
来源：http://tq.521024.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gy.szsharing.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://br.9csxet.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dc.jctech888.com.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://pq.huixiangedu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wh.nszjky.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gf.huanxung.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ab.gzmigu.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ge.huanxung.cn

[D25] Set 集合去重与交并差
来源：http://bz.huixinmuqiang.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nd.lnxyls.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ix.panjiajie.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wx.jctech888.com.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vy.hnjuh.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://on.huixinmuqiang.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://fr.szsharing.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://py.wgjwhj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qn.jctech888.com.cn

[D26] 数组转字符串
来源：http://hk.lnxyls.cn

Py:   ", ".join(map(str, arr))
来源：http://md.huixinmuqiang.cn

PHP:  implode(", ", $arr);
来源：http://fn.szxytkj.cn

JS:   arr.join(", ")
来源：http://uc.muxihuayi.cn

TS:   arr.join(", ")
来源：http://wp.colortex.cn

Java: String.join(", ", list)
来源：http://fv.shxzskj.cn

Go:   strings.Join(strs, ", ")
来源：http://al.bjjhwx.cn

Ruby: arr.join(", ")
来源：http://un.chemitech.net.cn

C#:   string.Join(", ", list)
来源：http://re.yuexingan06.cn

================================================================================
来源：http://sv.shtwfgs.cn

E. 字符串处理
来源：http://eo.panjiajie.cn

================================================================================
来源：http://nb.bjjhwx.cn

[E01] 拼接字符串
来源：http://rq.huixiangedu.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xm.chemitech.net.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hq.muxihuayi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://te.panjiajie.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://yx.521024.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://kw.asd995.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yf.huixiangedu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://sm.huixinmuqiang.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://cm.521024.cn

[E02] 重复字符串
来源：http://pl.hnjuh.cn

Py:   "ab" * 3
来源：http://hk.yuntaijiaju.cn

PHP:  str_repeat("ab", 3);
来源：http://zt.yuexingan06.cn

JS:   "ab".repeat(3)
来源：http://hh.jctech888.com.cn

TS:   "ab".repeat(3)
来源：http://ae.huixinmuqiang.cn

Java: "ab".repeat(3)
来源：http://od.huixinmuqiang.cn

Go:   strings.Repeat("ab", 3)
来源：http://ts.colortex.cn

Ruby: "ab" * 3
来源：http://an.shxzskj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qr.yuntaijiaju.cn

[E03] 截取子串
来源：http://ho.yuexingan06.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ym.yuexingan06.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vf.huixinmuqiang.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ks.yuntaijiaju.cn

TS:   s.slice(1, 4)
来源：http://sk.shtwfgs.cn

Java: s.substring(1, 4)
来源：http://jp.colortex.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://iz.shtwfgs.cn

Ruby: s[1, 3];  s[1..3]
来源：http://pi.hnjuh.cn

C#:   s.Substring(1, 3)
来源：http://bo.asd995.cn

[E04] 查找子串位置
来源：http://zg.hnjuh.cn

Py:   s.find("x");  s.index("x")
来源：http://sd.jianghongdianzi.cn

PHP:  strpos($s, "x");
来源：http://lj.shtwfgs.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ns.muxihuayi.cn

TS:   s.indexOf("x")
来源：http://dc.chemitech.net.cn

Java: s.indexOf("x")
来源：http://sd.nicolike.cn

Go:   strings.Index(s, "x")
来源：http://jh.shxzskj.cn

Ruby: s.index("x")
来源：http://au.hahajie.cn

C#:   s.IndexOf("x")
来源：http://fj.jianghongdianzi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://fx.muxihuayi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wj.shtwfgs.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fm.huixinmuqiang.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bc.nicolike.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://cq.jctech888.com.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ag.haigaiapp.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hx.gzmigu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://eg.shxzukj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fp.huixinmuqiang.cn

[E06] 替换子串
来源：http://zo.9csxet.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://is.muxihuayi.cn

PHP:  str_replace("a", "b", $s);
来源：http://zs.asd995.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gx.panjiajie.cn

TS:   s.replaceAll("a", "b")
来源：http://qt.nszjky.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xm.asd995.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gz.bookmarksfly.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://rm.yuntaijiaju.cn

C#:   s.Replace("a", "b")
来源：http://wj.9csxet.cn

[E07] 按分隔符拆分
来源：http://gv.9csxet.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ty.yuexingan06.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gc.huanxung.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://lm.huixiangedu.cn

TS:   s.split(",")
来源：http://do.lnxyls.cn

Java: s.split(",");  s.split("\\s+")
来源：http://at.nicolike.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vg.nicolike.cn

Ruby: s.split(",");  s.split
来源：http://fj.jctech888.com.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jr.huanxung.cn

[E08] 数组按分隔符合并
来源：http://zh.yuexingan06.cn

Py:   ",".join(items)
来源：http://lo.521024.cn

PHP:  implode(",", $items);
来源：http://hj.521024.cn

JS:   items.join(",")
来源：http://yr.newstarts.cn

TS:   items.join(",")
来源：http://la.muxihuayi.cn

Java: String.join(",", items)
来源：http://fm.shtwfgs.cn

Go:   strings.Join(items, ",")
来源：http://hi.muxihuayi.cn

Ruby: items.join(",")
来源：http://de.huixinmuqiang.cn

C#:   string.Join(",", items)
来源：http://bw.muxihuayi.cn

[E09] 去除所有空白字符
来源：http://bt.jianghongdianzi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pw.asd995.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jw.yuntaijiaju.cn

JS:   s.replace(/\s+/g, "")
来源：http://es.shxzskj.cn

TS:   s.replace(/\s+/g, "")
来源：http://xl.yuntaijiaju.cn

Java: s.replaceAll("\\s+", "")
来源：http://pe.chemitech.net.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://oz.szsharing.cn

Ruby: s.gsub(/\s+/, "")
来源：http://mn.hnjuh.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://nz.szsharing.cn

[E10] 左侧补零 / 定长填充
来源：http://pn.chemitech.net.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://pr.haigaiapp.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://yv.panjiajie.cn

JS:   "7".padStart(3, "0")
来源：http://xt.gzmigu.cn

TS:   "7".padStart(3, "0")
来源：http://qk.newstarts.cn

Java: String.format("%03d", 7)
来源：http://pm.bookmarksfly.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://cj.yuntaijiaju.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://je.panjiajie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://sx.shxzskj.cn

[E11] 反转字符串
来源：http://en.521024.cn

Py:   s[::-1]
来源：http://ze.yuntaijiaju.cn

PHP:  strrev($s);
来源：http://to.szsharing.cn

JS:   [...s].reverse().join("")
来源：http://wv.yuntaijiaju.cn

TS:   [...s].reverse().join("")
来源：http://jy.yuntaijiaju.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://no.huixinmuqiang.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://qa.nszjky.cn

Ruby: s.reverse
来源：http://jq.jctech888.com.cn

C#:   new string(s.Reverse().ToArray())
来源：http://qe.521024.cn

[E12] 统计某字符出现次数
来源：http://rb.9csxet.cn

Py:   s.count("a")
来源：http://ik.newstarts.cn

PHP:  substr_count($s, "a");
来源：http://ma.newstarts.cn

JS:   s.split("a").length - 1
来源：http://zv.yuexingan06.cn

TS:   s.split("a").length - 1
来源：http://sb.szsharing.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ax.haigaiapp.cn

Go:   strings.Count(s, "a")
来源：http://dc.wgjwhj.cn

Ruby: s.count("a")
来源：http://cm.hnjuh.cn

C#:   s.Count(c => c == 'a')
来源：http://al.asd995.cn

[E13] 逐字符遍历
来源：http://wk.muxihuayi.cn

Py:   for ch in s: print(ch)
来源：http://lg.szxytkj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tp.bookmarksfly.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://xb.wgjwhj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://nk.szxytkj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ee.panjiajie.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wd.asd995.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://bk.shxzukj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qp.gzmigu.cn

[E14] URL 编码与 Base64
来源：http://ei.shxzskj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://sa.shxzukj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://dt.bookmarksfly.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://pr.lnxyls.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://sh.haigaiapp.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://yk.shxzskj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gn.shtwfgs.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rd.shxzskj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://by.bookmarksfly.cn

[E15] HTML 转义 / 反转义
来源：http://vf.huanxung.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://tt.yuexingan06.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rc.muxihuayi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://sy.nszjky.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://lf.hahajie.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://cg.huanxung.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fw.haigaiapp.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://au.521024.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bg.hnjuh.cn

[E16] 数字千分位
来源：http://ap.newstarts.cn

Py:   f"{1234567:,}"
来源：http://ul.colortex.cn

PHP:  number_format(1234567);
来源：http://en.panjiajie.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ms.haigaiapp.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://wh.chemitech.net.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ch.shxzskj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://uu.521024.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vx.hnjuh.cn

C#:   1234567.ToString("N0")
来源：http://cb.shtwfgs.cn

[E17] 首字母大写
来源：http://bx.shxzukj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fz.shtwfgs.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://pm.521024.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zr.szsharing.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://he.haigaiapp.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vi.shtwfgs.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kx.wgjwhj.cn

Ruby: s.capitalize
来源：http://nk.hahajie.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dw.shxzukj.cn

[E18] 模板占位符替换
来源：http://nq.haigaiapp.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qj.szsharing.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fw.yuexingan06.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://lr.yuexingan06.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://kn.yuexingan06.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ia.huanxung.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jw.shxzskj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ni.muxihuayi.cn


<!-- 参考信息 -->