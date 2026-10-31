代发 wailian999

C#:   list.Reverse();
来源：http://qi.jianghongdianzi.cn

[D12] 查找元素下标
来源：http://zf.shxzukj.cn

Py:   arr.index(x);  x in arr
来源：http://fs.szxytkj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dp.hahajie.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ci.yuntaijiaju.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ds.shxzukj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://iz.haigaiapp.cn

Go:   slices.Index(arr, x)
来源：http://kw.nicolike.cn

Ruby: arr.index(x)
来源：http://jd.chemitech.net.cn

C#:   list.IndexOf(x);
来源：http://wo.colortex.cn

[D13] 过滤（保留满足条件的）
来源：http://rz.nicolike.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vq.szsharing.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qu.chemitech.net.cn

JS:   arr.filter(x => x > 3)
来源：http://co.muxihuayi.cn

TS:   arr.filter(x => x > 3)
来源：http://jt.chemitech.net.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://nk.asd995.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://yj.huanxung.cn

Ruby: arr.select { |x| x > 3 }
来源：http://xp.chemitech.net.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://za.nszjky.cn

[D14] 映射转换（每个元素变形）
来源：http://dc.newstarts.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rk.shxzskj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fv.yuntaijiaju.cn

JS:   arr.map(x => x * 2)
来源：http://ho.colortex.cn

TS:   arr.map(x => x * 2)
来源：http://ac.muxihuayi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://un.yuntaijiaju.cn

Go:   // 手写循环
来源：http://gt.hnjuh.cn

Ruby: arr.map { |x| x * 2 }
来源：http://cy.haigaiapp.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://li.shxzukj.cn

[D15] 去重
来源：http://jm.colortex.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xh.shtwfgs.cn

PHP:  array_unique($arr);
来源：http://ds.hnjuh.cn

JS:   [...new Set(arr)]
来源：http://uv.shxzukj.cn

TS:   [...new Set(arr)]
来源：http://mf.jianghongdianzi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cs.hnjuh.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ta.colortex.cn

Ruby: arr.uniq
来源：http://lz.szxytkj.cn

C#:   list.Distinct().ToList()
来源：http://dk.huixiangedu.cn

[D16] 求和与平均值
来源：http://jx.hahajie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://pu.bookmarksfly.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://io.gzmigu.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://sr.bookmarksfly.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://pm.lnxyls.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://re.9csxet.cn

Go:   // 手写循环累加
来源：http://xy.jianghongdianzi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://cb.bookmarksfly.cn

C#:   list.Sum();  list.Average()
来源：http://mh.huanxung.cn

[D17] 最大值与最小值
来源：http://tw.asd995.cn

Py:   max(arr);  min(arr)
来源：http://ct.nszjky.cn

PHP:  max($arr);  min($arr);
来源：http://lg.shxzukj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gc.nicolike.cn

TS:   Math.max(...arr);
来源：http://sr.szxytkj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://et.szsharing.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://eq.9csxet.cn

Ruby: arr.max;  arr.min
来源：http://ud.wgjwhj.cn

C#:   list.Max();  list.Min()
来源：http://ur.szxytkj.cn

[D18] 扁平化嵌套数组
来源：http://cz.hnjuh.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://aa.jctech888.com.cn

PHP:  array_merge(...$nested);
来源：http://bu.jianghongdianzi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hp.chemitech.net.cn

TS:   nested.flat();
来源：http://ck.jianghongdianzi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ac.gzmigu.cn

Go:   // 手写双层循环
来源：http://wo.muxihuayi.cn

Ruby: nested.flatten
来源：http://uy.muxihuayi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://zf.asd995.cn

[D19] 按字段分组
来源：http://kz.bookmarksfly.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zk.9csxet.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://gx.haigaiapp.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ns.nicolike.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.yuexingan06.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yb.chemitech.net.cn

Go:   // 手写 map[string][]T
来源：http://um.asd995.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ce.panjiajie.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lh.szxytkj.cn

