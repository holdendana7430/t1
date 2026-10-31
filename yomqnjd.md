代发 wailian999

C#:   list.Reverse();
来源：http://kq.haigaiapp.cn

[D12] 查找元素下标
来源：http://oz.yuntaijiaju.cn

Py:   arr.index(x);  x in arr
来源：http://zh.colortex.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://uq.panjiajie.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jy.gzmigu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nf.shxzukj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ia.szsharing.cn

Go:   slices.Index(arr, x)
来源：http://ex.szsharing.cn

Ruby: arr.index(x)
来源：http://fo.lnxyls.cn

C#:   list.IndexOf(x);
来源：http://vk.nicolike.cn

[D13] 过滤（保留满足条件的）
来源：http://rc.asd995.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://go.szsharing.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ds.jctech888.com.cn

JS:   arr.filter(x => x > 3)
来源：http://vu.gzmigu.cn

TS:   arr.filter(x => x > 3)
来源：http://uz.haigaiapp.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://nm.bookmarksfly.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://us.hnjuh.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ge.nszjky.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://tv.muxihuayi.cn

[D14] 映射转换（每个元素变形）
来源：http://pj.nszjky.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ng.chemitech.net.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ln.jianghongdianzi.cn

JS:   arr.map(x => x * 2)
来源：http://yq.gzmigu.cn

TS:   arr.map(x => x * 2)
来源：http://mr.nszjky.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ot.shtwfgs.cn

Go:   // 手写循环
来源：http://eu.shxzskj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://nv.chemitech.net.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://oe.gzmigu.cn

[D15] 去重
来源：http://nu.yuntaijiaju.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nh.gzmigu.cn

PHP:  array_unique($arr);
来源：http://eb.szxytkj.cn

JS:   [...new Set(arr)]
来源：http://br.shxzskj.cn

TS:   [...new Set(arr)]
来源：http://yb.yuntaijiaju.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rj.bookmarksfly.cn

Go:   // 用 map[T]struct{} 手写
来源：http://xu.chemitech.net.cn

Ruby: arr.uniq
来源：http://eq.asd995.cn

C#:   list.Distinct().ToList()
来源：http://od.chemitech.net.cn

[D16] 求和与平均值
来源：http://pr.yuexingan06.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nj.szsharing.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xe.yuntaijiaju.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hh.yuexingan06.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://oo.shtwfgs.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hk.jianghongdianzi.cn

Go:   // 手写循环累加
来源：http://es.nszjky.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hx.asd995.cn

C#:   list.Sum();  list.Average()
来源：http://qo.nicolike.cn

[D17] 最大值与最小值
来源：http://bp.gzmigu.cn

Py:   max(arr);  min(arr)
来源：http://fs.bookmarksfly.cn

PHP:  max($arr);  min($arr);
来源：http://pb.9csxet.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://cz.521024.cn

TS:   Math.max(...arr);
来源：http://ci.huanxung.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://iw.gzmigu.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qj.bjjhwx.cn

Ruby: arr.max;  arr.min
来源：http://dt.bjjhwx.cn

C#:   list.Max();  list.Min()
来源：http://fe.nszjky.cn

[D18] 扁平化嵌套数组
来源：http://gz.hnjuh.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fh.muxihuayi.cn

PHP:  array_merge(...$nested);
来源：http://sc.huanxung.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fj.asd995.cn

TS:   nested.flat();
来源：http://mm.hnjuh.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://sq.szxytkj.cn

Go:   // 手写双层循环
来源：http://sx.nszjky.cn

Ruby: nested.flatten
来源：http://fv.jctech888.com.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://lt.yuntaijiaju.cn

[D19] 按字段分组
来源：http://dm.wgjwhj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://cv.huanxung.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ow.nicolike.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ml.panjiajie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://cy.lnxyls.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ll.nicolike.cn

Go:   // 手写 map[string][]T
来源：http://mt.asd995.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://mv.chemitech.net.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vy.muxihuayi.cn

