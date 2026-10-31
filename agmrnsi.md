代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://su.haigaiapp.cn

C#:   a.Concat(b).ToList()
来源：http://tj.yuntaijiaju.cn

[D09] 排序（升序）
来源：http://ue.shxzskj.cn

Py:   sorted(arr);  arr.sort()
来源：http://fi.lnxyls.cn

PHP:  sort($arr);
来源：http://ue.asd995.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://yo.gzmigu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://dj.yuntaijiaju.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://eh.newstarts.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://as.521024.cn

Ruby: arr.sort
来源：http://bp.huixinmuqiang.cn

C#:   list.Sort();
来源：http://rm.shtwfgs.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://zf.colortex.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://lv.panjiajie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wx.bjjhwx.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hy.panjiajie.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://yh.muxihuayi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jv.wgjwhj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://gz.hahajie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xh.bookmarksfly.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yz.nszjky.cn

[D11] 反转数组
来源：http://ak.shxzukj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://qx.szsharing.cn

PHP:  array_reverse($arr);
来源：http://ui.shxzukj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://my.shxzukj.cn

TS:   [...arr].reverse();
来源：http://yj.huixiangedu.cn

Java: Collections.reverse(list);
来源：http://th.lnxyls.cn

Go:   slices.Reverse(arr)
来源：http://hi.huixiangedu.cn

Ruby: arr.reverse
来源：http://ub.jianghongdianzi.cn

C#:   list.Reverse();
来源：http://mw.lnxyls.cn

[D12] 查找元素下标
来源：http://dy.huanxung.cn

Py:   arr.index(x);  x in arr
来源：http://ba.jctech888.com.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vl.jianghongdianzi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://db.yuntaijiaju.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qy.nszjky.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wc.jctech888.com.cn

Go:   slices.Index(arr, x)
来源：http://vu.muxihuayi.cn

Ruby: arr.index(x)
来源：http://ga.9csxet.cn

C#:   list.IndexOf(x);
来源：http://te.huanxung.cn

[D13] 过滤（保留满足条件的）
来源：http://yj.bjjhwx.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nc.huanxung.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://el.shxzukj.cn

JS:   arr.filter(x => x > 3)
来源：http://sx.hnjuh.cn

TS:   arr.filter(x => x > 3)
来源：http://yr.asd995.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://uh.panjiajie.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://su.szxytkj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://mc.nszjky.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://vm.jctech888.com.cn

[D14] 映射转换（每个元素变形）
来源：http://rd.haigaiapp.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://am.bjjhwx.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://pe.shxzskj.cn

JS:   arr.map(x => x * 2)
来源：http://vy.wgjwhj.cn

TS:   arr.map(x => x * 2)
来源：http://ir.muxihuayi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://lr.huanxung.cn

Go:   // 手写循环
来源：http://gq.hnjuh.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ez.gzmigu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://pn.muxihuayi.cn

[D15] 去重
来源：http://op.jianghongdianzi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xr.wgjwhj.cn

PHP:  array_unique($arr);
来源：http://rc.colortex.cn

JS:   [...new Set(arr)]
来源：http://bi.gzmigu.cn

TS:   [...new Set(arr)]
来源：http://on.haigaiapp.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://tz.yuntaijiaju.cn

Go:   // 用 map[T]struct{} 手写
来源：http://mk.nicolike.cn

Ruby: arr.uniq
来源：http://ge.hahajie.cn

C#:   list.Distinct().ToList()
来源：http://jm.wgjwhj.cn

[D16] 求和与平均值
来源：http://dq.asd995.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gt.chemitech.net.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nu.asd995.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://cf.bjjhwx.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qj.wgjwhj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://la.jianghongdianzi.cn

Go:   // 手写循环累加
来源：http://dn.jianghongdianzi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://kt.jianghongdianzi.cn

C#:   list.Sum();  list.Average()
来源：http://ly.bjjhwx.cn

[D17] 最大值与最小值
来源：http://xp.bookmarksfly.cn

