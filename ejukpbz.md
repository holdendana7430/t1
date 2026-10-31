代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ge.yuntaijiaju.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kx.newstarts.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ll.yuntaijiaju.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hc.shtwfgs.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://lu.panjiajie.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mc.huixinmuqiang.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://nu.colortex.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tg.huanxung.cn

[D11] 反转数组
来源：http://oo.muxihuayi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://lq.hahajie.cn

PHP:  array_reverse($arr);
来源：http://oz.huanxung.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://js.nszjky.cn

TS:   [...arr].reverse();
来源：http://fh.nszjky.cn

Java: Collections.reverse(list);
来源：http://ou.yuntaijiaju.cn

Go:   slices.Reverse(arr)
来源：http://ao.bookmarksfly.cn

Ruby: arr.reverse
来源：http://hg.szxytkj.cn

C#:   list.Reverse();
来源：http://mh.gzmigu.cn

[D12] 查找元素下标
来源：http://ku.colortex.cn

Py:   arr.index(x);  x in arr
来源：http://rm.shxzukj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://uv.9csxet.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://iq.shxzukj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yq.hahajie.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xv.shxzskj.cn

Go:   slices.Index(arr, x)
来源：http://ut.bjjhwx.cn

Ruby: arr.index(x)
来源：http://pb.521024.cn

C#:   list.IndexOf(x);
来源：http://vn.shtwfgs.cn

[D13] 过滤（保留满足条件的）
来源：http://hb.gzmigu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ma.gzmigu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ay.asd995.cn

JS:   arr.filter(x => x > 3)
来源：http://cc.szsharing.cn

TS:   arr.filter(x => x > 3)
来源：http://cv.asd995.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://us.yuexingan06.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qf.muxihuayi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ci.hahajie.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://wk.yuntaijiaju.cn

[D14] 映射转换（每个元素变形）
来源：http://xx.chemitech.net.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hu.9csxet.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://bs.haigaiapp.cn

JS:   arr.map(x => x * 2)
来源：http://rr.huanxung.cn

TS:   arr.map(x => x * 2)
来源：http://fr.yuntaijiaju.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://og.huixiangedu.cn

Go:   // 手写循环
来源：http://ak.hnjuh.cn

Ruby: arr.map { |x| x * 2 }
来源：http://lz.gzmigu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://qc.bjjhwx.cn

[D15] 去重
来源：http://db.jctech888.com.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bf.muxihuayi.cn

PHP:  array_unique($arr);
来源：http://it.hnjuh.cn

JS:   [...new Set(arr)]
来源：http://th.huixinmuqiang.cn

TS:   [...new Set(arr)]
来源：http://ub.szsharing.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cy.gzmigu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://kf.nszjky.cn

Ruby: arr.uniq
来源：http://nw.newstarts.cn

C#:   list.Distinct().ToList()
来源：http://qn.wgjwhj.cn

[D16] 求和与平均值
来源：http://hp.newstarts.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wq.jianghongdianzi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ta.shxzskj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ma.gzmigu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xw.yuexingan06.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://of.chemitech.net.cn

Go:   // 手写循环累加
来源：http://vq.gzmigu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fw.521024.cn

C#:   list.Sum();  list.Average()
来源：http://po.huixiangedu.cn

[D17] 最大值与最小值
来源：http://sc.huixiangedu.cn

Py:   max(arr);  min(arr)
来源：http://bu.shxzukj.cn

PHP:  max($arr);  min($arr);
来源：http://xr.muxihuayi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qx.nicolike.cn

TS:   Math.max(...arr);
来源：http://iq.huanxung.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://sd.newstarts.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://kr.shxzukj.cn

Ruby: arr.max;  arr.min
来源：http://zc.huanxung.cn

C#:   list.Max();  list.Min()
来源：http://jd.jctech888.com.cn

[D18] 扁平化嵌套数组
来源：http://db.asd995.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://yo.lnxyls.cn

