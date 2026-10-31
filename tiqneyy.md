代发 wailian999

[D11] 反转数组
来源：http://mc.bjjhwx.cn

Py:   arr[::-1];  arr.reverse()
来源：http://xw.jctech888.com.cn

PHP:  array_reverse($arr);
来源：http://pw.newstarts.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ee.bjjhwx.cn

TS:   [...arr].reverse();
来源：http://ft.shxzukj.cn

Java: Collections.reverse(list);
来源：http://yh.huixinmuqiang.cn

Go:   slices.Reverse(arr)
来源：http://mk.bookmarksfly.cn

Ruby: arr.reverse
来源：http://ec.chemitech.net.cn

C#:   list.Reverse();
来源：http://xk.panjiajie.cn

[D12] 查找元素下标
来源：http://po.bjjhwx.cn

Py:   arr.index(x);  x in arr
来源：http://ra.yuntaijiaju.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hp.9csxet.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ou.huanxung.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pi.panjiajie.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fk.chemitech.net.cn

Go:   slices.Index(arr, x)
来源：http://iy.lnxyls.cn

Ruby: arr.index(x)
来源：http://mt.yuntaijiaju.cn

C#:   list.IndexOf(x);
来源：http://jw.nszjky.cn

[D13] 过滤（保留满足条件的）
来源：http://vz.yuexingan06.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://oc.nszjky.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fi.bjjhwx.cn

JS:   arr.filter(x => x > 3)
来源：http://jd.asd995.cn

TS:   arr.filter(x => x > 3)
来源：http://ng.newstarts.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ki.gzmigu.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://va.gzmigu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ck.hahajie.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://jp.lnxyls.cn

[D14] 映射转换（每个元素变形）
来源：http://xq.521024.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://to.muxihuayi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ff.bookmarksfly.cn

JS:   arr.map(x => x * 2)
来源：http://ex.szsharing.cn

TS:   arr.map(x => x * 2)
来源：http://gb.colortex.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://he.yuexingan06.cn

Go:   // 手写循环
来源：http://eg.wgjwhj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://xj.hahajie.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://cm.hnjuh.cn

[D15] 去重
来源：http://xs.nicolike.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xt.gzmigu.cn

PHP:  array_unique($arr);
来源：http://qm.shtwfgs.cn

JS:   [...new Set(arr)]
来源：http://cu.muxihuayi.cn

TS:   [...new Set(arr)]
来源：http://ix.yuntaijiaju.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://tb.shtwfgs.cn

Go:   // 用 map[T]struct{} 手写
来源：http://va.jctech888.com.cn

Ruby: arr.uniq
来源：http://jf.jctech888.com.cn

C#:   list.Distinct().ToList()
来源：http://mb.haigaiapp.cn

[D16] 求和与平均值
来源：http://sr.colortex.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zt.521024.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cx.newstarts.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://co.newstarts.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qx.chemitech.net.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://so.colortex.cn

Go:   // 手写循环累加
来源：http://mt.bjjhwx.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gp.muxihuayi.cn

C#:   list.Sum();  list.Average()
来源：http://zf.newstarts.cn

[D17] 最大值与最小值
来源：http://cq.nszjky.cn

Py:   max(arr);  min(arr)
来源：http://fk.bookmarksfly.cn

PHP:  max($arr);  min($arr);
来源：http://rf.huanxung.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fh.szsharing.cn

TS:   Math.max(...arr);
来源：http://ju.521024.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://zh.shxzukj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://im.haigaiapp.cn

Ruby: arr.max;  arr.min
来源：http://tf.hahajie.cn

C#:   list.Max();  list.Min()
来源：http://aa.asd995.cn

[D18] 扁平化嵌套数组
来源：http://dn.yuntaijiaju.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rt.bjjhwx.cn

PHP:  array_merge(...$nested);
来源：http://lr.lnxyls.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fe.bjjhwx.cn

TS:   nested.flat();
来源：http://bd.jctech888.com.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pj.newstarts.cn

