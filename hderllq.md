代发 wailian999

PHP:  sort($arr);
来源：http://ec.bjjhwx.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ne.yuntaijiaju.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://uy.asd995.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://hx.panjiajie.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://uu.nszjky.cn

Ruby: arr.sort
来源：http://qm.521024.cn

C#:   list.Sort();
来源：http://yw.nszjky.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://iq.muxihuayi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rv.9csxet.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hf.hnjuh.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://yi.wgjwhj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bn.szxytkj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ie.haigaiapp.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://oy.jianghongdianzi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://px.haigaiapp.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://eq.yuexingan06.cn

[D11] 反转数组
来源：http://tw.asd995.cn

Py:   arr[::-1];  arr.reverse()
来源：http://yg.nicolike.cn

PHP:  array_reverse($arr);
来源：http://ur.szsharing.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yh.colortex.cn

TS:   [...arr].reverse();
来源：http://ne.shtwfgs.cn

Java: Collections.reverse(list);
来源：http://kg.nszjky.cn

Go:   slices.Reverse(arr)
来源：http://wk.chemitech.net.cn

Ruby: arr.reverse
来源：http://el.huanxung.cn

C#:   list.Reverse();
来源：http://wh.hahajie.cn

[D12] 查找元素下标
来源：http://tw.chemitech.net.cn

Py:   arr.index(x);  x in arr
来源：http://yg.haigaiapp.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zb.shxzukj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ri.huixiangedu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dk.wgjwhj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ni.lnxyls.cn

Go:   slices.Index(arr, x)
来源：http://yb.bjjhwx.cn

Ruby: arr.index(x)
来源：http://bn.shxzukj.cn

C#:   list.IndexOf(x);
来源：http://mi.huixiangedu.cn

[D13] 过滤（保留满足条件的）
来源：http://ov.yuntaijiaju.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xs.huixiangedu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hl.haigaiapp.cn

JS:   arr.filter(x => x > 3)
来源：http://sd.gzmigu.cn

TS:   arr.filter(x => x > 3)
来源：http://ut.lnxyls.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ai.haigaiapp.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wa.huixinmuqiang.cn

Ruby: arr.select { |x| x > 3 }
来源：http://sd.jctech888.com.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ta.shxzukj.cn

[D14] 映射转换（每个元素变形）
来源：http://hf.huixiangedu.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://aj.huixinmuqiang.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://km.muxihuayi.cn

JS:   arr.map(x => x * 2)
来源：http://wp.jianghongdianzi.cn

TS:   arr.map(x => x * 2)
来源：http://rd.chemitech.net.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://rg.huanxung.cn

Go:   // 手写循环
来源：http://ne.gzmigu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://hs.shxzskj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://hu.colortex.cn

[D15] 去重
来源：http://oz.huixiangedu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zz.wgjwhj.cn

PHP:  array_unique($arr);
来源：http://hp.newstarts.cn

JS:   [...new Set(arr)]
来源：http://ok.jctech888.com.cn

TS:   [...new Set(arr)]
来源：http://gj.asd995.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ec.colortex.cn

Go:   // 用 map[T]struct{} 手写
来源：http://lc.jianghongdianzi.cn

Ruby: arr.uniq
来源：http://vj.panjiajie.cn

C#:   list.Distinct().ToList()
来源：http://ax.nicolike.cn

[D16] 求和与平均值
来源：http://hl.chemitech.net.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hi.shtwfgs.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ry.lnxyls.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://il.yuexingan06.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wt.huixiangedu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ae.huanxung.cn

Go:   // 手写循环累加
来源：http://zg.jctech888.com.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://te.huixiangedu.cn

C#:   list.Sum();  list.Average()
来源：http://kc.shtwfgs.cn

[D17] 最大值与最小值
来源：http://ap.wgjwhj.cn

Py:   max(arr);  min(arr)
来源：http://bo.hahajie.cn

PHP:  max($arr);  min($arr);
来源：http://wg.lnxyls.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wl.szxytkj.cn

