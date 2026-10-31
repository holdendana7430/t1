代发 wailian999

PHP:  sort($arr);
来源：http://gq.newstarts.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ro.chemitech.net.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ty.szsharing.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://yc.chemitech.net.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://il.521024.cn

Ruby: arr.sort
来源：http://kb.yuexingan06.cn

C#:   list.Sort();
来源：http://fy.521024.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://gd.nicolike.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pv.yuntaijiaju.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fq.yuexingan06.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://yj.shtwfgs.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wi.wgjwhj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mn.huixinmuqiang.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mi.shtwfgs.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qn.jctech888.com.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yx.9csxet.cn

[D11] 反转数组
来源：http://dd.haigaiapp.cn

Py:   arr[::-1];  arr.reverse()
来源：http://xi.shxzskj.cn

PHP:  array_reverse($arr);
来源：http://id.huixinmuqiang.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vb.huixiangedu.cn

TS:   [...arr].reverse();
来源：http://pc.9csxet.cn

Java: Collections.reverse(list);
来源：http://qq.gzmigu.cn

Go:   slices.Reverse(arr)
来源：http://xw.gzmigu.cn

Ruby: arr.reverse
来源：http://et.panjiajie.cn

C#:   list.Reverse();
来源：http://au.bjjhwx.cn

[D12] 查找元素下标
来源：http://kw.asd995.cn

Py:   arr.index(x);  x in arr
来源：http://gy.yuexingan06.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://sn.yuexingan06.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dh.huanxung.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dj.jianghongdianzi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ca.szxytkj.cn

Go:   slices.Index(arr, x)
来源：http://xs.szsharing.cn

Ruby: arr.index(x)
来源：http://yx.newstarts.cn

C#:   list.IndexOf(x);
来源：http://jj.shxzskj.cn

[D13] 过滤（保留满足条件的）
来源：http://az.szsharing.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vo.shxzukj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://po.shxzskj.cn

JS:   arr.filter(x => x > 3)
来源：http://cy.521024.cn

TS:   arr.filter(x => x > 3)
来源：http://tu.wgjwhj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ml.9csxet.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ix.haigaiapp.cn

Ruby: arr.select { |x| x > 3 }
来源：http://to.nicolike.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://wm.jianghongdianzi.cn

[D14] 映射转换（每个元素变形）
来源：http://mr.hahajie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hg.asd995.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://bk.colortex.cn

JS:   arr.map(x => x * 2)
来源：http://ol.jianghongdianzi.cn

TS:   arr.map(x => x * 2)
来源：http://qo.521024.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://sq.wgjwhj.cn

Go:   // 手写循环
来源：http://bf.hnjuh.cn

Ruby: arr.map { |x| x * 2 }
来源：http://xw.wgjwhj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://pj.gzmigu.cn

[D15] 去重
来源：http://st.yuntaijiaju.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ry.asd995.cn

PHP:  array_unique($arr);
来源：http://qp.asd995.cn

JS:   [...new Set(arr)]
来源：http://oe.colortex.cn

TS:   [...new Set(arr)]
来源：http://ks.shxzskj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bg.wgjwhj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://kj.jianghongdianzi.cn

Ruby: arr.uniq
来源：http://ue.colortex.cn

C#:   list.Distinct().ToList()
来源：http://jk.bookmarksfly.cn

[D16] 求和与平均值
来源：http://rr.huixiangedu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://du.huixiangedu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qw.9csxet.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://nz.huixinmuqiang.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qc.shtwfgs.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vf.521024.cn

Go:   // 手写循环累加
来源：http://ri.yuntaijiaju.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xm.shxzskj.cn

C#:   list.Sum();  list.Average()
来源：http://vb.chemitech.net.cn

[D17] 最大值与最小值
来源：http://qh.hahajie.cn

Py:   max(arr);  min(arr)
来源：http://wu.bookmarksfly.cn

PHP:  max($arr);  min($arr);
来源：http://up.szxytkj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qn.shxzskj.cn

