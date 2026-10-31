代发 wailian999

TS:   [...arr].reverse();
来源：http://ns.yuexingan06.cn

Java: Collections.reverse(list);
来源：http://ph.haigaiapp.cn

Go:   slices.Reverse(arr)
来源：http://jh.muxihuayi.cn

Ruby: arr.reverse
来源：http://bv.shtwfgs.cn

C#:   list.Reverse();
来源：http://oo.colortex.cn

[D12] 查找元素下标
来源：http://st.nicolike.cn

Py:   arr.index(x);  x in arr
来源：http://rr.hahajie.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qd.newstarts.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sb.shtwfgs.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qh.shxzskj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://iw.gzmigu.cn

Go:   slices.Index(arr, x)
来源：http://pc.colortex.cn

Ruby: arr.index(x)
来源：http://jx.bookmarksfly.cn

C#:   list.IndexOf(x);
来源：http://uu.panjiajie.cn

[D13] 过滤（保留满足条件的）
来源：http://cf.newstarts.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ma.shtwfgs.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ju.jctech888.com.cn

JS:   arr.filter(x => x > 3)
来源：http://dl.9csxet.cn

TS:   arr.filter(x => x > 3)
来源：http://ld.colortex.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://er.huixiangedu.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tz.chemitech.net.cn

Ruby: arr.select { |x| x > 3 }
来源：http://qs.asd995.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://qs.bjjhwx.cn

[D14] 映射转换（每个元素变形）
来源：http://ha.shxzukj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://io.jianghongdianzi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ux.gzmigu.cn

JS:   arr.map(x => x * 2)
来源：http://dy.jianghongdianzi.cn

TS:   arr.map(x => x * 2)
来源：http://kh.huanxung.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ww.huixiangedu.cn

Go:   // 手写循环
来源：http://yz.gzmigu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://vc.shxzskj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://az.huanxung.cn

[D15] 去重
来源：http://fw.shtwfgs.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vt.gzmigu.cn

PHP:  array_unique($arr);
来源：http://un.colortex.cn

JS:   [...new Set(arr)]
来源：http://ue.asd995.cn

TS:   [...new Set(arr)]
来源：http://vt.wgjwhj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zq.shxzukj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://et.shxzukj.cn

Ruby: arr.uniq
来源：http://bw.yuntaijiaju.cn

C#:   list.Distinct().ToList()
来源：http://cg.wgjwhj.cn

[D16] 求和与平均值
来源：http://hd.yuexingan06.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ip.jctech888.com.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jw.shtwfgs.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xf.bookmarksfly.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://us.521024.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ec.huixiangedu.cn

Go:   // 手写循环累加
来源：http://su.521024.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nc.huixiangedu.cn

C#:   list.Sum();  list.Average()
来源：http://oa.asd995.cn

[D17] 最大值与最小值
来源：http://ae.szxytkj.cn

Py:   max(arr);  min(arr)
来源：http://nj.nicolike.cn

PHP:  max($arr);  min($arr);
来源：http://ot.haigaiapp.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://kb.lnxyls.cn

TS:   Math.max(...arr);
来源：http://nk.huanxung.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://nm.9csxet.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ug.521024.cn

Ruby: arr.max;  arr.min
来源：http://dk.bjjhwx.cn

C#:   list.Max();  list.Min()
来源：http://oe.9csxet.cn

[D18] 扁平化嵌套数组
来源：http://bq.panjiajie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ov.newstarts.cn

PHP:  array_merge(...$nested);
来源：http://ew.9csxet.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://uj.shxzukj.cn

TS:   nested.flat();
来源：http://mx.lnxyls.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wt.huixiangedu.cn

Go:   // 手写双层循环
来源：http://aj.wgjwhj.cn

Ruby: nested.flatten
来源：http://au.yuntaijiaju.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://yv.bookmarksfly.cn

