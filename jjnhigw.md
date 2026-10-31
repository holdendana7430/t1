代发 wailian999

TS:   [...arr].reverse();
来源：http://ml.haigaiapp.cn

Java: Collections.reverse(list);
来源：http://jd.shxzskj.cn

Go:   slices.Reverse(arr)
来源：http://me.shxzskj.cn

Ruby: arr.reverse
来源：http://oj.bookmarksfly.cn

C#:   list.Reverse();
来源：http://nc.chemitech.net.cn

[D12] 查找元素下标
来源：http://bd.asd995.cn

Py:   arr.index(x);  x in arr
来源：http://od.huixiangedu.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lb.colortex.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kp.shxzukj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ps.jctech888.com.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vu.colortex.cn

Go:   slices.Index(arr, x)
来源：http://dz.bjjhwx.cn

Ruby: arr.index(x)
来源：http://hp.bookmarksfly.cn

C#:   list.IndexOf(x);
来源：http://hm.wgjwhj.cn

[D13] 过滤（保留满足条件的）
来源：http://we.hahajie.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ll.bjjhwx.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://lk.szsharing.cn

JS:   arr.filter(x => x > 3)
来源：http://fv.chemitech.net.cn

TS:   arr.filter(x => x > 3)
来源：http://ye.nicolike.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://yl.colortex.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tc.huanxung.cn

Ruby: arr.select { |x| x > 3 }
来源：http://sx.nszjky.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ww.gzmigu.cn

[D14] 映射转换（每个元素变形）
来源：http://wg.shtwfgs.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hi.newstarts.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://to.yuntaijiaju.cn

JS:   arr.map(x => x * 2)
来源：http://da.haigaiapp.cn

TS:   arr.map(x => x * 2)
来源：http://le.9csxet.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://uc.wgjwhj.cn

Go:   // 手写循环
来源：http://jg.jctech888.com.cn

Ruby: arr.map { |x| x * 2 }
来源：http://uv.huixinmuqiang.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://wy.haigaiapp.cn

[D15] 去重
来源：http://gt.hahajie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fd.gzmigu.cn

PHP:  array_unique($arr);
来源：http://go.9csxet.cn

JS:   [...new Set(arr)]
来源：http://ua.yuntaijiaju.cn

TS:   [...new Set(arr)]
来源：http://lh.lnxyls.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ze.szxytkj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://xv.9csxet.cn

Ruby: arr.uniq
来源：http://mv.colortex.cn

C#:   list.Distinct().ToList()
来源：http://iy.szsharing.cn

[D16] 求和与平均值
来源：http://uy.hahajie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ge.panjiajie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://uy.muxihuayi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://kp.lnxyls.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dx.yuntaijiaju.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ji.szxytkj.cn

Go:   // 手写循环累加
来源：http://cl.chemitech.net.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://sb.nszjky.cn

C#:   list.Sum();  list.Average()
来源：http://fm.yuexingan06.cn

[D17] 最大值与最小值
来源：http://qx.muxihuayi.cn

Py:   max(arr);  min(arr)
来源：http://te.hahajie.cn

PHP:  max($arr);  min($arr);
来源：http://fo.huixiangedu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fp.colortex.cn

TS:   Math.max(...arr);
来源：http://zf.shtwfgs.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://rl.bjjhwx.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://oa.szsharing.cn

Ruby: arr.max;  arr.min
来源：http://rd.shxzskj.cn

C#:   list.Max();  list.Min()
来源：http://ky.bjjhwx.cn

[D18] 扁平化嵌套数组
来源：http://vi.wgjwhj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://it.huixinmuqiang.cn

PHP:  array_merge(...$nested);
来源：http://xf.nszjky.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mk.521024.cn

TS:   nested.flat();
来源：http://yl.chemitech.net.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fe.wgjwhj.cn

Go:   // 手写双层循环
来源：http://nn.panjiajie.cn

Ruby: nested.flatten
来源：http://fo.asd995.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://io.shtwfgs.cn

