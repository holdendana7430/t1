代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yk.shxzskj.cn

Ruby: arr.sort
来源：http://hf.shxzukj.cn

C#:   list.Sort();
来源：http://gz.hnjuh.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://mm.colortex.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hr.szsharing.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ba.huixiangedu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://de.huixiangedu.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nu.bjjhwx.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vk.huanxung.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://kv.bookmarksfly.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tw.shxzskj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xi.521024.cn

[D11] 反转数组
来源：http://qu.521024.cn

Py:   arr[::-1];  arr.reverse()
来源：http://sx.huixinmuqiang.cn

PHP:  array_reverse($arr);
来源：http://fq.jianghongdianzi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lp.521024.cn

TS:   [...arr].reverse();
来源：http://hz.bjjhwx.cn

Java: Collections.reverse(list);
来源：http://ev.hahajie.cn

Go:   slices.Reverse(arr)
来源：http://fp.shtwfgs.cn

Ruby: arr.reverse
来源：http://bu.hahajie.cn

C#:   list.Reverse();
来源：http://ba.huixinmuqiang.cn

[D12] 查找元素下标
来源：http://py.huanxung.cn

Py:   arr.index(x);  x in arr
来源：http://sb.yuntaijiaju.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://cd.jctech888.com.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ni.lnxyls.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://oy.nicolike.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://if.nszjky.cn

Go:   slices.Index(arr, x)
来源：http://yx.huanxung.cn

Ruby: arr.index(x)
来源：http://gj.hnjuh.cn

C#:   list.IndexOf(x);
来源：http://zv.bookmarksfly.cn

[D13] 过滤（保留满足条件的）
来源：http://yb.jctech888.com.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ey.521024.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fe.huixinmuqiang.cn

JS:   arr.filter(x => x > 3)
来源：http://eg.huanxung.cn

TS:   arr.filter(x => x > 3)
来源：http://xu.nicolike.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lc.shxzukj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jy.newstarts.cn

Ruby: arr.select { |x| x > 3 }
来源：http://en.521024.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://mw.bookmarksfly.cn

[D14] 映射转换（每个元素变形）
来源：http://jy.gzmigu.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bg.wgjwhj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dd.colortex.cn

JS:   arr.map(x => x * 2)
来源：http://co.nszjky.cn

TS:   arr.map(x => x * 2)
来源：http://ho.asd995.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://yq.shtwfgs.cn

Go:   // 手写循环
来源：http://tt.huixinmuqiang.cn

Ruby: arr.map { |x| x * 2 }
来源：http://jd.hnjuh.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://al.huanxung.cn

[D15] 去重
来源：http://op.newstarts.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zc.huixinmuqiang.cn

PHP:  array_unique($arr);
来源：http://op.muxihuayi.cn

JS:   [...new Set(arr)]
来源：http://ph.9csxet.cn

TS:   [...new Set(arr)]
来源：http://uk.szxytkj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kn.newstarts.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ri.asd995.cn

Ruby: arr.uniq
来源：http://zm.muxihuayi.cn

C#:   list.Distinct().ToList()
来源：http://av.shxzskj.cn

[D16] 求和与平均值
来源：http://lh.521024.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ux.hnjuh.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wj.hnjuh.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ij.jctech888.com.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ig.hahajie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bx.yuexingan06.cn

Go:   // 手写循环累加
来源：http://ac.shxzukj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://na.jianghongdianzi.cn

C#:   list.Sum();  list.Average()
来源：http://yi.wgjwhj.cn

[D17] 最大值与最小值
来源：http://aj.nszjky.cn

Py:   max(arr);  min(arr)
来源：http://nh.yuexingan06.cn

PHP:  max($arr);  min($arr);
来源：http://he.nszjky.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://yn.shxzukj.cn

TS:   Math.max(...arr);
来源：http://px.yuexingan06.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://op.nszjky.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://co.lnxyls.cn

Ruby: arr.max;  arr.min
来源：http://ar.haigaiapp.cn