[D20] 统计每个元素出现次数
来源：http://oo.shxzskj.cn

Py:   Counter(arr)
来源：http://sf.chemitech.net.cn

PHP:  array_count_values($arr);
来源：http://eo.jianghongdianzi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xt.muxihuayi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lc.yuntaijiaju.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ys.shxzskj.cn

Go:   // 手写 map[T]int
来源：http://sc.szsharing.cn

Ruby: arr.tally
来源：http://fs.yuntaijiaju.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://gn.gzmigu.cn

[D21] 判断是否包含某元素
来源：http://oi.wgjwhj.cn

Py:   x in arr
来源：http://fd.bjjhwx.cn

PHP:  in_array($x, $arr, true);
来源：http://jt.huanxung.cn

JS:   arr.includes(x)
来源：http://ki.szxytkj.cn

TS:   arr.includes(x)
来源：http://kz.huanxung.cn

Java: list.contains(x)
来源：http://uc.huixinmuqiang.cn

Go:   slices.Contains(arr, x)
来源：http://dr.colortex.cn

Ruby: arr.include?(x)
来源：http://me.muxihuayi.cn

C#:   list.Contains(x)
来源：http://md.521024.cn

[D22] 复制数组（避免共享引用）
来源：http://kk.colortex.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nz.hnjuh.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gw.jianghongdianzi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wd.nszjky.cn

TS:   [...arr];
来源：http://fn.chemitech.net.cn

Java: new ArrayList<>(list);
来源：http://kh.colortex.cn

Go:   copied := append([]int(nil), arr...)
来源：http://nz.bookmarksfly.cn

Ruby: arr.dup;  arr.clone
来源：http://qp.panjiajie.cn

C#:   new List<int>(list);
来源：http://qd.szsharing.cn

[D23] reduce 累积计算
来源：http://wh.hnjuh.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://iv.jianghongdianzi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://km.521024.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gk.521024.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hi.szxytkj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://om.panjiajie.cn

Go:   // 手写循环
来源：http://qt.hahajie.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zr.szxytkj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://yi.yuexingan06.cn

[D24] 字典 / Map 基本操作
来源：http://cr.chemitech.net.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ui.hahajie.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://sy.nszjky.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://sl.nicolike.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cg.shxzukj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hx.szsharing.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qy.szsharing.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://av.colortex.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jl.chemitech.net.cn

[D25] Set 集合去重与交并差
来源：http://zl.bjjhwx.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jf.chemitech.net.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dq.lnxyls.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ax.panjiajie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ef.muxihuayi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hm.szsharing.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://bn.lnxyls.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://rx.asd995.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://st.szsharing.cn

[D26] 数组转字符串
来源：http://kg.wgjwhj.cn

Py:   ", ".join(map(str, arr))
来源：http://ik.gzmigu.cn

PHP:  implode(", ", $arr);
来源：http://xf.yuexingan06.cn

JS:   arr.join(", ")
来源：http://ax.szxytkj.cn

TS:   arr.join(", ")
来源：http://tf.muxihuayi.cn

Java: String.join(", ", list)
来源：http://dq.shtwfgs.cn

Go:   strings.Join(strs, ", ")
来源：http://bf.hnjuh.cn

Ruby: arr.join(", ")
来源：http://od.szxytkj.cn

C#:   string.Join(", ", list)
来源：http://hn.yuexingan06.cn

================================================================================
来源：http://hj.huixiangedu.cn

E. 字符串处理
来源：http://bw.yuexingan06.cn

================================================================================
来源：http://qn.yuexingan06.cn

[E01] 拼接字符串
来源：http://vc.jctech888.com.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bw.hnjuh.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xs.shxzskj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ll.yuexingan06.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xd.huixinmuqiang.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://an.shxzskj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dn.chemitech.net.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://md.nszjky.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ca.bookmarksfly.cn