PHP:  array_merge(...$nested);
来源：http://vd.hnjuh.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qy.wgjwhj.cn

TS:   nested.flat();
来源：http://uw.bjjhwx.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fx.muxihuayi.cn

Go:   // 手写双层循环
来源：http://mj.shtwfgs.cn

Ruby: nested.flatten
来源：http://qk.9csxet.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://li.wgjwhj.cn

[D19] 按字段分组
来源：http://hb.shtwfgs.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gp.muxihuayi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://rr.szxytkj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://di.newstarts.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ca.szxytkj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rw.wgjwhj.cn

Go:   // 手写 map[string][]T
来源：http://tr.lnxyls.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://yb.jctech888.com.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lk.szxytkj.cn

[D20] 统计每个元素出现次数
来源：http://zv.hnjuh.cn

Py:   Counter(arr)
来源：http://yt.muxihuayi.cn

PHP:  array_count_values($arr);
来源：http://pr.lnxyls.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jl.szxytkj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lz.yuntaijiaju.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://sf.huanxung.cn

Go:   // 手写 map[T]int
来源：http://tx.nicolike.cn

Ruby: arr.tally
来源：http://rm.nszjky.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cj.newstarts.cn

[D21] 判断是否包含某元素
来源：http://bv.bookmarksfly.cn

Py:   x in arr
来源：http://rb.shtwfgs.cn

PHP:  in_array($x, $arr, true);
来源：http://gl.newstarts.cn

JS:   arr.includes(x)
来源：http://dq.jctech888.com.cn

TS:   arr.includes(x)
来源：http://om.asd995.cn

Java: list.contains(x)
来源：http://pi.haigaiapp.cn

Go:   slices.Contains(arr, x)
来源：http://nc.bjjhwx.cn

Ruby: arr.include?(x)
来源：http://ru.hnjuh.cn

C#:   list.Contains(x)
来源：http://cx.huixinmuqiang.cn

[D22] 复制数组（避免共享引用）
来源：http://dv.huixinmuqiang.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ll.nicolike.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ew.colortex.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fu.colortex.cn

TS:   [...arr];
来源：http://xp.9csxet.cn

Java: new ArrayList<>(list);
来源：http://ii.huixiangedu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://sp.asd995.cn

Ruby: arr.dup;  arr.clone
来源：http://zp.chemitech.net.cn

C#:   new List<int>(list);
来源：http://do.hahajie.cn

[D23] reduce 累积计算
来源：http://au.yuexingan06.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xm.bookmarksfly.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pg.jctech888.com.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nr.521024.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mk.hnjuh.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://uh.shxzskj.cn

Go:   // 手写循环
来源：http://rl.asd995.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wv.gzmigu.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://sc.asd995.cn

[D24] 字典 / Map 基本操作
来源：http://jt.huanxung.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.lnxyls.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kj.muxihuayi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://sc.hnjuh.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fw.bjjhwx.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ht.haigaiapp.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ul.yuntaijiaju.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://uw.muxihuayi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wb.newstarts.cn

[D25] Set 集合去重与交并差
来源：http://sv.muxihuayi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ru.huixinmuqiang.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dj.huixinmuqiang.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hv.yuexingan06.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ci.wgjwhj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ut.hahajie.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ve.muxihuayi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://uo.9csxet.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://tx.huixiangedu.cn

[D26] 数组转字符串
来源：http://ua.nicolike.cn

Py:   ", ".join(map(str, arr))
来源：http://ev.yuntaijiaju.cn

PHP:  implode(", ", $arr);
来源：http://kj.nszjky.cn

JS:   arr.join(", ")
来源：http://oc.huixinmuqiang.cn

TS:   arr.join(", ")
来源：http://ym.newstarts.cn

Java: String.join(", ", list)
来源：http://rb.colortex.cn

Go:   strings.Join(strs, ", ")
来源：http://yp.9csxet.cn

Ruby: arr.join(", ")
来源：http://bu.hnjuh.cn