[D19] 按字段分组
来源：http://zf.huixiangedu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://sp.yuexingan06.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xe.huanxung.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gf.huanxung.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://pq.haigaiapp.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://pm.gzmigu.cn

Go:   // 手写 map[string][]T
来源：http://xx.szxytkj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://gx.yuntaijiaju.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yu.huanxung.cn

[D20] 统计每个元素出现次数
来源：http://rw.shxzskj.cn

Py:   Counter(arr)
来源：http://qk.521024.cn

PHP:  array_count_values($arr);
来源：http://av.haigaiapp.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://to.haigaiapp.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://im.yuexingan06.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vi.shtwfgs.cn

Go:   // 手写 map[T]int
来源：http://hn.yuntaijiaju.cn

Ruby: arr.tally
来源：http://dx.hnjuh.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hr.chemitech.net.cn

[D21] 判断是否包含某元素
来源：http://yp.521024.cn

Py:   x in arr
来源：http://mi.hnjuh.cn

PHP:  in_array($x, $arr, true);
来源：http://gq.nszjky.cn

JS:   arr.includes(x)
来源：http://ad.shtwfgs.cn

TS:   arr.includes(x)
来源：http://cm.chemitech.net.cn

Java: list.contains(x)
来源：http://gw.huanxung.cn

Go:   slices.Contains(arr, x)
来源：http://uq.521024.cn

Ruby: arr.include?(x)
来源：http://uv.jianghongdianzi.cn

C#:   list.Contains(x)
来源：http://pn.shtwfgs.cn

[D22] 复制数组（避免共享引用）
来源：http://ql.shxzukj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hd.jianghongdianzi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xo.hnjuh.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bq.szsharing.cn

TS:   [...arr];
来源：http://vv.shtwfgs.cn

Java: new ArrayList<>(list);
来源：http://jo.shxzskj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://tk.hahajie.cn

Ruby: arr.dup;  arr.clone
来源：http://ty.hahajie.cn

C#:   new List<int>(list);
来源：http://rd.huanxung.cn

[D23] reduce 累积计算
来源：http://me.shtwfgs.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gy.9csxet.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cl.bjjhwx.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wl.jctech888.com.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fa.huixiangedu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://tx.shxzskj.cn

Go:   // 手写循环
来源：http://fd.huixinmuqiang.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gy.gzmigu.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://aa.shxzukj.cn

[D24] 字典 / Map 基本操作
来源：http://of.nicolike.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://uq.bjjhwx.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bc.nszjky.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ak.panjiajie.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://az.shxzukj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bn.hnjuh.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xh.bookmarksfly.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ti.bookmarksfly.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qo.nszjky.cn

[D25] Set 集合去重与交并差
来源：http://pq.szxytkj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ya.huanxung.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://on.muxihuayi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gj.shxzukj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ym.nszjky.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://sw.hnjuh.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jq.panjiajie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://sz.nszjky.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jl.newstarts.cn

[D26] 数组转字符串
来源：http://jd.huixiangedu.cn

Py:   ", ".join(map(str, arr))
来源：http://dn.bookmarksfly.cn

PHP:  implode(", ", $arr);
来源：http://ax.szxytkj.cn

JS:   arr.join(", ")
来源：http://tx.chemitech.net.cn

TS:   arr.join(", ")
来源：http://vi.shxzukj.cn

Java: String.join(", ", list)
来源：http://xg.521024.cn

Go:   strings.Join(strs, ", ")
来源：http://px.bjjhwx.cn

Ruby: arr.join(", ")
来源：http://nt.huanxung.cn

C#:   string.Join(", ", list)
来源：http://dk.huanxung.cn

================================================================================
来源：http://vt.colortex.cn

E. 字符串处理
来源：http://qr.gzmigu.cn

================================================================================
来源：http://xp.huanxung.cn

[E01] 拼接字符串
来源：http://or.szsharing.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gs.hahajie.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ca.szsharing.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://to.muxihuayi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://sj.shxzukj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://bn.gzmigu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://uv.shxzukj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://eg.szxytkj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hg.nszjky.cn

