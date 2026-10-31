代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://he.huixinmuqiang.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zx.hahajie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://if.9csxet.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bi.asd995.cn

[D11] 反转数组
来源：http://th.gzmigu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://fr.huixiangedu.cn

PHP:  array_reverse($arr);
来源：http://xk.bjjhwx.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xu.bookmarksfly.cn

TS:   [...arr].reverse();
来源：http://lw.jctech888.com.cn

Java: Collections.reverse(list);
来源：http://rq.hnjuh.cn

Go:   slices.Reverse(arr)
来源：http://gb.shxzukj.cn

Ruby: arr.reverse
来源：http://fp.jctech888.com.cn

C#:   list.Reverse();
来源：http://db.hahajie.cn

[D12] 查找元素下标
来源：http://wt.hnjuh.cn

Py:   arr.index(x);  x in arr
来源：http://nn.nicolike.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ui.gzmigu.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wi.asd995.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uv.lnxyls.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mj.nicolike.cn

Go:   slices.Index(arr, x)
来源：http://pt.wgjwhj.cn

Ruby: arr.index(x)
来源：http://fx.colortex.cn

C#:   list.IndexOf(x);
来源：http://pz.haigaiapp.cn

[D13] 过滤（保留满足条件的）
来源：http://mp.shxzukj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ns.jianghongdianzi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://sz.asd995.cn

JS:   arr.filter(x => x > 3)
来源：http://fu.wgjwhj.cn

TS:   arr.filter(x => x > 3)
来源：http://yu.huixiangedu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tk.bjjhwx.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kz.yuntaijiaju.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ob.asd995.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ej.huanxung.cn

[D14] 映射转换（每个元素变形）
来源：http://au.jianghongdianzi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ow.shtwfgs.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qp.521024.cn

JS:   arr.map(x => x * 2)
来源：http://ja.nszjky.cn

TS:   arr.map(x => x * 2)
来源：http://hu.nszjky.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://uc.bjjhwx.cn

Go:   // 手写循环
来源：http://kz.9csxet.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ty.szxytkj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://zu.521024.cn

[D15] 去重
来源：http://ox.yuexingan06.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cp.wgjwhj.cn

PHP:  array_unique($arr);
来源：http://xk.szsharing.cn

JS:   [...new Set(arr)]
来源：http://to.chemitech.net.cn

TS:   [...new Set(arr)]
来源：http://yt.nszjky.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://vl.newstarts.cn

Go:   // 用 map[T]struct{} 手写
来源：http://bu.hahajie.cn

Ruby: arr.uniq
来源：http://lz.shxzukj.cn

C#:   list.Distinct().ToList()
来源：http://up.shtwfgs.cn

[D16] 求和与平均值
来源：http://vs.yuexingan06.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dd.hahajie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ri.jianghongdianzi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ki.9csxet.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://sb.jctech888.com.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qj.bookmarksfly.cn

Go:   // 手写循环累加
来源：http://bq.bjjhwx.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://eo.szxytkj.cn

C#:   list.Sum();  list.Average()
来源：http://ez.yuexingan06.cn

[D17] 最大值与最小值
来源：http://ra.nszjky.cn

Py:   max(arr);  min(arr)
来源：http://dx.jianghongdianzi.cn

PHP:  max($arr);  min($arr);
来源：http://kr.szxytkj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xy.nszjky.cn

TS:   Math.max(...arr);
来源：http://sj.jctech888.com.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ox.chemitech.net.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lp.chemitech.net.cn

Ruby: arr.max;  arr.min
来源：http://qq.muxihuayi.cn

C#:   list.Max();  list.Min()
来源：http://bk.szxytkj.cn

[D18] 扁平化嵌套数组
来源：http://vn.bjjhwx.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xc.wgjwhj.cn

PHP:  array_merge(...$nested);
来源：http://qy.hahajie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ob.jctech888.com.cn

TS:   nested.flat();
来源：http://po.haigaiapp.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kf.muxihuayi.cn

