代发 wailian999

C#:   list.Reverse();
来源：http://mv.521024.cn

[D12] 查找元素下标
来源：http://yg.szxytkj.cn

Py:   arr.index(x);  x in arr
来源：http://tt.colortex.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://yg.jctech888.com.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://re.huixinmuqiang.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ib.jctech888.com.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ou.colortex.cn

Go:   slices.Index(arr, x)
来源：http://mc.wgjwhj.cn

Ruby: arr.index(x)
来源：http://kp.shtwfgs.cn

C#:   list.IndexOf(x);
来源：http://zd.chemitech.net.cn

[D13] 过滤（保留满足条件的）
来源：http://ry.hnjuh.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mg.nszjky.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://li.jctech888.com.cn

JS:   arr.filter(x => x > 3)
来源：http://va.nicolike.cn

TS:   arr.filter(x => x > 3)
来源：http://ua.colortex.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ax.yuexingan06.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rl.yuntaijiaju.cn

Ruby: arr.select { |x| x > 3 }
来源：http://fz.9csxet.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://bd.bookmarksfly.cn

[D14] 映射转换（每个元素变形）
来源：http://px.wgjwhj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ou.huixinmuqiang.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zz.shtwfgs.cn

JS:   arr.map(x => x * 2)
来源：http://zd.yuexingan06.cn

TS:   arr.map(x => x * 2)
来源：http://bb.nicolike.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://nw.9csxet.cn

Go:   // 手写循环
来源：http://qb.colortex.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ff.szsharing.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://mf.muxihuayi.cn

[D15] 去重
来源：http://gu.szxytkj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://oq.jctech888.com.cn

PHP:  array_unique($arr);
来源：http://aj.521024.cn

JS:   [...new Set(arr)]
来源：http://qi.shxzukj.cn

TS:   [...new Set(arr)]
来源：http://ab.muxihuayi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qf.shtwfgs.cn

Go:   // 用 map[T]struct{} 手写
来源：http://eb.gzmigu.cn

Ruby: arr.uniq
来源：http://lt.szsharing.cn

C#:   list.Distinct().ToList()
来源：http://il.521024.cn

[D16] 求和与平均值
来源：http://ny.521024.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://de.newstarts.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qk.hnjuh.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gu.asd995.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://aq.haigaiapp.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qu.huanxung.cn

Go:   // 手写循环累加
来源：http://to.szsharing.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://pb.haigaiapp.cn

C#:   list.Sum();  list.Average()
来源：http://yq.9csxet.cn

[D17] 最大值与最小值
来源：http://ev.bookmarksfly.cn

Py:   max(arr);  min(arr)
来源：http://kt.bjjhwx.cn

PHP:  max($arr);  min($arr);
来源：http://ks.jctech888.com.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zh.newstarts.cn

TS:   Math.max(...arr);
来源：http://nm.huanxung.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://la.nszjky.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mc.lnxyls.cn

Ruby: arr.max;  arr.min
来源：http://vn.chemitech.net.cn

C#:   list.Max();  list.Min()
来源：http://ew.colortex.cn

[D18] 扁平化嵌套数组
来源：http://cz.nszjky.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lx.nszjky.cn

PHP:  array_merge(...$nested);
来源：http://vw.panjiajie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xo.521024.cn

TS:   nested.flat();
来源：http://fv.521024.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hc.hahajie.cn

Go:   // 手写双层循环
来源：http://hy.wgjwhj.cn

Ruby: nested.flatten
来源：http://eh.huixinmuqiang.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://xj.yuexingan06.cn

[D19] 按字段分组
来源：http://pq.szsharing.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ep.colortex.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hk.nszjky.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ka.nszjky.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://qw.hahajie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://aq.nszjky.cn

Go:   // 手写 map[string][]T
来源：http://dn.szsharing.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://km.jctech888.com.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bu.huanxung.cn

[D20] 统计每个元素出现次数
来源：http://ri.lnxyls.cn

Py:   Counter(arr)
来源：http://zt.lnxyls.cn

PHP:  array_count_values($arr);
来源：http://pq.521024.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fu.huixiangedu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fm.bookmarksfly.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://la.panjiajie.cn

Go:   // 手写 map[T]int
来源：http://zk.jianghongdianzi.cn

Ruby: arr.tally
来源：http://is.chemitech.net.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://js.huanxung.cn

[D21] 判断是否包含某元素
来源：http://tt.huixiangedu.cn

Py:   x in arr
来源：http://hy.jctech888.com.cn

PHP:  in_array($x, $arr, true);
来源：http://xi.nszjky.cn

JS:   arr.includes(x)
来源：http://cr.jianghongdianzi.cn

TS:   arr.includes(x)
来源：http://tx.jianghongdianzi.cn

Java: list.contains(x)
来源：http://ff.shxzukj.cn

Go:   slices.Contains(arr, x)
来源：http://du.huanxung.cn

Ruby: arr.include?(x)
来源：http://ha.huixiangedu.cn

C#:   list.Contains(x)
来源：http://vb.hahajie.cn

[D22] 复制数组（避免共享引用）
来源：http://kv.gzmigu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pm.newstarts.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jy.9csxet.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bx.huixiangedu.cn

