代发 wailian999

TS:   [...arr].reverse();
来源：http://fc.wgjwhj.cn

Java: Collections.reverse(list);
来源：http://hx.szsharing.cn

Go:   slices.Reverse(arr)
来源：http://yr.bookmarksfly.cn

Ruby: arr.reverse
来源：http://ie.nicolike.cn

C#:   list.Reverse();
来源：http://rl.shxzukj.cn

[D12] 查找元素下标
来源：http://np.colortex.cn

Py:   arr.index(x);  x in arr
来源：http://zs.yuntaijiaju.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gv.nicolike.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pv.shtwfgs.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mf.nicolike.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hk.chemitech.net.cn

Go:   slices.Index(arr, x)
来源：http://nz.huixinmuqiang.cn

Ruby: arr.index(x)
来源：http://yn.hahajie.cn

C#:   list.IndexOf(x);
来源：http://qr.newstarts.cn

[D13] 过滤（保留满足条件的）
来源：http://hr.gzmigu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://be.jianghongdianzi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://re.hnjuh.cn

JS:   arr.filter(x => x > 3)
来源：http://ij.hahajie.cn

TS:   arr.filter(x => x > 3)
来源：http://sp.shtwfgs.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://pb.gzmigu.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://iy.shxzskj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://sn.gzmigu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://wc.bjjhwx.cn

[D14] 映射转换（每个元素变形）
来源：http://it.muxihuayi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gm.panjiajie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qm.wgjwhj.cn

JS:   arr.map(x => x * 2)
来源：http://rr.bjjhwx.cn

TS:   arr.map(x => x * 2)
来源：http://lz.chemitech.net.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://br.lnxyls.cn

Go:   // 手写循环
来源：http://od.huixinmuqiang.cn

Ruby: arr.map { |x| x * 2 }
来源：http://lf.nszjky.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://cp.gzmigu.cn

[D15] 去重
来源：http://ti.panjiajie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://sa.nszjky.cn

PHP:  array_unique($arr);
来源：http://lb.hahajie.cn

JS:   [...new Set(arr)]
来源：http://dt.9csxet.cn

TS:   [...new Set(arr)]
来源：http://sm.hnjuh.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://li.shtwfgs.cn

Go:   // 用 map[T]struct{} 手写
来源：http://uk.shxzukj.cn

Ruby: arr.uniq
来源：http://yl.colortex.cn

C#:   list.Distinct().ToList()
来源：http://uy.yuntaijiaju.cn

[D16] 求和与平均值
来源：http://xz.hnjuh.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nt.9csxet.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mn.bookmarksfly.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://eo.jianghongdianzi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xu.jctech888.com.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://by.yuexingan06.cn

Go:   // 手写循环累加
来源：http://av.yuntaijiaju.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://te.521024.cn

C#:   list.Sum();  list.Average()
来源：http://eq.muxihuayi.cn

[D17] 最大值与最小值
来源：http://of.chemitech.net.cn

Py:   max(arr);  min(arr)
来源：http://gl.colortex.cn

PHP:  max($arr);  min($arr);
来源：http://lv.lnxyls.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ip.nszjky.cn

TS:   Math.max(...arr);
来源：http://kd.9csxet.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ca.szxytkj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vd.shxzukj.cn

Ruby: arr.max;  arr.min
来源：http://nk.shxzskj.cn

C#:   list.Max();  list.Min()
来源：http://dv.panjiajie.cn

[D18] 扁平化嵌套数组
来源：http://tx.panjiajie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zp.9csxet.cn

PHP:  array_merge(...$nested);
来源：http://od.bjjhwx.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ri.gzmigu.cn

TS:   nested.flat();
来源：http://gh.shxzukj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ye.bookmarksfly.cn

Go:   // 手写双层循环
来源：http://xa.huixiangedu.cn

Ruby: nested.flatten
来源：http://rd.szxytkj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://fj.panjiajie.cn