[D19] 按字段分组
来源：http://xb.lnxyls.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://je.yuexingan06.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ux.newstarts.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fh.nicolike.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://vt.jianghongdianzi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jv.colortex.cn

Go:   // 手写 map[string][]T
来源：http://mw.nszjky.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://nw.huanxung.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://su.szsharing.cn

[D20] 统计每个元素出现次数
来源：http://mv.gzmigu.cn

Py:   Counter(arr)
来源：http://vf.shtwfgs.cn

PHP:  array_count_values($arr);
来源：http://cx.521024.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cm.yuntaijiaju.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ys.muxihuayi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bd.bjjhwx.cn

Go:   // 手写 map[T]int
来源：http://jw.szxytkj.cn

Ruby: arr.tally
来源：http://ee.shxzskj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vj.gzmigu.cn

[D21] 判断是否包含某元素
来源：http://em.newstarts.cn

Py:   x in arr
来源：http://cl.bjjhwx.cn

PHP:  in_array($x, $arr, true);
来源：http://lk.wgjwhj.cn

JS:   arr.includes(x)
来源：http://tb.muxihuayi.cn

TS:   arr.includes(x)
来源：http://hw.colortex.cn

Java: list.contains(x)
来源：http://kt.lnxyls.cn

Go:   slices.Contains(arr, x)
来源：http://mg.shtwfgs.cn

Ruby: arr.include?(x)
来源：http://vh.newstarts.cn

C#:   list.Contains(x)
来源：http://ly.asd995.cn

[D22] 复制数组（避免共享引用）
来源：http://jw.shxzskj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pc.521024.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wy.yuexingan06.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zw.colortex.cn

TS:   [...arr];
来源：http://nc.hnjuh.cn

Java: new ArrayList<>(list);
来源：http://zg.yuexingan06.cn

Go:   copied := append([]int(nil), arr...)
来源：http://wq.hahajie.cn

Ruby: arr.dup;  arr.clone
来源：http://sq.bjjhwx.cn

C#:   new List<int>(list);
来源：http://ms.muxihuayi.cn

[D23] reduce 累积计算
来源：http://nj.gzmigu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yp.bookmarksfly.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://lg.bookmarksfly.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qr.panjiajie.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ig.shxzskj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://cr.nszjky.cn

Go:   // 手写循环
来源：http://nw.gzmigu.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hk.nszjky.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://am.newstarts.cn

[D24] 字典 / Map 基本操作
来源：http://os.jianghongdianzi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ob.jianghongdianzi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://yp.szsharing.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ru.gzmigu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nq.bjjhwx.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://aw.bookmarksfly.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zw.bookmarksfly.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ex.colortex.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dw.huixinmuqiang.cn

[D25] Set 集合去重与交并差
来源：http://bm.colortex.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://cd.gzmigu.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ii.jianghongdianzi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://aw.yuexingan06.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://tk.shtwfgs.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ib.yuexingan06.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ax.yuntaijiaju.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://sh.muxihuayi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://kj.hnjuh.cn

[D26] 数组转字符串
来源：http://sn.shxzskj.cn

Py:   ", ".join(map(str, arr))
来源：http://hj.shxzukj.cn

PHP:  implode(", ", $arr);
来源：http://qk.shxzukj.cn

JS:   arr.join(", ")
来源：http://sf.asd995.cn

TS:   arr.join(", ")
来源：http://cn.asd995.cn

Java: String.join(", ", list)
来源：http://il.wgjwhj.cn

Go:   strings.Join(strs, ", ")
来源：http://sa.huixiangedu.cn

Ruby: arr.join(", ")
来源：http://yl.hnjuh.cn

C#:   string.Join(", ", list)
来源：http://zx.szxytkj.cn

================================================================================
来源：http://yg.jianghongdianzi.cn

E. 字符串处理
来源：http://mf.shtwfgs.cn

================================================================================
来源：http://zv.shxzskj.cn

