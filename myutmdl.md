代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xt.hahajie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ht.521024.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zx.521024.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://cm.newstarts.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ma.newstarts.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://td.yuntaijiaju.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gk.haigaiapp.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qq.shxzukj.cn

[D11] 反转数组
来源：http://nk.bjjhwx.cn

Py:   arr[::-1];  arr.reverse()
来源：http://wz.gzmigu.cn

PHP:  array_reverse($arr);
来源：http://wp.haigaiapp.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ew.yuexingan06.cn

TS:   [...arr].reverse();
来源：http://pg.hnjuh.cn

Java: Collections.reverse(list);
来源：http://dq.wgjwhj.cn

Go:   slices.Reverse(arr)
来源：http://qd.shxzukj.cn

Ruby: arr.reverse
来源：http://xj.haigaiapp.cn

C#:   list.Reverse();
来源：http://ig.yuexingan06.cn

[D12] 查找元素下标
来源：http://gw.panjiajie.cn

Py:   arr.index(x);  x in arr
来源：http://ag.panjiajie.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qn.szxytkj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yq.chemitech.net.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lz.szxytkj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qx.huixinmuqiang.cn

Go:   slices.Index(arr, x)
来源：http://ko.gzmigu.cn

Ruby: arr.index(x)
来源：http://hn.colortex.cn

C#:   list.IndexOf(x);
来源：http://da.9csxet.cn

[D13] 过滤（保留满足条件的）
来源：http://ua.panjiajie.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://au.huanxung.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fj.huanxung.cn

JS:   arr.filter(x => x > 3)
来源：http://zm.nicolike.cn

TS:   arr.filter(x => x > 3)
来源：http://xa.colortex.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://al.gzmigu.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wf.panjiajie.cn

Ruby: arr.select { |x| x > 3 }
来源：http://mo.bookmarksfly.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ep.huixiangedu.cn

[D14] 映射转换（每个元素变形）
来源：http://wi.huanxung.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://fw.chemitech.net.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://pa.9csxet.cn

JS:   arr.map(x => x * 2)
来源：http://zf.huixiangedu.cn

TS:   arr.map(x => x * 2)
来源：http://px.gzmigu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://bv.huanxung.cn

Go:   // 手写循环
来源：http://gc.asd995.cn

Ruby: arr.map { |x| x * 2 }
来源：http://zt.muxihuayi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://zp.bjjhwx.cn

[D15] 去重
来源：http://lx.nicolike.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wo.bjjhwx.cn

PHP:  array_unique($arr);
来源：http://ks.jianghongdianzi.cn

JS:   [...new Set(arr)]
来源：http://fk.wgjwhj.cn

TS:   [...new Set(arr)]
来源：http://kn.bookmarksfly.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qt.huixiangedu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://kz.chemitech.net.cn

Ruby: arr.uniq
来源：http://zm.nszjky.cn

C#:   list.Distinct().ToList()
来源：http://xq.muxihuayi.cn

[D16] 求和与平均值
来源：http://xr.wgjwhj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dj.newstarts.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qn.panjiajie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hw.huixiangedu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dg.hahajie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zh.nicolike.cn

Go:   // 手写循环累加
来源：http://nn.gzmigu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ou.jianghongdianzi.cn

C#:   list.Sum();  list.Average()
来源：http://qg.szsharing.cn

[D17] 最大值与最小值
来源：http://zi.gzmigu.cn

Py:   max(arr);  min(arr)
来源：http://qg.lnxyls.cn

PHP:  max($arr);  min($arr);
来源：http://bm.nszjky.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ko.huixinmuqiang.cn

TS:   Math.max(...arr);
来源：http://av.chemitech.net.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://an.shtwfgs.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rc.jctech888.com.cn

Ruby: arr.max;  arr.min
来源：http://ia.nicolike.cn

C#:   list.Max();  list.Min()
来源：http://fm.shtwfgs.cn

[D18] 扁平化嵌套数组
来源：http://hx.chemitech.net.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tf.yuntaijiaju.cn

