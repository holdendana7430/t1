代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yp.hnjuh.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ly.jianghongdianzi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gw.panjiajie.cn

Go:   slices.Index(arr, x)
来源：http://ql.muxihuayi.cn

Ruby: arr.index(x)
来源：http://iq.bjjhwx.cn

C#:   list.IndexOf(x);
来源：http://fr.szsharing.cn

[D13] 过滤（保留满足条件的）
来源：http://qv.9csxet.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jz.shxzukj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jo.jianghongdianzi.cn

JS:   arr.filter(x => x > 3)
来源：http://ja.nszjky.cn

TS:   arr.filter(x => x > 3)
来源：http://wi.gzmigu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gz.9csxet.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://uo.haigaiapp.cn

Ruby: arr.select { |x| x > 3 }
来源：http://dd.bookmarksfly.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ui.bjjhwx.cn

[D14] 映射转换（每个元素变形）
来源：http://ig.wgjwhj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qr.jianghongdianzi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zc.chemitech.net.cn

JS:   arr.map(x => x * 2)
来源：http://gk.nicolike.cn

TS:   arr.map(x => x * 2)
来源：http://zy.panjiajie.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ny.huanxung.cn

Go:   // 手写循环
来源：http://ov.szsharing.cn

Ruby: arr.map { |x| x * 2 }
来源：http://bg.shxzskj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://nj.yuntaijiaju.cn

[D15] 去重
来源：http://ik.szsharing.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yb.yuntaijiaju.cn

PHP:  array_unique($arr);
来源：http://pg.shtwfgs.cn

JS:   [...new Set(arr)]
来源：http://cu.jianghongdianzi.cn

TS:   [...new Set(arr)]
来源：http://ym.9csxet.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fe.szxytkj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://co.panjiajie.cn

Ruby: arr.uniq
来源：http://dc.jianghongdianzi.cn

C#:   list.Distinct().ToList()
来源：http://gt.huixiangedu.cn

[D16] 求和与平均值
来源：http://dk.521024.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lz.521024.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ee.huixinmuqiang.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://nc.bjjhwx.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jg.panjiajie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://la.huanxung.cn

Go:   // 手写循环累加
来源：http://hs.wgjwhj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qv.panjiajie.cn

C#:   list.Sum();  list.Average()
来源：http://hx.shxzskj.cn

[D17] 最大值与最小值
来源：http://id.jianghongdianzi.cn

Py:   max(arr);  min(arr)
来源：http://zc.hnjuh.cn

PHP:  max($arr);  min($arr);
来源：http://sh.lnxyls.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ft.521024.cn

TS:   Math.max(...arr);
来源：http://rc.9csxet.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ta.huixiangedu.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qv.szsharing.cn

Ruby: arr.max;  arr.min
来源：http://jt.huixinmuqiang.cn

C#:   list.Max();  list.Min()
来源：http://px.colortex.cn

[D18] 扁平化嵌套数组
来源：http://kh.lnxyls.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.huixinmuqiang.cn

PHP:  array_merge(...$nested);
来源：http://ka.wgjwhj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ov.yuexingan06.cn

TS:   nested.flat();
来源：http://xj.panjiajie.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ob.asd995.cn

Go:   // 手写双层循环
来源：http://tq.shxzskj.cn

Ruby: nested.flatten
来源：http://bw.nszjky.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://cf.huixiangedu.cn

[D19] 按字段分组
来源：http://nq.szxytkj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://su.shxzskj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://yv.9csxet.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ax.hnjuh.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://xz.shtwfgs.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://eu.muxihuayi.cn

Go:   // 手写 map[string][]T
来源：http://vk.lnxyls.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://sp.newstarts.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ex.colortex.cn

[D20] 统计每个元素出现次数
来源：http://za.nszjky.cn

Py:   Counter(arr)
来源：http://tr.huixiangedu.cn