[E02] 重复字符串
来源：http://ic.shxzukj.cn

Py:   "ab" * 3
来源：http://ya.yuexingan06.cn

PHP:  str_repeat("ab", 3);
来源：http://xy.bookmarksfly.cn

JS:   "ab".repeat(3)
来源：http://au.chemitech.net.cn

TS:   "ab".repeat(3)
来源：http://xi.hahajie.cn

Java: "ab".repeat(3)
来源：http://lp.yuntaijiaju.cn

Go:   strings.Repeat("ab", 3)
来源：http://an.yuexingan06.cn

Ruby: "ab" * 3
来源：http://ew.hnjuh.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dl.bjjhwx.cn

[E03] 截取子串
来源：http://xe.yuexingan06.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wr.asd995.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://py.521024.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vv.shxzukj.cn

TS:   s.slice(1, 4)
来源：http://oi.huixinmuqiang.cn

Java: s.substring(1, 4)
来源：http://bs.hnjuh.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xo.jctech888.com.cn

Ruby: s[1, 3];  s[1..3]
来源：http://uq.shxzskj.cn

C#:   s.Substring(1, 3)
来源：http://ew.panjiajie.cn

[E04] 查找子串位置
来源：http://jz.wgjwhj.cn

Py:   s.find("x");  s.index("x")
来源：http://ly.gzmigu.cn

PHP:  strpos($s, "x");
来源：http://km.hahajie.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://lb.9csxet.cn

TS:   s.indexOf("x")
来源：http://mx.shxzukj.cn

Java: s.indexOf("x")
来源：http://gt.lnxyls.cn

Go:   strings.Index(s, "x")
来源：http://dq.wgjwhj.cn

Ruby: s.index("x")
来源：http://mv.bjjhwx.cn

C#:   s.IndexOf("x")
来源：http://hd.jctech888.com.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ub.bookmarksfly.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://tt.asd995.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://rj.9csxet.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://am.nicolike.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://oy.shtwfgs.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ae.huixiangedu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://vx.yuntaijiaju.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://kk.shxzskj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jv.jianghongdianzi.cn

[E06] 替换子串
来源：http://kc.haigaiapp.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://oi.panjiajie.cn

PHP:  str_replace("a", "b", $s);
来源：http://qh.nicolike.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zd.jctech888.com.cn

TS:   s.replaceAll("a", "b")
来源：http://ke.newstarts.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rq.gzmigu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bp.chemitech.net.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ls.chemitech.net.cn

C#:   s.Replace("a", "b")
来源：http://mx.gzmigu.cn

[E07] 按分隔符拆分
来源：http://xo.muxihuayi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gy.asd995.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hn.asd995.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ae.wgjwhj.cn

TS:   s.split(",")
来源：http://ys.haigaiapp.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ae.asd995.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://de.haigaiapp.cn

Ruby: s.split(",");  s.split
来源：http://xp.jctech888.com.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wx.huixiangedu.cn

[E08] 数组按分隔符合并
来源：http://tz.nicolike.cn

Py:   ",".join(items)
来源：http://sp.panjiajie.cn

PHP:  implode(",", $items);
来源：http://ji.colortex.cn

JS:   items.join(",")
来源：http://sw.huixiangedu.cn

TS:   items.join(",")
来源：http://bz.huixiangedu.cn

Java: String.join(",", items)
来源：http://uy.panjiajie.cn

Go:   strings.Join(items, ",")
来源：http://do.yuntaijiaju.cn

Ruby: items.join(",")
来源：http://kh.asd995.cn

C#:   string.Join(",", items)
来源：http://wp.jctech888.com.cn

[E09] 去除所有空白字符
来源：http://op.hnjuh.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://we.hahajie.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wk.muxihuayi.cn

JS:   s.replace(/\s+/g, "")
来源：http://sh.szsharing.cn

TS:   s.replace(/\s+/g, "")
来源：http://sb.9csxet.cn

