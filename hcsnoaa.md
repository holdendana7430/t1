代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mm.shxzukj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sq.nszjky.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://co.chemitech.net.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hs.shxzukj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wq.shxzukj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ej.shxzukj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mq.bookmarksfly.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://pp.shtwfgs.cn

[D11] 反转数组
来源：http://ik.shxzukj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://bl.bookmarksfly.cn

PHP:  array_reverse($arr);
来源：http://cl.asd995.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xr.muxihuayi.cn

TS:   [...arr].reverse();
来源：http://ax.nszjky.cn

Java: Collections.reverse(list);
来源：http://fr.shxzskj.cn

Go:   slices.Reverse(arr)
来源：http://zm.chemitech.net.cn

Ruby: arr.reverse
来源：http://tc.yuntaijiaju.cn

C#:   list.Reverse();
来源：http://be.hahajie.cn

[D12] 查找元素下标
来源：http://rk.jianghongdianzi.cn

Py:   arr.index(x);  x in arr
来源：http://fb.jctech888.com.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lm.muxihuayi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fm.nszjky.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://do.jctech888.com.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://se.521024.cn

Go:   slices.Index(arr, x)
来源：http://kz.hnjuh.cn

Ruby: arr.index(x)
来源：http://pg.yuntaijiaju.cn

C#:   list.IndexOf(x);
来源：http://nh.jctech888.com.cn

[D13] 过滤（保留满足条件的）
来源：http://nv.nicolike.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://le.shxzskj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ig.nicolike.cn

JS:   arr.filter(x => x > 3)
来源：http://sw.shxzukj.cn

TS:   arr.filter(x => x > 3)
来源：http://rk.nszjky.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://im.shxzskj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://pj.shtwfgs.cn

Ruby: arr.select { |x| x > 3 }
来源：http://vw.szxytkj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://kz.panjiajie.cn

[D14] 映射转换（每个元素变形）
来源：http://zq.bjjhwx.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dk.bjjhwx.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ra.nicolike.cn

JS:   arr.map(x => x * 2)
来源：http://xl.yuntaijiaju.cn

TS:   arr.map(x => x * 2)
来源：http://eq.huanxung.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://qp.wgjwhj.cn

Go:   // 手写循环
来源：http://ow.nicolike.cn

Ruby: arr.map { |x| x * 2 }
来源：http://za.bookmarksfly.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://kg.chemitech.net.cn

[D15] 去重
来源：http://re.bookmarksfly.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cx.bookmarksfly.cn

PHP:  array_unique($arr);
来源：http://wg.hahajie.cn

JS:   [...new Set(arr)]
来源：http://mo.yuntaijiaju.cn

TS:   [...new Set(arr)]
来源：http://vm.9csxet.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dm.nszjky.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ox.521024.cn

Ruby: arr.uniq
来源：http://iu.gzmigu.cn

C#:   list.Distinct().ToList()
来源：http://kg.lnxyls.cn

[D16] 求和与平均值
来源：http://hh.nicolike.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mf.huanxung.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://es.lnxyls.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fk.yuexingan06.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kn.bjjhwx.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://aa.yuexingan06.cn

Go:   // 手写循环累加
来源：http://oc.haigaiapp.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qh.bjjhwx.cn

C#:   list.Sum();  list.Average()
来源：http://rd.yuexingan06.cn

[D17] 最大值与最小值
来源：http://xv.panjiajie.cn

Py:   max(arr);  min(arr)
来源：http://dn.huixinmuqiang.cn

PHP:  max($arr);  min($arr);
来源：http://cy.hnjuh.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wa.newstarts.cn

TS:   Math.max(...arr);
来源：http://hm.haigaiapp.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://tp.jctech888.com.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tg.bookmarksfly.cn

Ruby: arr.max;  arr.min
来源：http://pk.shxzukj.cn

C#:   list.Max();  list.Min()
来源：http://dt.szxytkj.cn