PHP:  array_count_values($arr);
来源：http://lw.nicolike.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pk.bjjhwx.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://za.nszjky.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ui.jianghongdianzi.cn

Go:   // 手写 map[T]int
来源：http://gw.nicolike.cn

Ruby: arr.tally
来源：http://oe.panjiajie.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kk.newstarts.cn

[D21] 判断是否包含某元素
来源：http://tg.9csxet.cn

Py:   x in arr
来源：http://db.bookmarksfly.cn

PHP:  in_array($x, $arr, true);
来源：http://ci.nicolike.cn

JS:   arr.includes(x)
来源：http://gs.newstarts.cn

TS:   arr.includes(x)
来源：http://uu.hahajie.cn

Java: list.contains(x)
来源：http://bd.colortex.cn

Go:   slices.Contains(arr, x)
来源：http://bo.bjjhwx.cn

Ruby: arr.include?(x)
来源：http://wi.lnxyls.cn

C#:   list.Contains(x)
来源：http://nh.yuntaijiaju.cn

[D22] 复制数组（避免共享引用）
来源：http://ua.hnjuh.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://km.asd995.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ha.newstarts.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://pj.wgjwhj.cn

TS:   [...arr];
来源：http://uw.yuntaijiaju.cn

Java: new ArrayList<>(list);
来源：http://rj.wgjwhj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://md.lnxyls.cn

Ruby: arr.dup;  arr.clone
来源：http://el.jctech888.com.cn

C#:   new List<int>(list);
来源：http://vz.chemitech.net.cn

[D23] reduce 累积计算
来源：http://wd.szsharing.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bo.huanxung.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zm.newstarts.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vy.bookmarksfly.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sw.yuexingan06.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://mc.colortex.cn

Go:   // 手写循环
来源：http://es.yuexingan06.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ey.shxzukj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://bt.haigaiapp.cn

[D24] 字典 / Map 基本操作
来源：http://qb.szsharing.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ot.jctech888.com.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hr.asd995.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qi.yuexingan06.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://aj.gzmigu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://es.wgjwhj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hs.shtwfgs.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://sd.hahajie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://um.hahajie.cn

[D25] Set 集合去重与交并差
来源：http://go.9csxet.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hr.panjiajie.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bc.yuntaijiaju.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xg.lnxyls.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://pq.yuntaijiaju.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ix.jctech888.com.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://cu.hahajie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dq.shxzukj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xa.huanxung.cn

[D26] 数组转字符串
来源：http://yx.szxytkj.cn

Py:   ", ".join(map(str, arr))
来源：http://gn.haigaiapp.cn

PHP:  implode(", ", $arr);
来源：http://xx.muxihuayi.cn

JS:   arr.join(", ")
来源：http://px.chemitech.net.cn

TS:   arr.join(", ")
来源：http://jr.szsharing.cn

Java: String.join(", ", list)
来源：http://yj.muxihuayi.cn

Go:   strings.Join(strs, ", ")
来源：http://nb.9csxet.cn

Ruby: arr.join(", ")
来源：http://yu.bjjhwx.cn

C#:   string.Join(", ", list)
来源：http://fo.huixiangedu.cn

================================================================================
来源：http://ea.asd995.cn

E. 字符串处理
来源：http://op.chemitech.net.cn

================================================================================
来源：http://ie.newstarts.cn

[E01] 拼接字符串
来源：http://ba.shtwfgs.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gb.jctech888.com.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://td.colortex.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ql.colortex.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zr.nszjky.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qi.shtwfgs.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jh.lnxyls.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wo.colortex.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ph.shxzukj.cn

[E02] 重复字符串
来源：http://af.jctech888.com.cn

Py:   "ab" * 3
来源：http://oj.lnxyls.cn

PHP:  str_repeat("ab", 3);
来源：http://jp.nszjky.cn

JS:   "ab".repeat(3)
来源：http://ux.szsharing.cn