Go:   // 手写双层循环
来源：http://rt.bjjhwx.cn

Ruby: nested.flatten
来源：http://gj.colortex.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://rr.huanxung.cn

[D19] 按字段分组
来源：http://qs.nszjky.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://uh.hahajie.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://nk.yuntaijiaju.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tu.nszjky.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://bv.shxzukj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vw.wgjwhj.cn

Go:   // 手写 map[string][]T
来源：http://vk.yuexingan06.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://yh.yuexingan06.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://an.521024.cn

[D20] 统计每个元素出现次数
来源：http://kl.hnjuh.cn

Py:   Counter(arr)
来源：http://yg.bjjhwx.cn

PHP:  array_count_values($arr);
来源：http://cw.huixiangedu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dh.colortex.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zr.panjiajie.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jc.gzmigu.cn

Go:   // 手写 map[T]int
来源：http://av.muxihuayi.cn

Ruby: arr.tally
来源：http://xo.shtwfgs.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://sn.jctech888.com.cn

[D21] 判断是否包含某元素
来源：http://gx.yuexingan06.cn

Py:   x in arr
来源：http://lq.chemitech.net.cn

PHP:  in_array($x, $arr, true);
来源：http://eb.bjjhwx.cn

JS:   arr.includes(x)
来源：http://bn.shxzukj.cn

TS:   arr.includes(x)
来源：http://ui.yuntaijiaju.cn

Java: list.contains(x)
来源：http://rz.hnjuh.cn

Go:   slices.Contains(arr, x)
来源：http://fq.jianghongdianzi.cn

Ruby: arr.include?(x)
来源：http://si.panjiajie.cn

C#:   list.Contains(x)
来源：http://ft.szsharing.cn

[D22] 复制数组（避免共享引用）
来源：http://np.asd995.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hj.chemitech.net.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://co.newstarts.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mm.wgjwhj.cn

TS:   [...arr];
来源：http://sh.haigaiapp.cn

Java: new ArrayList<>(list);
来源：http://vu.bjjhwx.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ie.panjiajie.cn

Ruby: arr.dup;  arr.clone
来源：http://fx.muxihuayi.cn

C#:   new List<int>(list);
来源：http://sj.wgjwhj.cn

[D23] reduce 累积计算
来源：http://cv.haigaiapp.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ng.newstarts.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://sl.huixinmuqiang.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mj.haigaiapp.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://et.huixiangedu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://wa.yuntaijiaju.cn

Go:   // 手写循环
来源：http://hj.9csxet.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bi.jctech888.com.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ye.jctech888.com.cn

[D24] 字典 / Map 基本操作
来源：http://kp.newstarts.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qb.huanxung.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://iv.jctech888.com.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ew.shtwfgs.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ov.colortex.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wk.yuexingan06.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qx.lnxyls.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://dj.wgjwhj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kb.yuntaijiaju.cn

[D25] Set 集合去重与交并差
来源：http://ki.wgjwhj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kc.wgjwhj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hl.jianghongdianzi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rv.nicolike.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zc.gzmigu.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ti.shtwfgs.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gk.newstarts.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ew.hahajie.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jh.bjjhwx.cn

[D26] 数组转字符串
来源：http://pi.chemitech.net.cn

Py:   ", ".join(map(str, arr))
来源：http://fm.hahajie.cn

PHP:  implode(", ", $arr);
来源：http://mc.asd995.cn

JS:   arr.join(", ")
来源：http://ns.muxihuayi.cn

TS:   arr.join(", ")
来源：http://fi.huixiangedu.cn

Java: String.join(", ", list)
来源：http://ih.shxzskj.cn

Go:   strings.Join(strs, ", ")
来源：http://vl.hahajie.cn

Ruby: arr.join(", ")
来源：http://ul.gzmigu.cn

C#:   string.Join(", ", list)
来源：http://gy.huanxung.cn