TS:   Math.max(...arr);
来源：http://az.asd995.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ck.shxzskj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gb.lnxyls.cn

Ruby: arr.max;  arr.min
来源：http://rj.shtwfgs.cn

C#:   list.Max();  list.Min()
来源：http://gp.szxytkj.cn

[D18] 扁平化嵌套数组
来源：http://kx.newstarts.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://so.chemitech.net.cn

PHP:  array_merge(...$nested);
来源：http://ol.chemitech.net.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xs.gzmigu.cn

TS:   nested.flat();
来源：http://kk.newstarts.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gr.gzmigu.cn

Go:   // 手写双层循环
来源：http://uy.gzmigu.cn

Ruby: nested.flatten
来源：http://wf.hnjuh.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://td.yuntaijiaju.cn

[D19] 按字段分组
来源：http://sz.nszjky.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ij.gzmigu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://to.huixiangedu.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bs.hnjuh.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://qw.szxytkj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ff.lnxyls.cn

Go:   // 手写 map[string][]T
来源：http://zp.bjjhwx.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://tj.shxzskj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nh.szsharing.cn

[D20] 统计每个元素出现次数
来源：http://bv.gzmigu.cn

Py:   Counter(arr)
来源：http://lv.jianghongdianzi.cn

PHP:  array_count_values($arr);
来源：http://ib.chemitech.net.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jianghongdianzi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://za.nicolike.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jh.hnjuh.cn

Go:   // 手写 map[T]int
来源：http://wh.521024.cn

Ruby: arr.tally
来源：http://yw.lnxyls.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mj.bjjhwx.cn

[D21] 判断是否包含某元素
来源：http://im.nicolike.cn

Py:   x in arr
来源：http://if.gzmigu.cn

PHP:  in_array($x, $arr, true);
来源：http://jo.yuexingan06.cn

JS:   arr.includes(x)
来源：http://qi.szxytkj.cn

TS:   arr.includes(x)
来源：http://wk.hnjuh.cn

Java: list.contains(x)
来源：http://lt.asd995.cn

Go:   slices.Contains(arr, x)
来源：http://pe.9csxet.cn

Ruby: arr.include?(x)
来源：http://nz.hnjuh.cn

C#:   list.Contains(x)
来源：http://rq.colortex.cn

[D22] 复制数组（避免共享引用）
来源：http://os.colortex.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://av.yuexingan06.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rk.jianghongdianzi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zx.shxzskj.cn

TS:   [...arr];
来源：http://cr.bookmarksfly.cn

Java: new ArrayList<>(list);
来源：http://pf.hahajie.cn

Go:   copied := append([]int(nil), arr...)
来源：http://cw.muxihuayi.cn

Ruby: arr.dup;  arr.clone
来源：http://dc.wgjwhj.cn

C#:   new List<int>(list);
来源：http://df.bookmarksfly.cn

[D23] reduce 累积计算
来源：http://ed.muxihuayi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://id.huanxung.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ox.lnxyls.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ni.9csxet.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dy.huixinmuqiang.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://yn.lnxyls.cn

Go:   // 手写循环
来源：http://tw.shxzukj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bn.jctech888.com.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ue.panjiajie.cn

[D24] 字典 / Map 基本操作
来源：http://uo.521024.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qn.newstarts.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ds.huixiangedu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://oy.newstarts.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mb.newstarts.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hc.nicolike.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wa.newstarts.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ce.521024.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dm.huanxung.cn

[D25] Set 集合去重与交并差
来源：http://qk.haigaiapp.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ay.bjjhwx.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://oz.szxytkj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://kl.bookmarksfly.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://sz.colortex.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://le.muxihuayi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hu.lnxyls.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://oz.nszjky.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wn.huanxung.cn

[D26] 数组转字符串
来源：http://co.asd995.cn

Py:   ", ".join(map(str, arr))
来源：http://oe.chemitech.net.cn

PHP:  implode(", ", $arr);
来源：http://aw.szsharing.cn

