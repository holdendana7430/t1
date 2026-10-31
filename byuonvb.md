代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vq.hahajie.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xo.huixiangedu.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zg.9csxet.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fg.hnjuh.cn

[D11] 反转数组
来源：http://zm.shxzukj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://gv.wgjwhj.cn

PHP:  array_reverse($arr);
来源：http://hl.asd995.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://tf.huixiangedu.cn

TS:   [...arr].reverse();
来源：http://sa.9csxet.cn

Java: Collections.reverse(list);
来源：http://zo.521024.cn

Go:   slices.Reverse(arr)
来源：http://ys.hnjuh.cn

Ruby: arr.reverse
来源：http://ex.huanxung.cn

C#:   list.Reverse();
来源：http://tp.9csxet.cn

[D12] 查找元素下标
来源：http://wv.bookmarksfly.cn

Py:   arr.index(x);  x in arr
来源：http://fe.nicolike.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://aa.asd995.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cg.hnjuh.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mi.shxzukj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qk.9csxet.cn

Go:   slices.Index(arr, x)
来源：http://ih.shtwfgs.cn

Ruby: arr.index(x)
来源：http://cf.panjiajie.cn

C#:   list.IndexOf(x);
来源：http://ja.gzmigu.cn

[D13] 过滤（保留满足条件的）
来源：http://qk.szxytkj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wx.hahajie.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://nw.shxzukj.cn

JS:   arr.filter(x => x > 3)
来源：http://fs.hnjuh.cn

TS:   arr.filter(x => x > 3)
来源：http://ew.shtwfgs.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jj.nszjky.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rx.haigaiapp.cn

Ruby: arr.select { |x| x > 3 }
来源：http://jz.asd995.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ik.haigaiapp.cn

[D14] 映射转换（每个元素变形）
来源：http://ph.hnjuh.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xh.jctech888.com.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dl.nicolike.cn

JS:   arr.map(x => x * 2)
来源：http://oc.wgjwhj.cn

TS:   arr.map(x => x * 2)
来源：http://yv.asd995.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ts.chemitech.net.cn

Go:   // 手写循环
来源：http://xo.huanxung.cn

Ruby: arr.map { |x| x * 2 }
来源：http://be.nicolike.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://pv.yuexingan06.cn

[D15] 去重
来源：http://cg.huanxung.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://az.bjjhwx.cn

PHP:  array_unique($arr);
来源：http://jo.colortex.cn

JS:   [...new Set(arr)]
来源：http://ir.wgjwhj.cn

TS:   [...new Set(arr)]
来源：http://yt.hahajie.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ul.wgjwhj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ci.bjjhwx.cn

Ruby: arr.uniq
来源：http://ve.yuntaijiaju.cn

C#:   list.Distinct().ToList()
来源：http://ek.szxytkj.cn

[D16] 求和与平均值
来源：http://jk.hnjuh.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dq.muxihuayi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mp.asd995.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fx.jianghongdianzi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fy.newstarts.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fc.shxzukj.cn

Go:   // 手写循环累加
来源：http://wg.nicolike.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://in.shxzukj.cn

C#:   list.Sum();  list.Average()
来源：http://oe.huixinmuqiang.cn

[D17] 最大值与最小值
来源：http://up.jianghongdianzi.cn

Py:   max(arr);  min(arr)
来源：http://it.521024.cn

PHP:  max($arr);  min($arr);
来源：http://gu.gzmigu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://za.jctech888.com.cn

TS:   Math.max(...arr);
来源：http://bh.szsharing.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ya.wgjwhj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zg.panjiajie.cn

Ruby: arr.max;  arr.min
来源：http://es.haigaiapp.cn

C#:   list.Max();  list.Min()
来源：http://fl.asd995.cn

[D18] 扁平化嵌套数组
来源：http://nq.hahajie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ks.muxihuayi.cn

PHP:  array_merge(...$nested);
来源：http://pz.shtwfgs.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://nv.szxytkj.cn