Py:   max(arr);  min(arr)
来源：http://tj.shxzskj.cn

PHP:  max($arr);  min($arr);
来源：http://hy.shxzskj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://yq.jianghongdianzi.cn

TS:   Math.max(...arr);
来源：http://uy.hnjuh.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://up.szsharing.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xb.521024.cn

Ruby: arr.max;  arr.min
来源：http://ee.wgjwhj.cn

C#:   list.Max();  list.Min()
来源：http://ck.shtwfgs.cn

[D18] 扁平化嵌套数组
来源：http://ym.shxzskj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xo.gzmigu.cn

PHP:  array_merge(...$nested);
来源：http://do.yuntaijiaju.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hx.shtwfgs.cn

TS:   nested.flat();
来源：http://ug.jctech888.com.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://eu.hnjuh.cn

Go:   // 手写双层循环
来源：http://yi.bjjhwx.cn

Ruby: nested.flatten
来源：http://jp.521024.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://va.hnjuh.cn

[D19] 按字段分组
来源：http://fm.hnjuh.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ne.jianghongdianzi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fi.wgjwhj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://yy.521024.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://wa.shxzukj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://na.colortex.cn

Go:   // 手写 map[string][]T
来源：http://gf.muxihuayi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://nk.asd995.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://le.gzmigu.cn

[D20] 统计每个元素出现次数
来源：http://ru.muxihuayi.cn

Py:   Counter(arr)
来源：http://lw.gzmigu.cn

PHP:  array_count_values($arr);
来源：http://gu.szsharing.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pd.asd995.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://km.huixinmuqiang.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://pr.bjjhwx.cn

Go:   // 手写 map[T]int
来源：http://kp.wgjwhj.cn

Ruby: arr.tally
来源：http://dp.yuntaijiaju.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ls.huixiangedu.cn

[D21] 判断是否包含某元素
来源：http://kg.shxzskj.cn

Py:   x in arr
来源：http://sl.jianghongdianzi.cn

PHP:  in_array($x, $arr, true);
来源：http://nj.szxytkj.cn

JS:   arr.includes(x)
来源：http://wv.haigaiapp.cn

TS:   arr.includes(x)
来源：http://gz.wgjwhj.cn

Java: list.contains(x)
来源：http://jk.colortex.cn

Go:   slices.Contains(arr, x)
来源：http://rq.asd995.cn

Ruby: arr.include?(x)
来源：http://wf.huixinmuqiang.cn

C#:   list.Contains(x)
来源：http://fp.huanxung.cn

[D22] 复制数组（避免共享引用）
来源：http://sg.shxzukj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vu.huixiangedu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://lr.gzmigu.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jc.shxzskj.cn

TS:   [...arr];
来源：http://qz.gzmigu.cn

Java: new ArrayList<>(list);
来源：http://gr.szsharing.cn

Go:   copied := append([]int(nil), arr...)
来源：http://vv.bjjhwx.cn

Ruby: arr.dup;  arr.clone
来源：http://fq.asd995.cn

C#:   new List<int>(list);
来源：http://yj.wgjwhj.cn

[D23] reduce 累积计算
来源：http://oy.jctech888.com.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://im.newstarts.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ga.shtwfgs.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ld.9csxet.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gl.yuexingan06.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://xs.jctech888.com.cn

Go:   // 手写循环
来源：http://bo.hahajie.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ei.asd995.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ia.szxytkj.cn

[D24] 字典 / Map 基本操作
来源：http://jl.shxzskj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://fg.huixiangedu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hy.hnjuh.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vv.shtwfgs.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://of.bjjhwx.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vs.nicolike.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://li.haigaiapp.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ik.haigaiapp.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fk.panjiajie.cn

[D25] Set 集合去重与交并差
来源：http://wf.bjjhwx.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://oe.jianghongdianzi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zi.nicolike.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rw.nszjky.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rs.bookmarksfly.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://td.nicolike.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://re.haigaiapp.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ln.shxzukj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fq.wgjwhj.cn

