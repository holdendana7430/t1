代发 wailian999

TS:   [...arr].reverse();
来源：http://vb.chemitech.net.cn

Java: Collections.reverse(list);
来源：http://cl.nszjky.cn

Go:   slices.Reverse(arr)
来源：http://ig.lnxyls.cn

Ruby: arr.reverse
来源：http://jn.colortex.cn

C#:   list.Reverse();
来源：http://os.shxzskj.cn

[D12] 查找元素下标
来源：http://xk.hahajie.cn

Py:   arr.index(x);  x in arr
来源：http://zp.yuntaijiaju.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fy.wgjwhj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gt.jianghongdianzi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vo.bjjhwx.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qi.panjiajie.cn

Go:   slices.Index(arr, x)
来源：http://oy.hnjuh.cn

Ruby: arr.index(x)
来源：http://kt.gzmigu.cn

C#:   list.IndexOf(x);
来源：http://ll.chemitech.net.cn

[D13] 过滤（保留满足条件的）
来源：http://dt.szxytkj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://en.panjiajie.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xg.newstarts.cn

JS:   arr.filter(x => x > 3)
来源：http://bs.nszjky.cn

TS:   arr.filter(x => x > 3)
来源：http://bv.521024.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://cs.szsharing.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mp.shtwfgs.cn

Ruby: arr.select { |x| x > 3 }
来源：http://dp.hnjuh.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://zp.yuntaijiaju.cn

[D14] 映射转换（每个元素变形）
来源：http://bl.haigaiapp.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://yd.lnxyls.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qr.huixinmuqiang.cn

JS:   arr.map(x => x * 2)
来源：http://wb.huixiangedu.cn

TS:   arr.map(x => x * 2)
来源：http://sx.nicolike.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://if.szxytkj.cn

Go:   // 手写循环
来源：http://rd.jianghongdianzi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://co.wgjwhj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://uj.szsharing.cn

[D15] 去重
来源：http://zy.bookmarksfly.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kc.hahajie.cn

PHP:  array_unique($arr);
来源：http://vx.szsharing.cn

JS:   [...new Set(arr)]
来源：http://aj.haigaiapp.cn

TS:   [...new Set(arr)]
来源：http://nc.hnjuh.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qk.jianghongdianzi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://bg.yuexingan06.cn

Ruby: arr.uniq
来源：http://bv.shxzskj.cn

C#:   list.Distinct().ToList()
来源：http://ih.gzmigu.cn

[D16] 求和与平均值
来源：http://xe.szsharing.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://as.nszjky.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://lt.gzmigu.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xy.jianghongdianzi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ad.shtwfgs.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://re.yuexingan06.cn

Go:   // 手写循环累加
来源：http://hq.jctech888.com.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ki.gzmigu.cn

C#:   list.Sum();  list.Average()
来源：http://rn.huixiangedu.cn

[D17] 最大值与最小值
来源：http://aa.huixiangedu.cn

Py:   max(arr);  min(arr)
来源：http://rq.nszjky.cn

PHP:  max($arr);  min($arr);
来源：http://ab.9csxet.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://br.colortex.cn

TS:   Math.max(...arr);
来源：http://bq.hahajie.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://lk.huanxung.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://cm.shtwfgs.cn

Ruby: arr.max;  arr.min
来源：http://wy.bjjhwx.cn

C#:   list.Max();  list.Min()
来源：http://py.jianghongdianzi.cn

[D18] 扁平化嵌套数组
来源：http://dw.colortex.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://uz.panjiajie.cn

PHP:  array_merge(...$nested);
来源：http://ar.szxytkj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mn.colortex.cn

TS:   nested.flat();
来源：http://sm.lnxyls.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fl.shtwfgs.cn

Go:   // 手写双层循环
来源：http://vi.huixinmuqiang.cn

Ruby: nested.flatten
来源：http://nk.jctech888.com.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ao.haigaiapp.cn