C#:   string.Join(", ", list)
来源：http://qq.nszjky.cn

================================================================================
来源：http://hi.colortex.cn

E. 字符串处理
来源：http://tb.bookmarksfly.cn

================================================================================
来源：http://qg.colortex.cn

[E01] 拼接字符串
来源：http://zy.lnxyls.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://io.9csxet.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ai.yuntaijiaju.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dl.asd995.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nn.gzmigu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vl.szsharing.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://uk.szxytkj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gr.hahajie.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kg.shtwfgs.cn

[E02] 重复字符串
来源：http://at.lnxyls.cn

Py:   "ab" * 3
来源：http://pi.shtwfgs.cn

PHP:  str_repeat("ab", 3);
来源：http://bm.bjjhwx.cn

JS:   "ab".repeat(3)
来源：http://dl.hnjuh.cn

TS:   "ab".repeat(3)
来源：http://pa.yuexingan06.cn

Java: "ab".repeat(3)
来源：http://ur.huanxung.cn

Go:   strings.Repeat("ab", 3)
来源：http://bk.nicolike.cn

Ruby: "ab" * 3
来源：http://ps.muxihuayi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ek.bookmarksfly.cn

[E03] 截取子串
来源：http://nl.huixiangedu.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xj.szsharing.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://br.yuntaijiaju.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ut.hnjuh.cn

TS:   s.slice(1, 4)
来源：http://wd.haigaiapp.cn

Java: s.substring(1, 4)
来源：http://ps.shxzukj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ul.huixinmuqiang.cn

Ruby: s[1, 3];  s[1..3]
来源：http://bm.9csxet.cn

C#:   s.Substring(1, 3)
来源：http://ky.muxihuayi.cn

[E04] 查找子串位置
来源：http://tv.shxzukj.cn

Py:   s.find("x");  s.index("x")
来源：http://mo.huanxung.cn

PHP:  strpos($s, "x");
来源：http://gv.colortex.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ms.haigaiapp.cn

TS:   s.indexOf("x")
来源：http://gp.asd995.cn

Java: s.indexOf("x")
来源：http://tl.colortex.cn

Go:   strings.Index(s, "x")
来源：http://fg.bjjhwx.cn

Ruby: s.index("x")
来源：http://do.huixiangedu.cn

C#:   s.IndexOf("x")
来源：http://tj.huanxung.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ja.gzmigu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://du.shtwfgs.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://cj.hnjuh.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nl.shtwfgs.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://bp.nicolike.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sw.nszjky.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ap.huanxung.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://by.huixinmuqiang.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://eu.shtwfgs.cn

[E06] 替换子串
来源：http://is.chemitech.net.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://af.chemitech.net.cn

PHP:  str_replace("a", "b", $s);
来源：http://gy.newstarts.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wu.bjjhwx.cn

TS:   s.replaceAll("a", "b")
来源：http://ns.colortex.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://im.szxytkj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rp.szsharing.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qu.nicolike.cn

C#:   s.Replace("a", "b")
来源：http://ct.chemitech.net.cn

[E07] 按分隔符拆分
来源：http://ks.gzmigu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://nz.521024.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://yn.gzmigu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://rj.shxzukj.cn

TS:   s.split(",")
来源：http://kg.shxzskj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://br.gzmigu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://za.muxihuayi.cn

Ruby: s.split(",");  s.split
来源：http://hx.shxzskj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kk.chemitech.net.cn

[E08] 数组按分隔符合并
来源：http://jv.nicolike.cn

Py:   ",".join(items)
来源：http://wy.panjiajie.cn

PHP:  implode(",", $items);
来源：http://ut.szxytkj.cn

JS:   items.join(",")
来源：http://yt.gzmigu.cn

TS:   items.join(",")
来源：http://ce.colortex.cn

Java: String.join(",", items)
来源：http://qu.shtwfgs.cn

