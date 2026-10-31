代发 wailian999

TS:   [...arr].reverse();
来源：http://nv.asd995.cn

Java: Collections.reverse(list);
来源：http://xl.hnjuh.cn

Go:   slices.Reverse(arr)
来源：http://op.asd995.cn

Ruby: arr.reverse
来源：http://nx.muxihuayi.cn

C#:   list.Reverse();
来源：http://sw.panjiajie.cn

[D12] 查找元素下标
来源：http://ke.nszjky.cn

Py:   arr.index(x);  x in arr
来源：http://sb.shxzskj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tt.9csxet.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ho.yuntaijiaju.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dz.gzmigu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cn.yuexingan06.cn

Go:   slices.Index(arr, x)
来源：http://vu.hnjuh.cn

Ruby: arr.index(x)
来源：http://pt.wgjwhj.cn

C#:   list.IndexOf(x);
来源：http://dp.bjjhwx.cn

[D13] 过滤（保留满足条件的）
来源：http://iy.hnjuh.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://kn.szsharing.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hg.shxzukj.cn

JS:   arr.filter(x => x > 3)
来源：http://mn.521024.cn

TS:   arr.filter(x => x > 3)
来源：http://fx.huanxung.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://po.bookmarksfly.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://yx.huanxung.cn

Ruby: arr.select { |x| x > 3 }
来源：http://jh.chemitech.net.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://lr.panjiajie.cn

[D14] 映射转换（每个元素变形）
来源：http://bm.panjiajie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nq.huixinmuqiang.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fe.gzmigu.cn

JS:   arr.map(x => x * 2)
来源：http://ej.nicolike.cn

TS:   arr.map(x => x * 2)
来源：http://no.521024.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://xu.huixinmuqiang.cn

Go:   // 手写循环
来源：http://sy.yuexingan06.cn

Ruby: arr.map { |x| x * 2 }
来源：http://eu.haigaiapp.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://de.nicolike.cn

[D15] 去重
来源：http://su.yuexingan06.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lx.shxzukj.cn

PHP:  array_unique($arr);
来源：http://lj.lnxyls.cn

JS:   [...new Set(arr)]
来源：http://ie.gzmigu.cn

TS:   [...new Set(arr)]
来源：http://pr.muxihuayi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mt.jianghongdianzi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://hs.wgjwhj.cn

Ruby: arr.uniq
来源：http://hi.shtwfgs.cn

C#:   list.Distinct().ToList()
来源：http://bb.asd995.cn

[D16] 求和与平均值
来源：http://co.9csxet.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lv.wgjwhj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://io.asd995.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ca.hnjuh.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ih.bookmarksfly.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ex.9csxet.cn

Go:   // 手写循环累加
来源：http://hs.shtwfgs.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://my.hahajie.cn

C#:   list.Sum();  list.Average()
来源：http://ep.yuntaijiaju.cn

[D17] 最大值与最小值
来源：http://zk.huanxung.cn

Py:   max(arr);  min(arr)
来源：http://dw.newstarts.cn

PHP:  max($arr);  min($arr);
来源：http://yc.shtwfgs.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qa.huixinmuqiang.cn

TS:   Math.max(...arr);
来源：http://qa.lnxyls.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://dq.huanxung.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://cn.szsharing.cn

Ruby: arr.max;  arr.min
来源：http://tt.jianghongdianzi.cn

C#:   list.Max();  list.Min()
来源：http://ed.huanxung.cn

[D18] 扁平化嵌套数组
来源：http://rq.hahajie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://en.shtwfgs.cn

PHP:  array_merge(...$nested);
来源：http://ig.nicolike.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://uz.yuntaijiaju.cn

TS:   nested.flat();
来源：http://jv.huixinmuqiang.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ti.hnjuh.cn

Go:   // 手写双层循环
来源：http://vm.shtwfgs.cn

Ruby: nested.flatten
来源：http://hi.szxytkj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ue.shxzukj.cn