[E01] 拼接字符串
来源：http://xs.yuntaijiaju.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ks.nicolike.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ds.huixiangedu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vq.nszjky.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fs.jctech888.com.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ai.huixinmuqiang.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rv.szxytkj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xw.shxzukj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://by.shxzukj.cn

[E02] 重复字符串
来源：http://tw.jianghongdianzi.cn

Py:   "ab" * 3
来源：http://kd.yuntaijiaju.cn

PHP:  str_repeat("ab", 3);
来源：http://xi.huanxung.cn

JS:   "ab".repeat(3)
来源：http://nn.huixinmuqiang.cn

TS:   "ab".repeat(3)
来源：http://ts.newstarts.cn

Java: "ab".repeat(3)
来源：http://qw.huixiangedu.cn

Go:   strings.Repeat("ab", 3)
来源：http://tt.lnxyls.cn

Ruby: "ab" * 3
来源：http://pf.nicolike.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ep.newstarts.cn

[E03] 截取子串
来源：http://fr.newstarts.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qq.jctech888.com.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://rn.huanxung.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://tt.lnxyls.cn

TS:   s.slice(1, 4)
来源：http://hv.szsharing.cn

Java: s.substring(1, 4)
来源：http://wv.521024.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qb.szxytkj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://wx.szxytkj.cn

C#:   s.Substring(1, 3)
来源：http://ok.nicolike.cn

[E04] 查找子串位置
来源：http://rx.9csxet.cn

Py:   s.find("x");  s.index("x")
来源：http://ws.jctech888.com.cn

PHP:  strpos($s, "x");
来源：http://hh.jctech888.com.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://sx.huixinmuqiang.cn

TS:   s.indexOf("x")
来源：http://fi.9csxet.cn

Java: s.indexOf("x")
来源：http://gq.huixinmuqiang.cn

Go:   strings.Index(s, "x")
来源：http://wu.chemitech.net.cn

Ruby: s.index("x")
来源：http://zl.jianghongdianzi.cn

C#:   s.IndexOf("x")
来源：http://rk.shxzukj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://mn.panjiajie.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xj.jianghongdianzi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ua.bjjhwx.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ku.huanxung.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://jl.jctech888.com.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bv.muxihuayi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gw.wgjwhj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://yb.huixinmuqiang.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://no.haigaiapp.cn

[E06] 替换子串
来源：http://zw.gzmigu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wj.521024.cn

PHP:  str_replace("a", "b", $s);
来源：http://ye.haigaiapp.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mf.bookmarksfly.cn

TS:   s.replaceAll("a", "b")
来源：http://xn.nicolike.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kp.bjjhwx.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wv.shxzukj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://gd.huanxung.cn

C#:   s.Replace("a", "b")
来源：http://hh.huixinmuqiang.cn

[E07] 按分隔符拆分
来源：http://fl.hahajie.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ad.nszjky.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://sr.shxzskj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://bj.newstarts.cn

TS:   s.split(",")
来源：http://nj.huixiangedu.cn

Java: s.split(",");  s.split("\\s+")
来源：http://po.asd995.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fz.asd995.cn

Ruby: s.split(",");  s.split
来源：http://hr.nicolike.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ie.bookmarksfly.cn

[E08] 数组按分隔符合并
来源：http://hp.nicolike.cn

Py:   ",".join(items)
来源：http://yv.lnxyls.cn

PHP:  implode(",", $items);
来源：http://td.shxzskj.cn

JS:   items.join(",")
来源：http://fo.shxzskj.cn

TS:   items.join(",")
来源：http://nj.9csxet.cn

Java: String.join(",", items)
来源：http://pa.shxzukj.cn

Go:   strings.Join(items, ",")
来源：http://ld.yuntaijiaju.cn

Ruby: items.join(",")
来源：http://os.shxzukj.cn

C#:   string.Join(",", items)
来源：http://zw.hnjuh.cn

[E09] 去除所有空白字符
来源：http://sq.yuexingan06.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vn.nicolike.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qm.haigaiapp.cn