TS:   [...arr];
来源：http://xc.szxytkj.cn

Java: new ArrayList<>(list);
来源：http://eh.asd995.cn

Go:   copied := append([]int(nil), arr...)
来源：http://an.chemitech.net.cn

Ruby: arr.dup;  arr.clone
来源：http://vf.nszjky.cn

C#:   new List<int>(list);
来源：http://rt.nszjky.cn

[D23] reduce 累积计算
来源：http://es.szxytkj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hu.hahajie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://lw.nicolike.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://el.bookmarksfly.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://si.lnxyls.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://fc.shxzukj.cn

Go:   // 手写循环
来源：http://em.panjiajie.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://iw.szxytkj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ik.huanxung.cn

[D24] 字典 / Map 基本操作
来源：http://wq.wgjwhj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://lk.hahajie.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://eq.asd995.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vv.shxzskj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hk.yuexingan06.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ns.wgjwhj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ko.bjjhwx.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ig.huixiangedu.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://nq.yuexingan06.cn

[D25] Set 集合去重与交并差
来源：http://kr.nszjky.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ci.haigaiapp.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dc.521024.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jm.gzmigu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://yt.jianghongdianzi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://th.muxihuayi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ih.yuntaijiaju.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://iy.shxzskj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zz.huixiangedu.cn

[D26] 数组转字符串
来源：http://us.chemitech.net.cn

Py:   ", ".join(map(str, arr))
来源：http://uo.asd995.cn

PHP:  implode(", ", $arr);
来源：http://ie.wgjwhj.cn

JS:   arr.join(", ")
来源：http://ld.haigaiapp.cn

TS:   arr.join(", ")
来源：http://gr.haigaiapp.cn

Java: String.join(", ", list)
来源：http://gq.chemitech.net.cn

Go:   strings.Join(strs, ", ")
来源：http://xm.jianghongdianzi.cn

Ruby: arr.join(", ")
来源：http://zp.hnjuh.cn

C#:   string.Join(", ", list)
来源：http://ze.colortex.cn

================================================================================
来源：http://fr.asd995.cn

E. 字符串处理
来源：http://ki.jctech888.com.cn

================================================================================
来源：http://lh.jctech888.com.cn

[E01] 拼接字符串
来源：http://io.colortex.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://kw.hahajie.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vb.huixiangedu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nd.yuexingan06.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ru.colortex.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pp.hahajie.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rs.shtwfgs.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ya.shtwfgs.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://yu.shxzukj.cn

[E02] 重复字符串
来源：http://mp.huixinmuqiang.cn

Py:   "ab" * 3
来源：http://bi.chemitech.net.cn

PHP:  str_repeat("ab", 3);
来源：http://ed.jctech888.com.cn

JS:   "ab".repeat(3)
来源：http://up.jctech888.com.cn

TS:   "ab".repeat(3)
来源：http://bh.9csxet.cn

Java: "ab".repeat(3)
来源：http://eb.colortex.cn

Go:   strings.Repeat("ab", 3)
来源：http://is.hahajie.cn

Ruby: "ab" * 3
来源：http://mf.asd995.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://bb.hahajie.cn

[E03] 截取子串
来源：http://sy.yuexingan06.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://uz.huixinmuqiang.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fu.yuntaijiaju.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ek.bookmarksfly.cn

TS:   s.slice(1, 4)
来源：http://dz.szxytkj.cn

Java: s.substring(1, 4)
来源：http://ht.panjiajie.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ja.wgjwhj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://lb.szxytkj.cn

C#:   s.Substring(1, 3)
来源：http://gi.huixiangedu.cn

[E04] 查找子串位置
来源：http://vm.wgjwhj.cn

Py:   s.find("x");  s.index("x")
来源：http://gj.newstarts.cn

PHP:  strpos($s, "x");
来源：http://io.asd995.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://st.chemitech.net.cn

TS:   s.indexOf("x")
来源：http://el.jctech888.com.cn

Java: s.indexOf("x")
来源：http://ia.muxihuayi.cn

Go:   strings.Index(s, "x")
来源：http://zz.lnxyls.cn

Ruby: s.index("x")
来源：http://rd.szsharing.cn

C#:   s.IndexOf("x")
来源：http://ii.nicolike.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://fx.wgjwhj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://al.szxytkj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://sg.huixiangedu.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://in.yuntaijiaju.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://wu.shxzukj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gr.bjjhwx.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ym.yuntaijiaju.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://cc.huixinmuqiang.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://si.huixiangedu.cn

[E06] 替换子串
来源：http://hj.asd995.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://lz.9csxet.cn

PHP:  str_replace("a", "b", $s);
来源：http://aw.yuexingan06.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ez.asd995.cn

TS:   s.replaceAll("a", "b")
来源：http://yq.huixinmuqiang.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pn.wgjwhj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hu.jianghongdianzi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vu.szxytkj.cn

C#:   s.Replace("a", "b")
来源：http://gc.9csxet.cn

[E07] 按分隔符拆分
来源：http://au.chemitech.net.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ux.nszjky.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://lx.haigaiapp.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://sd.521024.cn