C#:   list.Max();  list.Min()
来源：http://ti.hnjuh.cn

[D18] 扁平化嵌套数组
来源：http://hb.shxzskj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xe.muxihuayi.cn

PHP:  array_merge(...$nested);
来源：http://wt.shtwfgs.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wl.panjiajie.cn

TS:   nested.flat();
来源：http://mh.521024.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tf.shtwfgs.cn

Go:   // 手写双层循环
来源：http://vk.nicolike.cn

Ruby: nested.flatten
来源：http://sv.newstarts.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://tc.shtwfgs.cn

[D19] 按字段分组
来源：http://pf.colortex.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://iq.szxytkj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lt.521024.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://co.jianghongdianzi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://tw.nszjky.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gh.huanxung.cn

Go:   // 手写 map[string][]T
来源：http://ee.yuexingan06.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ni.gzmigu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ut.nszjky.cn

[D20] 统计每个元素出现次数
来源：http://nl.newstarts.cn

Py:   Counter(arr)
来源：http://pv.shxzukj.cn

PHP:  array_count_values($arr);
来源：http://js.panjiajie.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ru.huanxung.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tw.bjjhwx.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zw.shtwfgs.cn

Go:   // 手写 map[T]int
来源：http://ir.huixinmuqiang.cn

Ruby: arr.tally
来源：http://df.muxihuayi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ax.shtwfgs.cn

[D21] 判断是否包含某元素
来源：http://en.huixinmuqiang.cn

Py:   x in arr
来源：http://iy.bookmarksfly.cn

PHP:  in_array($x, $arr, true);
来源：http://vh.szsharing.cn

JS:   arr.includes(x)
来源：http://rw.hahajie.cn

TS:   arr.includes(x)
来源：http://dj.huixiangedu.cn

Java: list.contains(x)
来源：http://ez.szsharing.cn

Go:   slices.Contains(arr, x)
来源：http://fd.shtwfgs.cn

Ruby: arr.include?(x)
来源：http://nx.newstarts.cn

C#:   list.Contains(x)
来源：http://lm.huixiangedu.cn

[D22] 复制数组（避免共享引用）
来源：http://fy.hahajie.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fl.lnxyls.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://pz.newstarts.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://pl.panjiajie.cn

TS:   [...arr];
来源：http://nr.bjjhwx.cn

Java: new ArrayList<>(list);
来源：http://ym.shxzukj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://mk.jianghongdianzi.cn

Ruby: arr.dup;  arr.clone
来源：http://ru.yuexingan06.cn

C#:   new List<int>(list);
来源：http://wa.szxytkj.cn

[D23] reduce 累积计算
来源：http://xv.newstarts.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://oy.nszjky.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://sj.panjiajie.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ko.wgjwhj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://db.521024.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://nm.yuntaijiaju.cn

Go:   // 手写循环
来源：http://kc.szsharing.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fo.wgjwhj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://sy.asd995.cn

[D24] 字典 / Map 基本操作
来源：http://ca.nszjky.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://dl.nicolike.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://cn.lnxyls.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wx.szxytkj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://kp.wgjwhj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://yn.shxzskj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qq.asd995.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ek.wgjwhj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://et.shtwfgs.cn

[D25] Set 集合去重与交并差
来源：http://oy.521024.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://dy.colortex.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ml.bookmarksfly.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fk.muxihuayi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://on.newstarts.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xy.huixiangedu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gg.huanxung.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hl.gzmigu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://gl.bookmarksfly.cn

[D26] 数组转字符串
来源：http://wn.hahajie.cn

Py:   ", ".join(map(str, arr))
来源：http://hw.yuntaijiaju.cn

PHP:  implode(", ", $arr);
来源：http://is.huixiangedu.cn

JS:   arr.join(", ")
来源：http://vi.yuexingan06.cn

TS:   arr.join(", ")
来源：http://le.bookmarksfly.cn

Java: String.join(", ", list)
来源：http://or.chemitech.net.cn