TS:   nested.flat();
来源：http://zo.colortex.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fs.nicolike.cn

Go:   // 手写双层循环
来源：http://xl.521024.cn

Ruby: nested.flatten
来源：http://vu.shtwfgs.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://yw.bookmarksfly.cn

[D19] 按字段分组
来源：http://om.huixiangedu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://al.nicolike.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kd.bookmarksfly.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qd.huanxung.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://kw.lnxyls.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dv.shtwfgs.cn

Go:   // 手写 map[string][]T
来源：http://uu.521024.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ab.haigaiapp.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xc.szxytkj.cn

[D20] 统计每个元素出现次数
来源：http://wy.haigaiapp.cn

Py:   Counter(arr)
来源：http://jk.muxihuayi.cn

PHP:  array_count_values($arr);
来源：http://dx.wgjwhj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rn.huixiangedu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qp.521024.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://pt.521024.cn

Go:   // 手写 map[T]int
来源：http://bd.szxytkj.cn

Ruby: arr.tally
来源：http://qa.colortex.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ht.yuexingan06.cn

[D21] 判断是否包含某元素
来源：http://jy.bookmarksfly.cn

Py:   x in arr
来源：http://zp.huanxung.cn

PHP:  in_array($x, $arr, true);
来源：http://xj.gzmigu.cn

JS:   arr.includes(x)
来源：http://rc.yuntaijiaju.cn

TS:   arr.includes(x)
来源：http://rd.muxihuayi.cn

Java: list.contains(x)
来源：http://lq.chemitech.net.cn

Go:   slices.Contains(arr, x)
来源：http://qw.huixinmuqiang.cn

Ruby: arr.include?(x)
来源：http://wh.yuexingan06.cn

C#:   list.Contains(x)
来源：http://zw.hnjuh.cn

[D22] 复制数组（避免共享引用）
来源：http://fr.bookmarksfly.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://rs.wgjwhj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://oz.jianghongdianzi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rm.bookmarksfly.cn

TS:   [...arr];
来源：http://hi.shtwfgs.cn

Java: new ArrayList<>(list);
来源：http://qa.hnjuh.cn

Go:   copied := append([]int(nil), arr...)
来源：http://el.shtwfgs.cn

Ruby: arr.dup;  arr.clone
来源：http://jk.hnjuh.cn

C#:   new List<int>(list);
来源：http://cl.huanxung.cn

[D23] reduce 累积计算
来源：http://ej.lnxyls.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://tf.521024.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://nu.chemitech.net.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qy.nszjky.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mq.shxzukj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://nz.yuexingan06.cn

Go:   // 手写循环
来源：http://vd.muxihuayi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kq.lnxyls.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://or.hnjuh.cn

[D24] 字典 / Map 基本操作
来源：http://gj.haigaiapp.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ap.521024.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kh.521024.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://js.szsharing.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rq.bookmarksfly.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://av.521024.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://sw.huanxung.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bz.gzmigu.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lj.jianghongdianzi.cn

[D25] Set 集合去重与交并差
来源：http://rx.gzmigu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zq.shtwfgs.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ve.wgjwhj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ij.szsharing.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xh.huixiangedu.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mc.bookmarksfly.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tx.hnjuh.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://po.shxzukj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://tx.szsharing.cn

[D26] 数组转字符串
来源：http://wv.huanxung.cn

Py:   ", ".join(map(str, arr))
来源：http://tn.asd995.cn

PHP:  implode(", ", $arr);
来源：http://sg.shxzskj.cn

JS:   arr.join(", ")
来源：http://gd.huixiangedu.cn

TS:   arr.join(", ")
来源：http://xe.9csxet.cn

Java: String.join(", ", list)
来源：http://ws.jianghongdianzi.cn

Go:   strings.Join(strs, ", ")
来源：http://xf.nicolike.cn

Ruby: arr.join(", ")
来源：http://fo.muxihuayi.cn