[D26] 数组转字符串
来源：http://vy.newstarts.cn

Py:   ", ".join(map(str, arr))
来源：http://ph.asd995.cn

PHP:  implode(", ", $arr);
来源：http://je.wgjwhj.cn

JS:   arr.join(", ")
来源：http://ng.bjjhwx.cn

TS:   arr.join(", ")
来源：http://mj.colortex.cn

Java: String.join(", ", list)
来源：http://qu.huanxung.cn

Go:   strings.Join(strs, ", ")
来源：http://sp.yuexingan06.cn

Ruby: arr.join(", ")
来源：http://er.521024.cn

C#:   string.Join(", ", list)
来源：http://sa.newstarts.cn

================================================================================
来源：http://gg.521024.cn

E. 字符串处理
来源：http://ym.huixiangedu.cn

================================================================================
来源：http://fg.chemitech.net.cn

[E01] 拼接字符串
来源：http://tf.panjiajie.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tw.muxihuayi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dr.newstarts.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ss.haigaiapp.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tc.yuexingan06.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://yl.jctech888.com.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://in.gzmigu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://sd.shxzskj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ys.gzmigu.cn

[E02] 重复字符串
来源：http://wu.hahajie.cn

Py:   "ab" * 3
来源：http://vv.shxzukj.cn

PHP:  str_repeat("ab", 3);
来源：http://zu.asd995.cn

JS:   "ab".repeat(3)
来源：http://yv.huanxung.cn

TS:   "ab".repeat(3)
来源：http://al.nicolike.cn

Java: "ab".repeat(3)
来源：http://ct.muxihuayi.cn

Go:   strings.Repeat("ab", 3)
来源：http://sd.chemitech.net.cn

Ruby: "ab" * 3
来源：http://oa.huanxung.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gs.panjiajie.cn

[E03] 截取子串
来源：http://te.lnxyls.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yz.szsharing.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://pb.bookmarksfly.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://eb.wgjwhj.cn

TS:   s.slice(1, 4)
来源：http://da.shxzukj.cn

Java: s.substring(1, 4)
来源：http://xw.chemitech.net.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hn.chemitech.net.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ci.newstarts.cn

C#:   s.Substring(1, 3)
来源：http://tt.huanxung.cn

[E04] 查找子串位置
来源：http://gh.shxzukj.cn

Py:   s.find("x");  s.index("x")
来源：http://qc.newstarts.cn

PHP:  strpos($s, "x");
来源：http://ge.shtwfgs.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gc.wgjwhj.cn

TS:   s.indexOf("x")
来源：http://ih.colortex.cn

Java: s.indexOf("x")
来源：http://tk.haigaiapp.cn

Go:   strings.Index(s, "x")
来源：http://hb.bjjhwx.cn

Ruby: s.index("x")
来源：http://ul.gzmigu.cn

C#:   s.IndexOf("x")
来源：http://tp.yuntaijiaju.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://aq.haigaiapp.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mh.newstarts.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xc.lnxyls.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pn.szsharing.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://oi.jianghongdianzi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pi.muxihuayi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ue.nicolike.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ru.nszjky.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gk.jianghongdianzi.cn

[E06] 替换子串
来源：http://se.newstarts.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ee.lnxyls.cn

PHP:  str_replace("a", "b", $s);
来源：http://wl.huixiangedu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mc.newstarts.cn

TS:   s.replaceAll("a", "b")
来源：http://ui.szsharing.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://im.newstarts.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://pl.chemitech.net.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kb.szsharing.cn

C#:   s.Replace("a", "b")
来源：http://rc.muxihuayi.cn

[E07] 按分隔符拆分
来源：http://qu.huixinmuqiang.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bc.szxytkj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qh.muxihuayi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ay.hnjuh.cn

TS:   s.split(",")
来源：http://bt.shxzskj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ys.bookmarksfly.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://gk.haigaiapp.cn