[D19] 按字段分组
来源：http://xr.521024.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://uv.szsharing.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kg.bjjhwx.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ty.jianghongdianzi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://fj.521024.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://nh.jctech888.com.cn

Go:   // 手写 map[string][]T
来源：http://md.jianghongdianzi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ep.szxytkj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://eq.shxzukj.cn

[D20] 统计每个元素出现次数
来源：http://bs.haigaiapp.cn

Py:   Counter(arr)
来源：http://cs.colortex.cn

PHP:  array_count_values($arr);
来源：http://fs.jianghongdianzi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uw.shxzskj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zd.huixiangedu.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zw.huixinmuqiang.cn

Go:   // 手写 map[T]int
来源：http://vv.521024.cn

Ruby: arr.tally
来源：http://zc.muxihuayi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://eu.wgjwhj.cn

[D21] 判断是否包含某元素
来源：http://eu.huixiangedu.cn

Py:   x in arr
来源：http://in.huanxung.cn

PHP:  in_array($x, $arr, true);
来源：http://qw.szsharing.cn

JS:   arr.includes(x)
来源：http://ao.huixinmuqiang.cn

TS:   arr.includes(x)
来源：http://wz.gzmigu.cn

Java: list.contains(x)
来源：http://cz.hnjuh.cn

Go:   slices.Contains(arr, x)
来源：http://gj.szsharing.cn

Ruby: arr.include?(x)
来源：http://km.521024.cn

C#:   list.Contains(x)
来源：http://yx.asd995.cn

[D22] 复制数组（避免共享引用）
来源：http://nw.lnxyls.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ko.nicolike.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://om.szxytkj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ly.shtwfgs.cn

TS:   [...arr];
来源：http://sf.wgjwhj.cn

Java: new ArrayList<>(list);
来源：http://fu.huanxung.cn

Go:   copied := append([]int(nil), arr...)
来源：http://xo.nicolike.cn

Ruby: arr.dup;  arr.clone
来源：http://kj.521024.cn

C#:   new List<int>(list);
来源：http://um.huixinmuqiang.cn

[D23] reduce 累积计算
来源：http://ui.shxzskj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://de.jctech888.com.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pl.haigaiapp.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ph.521024.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://eo.szsharing.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://vp.shxzskj.cn

Go:   // 手写循环
来源：http://ib.chemitech.net.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ex.szsharing.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rr.shtwfgs.cn

[D24] 字典 / Map 基本操作
来源：http://zg.panjiajie.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xs.nszjky.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wi.jianghongdianzi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://al.9csxet.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wv.gzmigu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://pw.haigaiapp.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://yn.shxzskj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gt.9csxet.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://su.chemitech.net.cn

[D25] Set 集合去重与交并差
来源：http://yg.shtwfgs.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kc.521024.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qz.huixiangedu.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xt.nicolike.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xl.9csxet.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://it.jianghongdianzi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wn.nicolike.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pn.wgjwhj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://py.shxzukj.cn

[D26] 数组转字符串
来源：http://nn.nicolike.cn

Py:   ", ".join(map(str, arr))
来源：http://zj.lnxyls.cn

PHP:  implode(", ", $arr);
来源：http://ic.chemitech.net.cn

JS:   arr.join(", ")
来源：http://rq.hahajie.cn

TS:   arr.join(", ")
来源：http://ir.lnxyls.cn

Java: String.join(", ", list)
来源：http://xk.lnxyls.cn

Go:   strings.Join(strs, ", ")
来源：http://jy.jctech888.com.cn

Ruby: arr.join(", ")
来源：http://fg.yuexingan06.cn

C#:   string.Join(", ", list)
来源：http://cc.shxzskj.cn

================================================================================
来源：http://ag.bjjhwx.cn

E. 字符串处理
来源：http://ns.jctech888.com.cn

================================================================================
来源：http://yq.asd995.cn