C#:   string.Join(", ", list)
来源：http://bc.shtwfgs.cn

================================================================================
来源：http://za.shxzukj.cn

E. 字符串处理
来源：http://vd.chemitech.net.cn

================================================================================
来源：http://ag.huixiangedu.cn

[E01] 拼接字符串
来源：http://yz.yuexingan06.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ji.jianghongdianzi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://in.colortex.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://oq.521024.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://iy.bjjhwx.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ai.hahajie.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://km.nszjky.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xj.huixiangedu.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://pi.huixiangedu.cn

[E02] 重复字符串
来源：http://gb.yuntaijiaju.cn

Py:   "ab" * 3
来源：http://vi.colortex.cn

PHP:  str_repeat("ab", 3);
来源：http://ur.panjiajie.cn

JS:   "ab".repeat(3)
来源：http://fa.chemitech.net.cn

TS:   "ab".repeat(3)
来源：http://px.bjjhwx.cn

Java: "ab".repeat(3)
来源：http://bp.bookmarksfly.cn

Go:   strings.Repeat("ab", 3)
来源：http://kx.gzmigu.cn

Ruby: "ab" * 3
来源：http://uf.nicolike.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://op.huanxung.cn

[E03] 截取子串
来源：http://nd.colortex.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://aw.newstarts.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://si.bjjhwx.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jl.bookmarksfly.cn

TS:   s.slice(1, 4)
来源：http://js.huanxung.cn

Java: s.substring(1, 4)
来源：http://ck.nszjky.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ii.shtwfgs.cn

Ruby: s[1, 3];  s[1..3]
来源：http://yz.shtwfgs.cn

C#:   s.Substring(1, 3)
来源：http://iu.bookmarksfly.cn

[E04] 查找子串位置
来源：http://oo.newstarts.cn

Py:   s.find("x");  s.index("x")
来源：http://mr.gzmigu.cn

PHP:  strpos($s, "x");
来源：http://ff.shxzskj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://yl.shxzukj.cn

TS:   s.indexOf("x")
来源：http://gu.muxihuayi.cn

Java: s.indexOf("x")
来源：http://wu.newstarts.cn

Go:   strings.Index(s, "x")
来源：http://jh.yuexingan06.cn

Ruby: s.index("x")
来源：http://bh.panjiajie.cn

C#:   s.IndexOf("x")
来源：http://av.hnjuh.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://us.shtwfgs.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dt.jctech888.com.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vp.gzmigu.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xy.haigaiapp.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://hf.hahajie.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://di.szxytkj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dj.huixiangedu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gj.newstarts.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mp.jctech888.com.cn

[E06] 替换子串
来源：http://tk.bjjhwx.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ix.gzmigu.cn

PHP:  str_replace("a", "b", $s);
来源：http://ay.jianghongdianzi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://id.9csxet.cn

TS:   s.replaceAll("a", "b")
来源：http://eb.newstarts.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://os.nszjky.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tn.yuexingan06.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ja.shxzskj.cn

C#:   s.Replace("a", "b")
来源：http://qv.szxytkj.cn

[E07] 按分隔符拆分
来源：http://ka.hnjuh.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://sp.szxytkj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fs.shxzukj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://up.hnjuh.cn

TS:   s.split(",")
来源：http://ni.nicolike.cn

Java: s.split(",");  s.split("\\s+")
来源：http://tw.muxihuayi.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://du.nszjky.cn

Ruby: s.split(",");  s.split
来源：http://cx.shxzukj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://cw.asd995.cn

[E08] 数组按分隔符合并
来源：http://eh.asd995.cn

Py:   ",".join(items)
来源：http://mn.jianghongdianzi.cn

PHP:  implode(",", $items);
来源：http://rz.hahajie.cn

JS:   items.join(",")
来源：http://as.panjiajie.cn

TS:   items.join(",")
来源：http://ou.newstarts.cn

Java: String.join(",", items)
来源：http://au.chemitech.net.cn