Ruby: s.split(",");  s.split
来源：http://ur.szxytkj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://au.9csxet.cn

[E08] 数组按分隔符合并
来源：http://lh.9csxet.cn

Py:   ",".join(items)
来源：http://yv.jctech888.com.cn

PHP:  implode(",", $items);
来源：http://yl.shxzukj.cn

JS:   items.join(",")
来源：http://bd.yuntaijiaju.cn

TS:   items.join(",")
来源：http://nx.muxihuayi.cn

Java: String.join(",", items)
来源：http://vy.shxzukj.cn

Go:   strings.Join(items, ",")
来源：http://tk.chemitech.net.cn

Ruby: items.join(",")
来源：http://yp.szxytkj.cn

C#:   string.Join(",", items)
来源：http://gf.521024.cn

[E09] 去除所有空白字符
来源：http://ts.huixinmuqiang.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bh.szxytkj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qe.newstarts.cn

JS:   s.replace(/\s+/g, "")
来源：http://vk.shxzskj.cn

TS:   s.replace(/\s+/g, "")
来源：http://gj.yuntaijiaju.cn

Java: s.replaceAll("\\s+", "")
来源：http://rf.shxzskj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ch.chemitech.net.cn

Ruby: s.gsub(/\s+/, "")
来源：http://mo.asd995.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cr.jianghongdianzi.cn

[E10] 左侧补零 / 定长填充
来源：http://wr.wgjwhj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ui.hnjuh.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://dc.panjiajie.cn

JS:   "7".padStart(3, "0")
来源：http://vw.521024.cn

TS:   "7".padStart(3, "0")
来源：http://pn.jctech888.com.cn

Java: String.format("%03d", 7)
来源：http://ar.nszjky.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://nv.hnjuh.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://yf.szxytkj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://lm.muxihuayi.cn

[E11] 反转字符串
来源：http://dp.nicolike.cn

Py:   s[::-1]
来源：http://jw.panjiajie.cn

PHP:  strrev($s);
来源：http://ke.jctech888.com.cn

JS:   [...s].reverse().join("")
来源：http://ap.huanxung.cn

TS:   [...s].reverse().join("")
来源：http://zn.nicolike.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://tj.bjjhwx.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://wd.bjjhwx.cn

Ruby: s.reverse
来源：http://gs.huixiangedu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://li.bjjhwx.cn

[E12] 统计某字符出现次数
来源：http://kk.jianghongdianzi.cn

Py:   s.count("a")
来源：http://ns.asd995.cn

PHP:  substr_count($s, "a");
来源：http://cf.wgjwhj.cn

JS:   s.split("a").length - 1
来源：http://ek.yuntaijiaju.cn

TS:   s.split("a").length - 1
来源：http://wd.gzmigu.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://on.yuexingan06.cn

Go:   strings.Count(s, "a")
来源：http://jw.lnxyls.cn

Ruby: s.count("a")
来源：http://im.shxzskj.cn

C#:   s.Count(c => c == 'a')
来源：http://pw.jianghongdianzi.cn

[E13] 逐字符遍历
来源：http://he.gzmigu.cn

Py:   for ch in s: print(ch)
来源：http://db.jctech888.com.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qm.9csxet.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://kq.huanxung.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://vs.szsharing.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://my.jianghongdianzi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vf.bookmarksfly.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://eb.szsharing.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://iy.wgjwhj.cn

[E14] URL 编码与 Base64
来源：http://xg.9csxet.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rd.yuexingan06.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://dw.521024.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rp.asd995.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ks.asd995.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://or.shxzskj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://aw.lnxyls.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://pz.colortex.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zh.lnxyls.cn

[E15] HTML 转义 / 反转义
来源：http://xh.521024.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ya.jctech888.com.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ky.jctech888.com.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mw.nszjky.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://wu.newstarts.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://uj.shtwfgs.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zd.shxzskj.cn


<!-- 参考信息 -->