[E01] 拼接字符串
来源：http://nb.jctech888.com.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rz.colortex.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://on.huanxung.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://yq.shtwfgs.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gu.521024.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tm.bookmarksfly.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vh.9csxet.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://el.gzmigu.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://io.muxihuayi.cn

[E02] 重复字符串
来源：http://yx.asd995.cn

Py:   "ab" * 3
来源：http://pg.chemitech.net.cn

PHP:  str_repeat("ab", 3);
来源：http://bj.hahajie.cn

JS:   "ab".repeat(3)
来源：http://tb.bookmarksfly.cn

TS:   "ab".repeat(3)
来源：http://gc.asd995.cn

Java: "ab".repeat(3)
来源：http://rp.haigaiapp.cn

Go:   strings.Repeat("ab", 3)
来源：http://zj.hahajie.cn

Ruby: "ab" * 3
来源：http://zw.bjjhwx.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hh.jianghongdianzi.cn

[E03] 截取子串
来源：http://iw.huixinmuqiang.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yk.9csxet.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fc.gzmigu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hd.shxzukj.cn

TS:   s.slice(1, 4)
来源：http://lr.huixinmuqiang.cn

Java: s.substring(1, 4)
来源：http://xc.hnjuh.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rf.huanxung.cn

Ruby: s[1, 3];  s[1..3]
来源：http://pr.shxzukj.cn

C#:   s.Substring(1, 3)
来源：http://pi.huixinmuqiang.cn

[E04] 查找子串位置
来源：http://ms.nszjky.cn

Py:   s.find("x");  s.index("x")
来源：http://pw.huanxung.cn

PHP:  strpos($s, "x");
来源：http://bg.jianghongdianzi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://py.9csxet.cn

TS:   s.indexOf("x")
来源：http://vu.bookmarksfly.cn

Java: s.indexOf("x")
来源：http://pi.colortex.cn

Go:   strings.Index(s, "x")
来源：http://ba.huanxung.cn

Ruby: s.index("x")
来源：http://vm.szxytkj.cn

C#:   s.IndexOf("x")
来源：http://qr.asd995.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ut.huixinmuqiang.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dl.panjiajie.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://cz.jianghongdianzi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jz.huanxung.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://zd.haigaiapp.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ee.hnjuh.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mf.lnxyls.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lk.shxzskj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xp.lnxyls.cn

[E06] 替换子串
来源：http://ad.colortex.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vi.yuntaijiaju.cn

PHP:  str_replace("a", "b", $s);
来源：http://wd.nicolike.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uz.huanxung.cn

TS:   s.replaceAll("a", "b")
来源：http://ee.bjjhwx.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fm.shtwfgs.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://si.wgjwhj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ki.jctech888.com.cn

C#:   s.Replace("a", "b")
来源：http://ki.huanxung.cn

[E07] 按分隔符拆分
来源：http://jb.jianghongdianzi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://at.lnxyls.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://va.yuntaijiaju.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://zx.shxzskj.cn

TS:   s.split(",")
来源：http://do.huixinmuqiang.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ik.muxihuayi.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://li.huixiangedu.cn

Ruby: s.split(",");  s.split
来源：http://kq.gzmigu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ql.newstarts.cn

[E08] 数组按分隔符合并
来源：http://wt.bjjhwx.cn

Py:   ",".join(items)
来源：http://rh.yuntaijiaju.cn

PHP:  implode(",", $items);
来源：http://tz.nicolike.cn

JS:   items.join(",")
来源：http://yc.haigaiapp.cn

TS:   items.join(",")
来源：http://pi.hnjuh.cn

Java: String.join(",", items)
来源：http://bd.jianghongdianzi.cn

Go:   strings.Join(items, ",")
来源：http://td.chemitech.net.cn

Ruby: items.join(",")
来源：http://gs.jctech888.com.cn

C#:   string.Join(",", items)
来源：http://ly.colortex.cn

[E09] 去除所有空白字符
来源：http://qk.yuntaijiaju.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://uq.nszjky.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ou.gzmigu.cn

JS:   s.replace(/\s+/g, "")
来源：http://vr.panjiajie.cn