[D20] 统计每个元素出现次数
来源：http://of.newstarts.cn

Py:   Counter(arr)
来源：http://vg.huixiangedu.cn

PHP:  array_count_values($arr);
来源：http://hw.szxytkj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vo.newstarts.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fb.hnjuh.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://py.lnxyls.cn

Go:   // 手写 map[T]int
来源：http://ug.9csxet.cn

Ruby: arr.tally
来源：http://ok.jctech888.com.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://yn.hahajie.cn

[D21] 判断是否包含某元素
来源：http://ql.9csxet.cn

Py:   x in arr
来源：http://xq.yuexingan06.cn

PHP:  in_array($x, $arr, true);
来源：http://wu.shtwfgs.cn

JS:   arr.includes(x)
来源：http://ma.yuntaijiaju.cn

TS:   arr.includes(x)
来源：http://xc.newstarts.cn

Java: list.contains(x)
来源：http://cu.lnxyls.cn

Go:   slices.Contains(arr, x)
来源：http://dp.huanxung.cn

Ruby: arr.include?(x)
来源：http://dq.yuexingan06.cn

C#:   list.Contains(x)
来源：http://vn.hahajie.cn

[D22] 复制数组（避免共享引用）
来源：http://ew.hahajie.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ot.hnjuh.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://co.panjiajie.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://yp.jctech888.com.cn

TS:   [...arr];
来源：http://xx.hahajie.cn

Java: new ArrayList<>(list);
来源：http://xd.huanxung.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ob.yuntaijiaju.cn

Ruby: arr.dup;  arr.clone
来源：http://le.asd995.cn

C#:   new List<int>(list);
来源：http://zt.jianghongdianzi.cn

[D23] reduce 累积计算
来源：http://nd.gzmigu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xi.haigaiapp.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://sl.hahajie.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ol.panjiajie.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zh.shxzskj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://iz.yuntaijiaju.cn

Go:   // 手写循环
来源：http://vc.shxzukj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://uo.newstarts.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zu.hnjuh.cn

[D24] 字典 / Map 基本操作
来源：http://jr.521024.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xi.yuexingan06.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vc.jctech888.com.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dh.bjjhwx.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dc.shtwfgs.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ao.newstarts.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://pw.jctech888.com.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nr.9csxet.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dp.nszjky.cn

[D25] Set 集合去重与交并差
来源：http://yr.shxzskj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mf.shxzskj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://yk.jctech888.com.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://sa.asd995.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ts.nicolike.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://il.huixinmuqiang.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tr.wgjwhj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://yf.nszjky.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dv.bookmarksfly.cn

[D26] 数组转字符串
来源：http://xy.bjjhwx.cn

Py:   ", ".join(map(str, arr))
来源：http://wd.9csxet.cn

PHP:  implode(", ", $arr);
来源：http://ut.yuntaijiaju.cn

JS:   arr.join(", ")
来源：http://bg.9csxet.cn

TS:   arr.join(", ")
来源：http://ov.gzmigu.cn

Java: String.join(", ", list)
来源：http://ka.bjjhwx.cn

Go:   strings.Join(strs, ", ")
来源：http://he.bjjhwx.cn

Ruby: arr.join(", ")
来源：http://pr.chemitech.net.cn

C#:   string.Join(", ", list)
来源：http://dv.nszjky.cn

================================================================================
来源：http://in.jctech888.com.cn

E. 字符串处理
来源：http://ra.nicolike.cn

================================================================================
来源：http://ey.yuexingan06.cn

[E01] 拼接字符串
来源：http://ll.bjjhwx.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lv.huanxung.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rv.yuntaijiaju.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qk.yuexingan06.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://po.huixiangedu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://or.panjiajie.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zm.asd995.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ss.szsharing.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fw.shxzukj.cn

[E02] 重复字符串
来源：http://oz.shxzukj.cn