Go:   // 手写双层循环
来源：http://bl.hahajie.cn

Ruby: nested.flatten
来源：http://zt.szxytkj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://kx.chemitech.net.cn

[D19] 按字段分组
来源：http://jp.asd995.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://tq.haigaiapp.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://cu.szsharing.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kg.yuntaijiaju.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://sn.haigaiapp.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hx.yuntaijiaju.cn

Go:   // 手写 map[string][]T
来源：http://ge.9csxet.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://jo.huanxung.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://st.chemitech.net.cn

[D20] 统计每个元素出现次数
来源：http://xd.huanxung.cn

Py:   Counter(arr)
来源：http://ac.9csxet.cn

PHP:  array_count_values($arr);
来源：http://hk.nicolike.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lk.lnxyls.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lr.gzmigu.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rp.hahajie.cn

Go:   // 手写 map[T]int
来源：http://ny.haigaiapp.cn

Ruby: arr.tally
来源：http://tq.asd995.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zq.jctech888.com.cn

[D21] 判断是否包含某元素
来源：http://io.haigaiapp.cn

Py:   x in arr
来源：http://nd.yuexingan06.cn

PHP:  in_array($x, $arr, true);
来源：http://ga.jctech888.com.cn

JS:   arr.includes(x)
来源：http://bd.huixiangedu.cn

TS:   arr.includes(x)
来源：http://gl.shxzukj.cn

Java: list.contains(x)
来源：http://le.chemitech.net.cn

Go:   slices.Contains(arr, x)
来源：http://po.muxihuayi.cn

Ruby: arr.include?(x)
来源：http://jw.yuntaijiaju.cn

C#:   list.Contains(x)
来源：http://mj.jctech888.com.cn

[D22] 复制数组（避免共享引用）
来源：http://ty.colortex.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://rb.9csxet.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://py.panjiajie.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://au.nszjky.cn

TS:   [...arr];
来源：http://mk.panjiajie.cn

Java: new ArrayList<>(list);
来源：http://em.huixiangedu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://yn.chemitech.net.cn

Ruby: arr.dup;  arr.clone
来源：http://kc.bookmarksfly.cn

C#:   new List<int>(list);
来源：http://wf.gzmigu.cn

[D23] reduce 累积计算
来源：http://uj.newstarts.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://za.szxytkj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fc.jianghongdianzi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fy.huixiangedu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vm.nszjky.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://mj.jctech888.com.cn

Go:   // 手写循环
来源：http://kl.newstarts.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://yv.szxytkj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://dt.hahajie.cn

[D24] 字典 / Map 基本操作
来源：http://wh.newstarts.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://nw.huanxung.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ys.muxihuayi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://di.huixinmuqiang.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nn.shtwfgs.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://um.bjjhwx.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lp.shxzukj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kc.huixiangedu.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://yo.hahajie.cn

[D25] Set 集合去重与交并差
来源：http://gz.huanxung.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://th.szsharing.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://je.yuexingan06.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wa.jianghongdianzi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dy.asd995.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://il.huixiangedu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ym.colortex.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://og.bookmarksfly.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hv.wgjwhj.cn

[D26] 数组转字符串
来源：http://lh.jctech888.com.cn

Py:   ", ".join(map(str, arr))
来源：http://ht.chemitech.net.cn

PHP:  implode(", ", $arr);
来源：http://fs.gzmigu.cn

JS:   arr.join(", ")
来源：http://bh.szxytkj.cn

TS:   arr.join(", ")
来源：http://mc.haigaiapp.cn

Java: String.join(", ", list)
来源：http://nd.huixinmuqiang.cn

Go:   strings.Join(strs, ", ")
来源：http://ul.shxzskj.cn

Ruby: arr.join(", ")
来源：http://wz.haigaiapp.cn

C#:   string.Join(", ", list)
来源：http://cb.haigaiapp.cn

================================================================================
来源：http://mh.szsharing.cn