================================================================================
来源：http://ok.hahajie.cn

E. 字符串处理
来源：http://yh.nicolike.cn

================================================================================
来源：http://sj.jianghongdianzi.cn

[E01] 拼接字符串
来源：http://mn.chemitech.net.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://sj.muxihuayi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wn.nicolike.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fr.haigaiapp.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gc.huixiangedu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://at.yuexingan06.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gz.szxytkj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://uw.jctech888.com.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://es.yuexingan06.cn

[E02] 重复字符串
来源：http://te.wgjwhj.cn

Py:   "ab" * 3
来源：http://jt.huanxung.cn

PHP:  str_repeat("ab", 3);
来源：http://ak.nszjky.cn

JS:   "ab".repeat(3)
来源：http://yy.haigaiapp.cn

TS:   "ab".repeat(3)
来源：http://uf.nicolike.cn

Java: "ab".repeat(3)
来源：http://cm.nicolike.cn

Go:   strings.Repeat("ab", 3)
来源：http://yo.muxihuayi.cn

Ruby: "ab" * 3
来源：http://fh.jianghongdianzi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ot.panjiajie.cn

[E03] 截取子串
来源：http://cy.panjiajie.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hs.panjiajie.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://al.szsharing.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qs.shxzskj.cn

TS:   s.slice(1, 4)
来源：http://ql.asd995.cn

Java: s.substring(1, 4)
来源：http://lh.newstarts.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xs.nszjky.cn

Ruby: s[1, 3];  s[1..3]
来源：http://yh.muxihuayi.cn

C#:   s.Substring(1, 3)
来源：http://oy.bookmarksfly.cn

[E04] 查找子串位置
来源：http://li.lnxyls.cn

Py:   s.find("x");  s.index("x")
来源：http://nn.jctech888.com.cn

PHP:  strpos($s, "x");
来源：http://bn.panjiajie.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ya.huanxung.cn

TS:   s.indexOf("x")
来源：http://ii.yuntaijiaju.cn

Java: s.indexOf("x")
来源：http://sy.yuntaijiaju.cn

Go:   strings.Index(s, "x")
来源：http://eq.nszjky.cn

Ruby: s.index("x")
来源：http://zi.panjiajie.cn

C#:   s.IndexOf("x")
来源：http://nl.shxzukj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://vn.shxzukj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://vf.chemitech.net.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jb.9csxet.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://at.panjiajie.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://vq.chemitech.net.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hp.wgjwhj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://sj.jianghongdianzi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qu.colortex.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fx.lnxyls.cn

[E06] 替换子串
来源：http://qm.asd995.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ys.panjiajie.cn

PHP:  str_replace("a", "b", $s);
来源：http://vt.521024.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ss.jianghongdianzi.cn

TS:   s.replaceAll("a", "b")
来源：http://mk.newstarts.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ey.shtwfgs.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://nm.chemitech.net.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nf.yuexingan06.cn

C#:   s.Replace("a", "b")
来源：http://vw.muxihuayi.cn

[E07] 按分隔符拆分
来源：http://wd.szsharing.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ms.521024.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fc.szsharing.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://qp.asd995.cn

TS:   s.split(",")
来源：http://lr.panjiajie.cn

Java: s.split(",");  s.split("\\s+")
来源：http://uq.521024.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ku.muxihuayi.cn

Ruby: s.split(",");  s.split
来源：http://sc.huanxung.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wm.shtwfgs.cn

[E08] 数组按分隔符合并
来源：http://te.bookmarksfly.cn

Py:   ",".join(items)
来源：http://se.hahajie.cn

PHP:  implode(",", $items);
来源：http://ws.yuexingan06.cn

JS:   items.join(",")
来源：http://gm.bjjhwx.cn

TS:   items.join(",")
来源：http://ra.bookmarksfly.cn

Java: String.join(",", items)
来源：http://sn.huanxung.cn

Go:   strings.Join(items, ",")
来源：http://tq.shtwfgs.cn