TS:   "ab".repeat(3)
来源：http://ll.szsharing.cn

Java: "ab".repeat(3)
来源：http://db.szsharing.cn

Go:   strings.Repeat("ab", 3)
来源：http://yz.chemitech.net.cn

Ruby: "ab" * 3
来源：http://jb.bookmarksfly.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lt.huixinmuqiang.cn

[E03] 截取子串
来源：http://ac.jianghongdianzi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://pd.shxzukj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qk.nicolike.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mr.lnxyls.cn

TS:   s.slice(1, 4)
来源：http://zv.nicolike.cn

Java: s.substring(1, 4)
来源：http://yj.huixinmuqiang.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ru.yuntaijiaju.cn

Ruby: s[1, 3];  s[1..3]
来源：http://vp.shxzskj.cn

C#:   s.Substring(1, 3)
来源：http://se.yuntaijiaju.cn

[E04] 查找子串位置
来源：http://xd.hnjuh.cn

Py:   s.find("x");  s.index("x")
来源：http://nt.bookmarksfly.cn

PHP:  strpos($s, "x");
来源：http://zl.lnxyls.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://td.shtwfgs.cn

TS:   s.indexOf("x")
来源：http://sw.huixinmuqiang.cn

Java: s.indexOf("x")
来源：http://qz.wgjwhj.cn

Go:   strings.Index(s, "x")
来源：http://fr.yuexingan06.cn

Ruby: s.index("x")
来源：http://yn.yuexingan06.cn

C#:   s.IndexOf("x")
来源：http://fu.hahajie.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://lg.hahajie.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://nk.huixinmuqiang.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qx.lnxyls.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jctech888.com.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://rq.jianghongdianzi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vh.chemitech.net.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ef.haigaiapp.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hu.hahajie.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bt.yuexingan06.cn

[E06] 替换子串
来源：http://cg.chemitech.net.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://tj.nszjky.cn

PHP:  str_replace("a", "b", $s);
来源：http://lc.wgjwhj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xu.9csxet.cn

TS:   s.replaceAll("a", "b")
来源：http://uf.huixiangedu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dg.shxzskj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rw.bookmarksfly.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qf.panjiajie.cn

C#:   s.Replace("a", "b")
来源：http://gc.bjjhwx.cn

[E07] 按分隔符拆分
来源：http://ud.huixinmuqiang.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vx.bookmarksfly.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fc.huixiangedu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ya.asd995.cn

TS:   s.split(",")
来源：http://rd.asd995.cn

Java: s.split(",");  s.split("\\s+")
来源：http://kp.szxytkj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zf.huixinmuqiang.cn

Ruby: s.split(",");  s.split
来源：http://fh.shxzukj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://se.shxzskj.cn

[E08] 数组按分隔符合并
来源：http://fk.yuntaijiaju.cn

Py:   ",".join(items)
来源：http://qt.9csxet.cn

PHP:  implode(",", $items);
来源：http://lm.panjiajie.cn

JS:   items.join(",")
来源：http://vn.shxzukj.cn

TS:   items.join(",")
来源：http://gt.huanxung.cn

Java: String.join(",", items)
来源：http://lp.nicolike.cn

Go:   strings.Join(items, ",")
来源：http://qy.haigaiapp.cn

Ruby: items.join(",")
来源：http://wg.panjiajie.cn

C#:   string.Join(",", items)
来源：http://zj.9csxet.cn

[E09] 去除所有空白字符
来源：http://gp.jctech888.com.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jr.yuexingan06.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hu.521024.cn

JS:   s.replace(/\s+/g, "")
来源：http://rm.muxihuayi.cn

TS:   s.replace(/\s+/g, "")
来源：http://ug.haigaiapp.cn

Java: s.replaceAll("\\s+", "")
来源：http://uy.shxzukj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://to.jianghongdianzi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://id.asd995.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mk.hahajie.cn