Go:   strings.Join(items, ",")
来源：http://xu.szxytkj.cn

Ruby: items.join(",")
来源：http://jg.szxytkj.cn

C#:   string.Join(",", items)
来源：http://dv.yuntaijiaju.cn

[E09] 去除所有空白字符
来源：http://hi.shtwfgs.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://oh.asd995.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wu.chemitech.net.cn

JS:   s.replace(/\s+/g, "")
来源：http://ao.9csxet.cn

TS:   s.replace(/\s+/g, "")
来源：http://fx.huixinmuqiang.cn

Java: s.replaceAll("\\s+", "")
来源：http://uh.521024.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://bk.jctech888.com.cn

Ruby: s.gsub(/\s+/, "")
来源：http://wf.nszjky.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xm.shxzukj.cn

[E10] 左侧补零 / 定长填充
来源：http://xg.lnxyls.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://uz.shxzukj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://po.wgjwhj.cn

JS:   "7".padStart(3, "0")
来源：http://cd.gzmigu.cn

TS:   "7".padStart(3, "0")
来源：http://kc.huanxung.cn

Java: String.format("%03d", 7)
来源：http://yy.colortex.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://lt.gzmigu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lo.nicolike.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qt.bookmarksfly.cn

[E11] 反转字符串
来源：http://qt.newstarts.cn

Py:   s[::-1]
来源：http://kf.huanxung.cn

PHP:  strrev($s);
来源：http://wi.chemitech.net.cn

JS:   [...s].reverse().join("")
来源：http://fp.asd995.cn

TS:   [...s].reverse().join("")
来源：http://yf.shxzskj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://kg.9csxet.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ms.nicolike.cn

Ruby: s.reverse
来源：http://pw.bjjhwx.cn

C#:   new string(s.Reverse().ToArray())
来源：http://zj.shtwfgs.cn

[E12] 统计某字符出现次数
来源：http://cy.shxzukj.cn

Py:   s.count("a")
来源：http://uw.szsharing.cn

PHP:  substr_count($s, "a");
来源：http://fd.jctech888.com.cn

JS:   s.split("a").length - 1
来源：http://xq.521024.cn

TS:   s.split("a").length - 1
来源：http://bv.shtwfgs.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://le.asd995.cn

Go:   strings.Count(s, "a")
来源：http://mq.hnjuh.cn

Ruby: s.count("a")
来源：http://ou.nicolike.cn

C#:   s.Count(c => c == 'a')
来源：http://pn.muxihuayi.cn

[E13] 逐字符遍历
来源：http://ip.szxytkj.cn

Py:   for ch in s: print(ch)
来源：http://qx.yuntaijiaju.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fs.colortex.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://tj.huixinmuqiang.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://em.asd995.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xt.chemitech.net.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hw.hahajie.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://cp.bjjhwx.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://yi.nszjky.cn

[E14] URL 编码与 Base64
来源：http://ax.szsharing.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ie.yuntaijiaju.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://zz.jianghongdianzi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://yq.nicolike.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://uh.asd995.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qi.yuntaijiaju.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bz.bjjhwx.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tr.nicolike.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xr.9csxet.cn

[E15] HTML 转义 / 反转义
来源：http://xp.9csxet.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://el.chemitech.net.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://de.521024.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wa.yuexingan06.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://vf.huanxung.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zg.haigaiapp.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qz.521024.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://br.huanxung.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vi.yuexingan06.cn

[E16] 数字千分位
来源：http://pe.szsharing.cn

Py:   f"{1234567:,}"
来源：http://we.huanxung.cn

PHP:  number_format(1234567);
来源：http://qi.lnxyls.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://jq.nicolike.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://iu.huanxung.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gy.shxzukj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ff.wgjwhj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hv.bookmarksfly.cn

C#:   1234567.ToString("N0")
来源：http://ys.bookmarksfly.cn

[E17] 首字母大写
来源：http://er.huanxung.cn


<!-- 参考信息 -->