[D19] 按字段分组
来源：http://lj.colortex.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fg.newstarts.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ac.huanxung.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ds.asd995.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://uv.panjiajie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://or.9csxet.cn

Go:   // 手写 map[string][]T
来源：http://js.hahajie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ik.haigaiapp.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yt.yuexingan06.cn

[D20] 统计每个元素出现次数
来源：http://kr.newstarts.cn

Py:   Counter(arr)
来源：http://kf.jianghongdianzi.cn

PHP:  array_count_values($arr);
来源：http://ni.yuexingan06.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mb.nszjky.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pk.hnjuh.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ov.bookmarksfly.cn

Go:   // 手写 map[T]int
来源：http://id.wgjwhj.cn

Ruby: arr.tally
来源：http://dc.gzmigu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ud.huanxung.cn

[D21] 判断是否包含某元素
来源：http://qb.muxihuayi.cn

Py:   x in arr
来源：http://ru.hnjuh.cn

PHP:  in_array($x, $arr, true);
来源：http://xe.nicolike.cn

JS:   arr.includes(x)
来源：http://fx.hahajie.cn

TS:   arr.includes(x)
来源：http://ow.yuntaijiaju.cn

Java: list.contains(x)
来源：http://vi.panjiajie.cn

Go:   slices.Contains(arr, x)
来源：http://vr.wgjwhj.cn

Ruby: arr.include?(x)
来源：http://oi.yuexingan06.cn

C#:   list.Contains(x)
来源：http://bl.huanxung.cn

[D22] 复制数组（避免共享引用）
来源：http://lg.huixinmuqiang.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lt.bookmarksfly.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jd.wgjwhj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dw.9csxet.cn

TS:   [...arr];
来源：http://tu.gzmigu.cn

Java: new ArrayList<>(list);
来源：http://ll.hahajie.cn

Go:   copied := append([]int(nil), arr...)
来源：http://wc.colortex.cn

Ruby: arr.dup;  arr.clone
来源：http://cm.yuexingan06.cn

C#:   new List<int>(list);
来源：http://tv.jctech888.com.cn

[D23] reduce 累积计算
来源：http://sr.nszjky.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xw.jianghongdianzi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zo.huanxung.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ah.hnjuh.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://px.jianghongdianzi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://cv.szxytkj.cn

Go:   // 手写循环
来源：http://ss.gzmigu.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pm.huixinmuqiang.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ro.shxzukj.cn

[D24] 字典 / Map 基本操作
来源：http://fk.shxzskj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wu.521024.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jw.bookmarksfly.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://cx.asd995.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fx.gzmigu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ua.panjiajie.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xr.nicolike.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wy.yuexingan06.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hb.gzmigu.cn

[D25] Set 集合去重与交并差
来源：http://bh.colortex.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kt.bookmarksfly.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jz.panjiajie.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wg.gzmigu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://uv.lnxyls.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ki.panjiajie.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ti.muxihuayi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dm.shtwfgs.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nz.haigaiapp.cn

[D26] 数组转字符串
来源：http://ey.wgjwhj.cn

Py:   ", ".join(map(str, arr))
来源：http://hw.huanxung.cn

PHP:  implode(", ", $arr);
来源：http://pd.hnjuh.cn

JS:   arr.join(", ")
来源：http://ag.gzmigu.cn

TS:   arr.join(", ")
来源：http://pt.muxihuayi.cn

Java: String.join(", ", list)
来源：http://qv.jctech888.com.cn

Go:   strings.Join(strs, ", ")
来源：http://yk.chemitech.net.cn

Ruby: arr.join(", ")
来源：http://wn.yuexingan06.cn

C#:   string.Join(", ", list)
来源：http://mb.asd995.cn

================================================================================
来源：http://ib.nszjky.cn

E. 字符串处理
来源：http://su.shtwfgs.cn

================================================================================
来源：http://ib.yuntaijiaju.cn

[E01] 拼接字符串
来源：http://xa.shxzukj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://il.jianghongdianzi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ts.panjiajie.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ch.nicolike.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://eu.szxytkj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://cf.shtwfgs.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vm.chemitech.net.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://to.jctech888.com.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ry.bjjhwx.cn