E. 字符串处理
来源：http://hj.hahajie.cn

================================================================================
来源：http://gs.bjjhwx.cn

[E01] 拼接字符串
来源：http://zb.521024.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://br.panjiajie.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jj.haigaiapp.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tj.nicolike.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://aj.nszjky.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://re.szsharing.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://oq.521024.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pq.newstarts.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vk.lnxyls.cn

[E02] 重复字符串
来源：http://is.muxihuayi.cn

Py:   "ab" * 3
来源：http://mo.521024.cn

PHP:  str_repeat("ab", 3);
来源：http://ca.szsharing.cn

JS:   "ab".repeat(3)
来源：http://yq.9csxet.cn

TS:   "ab".repeat(3)
来源：http://nn.nicolike.cn

Java: "ab".repeat(3)
来源：http://eg.szsharing.cn

Go:   strings.Repeat("ab", 3)
来源：http://hv.jianghongdianzi.cn

Ruby: "ab" * 3
来源：http://zc.hnjuh.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ux.shxzukj.cn

[E03] 截取子串
来源：http://kx.haigaiapp.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://an.bjjhwx.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dr.yuntaijiaju.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ee.jianghongdianzi.cn

TS:   s.slice(1, 4)
来源：http://tp.bjjhwx.cn

Java: s.substring(1, 4)
来源：http://pz.lnxyls.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gj.haigaiapp.cn

Ruby: s[1, 3];  s[1..3]
来源：http://zq.huanxung.cn

C#:   s.Substring(1, 3)
来源：http://zm.asd995.cn

[E04] 查找子串位置
来源：http://to.bjjhwx.cn

Py:   s.find("x");  s.index("x")
来源：http://ol.gzmigu.cn

PHP:  strpos($s, "x");
来源：http://at.huixiangedu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hc.muxihuayi.cn

TS:   s.indexOf("x")
来源：http://ib.lnxyls.cn

Java: s.indexOf("x")
来源：http://bd.yuntaijiaju.cn

Go:   strings.Index(s, "x")
来源：http://el.newstarts.cn

Ruby: s.index("x")
来源：http://lf.wgjwhj.cn

C#:   s.IndexOf("x")
来源：http://sa.9csxet.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://el.colortex.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mo.shxzukj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://uk.hahajie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yy.jianghongdianzi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://uz.shxzukj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ty.muxihuayi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bc.shxzskj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gn.huanxung.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jx.shxzukj.cn

[E06] 替换子串
来源：http://gy.hnjuh.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bs.bookmarksfly.cn

PHP:  str_replace("a", "b", $s);
来源：http://gw.huixiangedu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://de.huixiangedu.cn

TS:   s.replaceAll("a", "b")
来源：http://rq.yuexingan06.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ui.szsharing.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://id.huanxung.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vv.gzmigu.cn

C#:   s.Replace("a", "b")
来源：http://on.hahajie.cn

[E07] 按分隔符拆分
来源：http://ja.nszjky.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://cw.haigaiapp.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dm.shxzukj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://mm.haigaiapp.cn

TS:   s.split(",")
来源：http://zb.huixiangedu.cn

Java: s.split(",");  s.split("\\s+")
来源：http://yj.newstarts.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://in.hnjuh.cn

Ruby: s.split(",");  s.split
来源：http://vf.asd995.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pa.szsharing.cn

[E08] 数组按分隔符合并
来源：http://qf.colortex.cn

Py:   ",".join(items)
来源：http://rd.gzmigu.cn

PHP:  implode(",", $items);
来源：http://nc.asd995.cn

JS:   items.join(",")
来源：http://xp.colortex.cn

TS:   items.join(",")
来源：http://op.szsharing.cn

Java: String.join(",", items)
来源：http://fo.bookmarksfly.cn

Go:   strings.Join(items, ",")
来源：http://mr.newstarts.cn

Ruby: items.join(",")
来源：http://qd.hahajie.cn