Go:   strings.Join(items, ",")
来源：http://kn.newstarts.cn

Ruby: items.join(",")
来源：http://xd.nszjky.cn

C#:   string.Join(",", items)
来源：http://pv.huixiangedu.cn

[E09] 去除所有空白字符
来源：http://ce.9csxet.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://tc.huixiangedu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jq.haigaiapp.cn

JS:   s.replace(/\s+/g, "")
来源：http://wn.nicolike.cn

TS:   s.replace(/\s+/g, "")
来源：http://ys.huixinmuqiang.cn

Java: s.replaceAll("\\s+", "")
来源：http://cb.shtwfgs.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://xg.colortex.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ht.szxytkj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gn.muxihuayi.cn

[E10] 左侧补零 / 定长填充
来源：http://jm.huixinmuqiang.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cw.huanxung.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://sk.huanxung.cn

JS:   "7".padStart(3, "0")
来源：http://fy.huixinmuqiang.cn

TS:   "7".padStart(3, "0")
来源：http://bh.521024.cn

Java: String.format("%03d", 7)
来源：http://iw.9csxet.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://dk.jianghongdianzi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ud.shtwfgs.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qv.szsharing.cn

[E11] 反转字符串
来源：http://da.lnxyls.cn

Py:   s[::-1]
来源：http://xc.szsharing.cn

PHP:  strrev($s);
来源：http://uw.9csxet.cn

JS:   [...s].reverse().join("")
来源：http://im.chemitech.net.cn

TS:   [...s].reverse().join("")
来源：http://lf.jianghongdianzi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ic.muxihuayi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://mi.szxytkj.cn

Ruby: s.reverse
来源：http://kv.gzmigu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://bb.lnxyls.cn

[E12] 统计某字符出现次数
来源：http://hg.huanxung.cn

Py:   s.count("a")
来源：http://dz.jctech888.com.cn

PHP:  substr_count($s, "a");
来源：http://er.huanxung.cn

JS:   s.split("a").length - 1
来源：http://ka.panjiajie.cn

TS:   s.split("a").length - 1
来源：http://vx.hahajie.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://uv.hahajie.cn

Go:   strings.Count(s, "a")
来源：http://ld.asd995.cn

Ruby: s.count("a")
来源：http://or.nicolike.cn

C#:   s.Count(c => c == 'a')
来源：http://dz.lnxyls.cn

[E13] 逐字符遍历
来源：http://pt.asd995.cn

Py:   for ch in s: print(ch)
来源：http://vy.nicolike.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bl.hahajie.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://yx.jctech888.com.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://se.yuexingan06.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vw.chemitech.net.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tt.szsharing.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://vm.shxzskj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bu.wgjwhj.cn

[E14] URL 编码与 Base64
来源：http://ox.haigaiapp.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://tr.521024.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://cz.asd995.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ss.szxytkj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wg.panjiajie.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kj.newstarts.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ja.gzmigu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vd.shxzskj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ad.jctech888.com.cn

[E15] HTML 转义 / 反转义
来源：http://bo.wgjwhj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://mh.bookmarksfly.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://be.huanxung.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://su.chemitech.net.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://gy.newstarts.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zx.huixiangedu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://pq.jctech888.com.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xj.huixinmuqiang.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lf.shtwfgs.cn

[E16] 数字千分位
来源：http://bq.szxytkj.cn

Py:   f"{1234567:,}"
来源：http://al.szxytkj.cn

PHP:  number_format(1234567);
来源：http://zg.huixiangedu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://gg.szxytkj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ga.szsharing.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://pu.shxzskj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zb.huixinmuqiang.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://cc.bjjhwx.cn

C#:   1234567.ToString("N0")
来源：http://ty.haigaiapp.cn

[E17] 首字母大写
来源：http://bo.shxzukj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wd.yuexingan06.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://wl.newstarts.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mj.hnjuh.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rf.yuntaijiaju.cn


<!-- 参考信息 -->