Go:   strings.Join(strs, ", ")
来源：http://bu.bookmarksfly.cn

Ruby: arr.join(", ")
来源：http://ho.bjjhwx.cn

C#:   string.Join(", ", list)
来源：http://to.nicolike.cn

================================================================================
来源：http://fk.panjiajie.cn

E. 字符串处理
来源：http://fe.yuntaijiaju.cn

================================================================================
来源：http://dr.9csxet.cn

[E01] 拼接字符串
来源：http://ar.chemitech.net.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zl.huanxung.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tc.shxzukj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mo.hnjuh.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fr.colortex.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vl.wgjwhj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ll.panjiajie.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fy.asd995.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xr.yuntaijiaju.cn

[E02] 重复字符串
来源：http://zf.9csxet.cn

Py:   "ab" * 3
来源：http://fz.newstarts.cn

PHP:  str_repeat("ab", 3);
来源：http://cv.panjiajie.cn

JS:   "ab".repeat(3)
来源：http://vc.wgjwhj.cn

TS:   "ab".repeat(3)
来源：http://gz.wgjwhj.cn

Java: "ab".repeat(3)
来源：http://mk.9csxet.cn

Go:   strings.Repeat("ab", 3)
来源：http://hy.hahajie.cn

Ruby: "ab" * 3
来源：http://yf.jianghongdianzi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ih.huanxung.cn

[E03] 截取子串
来源：http://uv.szxytkj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://dj.shxzukj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ch.huanxung.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://tv.yuntaijiaju.cn

TS:   s.slice(1, 4)
来源：http://vz.colortex.cn

Java: s.substring(1, 4)
来源：http://ew.nszjky.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zd.lnxyls.cn

Ruby: s[1, 3];  s[1..3]
来源：http://df.shtwfgs.cn

C#:   s.Substring(1, 3)
来源：http://tj.panjiajie.cn

[E04] 查找子串位置
来源：http://rh.chemitech.net.cn

Py:   s.find("x");  s.index("x")
来源：http://wl.jianghongdianzi.cn

PHP:  strpos($s, "x");
来源：http://br.asd995.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://lm.huixinmuqiang.cn

TS:   s.indexOf("x")
来源：http://mz.jianghongdianzi.cn

Java: s.indexOf("x")
来源：http://zh.hahajie.cn

Go:   strings.Index(s, "x")
来源：http://ew.huixinmuqiang.cn

Ruby: s.index("x")
来源：http://wd.yuexingan06.cn

C#:   s.IndexOf("x")
来源：http://gi.hnjuh.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://kx.gzmigu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cm.haigaiapp.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://nj.lnxyls.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ih.nszjky.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ao.jctech888.com.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://oi.521024.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://le.yuexingan06.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://eo.newstarts.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://by.asd995.cn

[E06] 替换子串
来源：http://qe.shtwfgs.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://le.shxzukj.cn

PHP:  str_replace("a", "b", $s);
来源：http://dg.jctech888.com.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wv.chemitech.net.cn

TS:   s.replaceAll("a", "b")
来源：http://cn.hnjuh.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qu.huixiangedu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qn.newstarts.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://as.nszjky.cn

C#:   s.Replace("a", "b")
来源：http://jt.shtwfgs.cn

[E07] 按分隔符拆分
来源：http://pv.panjiajie.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ka.521024.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ex.szxytkj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://al.bookmarksfly.cn

TS:   s.split(",")
来源：http://by.yuexingan06.cn

Java: s.split(",");  s.split("\\s+")
来源：http://nv.gzmigu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ws.wgjwhj.cn

Ruby: s.split(",");  s.split
来源：http://du.jctech888.com.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://or.lnxyls.cn

[E08] 数组按分隔符合并
来源：http://yz.asd995.cn

Py:   ",".join(items)
来源：http://jl.gzmigu.cn

PHP:  implode(",", $items);
来源：http://wa.muxihuayi.cn

JS:   items.join(",")
来源：http://bc.asd995.cn