C#:   string.Join(",", items)
来源：http://wr.nicolike.cn

[E09] 去除所有空白字符
来源：http://ii.wgjwhj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://su.nicolike.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://uh.nszjky.cn

JS:   s.replace(/\s+/g, "")
来源：http://tq.yuexingan06.cn

TS:   s.replace(/\s+/g, "")
来源：http://uy.gzmigu.cn

Java: s.replaceAll("\\s+", "")
来源：http://fz.wgjwhj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://qn.521024.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ev.shtwfgs.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ch.shxzskj.cn

[E10] 左侧补零 / 定长填充
来源：http://tk.szxytkj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://iq.bookmarksfly.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wo.hahajie.cn

JS:   "7".padStart(3, "0")
来源：http://lc.huixiangedu.cn

TS:   "7".padStart(3, "0")
来源：http://xe.wgjwhj.cn

Java: String.format("%03d", 7)
来源：http://hh.panjiajie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ea.hahajie.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qv.jianghongdianzi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xj.shtwfgs.cn

[E11] 反转字符串
来源：http://sv.9csxet.cn

Py:   s[::-1]
来源：http://im.nszjky.cn

PHP:  strrev($s);
来源：http://dj.asd995.cn

JS:   [...s].reverse().join("")
来源：http://qo.nicolike.cn

TS:   [...s].reverse().join("")
来源：http://td.gzmigu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://sr.9csxet.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://pp.chemitech.net.cn

Ruby: s.reverse
来源：http://vj.nszjky.cn

C#:   new string(s.Reverse().ToArray())
来源：http://nc.colortex.cn

[E12] 统计某字符出现次数
来源：http://og.szxytkj.cn

Py:   s.count("a")
来源：http://rk.muxihuayi.cn

PHP:  substr_count($s, "a");
来源：http://bd.bookmarksfly.cn

JS:   s.split("a").length - 1
来源：http://pe.wgjwhj.cn

TS:   s.split("a").length - 1
来源：http://rr.lnxyls.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rk.newstarts.cn

Go:   strings.Count(s, "a")
来源：http://rj.gzmigu.cn

Ruby: s.count("a")
来源：http://ik.shxzskj.cn

C#:   s.Count(c => c == 'a')
来源：http://tx.huixinmuqiang.cn

[E13] 逐字符遍历
来源：http://se.521024.cn

Py:   for ch in s: print(ch)
来源：http://ha.huanxung.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ur.szsharing.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://dn.yuexingan06.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ay.chemitech.net.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rx.huanxung.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mg.gzmigu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://jv.shxzskj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://lv.lnxyls.cn

[E14] URL 编码与 Base64
来源：http://ne.muxihuayi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mp.szxytkj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://de.huixinmuqiang.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vx.chemitech.net.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://si.wgjwhj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ps.nicolike.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vw.lnxyls.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://yy.shtwfgs.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fv.newstarts.cn

[E15] HTML 转义 / 反转义
来源：http://cs.yuntaijiaju.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://rt.asd995.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jl.shxzskj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rw.bjjhwx.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://jt.huixinmuqiang.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://be.yuexingan06.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://if.newstarts.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ex.shxzukj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://gy.panjiajie.cn

[E16] 数字千分位
来源：http://cu.521024.cn

Py:   f"{1234567:,}"
来源：http://ed.521024.cn

PHP:  number_format(1234567);
来源：http://yu.nszjky.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://vm.colortex.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ap.szsharing.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://sg.huixinmuqiang.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zl.9csxet.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wk.bookmarksfly.cn

C#:   1234567.ToString("N0")
来源：http://ro.muxihuayi.cn

[E17] 首字母大写
来源：http://lk.huixiangedu.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ov.nicolike.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://az.asd995.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://za.9csxet.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://es.haigaiapp.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xy.bjjhwx.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://nq.9csxet.cn

Ruby: s.capitalize
来源：http://te.9csxet.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nb.yuntaijiaju.cn


<!-- 参考信息 -->