Java: s.replaceAll("\\s+", "")
来源：http://ox.jianghongdianzi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://zd.shtwfgs.cn

Ruby: s.gsub(/\s+/, "")
来源：http://pg.huixiangedu.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vn.muxihuayi.cn

[E10] 左侧补零 / 定长填充
来源：http://ne.521024.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wu.hnjuh.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fv.wgjwhj.cn

JS:   "7".padStart(3, "0")
来源：http://uz.huanxung.cn

TS:   "7".padStart(3, "0")
来源：http://ka.shxzskj.cn

Java: String.format("%03d", 7)
来源：http://bn.hahajie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://tj.shtwfgs.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://gf.wgjwhj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mn.colortex.cn

[E11] 反转字符串
来源：http://sn.521024.cn

Py:   s[::-1]
来源：http://qg.panjiajie.cn

PHP:  strrev($s);
来源：http://rt.nszjky.cn

JS:   [...s].reverse().join("")
来源：http://ot.chemitech.net.cn

TS:   [...s].reverse().join("")
来源：http://it.haigaiapp.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://am.yuexingan06.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ii.muxihuayi.cn

Ruby: s.reverse
来源：http://qe.huixinmuqiang.cn

C#:   new string(s.Reverse().ToArray())
来源：http://pj.huixiangedu.cn

[E12] 统计某字符出现次数
来源：http://ke.shxzukj.cn

Py:   s.count("a")
来源：http://kq.huixinmuqiang.cn

PHP:  substr_count($s, "a");
来源：http://la.hahajie.cn

JS:   s.split("a").length - 1
来源：http://qt.nszjky.cn

TS:   s.split("a").length - 1
来源：http://qr.yuexingan06.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ct.huanxung.cn

Go:   strings.Count(s, "a")
来源：http://ez.szxytkj.cn

Ruby: s.count("a")
来源：http://cx.huixiangedu.cn

C#:   s.Count(c => c == 'a')
来源：http://vw.yuexingan06.cn

[E13] 逐字符遍历
来源：http://du.bookmarksfly.cn

Py:   for ch in s: print(ch)
来源：http://hu.yuntaijiaju.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ue.hahajie.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://cb.jianghongdianzi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://dc.newstarts.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xk.asd995.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://os.gzmigu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://hn.huixiangedu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wi.9csxet.cn

[E14] URL 编码与 Base64
来源：http://ij.chemitech.net.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://eu.jianghongdianzi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://bn.muxihuayi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zq.bookmarksfly.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://lw.newstarts.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wd.colortex.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bs.yuexingan06.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://yw.bjjhwx.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ww.newstarts.cn

[E15] HTML 转义 / 反转义
来源：http://dy.jctech888.com.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://dd.panjiajie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bp.huanxung.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lh.jianghongdianzi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://jv.hahajie.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ka.shtwfgs.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://kl.bjjhwx.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mp.jctech888.com.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ui.wgjwhj.cn

[E16] 数字千分位
来源：http://iy.9csxet.cn

Py:   f"{1234567:,}"
来源：http://du.asd995.cn

PHP:  number_format(1234567);
来源：http://us.yuexingan06.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ms.chemitech.net.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://bp.nszjky.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rd.nicolike.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xw.bjjhwx.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dn.jianghongdianzi.cn

C#:   1234567.ToString("N0")
来源：http://hr.9csxet.cn

[E17] 首字母大写
来源：http://np.jianghongdianzi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hi.newstarts.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://as.colortex.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wm.asd995.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://em.szsharing.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ag.521024.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zi.shxzskj.cn

Ruby: s.capitalize
来源：http://gd.shtwfgs.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tw.szsharing.cn

[E18] 模板占位符替换
来源：http://xi.521024.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ar.jctech888.com.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ri.chemitech.net.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ec.muxihuayi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://jq.nicolike.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xp.gzmigu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://eg.jctech888.com.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://bv.asd995.cn


<!-- 参考信息 -->