Py:   "ab" * 3
来源：http://xf.lnxyls.cn

PHP:  str_repeat("ab", 3);
来源：http://ts.huanxung.cn

JS:   "ab".repeat(3)
来源：http://ks.hnjuh.cn

TS:   "ab".repeat(3)
来源：http://jz.colortex.cn

Java: "ab".repeat(3)
来源：http://pl.bjjhwx.cn

Go:   strings.Repeat("ab", 3)
来源：http://ce.nszjky.cn

Ruby: "ab" * 3
来源：http://wl.lnxyls.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ba.huixiangedu.cn

[E03] 截取子串
来源：http://ih.jianghongdianzi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://fk.newstarts.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fg.bookmarksfly.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qk.szxytkj.cn

TS:   s.slice(1, 4)
来源：http://yu.jctech888.com.cn

Java: s.substring(1, 4)
来源：http://hz.szsharing.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://an.bookmarksfly.cn

Ruby: s[1, 3];  s[1..3]
来源：http://fk.huanxung.cn

C#:   s.Substring(1, 3)
来源：http://pd.shxzukj.cn

[E04] 查找子串位置
来源：http://ga.huixinmuqiang.cn

Py:   s.find("x");  s.index("x")
来源：http://cj.panjiajie.cn

PHP:  strpos($s, "x");
来源：http://zw.haigaiapp.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qe.shtwfgs.cn

TS:   s.indexOf("x")
来源：http://ah.panjiajie.cn

Java: s.indexOf("x")
来源：http://og.lnxyls.cn

Go:   strings.Index(s, "x")
来源：http://hi.gzmigu.cn

Ruby: s.index("x")
来源：http://yr.asd995.cn

C#:   s.IndexOf("x")
来源：http://hp.521024.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://gi.nicolike.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://we.huixiangedu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://br.nicolike.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vo.bjjhwx.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://yy.huanxung.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sn.shxzukj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://yw.shtwfgs.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://sh.jianghongdianzi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mi.panjiajie.cn

[E06] 替换子串
来源：http://jm.colortex.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xn.gzmigu.cn

PHP:  str_replace("a", "b", $s);
来源：http://lg.huixinmuqiang.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uk.yuntaijiaju.cn

TS:   s.replaceAll("a", "b")
来源：http://sj.gzmigu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://iv.haigaiapp.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gg.huixiangedu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vr.wgjwhj.cn

C#:   s.Replace("a", "b")
来源：http://gl.gzmigu.cn

[E07] 按分隔符拆分
来源：http://uv.panjiajie.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fz.newstarts.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fh.haigaiapp.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ze.9csxet.cn

TS:   s.split(",")
来源：http://va.haigaiapp.cn

Java: s.split(",");  s.split("\\s+")
来源：http://xz.hnjuh.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://uu.huanxung.cn

Ruby: s.split(",");  s.split
来源：http://wl.newstarts.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rj.bookmarksfly.cn

[E08] 数组按分隔符合并
来源：http://yw.shtwfgs.cn

Py:   ",".join(items)
来源：http://mk.gzmigu.cn

PHP:  implode(",", $items);
来源：http://er.haigaiapp.cn

JS:   items.join(",")
来源：http://ht.jctech888.com.cn

TS:   items.join(",")
来源：http://pu.bjjhwx.cn

Java: String.join(",", items)
来源：http://td.huanxung.cn

Go:   strings.Join(items, ",")
来源：http://tr.haigaiapp.cn

Ruby: items.join(",")
来源：http://xo.bjjhwx.cn

C#:   string.Join(",", items)
来源：http://kx.colortex.cn

[E09] 去除所有空白字符
来源：http://yw.colortex.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ob.9csxet.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://us.muxihuayi.cn

JS:   s.replace(/\s+/g, "")
来源：http://lc.gzmigu.cn

TS:   s.replace(/\s+/g, "")
来源：http://lx.shxzukj.cn