TS:   Math.max(...arr);
来源：http://vs.nicolike.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://gc.bookmarksfly.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ki.colortex.cn

Ruby: arr.max;  arr.min
来源：http://rl.shxzukj.cn

C#:   list.Max();  list.Min()
来源：http://gv.521024.cn

[D18] 扁平化嵌套数组
来源：http://fv.bookmarksfly.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ut.asd995.cn

PHP:  array_merge(...$nested);
来源：http://xf.colortex.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ip.szxytkj.cn

TS:   nested.flat();
来源：http://ua.yuexingan06.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dn.szxytkj.cn

Go:   // 手写双层循环
来源：http://za.yuexingan06.cn

Ruby: nested.flatten
来源：http://qn.newstarts.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://vm.huanxung.cn

[D19] 按字段分组
来源：http://qj.wgjwhj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gq.jianghongdianzi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://gs.huanxung.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wm.lnxyls.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://jm.lnxyls.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://sw.521024.cn

Go:   // 手写 map[string][]T
来源：http://jv.newstarts.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://xz.jctech888.com.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zk.wgjwhj.cn

[D20] 统计每个元素出现次数
来源：http://sf.yuexingan06.cn

Py:   Counter(arr)
来源：http://hc.nszjky.cn

PHP:  array_count_values($arr);
来源：http://lb.gzmigu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kg.huanxung.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sd.asd995.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xm.bookmarksfly.cn

Go:   // 手写 map[T]int
来源：http://qy.bookmarksfly.cn

Ruby: arr.tally
来源：http://nt.jianghongdianzi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://bi.yuntaijiaju.cn

[D21] 判断是否包含某元素
来源：http://xg.nicolike.cn

Py:   x in arr
来源：http://zu.yuexingan06.cn

PHP:  in_array($x, $arr, true);
来源：http://zm.szsharing.cn

JS:   arr.includes(x)
来源：http://aw.shxzskj.cn

TS:   arr.includes(x)
来源：http://pt.wgjwhj.cn

Java: list.contains(x)
来源：http://sv.muxihuayi.cn

Go:   slices.Contains(arr, x)
来源：http://gp.wgjwhj.cn

Ruby: arr.include?(x)
来源：http://zy.nszjky.cn

C#:   list.Contains(x)
来源：http://kn.yuexingan06.cn

[D22] 复制数组（避免共享引用）
来源：http://bi.yuntaijiaju.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pj.jctech888.com.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://as.521024.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://yh.szxytkj.cn

TS:   [...arr];
来源：http://tv.shxzukj.cn

Java: new ArrayList<>(list);
来源：http://vc.yuexingan06.cn

Go:   copied := append([]int(nil), arr...)
来源：http://gh.nszjky.cn

Ruby: arr.dup;  arr.clone
来源：http://uu.muxihuayi.cn

C#:   new List<int>(list);
来源：http://vc.huanxung.cn

[D23] reduce 累积计算
来源：http://of.huanxung.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://le.chemitech.net.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jm.shxzskj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qp.huixiangedu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://aa.haigaiapp.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ck.szsharing.cn

Go:   // 手写循环
来源：http://so.szxytkj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://iu.lnxyls.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://te.haigaiapp.cn

[D24] 字典 / Map 基本操作
来源：http://ax.lnxyls.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pu.hahajie.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://cb.nszjky.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hb.shtwfgs.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://th.wgjwhj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://iv.yuntaijiaju.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://cl.shtwfgs.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bv.nszjky.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pp.wgjwhj.cn

[D25] Set 集合去重与交并差
来源：http://iy.nszjky.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ya.szsharing.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hu.shxzskj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://yx.yuntaijiaju.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ga.shxzskj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ks.bookmarksfly.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ym.9csxet.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zw.huixiangedu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qa.panjiajie.cn

[D26] 数组转字符串
来源：http://vo.colortex.cn

Py:   ", ".join(map(str, arr))
来源：http://oo.jctech888.com.cn