[D18] 扁平化嵌套数组
来源：http://nd.9csxet.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bd.hnjuh.cn

PHP:  array_merge(...$nested);
来源：http://wt.hahajie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ke.9csxet.cn

TS:   nested.flat();
来源：http://zl.521024.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vt.hnjuh.cn

Go:   // 手写双层循环
来源：http://zt.wgjwhj.cn

Ruby: nested.flatten
来源：http://gi.szxytkj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://gh.huixiangedu.cn

[D19] 按字段分组
来源：http://cu.bookmarksfly.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ro.yuexingan06.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jp.nszjky.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fg.shtwfgs.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://hm.huixiangedu.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://re.szsharing.cn

Go:   // 手写 map[string][]T
来源：http://ow.hahajie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://er.shtwfgs.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://pl.nicolike.cn

[D20] 统计每个元素出现次数
来源：http://mi.chemitech.net.cn

Py:   Counter(arr)
来源：http://wz.521024.cn

PHP:  array_count_values($arr);
来源：http://kn.521024.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dw.bjjhwx.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xm.huanxung.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://al.hahajie.cn

Go:   // 手写 map[T]int
来源：http://re.szxytkj.cn

Ruby: arr.tally
来源：http://kv.huixiangedu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jh.jctech888.com.cn

[D21] 判断是否包含某元素
来源：http://fo.asd995.cn

Py:   x in arr
来源：http://zd.lnxyls.cn

PHP:  in_array($x, $arr, true);
来源：http://hj.shtwfgs.cn

JS:   arr.includes(x)
来源：http://za.jctech888.com.cn

TS:   arr.includes(x)
来源：http://hb.yuexingan06.cn

Java: list.contains(x)
来源：http://wz.shxzskj.cn

Go:   slices.Contains(arr, x)
来源：http://jw.haigaiapp.cn

Ruby: arr.include?(x)
来源：http://fp.wgjwhj.cn

C#:   list.Contains(x)
来源：http://rj.muxihuayi.cn

[D22] 复制数组（避免共享引用）
来源：http://hj.bookmarksfly.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zu.panjiajie.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gp.panjiajie.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://tg.jctech888.com.cn

TS:   [...arr];
来源：http://yn.panjiajie.cn

Java: new ArrayList<>(list);
来源：http://ov.shtwfgs.cn

Go:   copied := append([]int(nil), arr...)
来源：http://up.yuexingan06.cn

Ruby: arr.dup;  arr.clone
来源：http://gq.shxzukj.cn

C#:   new List<int>(list);
来源：http://ht.gzmigu.cn

[D23] reduce 累积计算
来源：http://fu.wgjwhj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hg.shxzskj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ls.shxzskj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ho.jctech888.com.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kg.asd995.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://rk.colortex.cn

Go:   // 手写循环
来源：http://jf.hnjuh.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ma.shxzskj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jq.bjjhwx.cn

[D24] 字典 / Map 基本操作
来源：http://xm.jctech888.com.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://za.haigaiapp.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zo.shxzukj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xk.lnxyls.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://du.9csxet.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wo.haigaiapp.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bf.nszjky.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lx.haigaiapp.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lu.nszjky.cn

[D25] Set 集合去重与交并差
来源：http://il.bjjhwx.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qq.yuexingan06.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fq.shtwfgs.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xk.lnxyls.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://yp.huixinmuqiang.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cp.9csxet.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xg.hahajie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://oq.shtwfgs.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ef.yuexingan06.cn

[D26] 数组转字符串
来源：http://ht.panjiajie.cn

Py:   ", ".join(map(str, arr))
来源：http://ag.nszjky.cn

PHP:  implode(", ", $arr);
来源：http://wz.huanxung.cn

JS:   arr.join(", ")
来源：http://fo.nicolike.cn

TS:   arr.join(", ")
来源：http://ak.shtwfgs.cn

Java: String.join(", ", list)
来源：http://ft.chemitech.net.cn

Go:   strings.Join(strs, ", ")
来源：http://xs.nszjky.cn