PHP:  array_merge(...$nested);
来源：http://mh.shxzskj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mz.chemitech.net.cn

TS:   nested.flat();
来源：http://gj.shtwfgs.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://do.9csxet.cn

Go:   // 手写双层循环
来源：http://nu.nicolike.cn

Ruby: nested.flatten
来源：http://rg.bookmarksfly.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://wj.colortex.cn

[D19] 按字段分组
来源：http://qe.szxytkj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ga.hnjuh.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://st.wgjwhj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xs.yuexingan06.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://up.gzmigu.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ge.panjiajie.cn

Go:   // 手写 map[string][]T
来源：http://hw.gzmigu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://rp.haigaiapp.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qm.yuexingan06.cn

[D20] 统计每个元素出现次数
来源：http://dj.nicolike.cn

Py:   Counter(arr)
来源：http://ev.yuexingan06.cn

PHP:  array_count_values($arr);
来源：http://kc.haigaiapp.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://em.bookmarksfly.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ak.huanxung.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://in.colortex.cn

Go:   // 手写 map[T]int
来源：http://rf.huanxung.cn

Ruby: arr.tally
来源：http://dg.bjjhwx.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://sk.shxzskj.cn

[D21] 判断是否包含某元素
来源：http://cm.bjjhwx.cn

Py:   x in arr
来源：http://lk.shxzukj.cn

PHP:  in_array($x, $arr, true);
来源：http://tu.hnjuh.cn

JS:   arr.includes(x)
来源：http://lk.asd995.cn

TS:   arr.includes(x)
来源：http://wz.panjiajie.cn

Java: list.contains(x)
来源：http://wf.521024.cn

Go:   slices.Contains(arr, x)
来源：http://cw.huixinmuqiang.cn

Ruby: arr.include?(x)
来源：http://zz.jianghongdianzi.cn

C#:   list.Contains(x)
来源：http://lf.521024.cn

[D22] 复制数组（避免共享引用）
来源：http://zm.jianghongdianzi.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://tv.shtwfgs.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.jianghongdianzi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dh.shxzskj.cn

TS:   [...arr];
来源：http://xu.521024.cn

Java: new ArrayList<>(list);
来源：http://eu.lnxyls.cn

Go:   copied := append([]int(nil), arr...)
来源：http://uz.nicolike.cn

Ruby: arr.dup;  arr.clone
来源：http://ja.521024.cn

C#:   new List<int>(list);
来源：http://lk.yuexingan06.cn

[D23] reduce 累积计算
来源：http://ea.shxzukj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yn.huixinmuqiang.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cs.9csxet.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zo.lnxyls.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qg.yuntaijiaju.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://kg.colortex.cn

Go:   // 手写循环
来源：http://cq.haigaiapp.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ej.szxytkj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ub.colortex.cn

[D24] 字典 / Map 基本操作
来源：http://az.jianghongdianzi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://lv.panjiajie.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mp.haigaiapp.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.hahajie.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rq.shxzukj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bb.haigaiapp.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xq.chemitech.net.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gz.bookmarksfly.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zz.asd995.cn

[D25] Set 集合去重与交并差
来源：http://qc.gzmigu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rk.huixinmuqiang.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ds.lnxyls.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qk.nicolike.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zf.shxzskj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kw.hnjuh.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qj.jianghongdianzi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pf.huixiangedu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://et.yuntaijiaju.cn

[D26] 数组转字符串
来源：http://kc.jianghongdianzi.cn

Py:   ", ".join(map(str, arr))
来源：http://cn.shtwfgs.cn

PHP:  implode(", ", $arr);
来源：http://vu.yuntaijiaju.cn

JS:   arr.join(", ")
来源：http://kq.asd995.cn

TS:   arr.join(", ")
来源：http://pc.lnxyls.cn

Java: String.join(", ", list)
来源：http://am.hnjuh.cn

Go:   strings.Join(strs, ", ")
来源：http://hp.shxzskj.cn