[D19] 按字段分组
来源：http://ot.muxihuayi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fw.huixiangedu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ji.9csxet.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xb.hnjuh.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ae.yuntaijiaju.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://uz.huixiangedu.cn

Go:   // 手写 map[string][]T
来源：http://cz.bjjhwx.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ot.shtwfgs.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://az.chemitech.net.cn

[D20] 统计每个元素出现次数
来源：http://hr.wgjwhj.cn

Py:   Counter(arr)
来源：http://xe.colortex.cn

PHP:  array_count_values($arr);
来源：http://oj.chemitech.net.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ut.9csxet.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://es.lnxyls.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://md.gzmigu.cn

Go:   // 手写 map[T]int
来源：http://yq.nicolike.cn

Ruby: arr.tally
来源：http://lq.521024.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dr.shxzukj.cn

[D21] 判断是否包含某元素
来源：http://lt.wgjwhj.cn

Py:   x in arr
来源：http://ls.bookmarksfly.cn

PHP:  in_array($x, $arr, true);
来源：http://to.nszjky.cn

JS:   arr.includes(x)
来源：http://mi.bjjhwx.cn

TS:   arr.includes(x)
来源：http://tv.shxzukj.cn

Java: list.contains(x)
来源：http://ww.panjiajie.cn

Go:   slices.Contains(arr, x)
来源：http://um.szxytkj.cn

Ruby: arr.include?(x)
来源：http://ai.hahajie.cn

C#:   list.Contains(x)
来源：http://fm.yuexingan06.cn

[D22] 复制数组（避免共享引用）
来源：http://ff.bookmarksfly.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://dv.newstarts.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://me.jctech888.com.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://kr.asd995.cn

TS:   [...arr];
来源：http://uz.yuntaijiaju.cn

Java: new ArrayList<>(list);
来源：http://fi.asd995.cn

Go:   copied := append([]int(nil), arr...)
来源：http://do.huixiangedu.cn

Ruby: arr.dup;  arr.clone
来源：http://vb.yuexingan06.cn

C#:   new List<int>(list);
来源：http://kh.gzmigu.cn

[D23] reduce 累积计算
来源：http://iq.huixinmuqiang.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vl.huixiangedu.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xa.bookmarksfly.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bx.szsharing.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kw.huixiangedu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://st.shxzukj.cn

Go:   // 手写循环
来源：http://sl.shxzukj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bg.colortex.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qx.panjiajie.cn

[D24] 字典 / Map 基本操作
来源：http://ip.asd995.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://dp.521024.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://os.panjiajie.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ny.colortex.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rl.shxzukj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://io.muxihuayi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://kv.wgjwhj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pe.shtwfgs.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://yj.huixinmuqiang.cn

[D25] Set 集合去重与交并差
来源：http://cs.nszjky.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qq.nszjky.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://cs.shtwfgs.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wo.9csxet.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://uq.shxzskj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nz.wgjwhj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wg.yuntaijiaju.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://iu.nicolike.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://eh.bjjhwx.cn

[D26] 数组转字符串
来源：http://fu.huixinmuqiang.cn

Py:   ", ".join(map(str, arr))
来源：http://hy.jianghongdianzi.cn

PHP:  implode(", ", $arr);
来源：http://xz.nicolike.cn

JS:   arr.join(", ")
来源：http://fo.521024.cn

TS:   arr.join(", ")
来源：http://se.lnxyls.cn

Java: String.join(", ", list)
来源：http://hb.huixiangedu.cn

Go:   strings.Join(strs, ", ")
来源：http://pj.bookmarksfly.cn

Ruby: arr.join(", ")
来源：http://hl.hahajie.cn

C#:   string.Join(", ", list)
来源：http://tj.521024.cn

================================================================================
来源：http://or.hnjuh.cn

E. 字符串处理
来源：http://au.panjiajie.cn

================================================================================
来源：http://xh.shxzskj.cn