JS:   arr.join(", ")
来源：http://yf.nszjky.cn

TS:   arr.join(", ")
来源：http://jj.9csxet.cn

Java: String.join(", ", list)
来源：http://bc.yuntaijiaju.cn

Go:   strings.Join(strs, ", ")
来源：http://ks.nicolike.cn

Ruby: arr.join(", ")
来源：http://ou.panjiajie.cn

C#:   string.Join(", ", list)
来源：http://rk.9csxet.cn

================================================================================
来源：http://or.bookmarksfly.cn

E. 字符串处理
来源：http://tr.hahajie.cn

================================================================================
来源：http://pr.szsharing.cn

[E01] 拼接字符串
来源：http://ki.huanxung.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://eo.jctech888.com.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vt.huixinmuqiang.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xj.szxytkj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nr.shxzskj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://dd.shxzukj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fj.hahajie.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://oy.chemitech.net.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://uc.yuntaijiaju.cn

[E02] 重复字符串
来源：http://cb.bjjhwx.cn

Py:   "ab" * 3
来源：http://mg.shtwfgs.cn

PHP:  str_repeat("ab", 3);
来源：http://dv.gzmigu.cn

JS:   "ab".repeat(3)
来源：http://zp.521024.cn

TS:   "ab".repeat(3)
来源：http://mx.hahajie.cn

Java: "ab".repeat(3)
来源：http://lw.wgjwhj.cn

Go:   strings.Repeat("ab", 3)
来源：http://vs.newstarts.cn

Ruby: "ab" * 3
来源：http://kr.9csxet.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://nx.hahajie.cn

[E03] 截取子串
来源：http://ic.wgjwhj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nr.nicolike.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qq.521024.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gw.jctech888.com.cn

TS:   s.slice(1, 4)
来源：http://bm.shtwfgs.cn

Java: s.substring(1, 4)
来源：http://qi.nszjky.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wg.wgjwhj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://rd.chemitech.net.cn

C#:   s.Substring(1, 3)
来源：http://wq.hahajie.cn

[E04] 查找子串位置
来源：http://kf.yuexingan06.cn

Py:   s.find("x");  s.index("x")
来源：http://lo.lnxyls.cn

PHP:  strpos($s, "x");
来源：http://ii.gzmigu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ro.newstarts.cn

TS:   s.indexOf("x")
来源：http://bm.jianghongdianzi.cn

Java: s.indexOf("x")
来源：http://vm.wgjwhj.cn

Go:   strings.Index(s, "x")
来源：http://xt.jianghongdianzi.cn

Ruby: s.index("x")
来源：http://pf.hnjuh.cn

C#:   s.IndexOf("x")
来源：http://nq.gzmigu.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://xq.jctech888.com.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://bq.szsharing.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mr.szsharing.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sv.shxzukj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://sm.gzmigu.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cf.yuexingan06.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://do.panjiajie.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gh.huanxung.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://aj.nszjky.cn

[E06] 替换子串
来源：http://aw.wgjwhj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hq.lnxyls.cn

PHP:  str_replace("a", "b", $s);
来源：http://oh.jctech888.com.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pp.colortex.cn

TS:   s.replaceAll("a", "b")
来源：http://rt.hnjuh.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jv.huanxung.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qx.jianghongdianzi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ic.nszjky.cn

C#:   s.Replace("a", "b")
来源：http://on.colortex.cn

[E07] 按分隔符拆分
来源：http://nc.bookmarksfly.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rh.huixiangedu.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gv.panjiajie.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://bg.colortex.cn

TS:   s.split(",")
来源：http://qw.hnjuh.cn

Java: s.split(",");  s.split("\\s+")
来源：http://kv.wgjwhj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rm.shxzskj.cn

Ruby: s.split(",");  s.split
来源：http://xe.lnxyls.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://uf.yuntaijiaju.cn

[E08] 数组按分隔符合并
来源：http://df.hahajie.cn