Ruby: arr.join(", ")
来源：http://nz.yuntaijiaju.cn

C#:   string.Join(", ", list)
来源：http://rs.shtwfgs.cn

================================================================================
来源：http://ys.9csxet.cn

E. 字符串处理
来源：http://uu.chemitech.net.cn

================================================================================
来源：http://uw.huixinmuqiang.cn

[E01] 拼接字符串
来源：http://ca.nszjky.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wa.jctech888.com.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vy.huixiangedu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jk.newstarts.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ny.szxytkj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xx.jianghongdianzi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://if.huixiangedu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xa.huanxung.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zn.wgjwhj.cn

[E02] 重复字符串
来源：http://ld.muxihuayi.cn

Py:   "ab" * 3
来源：http://md.haigaiapp.cn

PHP:  str_repeat("ab", 3);
来源：http://ki.nicolike.cn

JS:   "ab".repeat(3)
来源：http://um.szxytkj.cn

TS:   "ab".repeat(3)
来源：http://gy.huixiangedu.cn

Java: "ab".repeat(3)
来源：http://yc.gzmigu.cn

Go:   strings.Repeat("ab", 3)
来源：http://xf.gzmigu.cn

Ruby: "ab" * 3
来源：http://su.muxihuayi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wd.9csxet.cn

[E03] 截取子串
来源：http://zp.muxihuayi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://dh.shtwfgs.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://yq.newstarts.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://my.gzmigu.cn

TS:   s.slice(1, 4)
来源：http://ah.haigaiapp.cn

Java: s.substring(1, 4)
来源：http://ru.hnjuh.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hs.hnjuh.cn

Ruby: s[1, 3];  s[1..3]
来源：http://wk.521024.cn

C#:   s.Substring(1, 3)
来源：http://dx.jctech888.com.cn

[E04] 查找子串位置
来源：http://oo.hahajie.cn

Py:   s.find("x");  s.index("x")
来源：http://fe.colortex.cn

PHP:  strpos($s, "x");
来源：http://yd.muxihuayi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mq.jianghongdianzi.cn

TS:   s.indexOf("x")
来源：http://ns.bookmarksfly.cn

Java: s.indexOf("x")
来源：http://wr.asd995.cn

Go:   strings.Index(s, "x")
来源：http://he.hahajie.cn

Ruby: s.index("x")
来源：http://qw.shxzukj.cn

C#:   s.IndexOf("x")
来源：http://bg.521024.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://bw.nszjky.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://kx.asd995.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ic.haigaiapp.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://iz.yuexingan06.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://xn.521024.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vk.huixiangedu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://yo.nszjky.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://dy.gzmigu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ra.nszjky.cn

[E06] 替换子串
来源：http://ws.huixinmuqiang.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ga.chemitech.net.cn

PHP:  str_replace("a", "b", $s);
来源：http://us.nicolike.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gp.jianghongdianzi.cn

TS:   s.replaceAll("a", "b")
来源：http://mr.bjjhwx.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ww.newstarts.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://yq.szsharing.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://cf.nicolike.cn

C#:   s.Replace("a", "b")
来源：http://gg.chemitech.net.cn

[E07] 按分隔符拆分
来源：http://xw.colortex.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wa.shxzskj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xv.lnxyls.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://bh.chemitech.net.cn

TS:   s.split(",")
来源：http://sy.shxzskj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://vq.bjjhwx.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://re.colortex.cn

Ruby: s.split(",");  s.split
来源：http://qj.szxytkj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lk.jianghongdianzi.cn

[E08] 数组按分隔符合并
来源：http://tq.wgjwhj.cn

Py:   ",".join(items)
来源：http://rv.wgjwhj.cn

PHP:  implode(",", $items);
来源：http://jl.huixinmuqiang.cn

JS:   items.join(",")
来源：http://vo.521024.cn

TS:   items.join(",")
来源：http://gl.bjjhwx.cn