[E02] 重复字符串
来源：http://mc.panjiajie.cn

Py:   "ab" * 3
来源：http://kl.asd995.cn

PHP:  str_repeat("ab", 3);
来源：http://qx.bjjhwx.cn

JS:   "ab".repeat(3)
来源：http://oy.shxzukj.cn

TS:   "ab".repeat(3)
来源：http://bv.wgjwhj.cn

Java: "ab".repeat(3)
来源：http://rr.lnxyls.cn

Go:   strings.Repeat("ab", 3)
来源：http://of.bookmarksfly.cn

Ruby: "ab" * 3
来源：http://cl.panjiajie.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ze.huixiangedu.cn

[E03] 截取子串
来源：http://bh.colortex.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qg.shxzskj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ht.colortex.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://re.nicolike.cn

TS:   s.slice(1, 4)
来源：http://tm.nszjky.cn

Java: s.substring(1, 4)
来源：http://uv.szsharing.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://yb.yuntaijiaju.cn

Ruby: s[1, 3];  s[1..3]
来源：http://mx.wgjwhj.cn

C#:   s.Substring(1, 3)
来源：http://dx.lnxyls.cn

[E04] 查找子串位置
来源：http://sh.huixinmuqiang.cn

Py:   s.find("x");  s.index("x")
来源：http://rj.bjjhwx.cn

PHP:  strpos($s, "x");
来源：http://rd.bjjhwx.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://nv.chemitech.net.cn

TS:   s.indexOf("x")
来源：http://uh.hahajie.cn

Java: s.indexOf("x")
来源：http://on.shxzskj.cn

Go:   strings.Index(s, "x")
来源：http://kq.nszjky.cn

Ruby: s.index("x")
来源：http://pk.yuntaijiaju.cn

C#:   s.IndexOf("x")
来源：http://qn.9csxet.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://iq.haigaiapp.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://lu.muxihuayi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ft.huanxung.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ts.gzmigu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://dz.szsharing.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gn.asd995.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zb.huixiangedu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zp.szxytkj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fp.shxzskj.cn

[E06] 替换子串
来源：http://zo.panjiajie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qk.shxzskj.cn

PHP:  str_replace("a", "b", $s);
来源：http://ca.muxihuayi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mu.shxzskj.cn

TS:   s.replaceAll("a", "b")
来源：http://mv.huixiangedu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hj.panjiajie.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tl.hahajie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hp.huixiangedu.cn

C#:   s.Replace("a", "b")
来源：http://ct.nszjky.cn

[E07] 按分隔符拆分
来源：http://rd.panjiajie.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lr.shxzukj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ei.nszjky.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ni.yuexingan06.cn

TS:   s.split(",")
来源：http://ck.asd995.cn

Java: s.split(",");  s.split("\\s+")
来源：http://cy.jctech888.com.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xt.lnxyls.cn

Ruby: s.split(",");  s.split
来源：http://xv.asd995.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://on.yuntaijiaju.cn

[E08] 数组按分隔符合并
来源：http://zu.colortex.cn

Py:   ",".join(items)
来源：http://ap.lnxyls.cn

PHP:  implode(",", $items);
来源：http://qw.colortex.cn

JS:   items.join(",")
来源：http://qt.szxytkj.cn

TS:   items.join(",")
来源：http://ot.huanxung.cn

Java: String.join(",", items)
来源：http://de.nicolike.cn

Go:   strings.Join(items, ",")
来源：http://ny.jctech888.com.cn

Ruby: items.join(",")
来源：http://tt.hahajie.cn

C#:   string.Join(",", items)
来源：http://xy.haigaiapp.cn

[E09] 去除所有空白字符
来源：http://lq.bjjhwx.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fm.hnjuh.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ak.521024.cn

JS:   s.replace(/\s+/g, "")
来源：http://yp.newstarts.cn