PHP:  implode(", ", $arr);
来源：http://gc.bjjhwx.cn

JS:   arr.join(", ")
来源：http://wp.wgjwhj.cn

TS:   arr.join(", ")
来源：http://rt.szxytkj.cn

Java: String.join(", ", list)
来源：http://nk.wgjwhj.cn

Go:   strings.Join(strs, ", ")
来源：http://ys.muxihuayi.cn

Ruby: arr.join(", ")
来源：http://wk.newstarts.cn

C#:   string.Join(", ", list)
来源：http://js.wgjwhj.cn

================================================================================
来源：http://rk.lnxyls.cn

E. 字符串处理
来源：http://wz.panjiajie.cn

================================================================================
来源：http://en.lnxyls.cn

[E01] 拼接字符串
来源：http://ql.shxzskj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cq.chemitech.net.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://sn.shxzskj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tw.lnxyls.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://oj.huanxung.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pp.gzmigu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vx.hnjuh.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pq.newstarts.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ab.shxzukj.cn

[E02] 重复字符串
来源：http://lf.lnxyls.cn

Py:   "ab" * 3
来源：http://sk.hnjuh.cn

PHP:  str_repeat("ab", 3);
来源：http://cv.huanxung.cn

JS:   "ab".repeat(3)
来源：http://hx.521024.cn

TS:   "ab".repeat(3)
来源：http://gx.nszjky.cn

Java: "ab".repeat(3)
来源：http://gp.huanxung.cn

Go:   strings.Repeat("ab", 3)
来源：http://iy.szsharing.cn

Ruby: "ab" * 3
来源：http://cq.521024.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rr.huixiangedu.cn

[E03] 截取子串
来源：http://cr.szxytkj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mw.lnxyls.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ff.lnxyls.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dp.lnxyls.cn

TS:   s.slice(1, 4)
来源：http://fh.shxzskj.cn

Java: s.substring(1, 4)
来源：http://fk.hahajie.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://yq.jianghongdianzi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://hx.huixiangedu.cn

C#:   s.Substring(1, 3)
来源：http://wi.nicolike.cn

[E04] 查找子串位置
来源：http://uz.szxytkj.cn

Py:   s.find("x");  s.index("x")
来源：http://oj.jctech888.com.cn

PHP:  strpos($s, "x");
来源：http://zf.huixiangedu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://oh.huanxung.cn

TS:   s.indexOf("x")
来源：http://br.huixinmuqiang.cn

Java: s.indexOf("x")
来源：http://tx.9csxet.cn

Go:   strings.Index(s, "x")
来源：http://fo.asd995.cn

Ruby: s.index("x")
来源：http://ux.shtwfgs.cn

C#:   s.IndexOf("x")
来源：http://rc.newstarts.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://rr.huixiangedu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xi.haigaiapp.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://um.nszjky.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://df.shtwfgs.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://kb.huixinmuqiang.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dr.shxzskj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dq.haigaiapp.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://nn.bjjhwx.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://lp.szsharing.cn

[E06] 替换子串
来源：http://sy.nicolike.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jd.haigaiapp.cn

PHP:  str_replace("a", "b", $s);
来源：http://er.chemitech.net.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://oa.shxzukj.cn

TS:   s.replaceAll("a", "b")
来源：http://un.hahajie.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://df.chemitech.net.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rx.shxzskj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://cf.huixinmuqiang.cn

C#:   s.Replace("a", "b")
来源：http://nt.panjiajie.cn

[E07] 按分隔符拆分
来源：http://pe.asd995.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qz.colortex.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://au.muxihuayi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://th.huanxung.cn

TS:   s.split(",")
来源：http://nn.shtwfgs.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ew.huanxung.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mt.jianghongdianzi.cn

Ruby: s.split(",");  s.split
来源：http://qg.jctech888.com.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qs.shxzukj.cn

[E08] 数组按分隔符合并
来源：http://me.szxytkj.cn