Java: s.replaceAll("\\s+", "")
来源：http://qh.yuexingan06.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://tz.jctech888.com.cn

Ruby: s.gsub(/\s+/, "")
来源：http://rh.shxzukj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qp.bookmarksfly.cn

[E10] 左侧补零 / 定长填充
来源：http://rx.colortex.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ok.jctech888.com.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://sz.huanxung.cn

JS:   "7".padStart(3, "0")
来源：http://fi.huixiangedu.cn

TS:   "7".padStart(3, "0")
来源：http://et.asd995.cn

Java: String.format("%03d", 7)
来源：http://mg.lnxyls.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://rs.gzmigu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ll.huanxung.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xa.521024.cn

[E11] 反转字符串
来源：http://iw.muxihuayi.cn

Py:   s[::-1]
来源：http://cs.shxzskj.cn

PHP:  strrev($s);
来源：http://jh.panjiajie.cn

JS:   [...s].reverse().join("")
来源：http://gv.bjjhwx.cn

TS:   [...s].reverse().join("")
来源：http://jm.wgjwhj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://nu.521024.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ww.jianghongdianzi.cn

Ruby: s.reverse
来源：http://yk.nicolike.cn

C#:   new string(s.Reverse().ToArray())
来源：http://aa.asd995.cn

[E12] 统计某字符出现次数
来源：http://iz.szxytkj.cn

Py:   s.count("a")
来源：http://cu.shtwfgs.cn

PHP:  substr_count($s, "a");
来源：http://xl.muxihuayi.cn

JS:   s.split("a").length - 1
来源：http://vm.bjjhwx.cn

TS:   s.split("a").length - 1
来源：http://xn.9csxet.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://eq.yuexingan06.cn

Go:   strings.Count(s, "a")
来源：http://qp.nicolike.cn

Ruby: s.count("a")
来源：http://pz.newstarts.cn

C#:   s.Count(c => c == 'a')
来源：http://no.muxihuayi.cn

[E13] 逐字符遍历
来源：http://th.jctech888.com.cn

Py:   for ch in s: print(ch)
来源：http://vu.huanxung.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wz.asd995.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://mk.hahajie.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://bs.nicolike.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wn.yuexingan06.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://is.szxytkj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://un.nszjky.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://yc.bjjhwx.cn

[E14] URL 编码与 Base64
来源：http://ss.nicolike.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fr.hahajie.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://rn.wgjwhj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://uz.panjiajie.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zw.shxzskj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://yt.gzmigu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mv.wgjwhj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://pe.bjjhwx.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://il.bjjhwx.cn

[E15] HTML 转义 / 反转义
来源：http://ak.jctech888.com.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://bw.shxzukj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://yd.szxytkj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cd.hnjuh.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://cx.nszjky.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://me.yuntaijiaju.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://aw.haigaiapp.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://uv.haigaiapp.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ga.hahajie.cn

[E16] 数字千分位
来源：http://ws.shtwfgs.cn

Py:   f"{1234567:,}"
来源：http://fy.newstarts.cn

PHP:  number_format(1234567);
来源：http://ig.jctech888.com.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://le.szxytkj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://kk.bookmarksfly.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://pc.szxytkj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://uo.521024.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://yw.asd995.cn

C#:   1234567.ToString("N0")
来源：http://nz.nszjky.cn

[E17] 首字母大写
来源：http://ul.hahajie.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://lw.hahajie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://pp.shxzskj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://as.huanxung.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jy.hahajie.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rn.colortex.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qc.shxzukj.cn

Ruby: s.capitalize
来源：http://lr.asd995.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ng.9csxet.cn

[E18] 模板占位符替换
来源：http://ne.nszjky.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gp.lnxyls.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fb.panjiajie.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://pi.shtwfgs.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://vf.chemitech.net.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lo.panjiajie.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gp.muxihuayi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://lz.haigaiapp.cn


<!-- 参考信息 -->