[E01] 拼接字符串
来源：http://rq.huixinmuqiang.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vz.hnjuh.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xj.szxytkj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gb.gzmigu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jr.huixinmuqiang.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://oo.muxihuayi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xy.9csxet.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cj.muxihuayi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nq.szxytkj.cn

[E02] 重复字符串
来源：http://cp.bookmarksfly.cn

Py:   "ab" * 3
来源：http://lv.panjiajie.cn

PHP:  str_repeat("ab", 3);
来源：http://ly.szsharing.cn

JS:   "ab".repeat(3)
来源：http://aa.muxihuayi.cn

TS:   "ab".repeat(3)
来源：http://gs.haigaiapp.cn

Java: "ab".repeat(3)
来源：http://bf.hahajie.cn

Go:   strings.Repeat("ab", 3)
来源：http://xm.huixiangedu.cn

Ruby: "ab" * 3
来源：http://nq.521024.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://eo.shxzskj.cn

[E03] 截取子串
来源：http://th.hnjuh.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://oy.chemitech.net.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jd.huixiangedu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hu.asd995.cn

TS:   s.slice(1, 4)
来源：http://wi.huanxung.cn

Java: s.substring(1, 4)
来源：http://xh.haigaiapp.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ug.huixiangedu.cn

Ruby: s[1, 3];  s[1..3]
来源：http://sj.chemitech.net.cn

C#:   s.Substring(1, 3)
来源：http://kl.szsharing.cn

[E04] 查找子串位置
来源：http://am.lnxyls.cn

Py:   s.find("x");  s.index("x")
来源：http://iv.szsharing.cn

PHP:  strpos($s, "x");
来源：http://jo.hahajie.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://im.huixiangedu.cn

TS:   s.indexOf("x")
来源：http://ir.wgjwhj.cn

Java: s.indexOf("x")
来源：http://ay.lnxyls.cn

Go:   strings.Index(s, "x")
来源：http://dc.huanxung.cn

Ruby: s.index("x")
来源：http://fj.nicolike.cn

C#:   s.IndexOf("x")
来源：http://au.shxzukj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ar.shxzskj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wz.shxzskj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ey.haigaiapp.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wt.colortex.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://vn.shtwfgs.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mw.wgjwhj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kr.lnxyls.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://is.yuntaijiaju.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ce.huixiangedu.cn

[E06] 替换子串
来源：http://fl.nicolike.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://or.bjjhwx.cn

PHP:  str_replace("a", "b", $s);
来源：http://lh.newstarts.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yr.newstarts.cn

TS:   s.replaceAll("a", "b")
来源：http://uv.panjiajie.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mk.9csxet.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kj.jctech888.com.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zq.jianghongdianzi.cn

C#:   s.Replace("a", "b")
来源：http://ud.bookmarksfly.cn

[E07] 按分隔符拆分
来源：http://og.yuntaijiaju.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ff.chemitech.net.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jz.nszjky.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ux.shxzskj.cn

TS:   s.split(",")
来源：http://cx.asd995.cn

Java: s.split(",");  s.split("\\s+")
来源：http://od.szsharing.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://sp.bookmarksfly.cn

Ruby: s.split(",");  s.split
来源：http://yq.bookmarksfly.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qg.9csxet.cn

[E08] 数组按分隔符合并
来源：http://cy.asd995.cn

Py:   ",".join(items)
来源：http://me.panjiajie.cn

PHP:  implode(",", $items);
来源：http://xa.huixinmuqiang.cn

JS:   items.join(",")
来源：http://ev.shxzukj.cn

TS:   items.join(",")
来源：http://en.hahajie.cn

Java: String.join(",", items)
来源：http://wn.szxytkj.cn

Go:   strings.Join(items, ",")
来源：http://rq.yuntaijiaju.cn

Ruby: items.join(",")
来源：http://hd.jctech888.com.cn

C#:   string.Join(",", items)
来源：http://vb.521024.cn

[E09] 去除所有空白字符
来源：http://oa.huanxung.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fp.panjiajie.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jw.gzmigu.cn

JS:   s.replace(/\s+/g, "")
来源：http://sv.hnjuh.cn