[E02] 重复字符串
来源：http://bf.chemitech.net.cn

Py:   "ab" * 3
来源：http://mh.asd995.cn

PHP:  str_repeat("ab", 3);
来源：http://mj.jctech888.com.cn

JS:   "ab".repeat(3)
来源：http://bc.bjjhwx.cn

TS:   "ab".repeat(3)
来源：http://sr.521024.cn

Java: "ab".repeat(3)
来源：http://su.yuexingan06.cn

Go:   strings.Repeat("ab", 3)
来源：http://sf.yuexingan06.cn

Ruby: "ab" * 3
来源：http://yy.jctech888.com.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ar.szsharing.cn

[E03] 截取子串
来源：http://ei.shtwfgs.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xt.9csxet.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ey.wgjwhj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://pr.huanxung.cn

TS:   s.slice(1, 4)
来源：http://cm.yuexingan06.cn

Java: s.substring(1, 4)
来源：http://zv.newstarts.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://iq.yuntaijiaju.cn

Ruby: s[1, 3];  s[1..3]
来源：http://xm.jianghongdianzi.cn

C#:   s.Substring(1, 3)
来源：http://xf.asd995.cn

[E04] 查找子串位置
来源：http://ag.jianghongdianzi.cn

Py:   s.find("x");  s.index("x")
来源：http://yf.colortex.cn

PHP:  strpos($s, "x");
来源：http://bl.haigaiapp.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://co.asd995.cn

TS:   s.indexOf("x")
来源：http://lt.muxihuayi.cn

Java: s.indexOf("x")
来源：http://fm.hahajie.cn

Go:   strings.Index(s, "x")
来源：http://wa.shxzukj.cn

Ruby: s.index("x")
来源：http://ch.nszjky.cn

C#:   s.IndexOf("x")
来源：http://pe.bjjhwx.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://tx.jianghongdianzi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ln.szsharing.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zu.panjiajie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ja.bjjhwx.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://au.hahajie.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yx.nicolike.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xy.jctech888.com.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fk.haigaiapp.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nk.bjjhwx.cn

[E06] 替换子串
来源：http://av.huixinmuqiang.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fk.newstarts.cn

PHP:  str_replace("a", "b", $s);
来源：http://js.hnjuh.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ek.gzmigu.cn

TS:   s.replaceAll("a", "b")
来源：http://tf.jianghongdianzi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kp.jianghongdianzi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ra.wgjwhj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qn.szxytkj.cn

C#:   s.Replace("a", "b")
来源：http://iq.shtwfgs.cn

[E07] 按分隔符拆分
来源：http://fx.jctech888.com.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://dc.muxihuayi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://iu.wgjwhj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://bf.nicolike.cn

TS:   s.split(",")
来源：http://bm.yuntaijiaju.cn

Java: s.split(",");  s.split("\\s+")
来源：http://bv.lnxyls.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://cm.hahajie.cn

Ruby: s.split(",");  s.split
来源：http://le.shxzskj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jo.newstarts.cn

[E08] 数组按分隔符合并
来源：http://ti.9csxet.cn

Py:   ",".join(items)
来源：http://sq.521024.cn

PHP:  implode(",", $items);
来源：http://fx.bookmarksfly.cn

JS:   items.join(",")
来源：http://ns.shtwfgs.cn

TS:   items.join(",")
来源：http://ko.gzmigu.cn

Java: String.join(",", items)
来源：http://qa.gzmigu.cn

Go:   strings.Join(items, ",")
来源：http://tz.haigaiapp.cn

Ruby: items.join(",")
来源：http://jq.jctech888.com.cn

C#:   string.Join(",", items)
来源：http://qb.hnjuh.cn

[E09] 去除所有空白字符
来源：http://ul.huixinmuqiang.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rh.wgjwhj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vq.wgjwhj.cn

JS:   s.replace(/\s+/g, "")
来源：http://yn.newstarts.cn