Ruby: arr.join(", ")
来源：http://mx.hahajie.cn

C#:   string.Join(", ", list)
来源：http://br.bookmarksfly.cn

================================================================================
来源：http://db.yuexingan06.cn

E. 字符串处理
来源：http://fn.9csxet.cn

================================================================================
来源：http://bd.haigaiapp.cn

[E01] 拼接字符串
来源：http://sx.bookmarksfly.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://nz.huanxung.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ow.jctech888.com.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vf.9csxet.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xw.jctech888.com.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zr.hahajie.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://aj.521024.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kt.9csxet.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ou.lnxyls.cn

[E02] 重复字符串
来源：http://rg.muxihuayi.cn

Py:   "ab" * 3
来源：http://ju.nszjky.cn

PHP:  str_repeat("ab", 3);
来源：http://ix.szsharing.cn

JS:   "ab".repeat(3)
来源：http://gw.shxzukj.cn

TS:   "ab".repeat(3)
来源：http://oy.hahajie.cn

Java: "ab".repeat(3)
来源：http://fq.wgjwhj.cn

Go:   strings.Repeat("ab", 3)
来源：http://aq.shtwfgs.cn

Ruby: "ab" * 3
来源：http://ab.yuexingan06.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://kv.521024.cn

[E03] 截取子串
来源：http://cv.szxytkj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://og.9csxet.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ma.lnxyls.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yx.colortex.cn

TS:   s.slice(1, 4)
来源：http://jk.jianghongdianzi.cn

Java: s.substring(1, 4)
来源：http://ra.newstarts.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kt.chemitech.net.cn

Ruby: s[1, 3];  s[1..3]
来源：http://gl.huixinmuqiang.cn

C#:   s.Substring(1, 3)
来源：http://lo.asd995.cn

[E04] 查找子串位置
来源：http://fh.szsharing.cn

Py:   s.find("x");  s.index("x")
来源：http://di.haigaiapp.cn

PHP:  strpos($s, "x");
来源：http://te.nicolike.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ot.huixiangedu.cn

TS:   s.indexOf("x")
来源：http://ja.asd995.cn

Java: s.indexOf("x")
来源：http://by.jctech888.com.cn

Go:   strings.Index(s, "x")
来源：http://ls.hahajie.cn

Ruby: s.index("x")
来源：http://jz.lnxyls.cn

C#:   s.IndexOf("x")
来源：http://gh.haigaiapp.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ra.hahajie.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://su.muxihuayi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://af.bookmarksfly.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://av.szxytkj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://et.chemitech.net.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://je.shxzskj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://oh.huanxung.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rc.panjiajie.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://la.yuntaijiaju.cn

[E06] 替换子串
来源：http://bp.wgjwhj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wz.panjiajie.cn

PHP:  str_replace("a", "b", $s);
来源：http://gv.521024.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tv.huixinmuqiang.cn

TS:   s.replaceAll("a", "b")
来源：http://dj.chemitech.net.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://da.panjiajie.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ed.huixiangedu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dy.wgjwhj.cn

C#:   s.Replace("a", "b")
来源：http://tw.jianghongdianzi.cn

[E07] 按分隔符拆分
来源：http://nx.hnjuh.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://kk.huixinmuqiang.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rh.huixinmuqiang.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://lw.shxzukj.cn

TS:   s.split(",")
来源：http://vh.asd995.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ua.bookmarksfly.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://oe.jctech888.com.cn

Ruby: s.split(",");  s.split
来源：http://av.bookmarksfly.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xz.lnxyls.cn

[E08] 数组按分隔符合并
来源：http://ri.szxytkj.cn

Py:   ",".join(items)
来源：http://gu.haigaiapp.cn

PHP:  implode(",", $items);
来源：http://tg.chemitech.net.cn

JS:   items.join(",")
来源：http://hy.nszjky.cn

TS:   items.join(",")
来源：http://bm.colortex.cn