Ruby: items.join(",")
来源：http://sl.huixiangedu.cn

C#:   string.Join(",", items)
来源：http://cx.9csxet.cn

[E09] 去除所有空白字符
来源：http://vx.huixiangedu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lp.panjiajie.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dc.szsharing.cn

JS:   s.replace(/\s+/g, "")
来源：http://zk.shxzskj.cn

TS:   s.replace(/\s+/g, "")
来源：http://nc.colortex.cn

Java: s.replaceAll("\\s+", "")
来源：http://bz.shxzukj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://tp.bookmarksfly.cn

Ruby: s.gsub(/\s+/, "")
来源：http://kj.jctech888.com.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://yu.shxzskj.cn

[E10] 左侧补零 / 定长填充
来源：http://kp.panjiajie.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wg.haigaiapp.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tm.bjjhwx.cn

JS:   "7".padStart(3, "0")
来源：http://me.9csxet.cn

TS:   "7".padStart(3, "0")
来源：http://ld.bjjhwx.cn

Java: String.format("%03d", 7)
来源：http://kb.chemitech.net.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ng.newstarts.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://eq.szsharing.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vg.9csxet.cn

[E11] 反转字符串
来源：http://cq.shxzskj.cn

Py:   s[::-1]
来源：http://me.yuntaijiaju.cn

PHP:  strrev($s);
来源：http://pd.huixinmuqiang.cn

JS:   [...s].reverse().join("")
来源：http://ut.huixiangedu.cn

TS:   [...s].reverse().join("")
来源：http://se.jctech888.com.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://vt.521024.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://fb.huixiangedu.cn

Ruby: s.reverse
来源：http://cu.muxihuayi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ck.nszjky.cn

[E12] 统计某字符出现次数
来源：http://tq.colortex.cn

Py:   s.count("a")
来源：http://dn.haigaiapp.cn

PHP:  substr_count($s, "a");
来源：http://qc.nszjky.cn

JS:   s.split("a").length - 1
来源：http://jc.shxzukj.cn

TS:   s.split("a").length - 1
来源：http://az.shxzskj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ef.haigaiapp.cn

Go:   strings.Count(s, "a")
来源：http://ll.huanxung.cn

Ruby: s.count("a")
来源：http://dr.panjiajie.cn

C#:   s.Count(c => c == 'a')
来源：http://ti.nszjky.cn

[E13] 逐字符遍历
来源：http://or.newstarts.cn

Py:   for ch in s: print(ch)
来源：http://sa.yuntaijiaju.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qs.hahajie.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://jo.yuexingan06.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://wc.shxzskj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ap.chemitech.net.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://as.nszjky.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://tb.szxytkj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dg.haigaiapp.cn

[E14] URL 编码与 Base64
来源：http://jv.nicolike.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://dm.yuexingan06.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ts.shxzukj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://iq.szxytkj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wf.lnxyls.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://sm.shxzukj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wd.521024.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xd.szxytkj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://or.521024.cn

[E15] HTML 转义 / 反转义
来源：http://da.szsharing.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://np.shtwfgs.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zf.lnxyls.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ub.muxihuayi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ro.huixinmuqiang.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://cc.newstarts.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rr.bookmarksfly.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jp.nicolike.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ct.hnjuh.cn

[E16] 数字千分位
来源：http://hv.newstarts.cn

Py:   f"{1234567:,}"
来源：http://mz.shxzskj.cn

PHP:  number_format(1234567);
来源：http://mb.hahajie.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://io.hahajie.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ih.huixinmuqiang.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fx.chemitech.net.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fj.shtwfgs.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://kh.hnjuh.cn

C#:   1234567.ToString("N0")
来源：http://th.yuntaijiaju.cn

[E17] 首字母大写
来源：http://mo.szsharing.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://eg.szsharing.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://xx.bjjhwx.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ak.hahajie.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jo.shxzukj.cn


<!-- 参考信息 -->