TS:   s.replace(/\s+/g, "")
来源：http://fu.hahajie.cn

Java: s.replaceAll("\\s+", "")
来源：http://va.chemitech.net.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://eg.asd995.cn

Ruby: s.gsub(/\s+/, "")
来源：http://vk.lnxyls.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mx.huixinmuqiang.cn

[E10] 左侧补零 / 定长填充
来源：http://eo.haigaiapp.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://px.gzmigu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tq.jianghongdianzi.cn

JS:   "7".padStart(3, "0")
来源：http://re.jianghongdianzi.cn

TS:   "7".padStart(3, "0")
来源：http://av.hnjuh.cn

Java: String.format("%03d", 7)
来源：http://sl.yuexingan06.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://sq.szxytkj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://os.haigaiapp.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ub.hahajie.cn

[E11] 反转字符串
来源：http://cv.lnxyls.cn

Py:   s[::-1]
来源：http://jo.shtwfgs.cn

PHP:  strrev($s);
来源：http://wo.huanxung.cn

JS:   [...s].reverse().join("")
来源：http://br.colortex.cn

TS:   [...s].reverse().join("")
来源：http://gi.gzmigu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://sq.muxihuayi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ma.lnxyls.cn

Ruby: s.reverse
来源：http://qi.colortex.cn

C#:   new string(s.Reverse().ToArray())
来源：http://mj.yuexingan06.cn

[E12] 统计某字符出现次数
来源：http://zr.wgjwhj.cn

Py:   s.count("a")
来源：http://qv.hahajie.cn

PHP:  substr_count($s, "a");
来源：http://bv.gzmigu.cn

JS:   s.split("a").length - 1
来源：http://bb.asd995.cn

TS:   s.split("a").length - 1
来源：http://zf.yuexingan06.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://bg.colortex.cn

Go:   strings.Count(s, "a")
来源：http://tg.jianghongdianzi.cn

Ruby: s.count("a")
来源：http://lu.muxihuayi.cn

C#:   s.Count(c => c == 'a')
来源：http://bk.jctech888.com.cn

[E13] 逐字符遍历
来源：http://sk.shxzskj.cn

Py:   for ch in s: print(ch)
来源：http://ya.asd995.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ho.huanxung.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://sz.muxihuayi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ca.haigaiapp.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://cp.shtwfgs.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://au.yuntaijiaju.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://xy.yuexingan06.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zj.panjiajie.cn

[E14] URL 编码与 Base64
来源：http://in.muxihuayi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vb.bookmarksfly.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://xe.shxzukj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ta.shtwfgs.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xe.gzmigu.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://op.yuexingan06.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tf.gzmigu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://it.szxytkj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://oc.jctech888.com.cn

[E15] HTML 转义 / 反转义
来源：http://cm.shxzukj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ns.bookmarksfly.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qt.shtwfgs.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vp.yuexingan06.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ql.gzmigu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vb.shxzukj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fe.shtwfgs.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mh.haigaiapp.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ae.bookmarksfly.cn

[E16] 数字千分位
来源：http://kc.nszjky.cn

Py:   f"{1234567:,}"
来源：http://ks.colortex.cn

PHP:  number_format(1234567);
来源：http://ep.szsharing.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://jp.huixinmuqiang.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://zd.huixiangedu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rc.yuexingan06.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lx.lnxyls.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://je.panjiajie.cn

C#:   1234567.ToString("N0")
来源：http://bg.jianghongdianzi.cn

[E17] 首字母大写
来源：http://hm.asd995.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gn.colortex.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://tx.chemitech.net.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rf.521024.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zr.huixinmuqiang.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ro.haigaiapp.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://sb.jianghongdianzi.cn

Ruby: s.capitalize
来源：http://uv.9csxet.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jd.9csxet.cn

[E18] 模板占位符替换
来源：http://sz.newstarts.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://pz.yuntaijiaju.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://cs.newstarts.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://hi.jctech888.com.cn


<!-- 参考信息 -->