JS:   s.replace(/\s+/g, "")
来源：http://km.yuntaijiaju.cn

TS:   s.replace(/\s+/g, "")
来源：http://gq.szsharing.cn

Java: s.replaceAll("\\s+", "")
来源：http://mh.panjiajie.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://bo.jctech888.com.cn

Ruby: s.gsub(/\s+/, "")
来源：http://fx.asd995.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cb.colortex.cn

[E10] 左侧补零 / 定长填充
来源：http://qx.gzmigu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ei.huixinmuqiang.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fb.hahajie.cn

JS:   "7".padStart(3, "0")
来源：http://mp.colortex.cn

TS:   "7".padStart(3, "0")
来源：http://zr.huanxung.cn

Java: String.format("%03d", 7)
来源：http://aw.9csxet.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://va.huixinmuqiang.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mk.newstarts.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ng.shtwfgs.cn

[E11] 反转字符串
来源：http://sw.haigaiapp.cn

Py:   s[::-1]
来源：http://jz.szxytkj.cn

PHP:  strrev($s);
来源：http://pj.bookmarksfly.cn

JS:   [...s].reverse().join("")
来源：http://ys.haigaiapp.cn

TS:   [...s].reverse().join("")
来源：http://ro.huanxung.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://un.huixiangedu.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://rs.nicolike.cn

Ruby: s.reverse
来源：http://wo.asd995.cn

C#:   new string(s.Reverse().ToArray())
来源：http://be.nicolike.cn

[E12] 统计某字符出现次数
来源：http://rb.shxzukj.cn

Py:   s.count("a")
来源：http://lh.asd995.cn

PHP:  substr_count($s, "a");
来源：http://it.haigaiapp.cn

JS:   s.split("a").length - 1
来源：http://mf.muxihuayi.cn

TS:   s.split("a").length - 1
来源：http://ta.panjiajie.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kv.yuntaijiaju.cn

Go:   strings.Count(s, "a")
来源：http://ui.chemitech.net.cn

Ruby: s.count("a")
来源：http://am.nicolike.cn

C#:   s.Count(c => c == 'a')
来源：http://tl.szxytkj.cn

[E13] 逐字符遍历
来源：http://wg.newstarts.cn

Py:   for ch in s: print(ch)
来源：http://mb.gzmigu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ni.szsharing.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://yo.panjiajie.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://wk.shxzskj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://cc.newstarts.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://lq.shtwfgs.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://cp.szxytkj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://he.jianghongdianzi.cn

[E14] URL 编码与 Base64
来源：http://tb.bjjhwx.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rz.jianghongdianzi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ob.shtwfgs.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://nr.wgjwhj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qj.9csxet.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kz.shxzukj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wt.huixinmuqiang.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://is.shtwfgs.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://yq.jctech888.com.cn

[E15] HTML 转义 / 反转义
来源：http://gu.bjjhwx.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://um.shtwfgs.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fc.asd995.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ni.szsharing.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://kf.asd995.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://sr.huixiangedu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bb.szxytkj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xe.shxzskj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bk.shxzskj.cn

[E16] 数字千分位
来源：http://fj.hnjuh.cn

Py:   f"{1234567:,}"
来源：http://bz.haigaiapp.cn

PHP:  number_format(1234567);
来源：http://ip.bjjhwx.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://gq.9csxet.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://rw.szxytkj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qf.shxzskj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ts.521024.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hj.szxytkj.cn

C#:   1234567.ToString("N0")
来源：http://oz.521024.cn

[E17] 首字母大写
来源：http://qu.panjiajie.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://os.huixiangedu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://jp.newstarts.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nv.chemitech.net.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sb.nszjky.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://uc.shxzukj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wq.szxytkj.cn

Ruby: s.capitalize
来源：http://wv.wgjwhj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ed.hnjuh.cn

[E18] 模板占位符替换
来源：http://vx.lnxyls.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qg.szxytkj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mu.muxihuayi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://vt.chemitech.net.cn


<!-- 参考信息 -->