TS:   s.replace(/\s+/g, "")
来源：http://og.newstarts.cn

Java: s.replaceAll("\\s+", "")
来源：http://pn.9csxet.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://pe.lnxyls.cn

Ruby: s.gsub(/\s+/, "")
来源：http://pc.9csxet.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://va.szsharing.cn

[E10] 左侧补零 / 定长填充
来源：http://pa.yuntaijiaju.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ov.shxzskj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://gp.colortex.cn

JS:   "7".padStart(3, "0")
来源：http://ng.yuexingan06.cn

TS:   "7".padStart(3, "0")
来源：http://ej.huanxung.cn

Java: String.format("%03d", 7)
来源：http://lm.chemitech.net.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://om.bookmarksfly.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ic.hnjuh.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://tr.huanxung.cn

[E11] 反转字符串
来源：http://al.huixinmuqiang.cn

Py:   s[::-1]
来源：http://bs.huixiangedu.cn

PHP:  strrev($s);
来源：http://ch.jianghongdianzi.cn

JS:   [...s].reverse().join("")
来源：http://mv.shxzskj.cn

TS:   [...s].reverse().join("")
来源：http://zr.shxzskj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://hp.wgjwhj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://en.521024.cn

Ruby: s.reverse
来源：http://lv.yuexingan06.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ze.shxzukj.cn

[E12] 统计某字符出现次数
来源：http://ng.nicolike.cn

Py:   s.count("a")
来源：http://eg.jianghongdianzi.cn

PHP:  substr_count($s, "a");
来源：http://ad.jctech888.com.cn

JS:   s.split("a").length - 1
来源：http://bx.bookmarksfly.cn

TS:   s.split("a").length - 1
来源：http://sj.muxihuayi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://us.szxytkj.cn

Go:   strings.Count(s, "a")
来源：http://hw.huixiangedu.cn

Ruby: s.count("a")
来源：http://lw.nszjky.cn

C#:   s.Count(c => c == 'a')
来源：http://qv.bookmarksfly.cn

[E13] 逐字符遍历
来源：http://ud.jctech888.com.cn

Py:   for ch in s: print(ch)
来源：http://vu.szxytkj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ds.huixiangedu.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ka.muxihuayi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ml.bjjhwx.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://uk.hnjuh.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nt.muxihuayi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://py.szsharing.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://yp.nicolike.cn

[E14] URL 编码与 Base64
来源：http://ic.shtwfgs.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://tm.huanxung.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://mm.bjjhwx.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://nc.jianghongdianzi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://sk.chemitech.net.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tb.521024.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cp.nicolike.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mn.nicolike.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wa.bookmarksfly.cn

[E15] HTML 转义 / 反转义
来源：http://xb.shxzskj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://bi.shxzukj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://cb.hnjuh.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://yl.asd995.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://fl.yuexingan06.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mu.huixiangedu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ge.9csxet.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ir.haigaiapp.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://xa.panjiajie.cn

[E16] 数字千分位
来源：http://xg.nszjky.cn

Py:   f"{1234567:,}"
来源：http://mf.wgjwhj.cn

PHP:  number_format(1234567);
来源：http://xp.haigaiapp.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://wm.panjiajie.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://cx.nszjky.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://yo.bjjhwx.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xy.hahajie.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://cp.bjjhwx.cn

C#:   1234567.ToString("N0")
来源：http://bt.huanxung.cn

[E17] 首字母大写
来源：http://zt.panjiajie.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xh.9csxet.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://df.huanxung.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lz.szsharing.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jp.521024.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bd.shtwfgs.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mb.shtwfgs.cn

Ruby: s.capitalize
来源：http://vq.shxzskj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ms.wgjwhj.cn

[E18] 模板占位符替换
来源：http://cr.huixiangedu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zq.huixinmuqiang.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ih.9csxet.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://qa.yuexingan06.cn


<!-- 参考信息 -->