Java: String.join(",", items)
来源：http://lb.shtwfgs.cn

Go:   strings.Join(items, ",")
来源：http://zk.szxytkj.cn

Ruby: items.join(",")
来源：http://ew.hahajie.cn

C#:   string.Join(",", items)
来源：http://so.huixiangedu.cn

[E09] 去除所有空白字符
来源：http://du.huixinmuqiang.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qc.chemitech.net.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ih.hnjuh.cn

JS:   s.replace(/\s+/g, "")
来源：http://kj.gzmigu.cn

TS:   s.replace(/\s+/g, "")
来源：http://um.hahajie.cn

Java: s.replaceAll("\\s+", "")
来源：http://lr.hahajie.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://gs.szxytkj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://hh.colortex.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://tj.hnjuh.cn

[E10] 左侧补零 / 定长填充
来源：http://xw.huanxung.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cn.asd995.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://dr.bookmarksfly.cn

JS:   "7".padStart(3, "0")
来源：http://qm.colortex.cn

TS:   "7".padStart(3, "0")
来源：http://py.chemitech.net.cn

Java: String.format("%03d", 7)
来源：http://lx.lnxyls.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://px.yuexingan06.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://bv.huanxung.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ok.newstarts.cn

[E11] 反转字符串
来源：http://lw.521024.cn

Py:   s[::-1]
来源：http://ua.shxzskj.cn

PHP:  strrev($s);
来源：http://wy.bjjhwx.cn

JS:   [...s].reverse().join("")
来源：http://ho.wgjwhj.cn

TS:   [...s].reverse().join("")
来源：http://wg.jianghongdianzi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://vv.shxzskj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://rj.shtwfgs.cn

Ruby: s.reverse
来源：http://os.nicolike.cn

C#:   new string(s.Reverse().ToArray())
来源：http://pi.hnjuh.cn

[E12] 统计某字符出现次数
来源：http://pc.yuexingan06.cn

Py:   s.count("a")
来源：http://fz.lnxyls.cn

PHP:  substr_count($s, "a");
来源：http://ed.chemitech.net.cn

JS:   s.split("a").length - 1
来源：http://my.panjiajie.cn

TS:   s.split("a").length - 1
来源：http://ao.lnxyls.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ir.huixiangedu.cn

Go:   strings.Count(s, "a")
来源：http://hz.muxihuayi.cn

Ruby: s.count("a")
来源：http://la.shtwfgs.cn

C#:   s.Count(c => c == 'a')
来源：http://hd.haigaiapp.cn

[E13] 逐字符遍历
来源：http://xy.9csxet.cn

Py:   for ch in s: print(ch)
来源：http://li.panjiajie.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rx.shxzskj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://tl.gzmigu.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://dd.colortex.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zt.jianghongdianzi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xl.521024.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://be.newstarts.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gl.szxytkj.cn

[E14] URL 编码与 Base64
来源：http://ph.hnjuh.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mh.huixiangedu.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://si.szxytkj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wq.yuexingan06.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://or.bjjhwx.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tb.gzmigu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://nx.wgjwhj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ze.chemitech.net.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://of.muxihuayi.cn

[E15] HTML 转义 / 反转义
来源：http://aw.szsharing.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ke.yuntaijiaju.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mj.chemitech.net.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gz.szsharing.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ru.szsharing.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ac.nszjky.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gf.nszjky.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qu.bookmarksfly.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://rz.jctech888.com.cn

[E16] 数字千分位
来源：http://dl.gzmigu.cn

Py:   f"{1234567:,}"
来源：http://vl.huixiangedu.cn

PHP:  number_format(1234567);
来源：http://rw.shxzskj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://of.bjjhwx.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://jj.colortex.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ej.jctech888.com.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ub.asd995.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fb.lnxyls.cn

C#:   1234567.ToString("N0")
来源：http://nk.lnxyls.cn

[E17] 首字母大写
来源：http://ny.shtwfgs.cn


<!-- 参考信息 -->