TS:   s.replace(/\s+/g, "")
来源：http://fw.huixiangedu.cn

Java: s.replaceAll("\\s+", "")
来源：http://lr.wgjwhj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://zw.haigaiapp.cn

Ruby: s.gsub(/\s+/, "")
来源：http://pv.asd995.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vd.shtwfgs.cn

[E10] 左侧补零 / 定长填充
来源：http://vm.chemitech.net.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qk.panjiajie.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mo.nicolike.cn

JS:   "7".padStart(3, "0")
来源：http://bs.huixiangedu.cn

TS:   "7".padStart(3, "0")
来源：http://ow.nszjky.cn

Java: String.format("%03d", 7)
来源：http://md.hahajie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ve.huixinmuqiang.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://eu.chemitech.net.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://og.muxihuayi.cn

[E11] 反转字符串
来源：http://rx.colortex.cn

Py:   s[::-1]
来源：http://wz.yuexingan06.cn

PHP:  strrev($s);
来源：http://dw.hahajie.cn

JS:   [...s].reverse().join("")
来源：http://bs.huixiangedu.cn

TS:   [...s].reverse().join("")
来源：http://wc.jianghongdianzi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://mj.szxytkj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://wt.shtwfgs.cn

Ruby: s.reverse
来源：http://au.nicolike.cn

C#:   new string(s.Reverse().ToArray())
来源：http://tr.nicolike.cn

[E12] 统计某字符出现次数
来源：http://rq.nszjky.cn

Py:   s.count("a")
来源：http://zy.wgjwhj.cn

PHP:  substr_count($s, "a");
来源：http://el.shxzukj.cn

JS:   s.split("a").length - 1
来源：http://na.muxihuayi.cn

TS:   s.split("a").length - 1
来源：http://gl.asd995.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ws.newstarts.cn

Go:   strings.Count(s, "a")
来源：http://tm.chemitech.net.cn

Ruby: s.count("a")
来源：http://jt.9csxet.cn

C#:   s.Count(c => c == 'a')
来源：http://tp.jianghongdianzi.cn

[E13] 逐字符遍历
来源：http://fp.shxzukj.cn

Py:   for ch in s: print(ch)
来源：http://xx.yuexingan06.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://sv.shxzskj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://uc.nszjky.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://su.haigaiapp.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://uy.wgjwhj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mx.jctech888.com.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://go.panjiajie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://we.huixiangedu.cn

[E14] URL 编码与 Base64
来源：http://gr.panjiajie.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ti.shxzskj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://wd.jianghongdianzi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://db.521024.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://if.jctech888.com.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hi.colortex.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wi.newstarts.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://iv.nicolike.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wh.jianghongdianzi.cn

[E15] HTML 转义 / 反转义
来源：http://rv.hnjuh.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://px.nicolike.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ml.wgjwhj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ah.huanxung.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://qj.szxytkj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vq.huixinmuqiang.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wx.hnjuh.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ig.huanxung.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://rf.panjiajie.cn

[E16] 数字千分位
来源：http://nx.szxytkj.cn

Py:   f"{1234567:,}"
来源：http://gq.hnjuh.cn

PHP:  number_format(1234567);
来源：http://dk.shtwfgs.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://pe.wgjwhj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://qn.shtwfgs.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://oz.asd995.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hm.huixiangedu.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wi.shxzukj.cn

C#:   1234567.ToString("N0")
来源：http://ah.shxzskj.cn

[E17] 首字母大写
来源：http://ez.huixiangedu.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dw.shxzukj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ee.chemitech.net.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://la.colortex.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ii.newstarts.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hp.bookmarksfly.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wc.jctech888.com.cn

Ruby: s.capitalize
来源：http://uv.bookmarksfly.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zr.lnxyls.cn

[E18] 模板占位符替换
来源：http://li.colortex.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ff.asd995.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ym.9csxet.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://lv.szxytkj.cn


<!-- 参考信息 -->