TS:   s.replace(/\s+/g, "")
来源：http://tq.huanxung.cn

Java: s.replaceAll("\\s+", "")
来源：http://ov.hahajie.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://tb.colortex.cn

Ruby: s.gsub(/\s+/, "")
来源：http://mx.newstarts.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hn.asd995.cn

[E10] 左侧补零 / 定长填充
来源：http://ik.jianghongdianzi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wa.shxzskj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tn.bjjhwx.cn

JS:   "7".padStart(3, "0")
来源：http://en.jianghongdianzi.cn

TS:   "7".padStart(3, "0")
来源：http://mi.huanxung.cn

Java: String.format("%03d", 7)
来源：http://wb.nicolike.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://op.szsharing.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pf.gzmigu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://up.wgjwhj.cn

[E11] 反转字符串
来源：http://yi.hahajie.cn

Py:   s[::-1]
来源：http://um.nszjky.cn

PHP:  strrev($s);
来源：http://yh.nszjky.cn

JS:   [...s].reverse().join("")
来源：http://zs.hahajie.cn

TS:   [...s].reverse().join("")
来源：http://xz.huixinmuqiang.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://gt.chemitech.net.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://fb.yuntaijiaju.cn

Ruby: s.reverse
来源：http://er.newstarts.cn

C#:   new string(s.Reverse().ToArray())
来源：http://qp.shxzukj.cn

[E12] 统计某字符出现次数
来源：http://cl.shxzskj.cn

Py:   s.count("a")
来源：http://mp.huixiangedu.cn

PHP:  substr_count($s, "a");
来源：http://uf.yuntaijiaju.cn

JS:   s.split("a").length - 1
来源：http://eu.haigaiapp.cn

TS:   s.split("a").length - 1
来源：http://xu.panjiajie.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fy.asd995.cn

Go:   strings.Count(s, "a")
来源：http://cf.huixiangedu.cn

Ruby: s.count("a")
来源：http://iy.yuntaijiaju.cn

C#:   s.Count(c => c == 'a')
来源：http://bm.jctech888.com.cn

[E13] 逐字符遍历
来源：http://yu.huixinmuqiang.cn

Py:   for ch in s: print(ch)
来源：http://gt.jctech888.com.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://do.gzmigu.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://dx.lnxyls.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://xe.szsharing.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://li.hnjuh.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://il.bookmarksfly.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://th.bookmarksfly.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ua.asd995.cn

[E14] URL 编码与 Base64
来源：http://se.yuexingan06.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ys.szxytkj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://sd.haigaiapp.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xx.521024.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jm.huixinmuqiang.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://sb.jctech888.com.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tu.colortex.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xr.jctech888.com.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dk.lnxyls.cn

[E15] HTML 转义 / 反转义
来源：http://xp.chemitech.net.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://an.nicolike.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://nn.newstarts.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gp.muxihuayi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://rf.colortex.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ip.gzmigu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ve.haigaiapp.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://kq.bookmarksfly.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ln.panjiajie.cn

[E16] 数字千分位
来源：http://xo.haigaiapp.cn

Py:   f"{1234567:,}"
来源：http://nx.9csxet.cn

PHP:  number_format(1234567);
来源：http://kb.nszjky.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://fu.hahajie.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://mt.yuexingan06.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hy.muxihuayi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://sn.asd995.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gt.huanxung.cn

C#:   1234567.ToString("N0")
来源：http://yy.szsharing.cn

[E17] 首字母大写
来源：http://no.521024.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://tg.wgjwhj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://gv.hnjuh.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yr.asd995.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://il.szxytkj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://cm.huixinmuqiang.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://my.nicolike.cn

Ruby: s.capitalize
来源：http://jl.haigaiapp.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://du.huixinmuqiang.cn

[E18] 模板占位符替换
来源：http://hw.szsharing.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ht.nicolike.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tt.haigaiapp.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://bk.szxytkj.cn


<!-- 参考信息 -->