TS:   items.join(",")
来源：http://xl.yuntaijiaju.cn

Java: String.join(",", items)
来源：http://dx.wgjwhj.cn

Go:   strings.Join(items, ",")
来源：http://dv.huixinmuqiang.cn

Ruby: items.join(",")
来源：http://ar.shtwfgs.cn

C#:   string.Join(",", items)
来源：http://pr.yuntaijiaju.cn

[E09] 去除所有空白字符
来源：http://yz.gzmigu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://od.nicolike.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dt.lnxyls.cn

JS:   s.replace(/\s+/g, "")
来源：http://wc.newstarts.cn

TS:   s.replace(/\s+/g, "")
来源：http://wt.wgjwhj.cn

Java: s.replaceAll("\\s+", "")
来源：http://wn.huixinmuqiang.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ar.hnjuh.cn

Ruby: s.gsub(/\s+/, "")
来源：http://cl.huixiangedu.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://aa.9csxet.cn

[E10] 左侧补零 / 定长填充
来源：http://bd.chemitech.net.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bd.chemitech.net.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ph.colortex.cn

JS:   "7".padStart(3, "0")
来源：http://to.jianghongdianzi.cn

TS:   "7".padStart(3, "0")
来源：http://jq.muxihuayi.cn

Java: String.format("%03d", 7)
来源：http://aj.wgjwhj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ju.muxihuayi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://yr.jctech888.com.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://lj.huixiangedu.cn

[E11] 反转字符串
来源：http://rq.chemitech.net.cn

Py:   s[::-1]
来源：http://vr.nicolike.cn

PHP:  strrev($s);
来源：http://ps.yuexingan06.cn

JS:   [...s].reverse().join("")
来源：http://hf.bjjhwx.cn

TS:   [...s].reverse().join("")
来源：http://eq.bookmarksfly.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://oa.muxihuayi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://lv.colortex.cn

Ruby: s.reverse
来源：http://vi.9csxet.cn

C#:   new string(s.Reverse().ToArray())
来源：http://wh.huanxung.cn

[E12] 统计某字符出现次数
来源：http://rn.shxzukj.cn

Py:   s.count("a")
来源：http://tt.hnjuh.cn

PHP:  substr_count($s, "a");
来源：http://ln.521024.cn

JS:   s.split("a").length - 1
来源：http://of.szsharing.cn

TS:   s.split("a").length - 1
来源：http://wv.chemitech.net.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vr.521024.cn

Go:   strings.Count(s, "a")
来源：http://en.chemitech.net.cn

Ruby: s.count("a")
来源：http://ec.lnxyls.cn

C#:   s.Count(c => c == 'a')
来源：http://kn.shtwfgs.cn

[E13] 逐字符遍历
来源：http://ir.haigaiapp.cn

Py:   for ch in s: print(ch)
来源：http://wg.gzmigu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ci.huixiangedu.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://dl.colortex.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://gb.nicolike.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vf.yuexingan06.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tm.nszjky.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://mg.yuexingan06.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hg.bookmarksfly.cn

[E14] URL 编码与 Base64
来源：http://bf.szsharing.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ip.jianghongdianzi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://yi.haigaiapp.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://un.yuntaijiaju.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ro.wgjwhj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ba.521024.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bn.haigaiapp.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://pr.yuntaijiaju.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://sp.nszjky.cn

[E15] HTML 转义 / 反转义
来源：http://yf.hnjuh.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://wa.huanxung.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://oi.colortex.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gy.9csxet.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://tb.shxzskj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xt.lnxyls.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://pz.hahajie.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vs.521024.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ij.newstarts.cn

[E16] 数字千分位
来源：http://lj.haigaiapp.cn

Py:   f"{1234567:,}"
来源：http://ax.bjjhwx.cn

PHP:  number_format(1234567);
来源：http://qb.521024.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://yw.hahajie.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://kf.chemitech.net.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xp.huixinmuqiang.cn


<!-- 参考信息 -->