Py:   ",".join(items)
来源：http://qz.yuexingan06.cn

PHP:  implode(",", $items);
来源：http://pa.jianghongdianzi.cn

JS:   items.join(",")
来源：http://kk.szxytkj.cn

TS:   items.join(",")
来源：http://jw.gzmigu.cn

Java: String.join(",", items)
来源：http://rn.jctech888.com.cn

Go:   strings.Join(items, ",")
来源：http://cm.hnjuh.cn

Ruby: items.join(",")
来源：http://ol.asd995.cn

C#:   string.Join(",", items)
来源：http://gs.yuexingan06.cn

[E09] 去除所有空白字符
来源：http://zu.jianghongdianzi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wu.haigaiapp.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ei.shxzukj.cn

JS:   s.replace(/\s+/g, "")
来源：http://lm.szxytkj.cn

TS:   s.replace(/\s+/g, "")
来源：http://mr.hnjuh.cn

Java: s.replaceAll("\\s+", "")
来源：http://uv.newstarts.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ef.bookmarksfly.cn

Ruby: s.gsub(/\s+/, "")
来源：http://vo.jctech888.com.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://he.hahajie.cn

[E10] 左侧补零 / 定长填充
来源：http://sw.521024.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zq.szxytkj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://um.shxzskj.cn

JS:   "7".padStart(3, "0")
来源：http://xq.bjjhwx.cn

TS:   "7".padStart(3, "0")
来源：http://je.huixinmuqiang.cn

Java: String.format("%03d", 7)
来源：http://jx.shxzukj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://qb.jctech888.com.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ki.521024.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rf.szxytkj.cn

[E11] 反转字符串
来源：http://vj.muxihuayi.cn

Py:   s[::-1]
来源：http://ee.hahajie.cn

PHP:  strrev($s);
来源：http://my.9csxet.cn

JS:   [...s].reverse().join("")
来源：http://or.colortex.cn

TS:   [...s].reverse().join("")
来源：http://oo.szsharing.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://iy.jctech888.com.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ty.521024.cn

Ruby: s.reverse
来源：http://yo.lnxyls.cn

C#:   new string(s.Reverse().ToArray())
来源：http://wi.jctech888.com.cn

[E12] 统计某字符出现次数
来源：http://wd.yuntaijiaju.cn

Py:   s.count("a")
来源：http://nv.newstarts.cn

PHP:  substr_count($s, "a");
来源：http://do.shtwfgs.cn

JS:   s.split("a").length - 1
来源：http://yn.lnxyls.cn

TS:   s.split("a").length - 1
来源：http://hc.chemitech.net.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zw.lnxyls.cn

Go:   strings.Count(s, "a")
来源：http://vw.huixiangedu.cn

Ruby: s.count("a")
来源：http://jp.szxytkj.cn

C#:   s.Count(c => c == 'a')
来源：http://am.gzmigu.cn

[E13] 逐字符遍历
来源：http://kt.9csxet.cn

Py:   for ch in s: print(ch)
来源：http://ym.bookmarksfly.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ry.lnxyls.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://kj.bookmarksfly.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ju.bookmarksfly.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://dg.muxihuayi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fr.yuntaijiaju.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://jn.lnxyls.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ay.gzmigu.cn

[E14] URL 编码与 Base64
来源：http://xi.shxzukj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://si.szxytkj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://uq.huanxung.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://sy.bookmarksfly.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://yz.yuntaijiaju.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ov.bjjhwx.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://sr.szsharing.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ow.muxihuayi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gk.lnxyls.cn

[E15] HTML 转义 / 反转义
来源：http://wc.nicolike.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ua.asd995.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://cs.huanxung.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://yb.nicolike.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://db.jianghongdianzi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://sw.9csxet.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mr.huixinmuqiang.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ob.huanxung.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wf.521024.cn

[E16] 数字千分位
来源：http://jo.shxzskj.cn

Py:   f"{1234567:,}"
来源：http://yz.shxzukj.cn


<!-- 参考信息 -->