[E10] 左侧补零 / 定长填充
来源：http://hk.newstarts.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ao.huixinmuqiang.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://za.lnxyls.cn

JS:   "7".padStart(3, "0")
来源：http://ux.muxihuayi.cn

TS:   "7".padStart(3, "0")
来源：http://in.yuntaijiaju.cn

Java: String.format("%03d", 7)
来源：http://fd.lnxyls.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://mr.haigaiapp.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vk.gzmigu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zq.szxytkj.cn

[E11] 反转字符串
来源：http://ua.wgjwhj.cn

Py:   s[::-1]
来源：http://ss.lnxyls.cn

PHP:  strrev($s);
来源：http://hy.yuntaijiaju.cn

JS:   [...s].reverse().join("")
来源：http://ex.huixiangedu.cn

TS:   [...s].reverse().join("")
来源：http://iq.nszjky.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://jr.asd995.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://zk.bjjhwx.cn

Ruby: s.reverse
来源：http://oe.panjiajie.cn

C#:   new string(s.Reverse().ToArray())
来源：http://lv.gzmigu.cn

[E12] 统计某字符出现次数
来源：http://ez.hahajie.cn

Py:   s.count("a")
来源：http://mu.newstarts.cn

PHP:  substr_count($s, "a");
来源：http://yl.yuntaijiaju.cn

JS:   s.split("a").length - 1
来源：http://vw.asd995.cn

TS:   s.split("a").length - 1
来源：http://qp.hnjuh.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yf.bjjhwx.cn

Go:   strings.Count(s, "a")
来源：http://xa.huanxung.cn

Ruby: s.count("a")
来源：http://ur.szxytkj.cn

C#:   s.Count(c => c == 'a')
来源：http://jg.haigaiapp.cn

[E13] 逐字符遍历
来源：http://ky.yuntaijiaju.cn

Py:   for ch in s: print(ch)
来源：http://td.colortex.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ad.haigaiapp.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://xz.bjjhwx.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ef.newstarts.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://si.jctech888.com.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ts.chemitech.net.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://uq.shxzukj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ob.shtwfgs.cn

[E14] URL 编码与 Base64
来源：http://ny.521024.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wz.521024.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://tw.asd995.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://uw.nszjky.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://yi.shxzskj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ec.haigaiapp.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ph.nszjky.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://sf.521024.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wk.bjjhwx.cn

[E15] HTML 转义 / 反转义
来源：http://rb.szxytkj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://gv.wgjwhj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fr.szsharing.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ys.wgjwhj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://dk.gzmigu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rn.wgjwhj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mo.521024.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xs.huanxung.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ct.jctech888.com.cn

[E16] 数字千分位
来源：http://qg.szxytkj.cn

Py:   f"{1234567:,}"
来源：http://wk.huixinmuqiang.cn

PHP:  number_format(1234567);
来源：http://ok.szsharing.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://cd.9csxet.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://cr.jianghongdianzi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wu.huixiangedu.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://gp.yuexingan06.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fe.hahajie.cn

C#:   1234567.ToString("N0")
来源：http://nj.newstarts.cn

[E17] 首字母大写
来源：http://bd.huixinmuqiang.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://sc.huanxung.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://zd.colortex.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ch.szsharing.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://od.521024.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jq.shxzukj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qt.bjjhwx.cn

Ruby: s.capitalize
来源：http://fn.jctech888.com.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ae.hnjuh.cn

[E18] 模板占位符替换
来源：http://aa.jianghongdianzi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hk.szxytkj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://el.jctech888.com.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://mk.jianghongdianzi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://nm.colortex.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lm.muxihuayi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qg.colortex.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ga.shxzukj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bv.nicolike.cn

[E19] 多行文本按行拆分
来源：http://vm.shxzukj.cn

Py:   s.splitlines()
来源：http://eq.yuntaijiaju.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qv.shtwfgs.cn


<!-- 参考信息 -->