Java: String.join(",", items)
来源：http://wx.huixiangedu.cn

Go:   strings.Join(items, ",")
来源：http://qj.asd995.cn

Ruby: items.join(",")
来源：http://de.shxzskj.cn

C#:   string.Join(",", items)
来源：http://oa.newstarts.cn

[E09] 去除所有空白字符
来源：http://nd.panjiajie.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ad.hahajie.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://id.haigaiapp.cn

JS:   s.replace(/\s+/g, "")
来源：http://jv.haigaiapp.cn

TS:   s.replace(/\s+/g, "")
来源：http://ll.panjiajie.cn

Java: s.replaceAll("\\s+", "")
来源：http://se.panjiajie.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://rt.huanxung.cn

Ruby: s.gsub(/\s+/, "")
来源：http://pe.hnjuh.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kq.yuntaijiaju.cn

[E10] 左侧补零 / 定长填充
来源：http://em.colortex.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://nm.yuntaijiaju.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://pg.521024.cn

JS:   "7".padStart(3, "0")
来源：http://wj.jctech888.com.cn

TS:   "7".padStart(3, "0")
来源：http://jw.nszjky.cn

Java: String.format("%03d", 7)
来源：http://we.jctech888.com.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://if.yuntaijiaju.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://cb.9csxet.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cy.9csxet.cn

[E11] 反转字符串
来源：http://gp.bookmarksfly.cn

Py:   s[::-1]
来源：http://ds.hnjuh.cn

PHP:  strrev($s);
来源：http://mh.gzmigu.cn

JS:   [...s].reverse().join("")
来源：http://ez.nicolike.cn

TS:   [...s].reverse().join("")
来源：http://vp.jctech888.com.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://el.gzmigu.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://in.yuexingan06.cn

Ruby: s.reverse
来源：http://sm.shxzukj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://hn.gzmigu.cn

[E12] 统计某字符出现次数
来源：http://jx.huanxung.cn

Py:   s.count("a")
来源：http://lh.shtwfgs.cn

PHP:  substr_count($s, "a");
来源：http://bk.nicolike.cn

JS:   s.split("a").length - 1
来源：http://zb.shxzukj.cn

TS:   s.split("a").length - 1
来源：http://kh.shxzskj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wl.shxzukj.cn

Go:   strings.Count(s, "a")
来源：http://cm.jctech888.com.cn

Ruby: s.count("a")
来源：http://es.panjiajie.cn

C#:   s.Count(c => c == 'a')
来源：http://ud.shtwfgs.cn

[E13] 逐字符遍历
来源：http://dc.haigaiapp.cn

Py:   for ch in s: print(ch)
来源：http://tr.jctech888.com.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dc.shxzukj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://zp.yuntaijiaju.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://fm.muxihuayi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fd.shxzskj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kc.shtwfgs.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://vp.yuntaijiaju.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qv.shxzukj.cn

[E14] URL 编码与 Base64
来源：http://kq.bookmarksfly.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://aj.521024.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://kw.shxzukj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://st.muxihuayi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fk.gzmigu.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zw.hahajie.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hk.shxzukj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tr.bookmarksfly.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xu.nszjky.cn

[E15] HTML 转义 / 反转义
来源：http://de.nicolike.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ct.shtwfgs.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ok.9csxet.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ol.huixinmuqiang.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ml.bookmarksfly.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://cj.chemitech.net.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://id.hnjuh.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://lh.9csxet.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://oq.colortex.cn

[E16] 数字千分位
来源：http://oq.shxzskj.cn

Py:   f"{1234567:,}"
来源：http://zw.szsharing.cn

PHP:  number_format(1234567);
来源：http://of.shxzukj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ik.huanxung.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://if.jianghongdianzi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ew.panjiajie.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://uj.newstarts.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hp.newstarts.cn

C#:   1234567.ToString("N0")
来源：http://bo.chemitech.net.cn

[E17] 首字母大写
来源：http://jz.521024.cn


<!-- 参考信息 -->