TS:   s.split(",")
来源：http://km.shxzukj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://xf.9csxet.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bu.yuexingan06.cn

Ruby: s.split(",");  s.split
来源：http://mr.chemitech.net.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xt.huixinmuqiang.cn

[E08] 数组按分隔符合并
来源：http://bu.huixinmuqiang.cn

Py:   ",".join(items)
来源：http://jt.shtwfgs.cn

PHP:  implode(",", $items);
来源：http://ts.yuntaijiaju.cn

JS:   items.join(",")
来源：http://ul.9csxet.cn

TS:   items.join(",")
来源：http://pv.huixinmuqiang.cn

Java: String.join(",", items)
来源：http://uz.nszjky.cn

Go:   strings.Join(items, ",")
来源：http://lr.asd995.cn

Ruby: items.join(",")
来源：http://na.yuntaijiaju.cn

C#:   string.Join(",", items)
来源：http://yu.9csxet.cn

[E09] 去除所有空白字符
来源：http://rh.chemitech.net.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pw.jctech888.com.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xz.shtwfgs.cn

JS:   s.replace(/\s+/g, "")
来源：http://zf.huanxung.cn

TS:   s.replace(/\s+/g, "")
来源：http://kj.haigaiapp.cn

Java: s.replaceAll("\\s+", "")
来源：http://kc.bookmarksfly.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://kw.huixiangedu.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ta.gzmigu.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://nx.jianghongdianzi.cn

[E10] 左侧补零 / 定长填充
来源：http://wh.jctech888.com.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ga.bjjhwx.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://uh.hnjuh.cn

JS:   "7".padStart(3, "0")
来源：http://ru.nszjky.cn

TS:   "7".padStart(3, "0")
来源：http://py.shxzskj.cn

Java: String.format("%03d", 7)
来源：http://qg.gzmigu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://um.nszjky.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://uj.shxzukj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wo.asd995.cn

[E11] 反转字符串
来源：http://it.jctech888.com.cn

Py:   s[::-1]
来源：http://bk.asd995.cn

PHP:  strrev($s);
来源：http://ma.lnxyls.cn

JS:   [...s].reverse().join("")
来源：http://ce.nszjky.cn

TS:   [...s].reverse().join("")
来源：http://zs.szsharing.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://hm.jctech888.com.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ln.hahajie.cn

Ruby: s.reverse
来源：http://vr.asd995.cn

C#:   new string(s.Reverse().ToArray())
来源：http://cu.jctech888.com.cn

[E12] 统计某字符出现次数
来源：http://id.nszjky.cn

Py:   s.count("a")
来源：http://yu.9csxet.cn

PHP:  substr_count($s, "a");
来源：http://nt.gzmigu.cn

JS:   s.split("a").length - 1
来源：http://ch.shxzskj.cn

TS:   s.split("a").length - 1
来源：http://st.szxytkj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vy.wgjwhj.cn

Go:   strings.Count(s, "a")
来源：http://ee.panjiajie.cn

Ruby: s.count("a")
来源：http://ys.huanxung.cn

C#:   s.Count(c => c == 'a')
来源：http://zs.huixiangedu.cn

[E13] 逐字符遍历
来源：http://ta.szxytkj.cn

Py:   for ch in s: print(ch)
来源：http://sw.haigaiapp.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jv.bjjhwx.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ov.shxzskj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://uh.jianghongdianzi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ww.colortex.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ws.newstarts.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ch.nicolike.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://oa.jctech888.com.cn

[E14] URL 编码与 Base64
来源：http://gc.yuexingan06.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://st.nicolike.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://is.bjjhwx.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://lv.yuntaijiaju.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ft.newstarts.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://cd.521024.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://yx.huixinmuqiang.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://pk.521024.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://pf.chemitech.net.cn

[E15] HTML 转义 / 反转义
来源：http://gy.bjjhwx.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://zm.yuntaijiaju.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://je.huanxung.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://as.colortex.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://zn.9csxet.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://aa.9csxet.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ga.szxytkj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fq.newstarts.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bk.shtwfgs.cn

[E16] 数字千分位
来源：http://dq.huanxung.cn

Py:   f"{1234567:,}"
来源：http://qv.nszjky.cn

PHP:  number_format(1234567);
来源：http://ea.jianghongdianzi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ug.muxihuayi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://zg.hnjuh.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fh.nszjky.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fb.panjiajie.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qx.521024.cn

C#:   1234567.ToString("N0")
来源：http://ub.chemitech.net.cn

[E17] 首字母大写
来源：http://ss.chemitech.net.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://no.szsharing.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://bh.jianghongdianzi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xk.521024.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zj.szsharing.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://at.nszjky.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wh.haigaiapp.cn

Ruby: s.capitalize
来源：http://ib.yuntaijiaju.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hq.colortex.cn

[E18] 模板占位符替换
来源：http://qr.gzmigu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ad.jianghongdianzi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://va.shtwfgs.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://fl.hnjuh.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://gc.colortex.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gv.huanxung.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://br.panjiajie.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://yl.muxihuayi.cn


<!-- 参考信息 -->