Py:   ",".join(items)
来源：http://eq.yuexingan06.cn

PHP:  implode(",", $items);
来源：http://yj.newstarts.cn

JS:   items.join(",")
来源：http://cg.szxytkj.cn

TS:   items.join(",")
来源：http://vj.bookmarksfly.cn

Java: String.join(",", items)
来源：http://lc.chemitech.net.cn

Go:   strings.Join(items, ",")
来源：http://sd.chemitech.net.cn

Ruby: items.join(",")
来源：http://ys.shxzskj.cn

C#:   string.Join(",", items)
来源：http://be.huixinmuqiang.cn

[E09] 去除所有空白字符
来源：http://xs.newstarts.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://aj.colortex.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://tz.asd995.cn

JS:   s.replace(/\s+/g, "")
来源：http://tk.nicolike.cn

TS:   s.replace(/\s+/g, "")
来源：http://xl.jctech888.com.cn

Java: s.replaceAll("\\s+", "")
来源：http://or.bookmarksfly.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ke.hnjuh.cn

Ruby: s.gsub(/\s+/, "")
来源：http://is.yuexingan06.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qo.shtwfgs.cn

[E10] 左侧补零 / 定长填充
来源：http://es.muxihuayi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xq.huanxung.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://gu.szxytkj.cn

JS:   "7".padStart(3, "0")
来源：http://xj.9csxet.cn

TS:   "7".padStart(3, "0")
来源：http://bv.wgjwhj.cn

Java: String.format("%03d", 7)
来源：http://tp.hahajie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://va.9csxet.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mo.huixinmuqiang.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zk.newstarts.cn

[E11] 反转字符串
来源：http://pk.haigaiapp.cn

Py:   s[::-1]
来源：http://bd.panjiajie.cn

PHP:  strrev($s);
来源：http://fk.lnxyls.cn

JS:   [...s].reverse().join("")
来源：http://lb.hahajie.cn

TS:   [...s].reverse().join("")
来源：http://xe.bookmarksfly.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://zr.nszjky.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://nj.hnjuh.cn

Ruby: s.reverse
来源：http://wi.bjjhwx.cn

C#:   new string(s.Reverse().ToArray())
来源：http://lm.jianghongdianzi.cn

[E12] 统计某字符出现次数
来源：http://dd.asd995.cn

Py:   s.count("a")
来源：http://pp.szxytkj.cn

PHP:  substr_count($s, "a");
来源：http://rn.yuexingan06.cn

JS:   s.split("a").length - 1
来源：http://ik.haigaiapp.cn

TS:   s.split("a").length - 1
来源：http://cr.jianghongdianzi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kl.lnxyls.cn

Go:   strings.Count(s, "a")
来源：http://mv.asd995.cn

Ruby: s.count("a")
来源：http://ol.panjiajie.cn

C#:   s.Count(c => c == 'a')
来源：http://gn.huixiangedu.cn

[E13] 逐字符遍历
来源：http://vf.bjjhwx.cn

Py:   for ch in s: print(ch)
来源：http://aa.newstarts.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://lr.asd995.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://fr.shxzukj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://lc.nszjky.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://un.hnjuh.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.yuexingan06.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://zm.huanxung.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mh.huixiangedu.cn

[E14] URL 编码与 Base64
来源：http://ax.nszjky.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://le.szxytkj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://dn.yuexingan06.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xh.panjiajie.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xk.jianghongdianzi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rk.bjjhwx.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tm.huixinmuqiang.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vi.yuexingan06.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nc.yuexingan06.cn

[E15] HTML 转义 / 反转义
来源：http://it.jctech888.com.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://rc.hnjuh.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://au.nicolike.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mk.nszjky.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://co.newstarts.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xp.muxihuayi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vr.szxytkj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ju.wgjwhj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ty.shxzskj.cn

[E16] 数字千分位
来源：http://dq.9csxet.cn

Py:   f"{1234567:,}"
来源：http://ou.nszjky.cn


<!-- 参考信息 -->