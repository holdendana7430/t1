代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://eu.huixiangedu.cn

Ruby: arr.sort
来源：http://mj.hahajie.cn

C#:   list.Sort();
来源：http://gj.chemitech.net.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://rc.szsharing.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://do.muxihuayi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://go.huanxung.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hh.yuexingan06.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fq.lnxyls.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mj.nszjky.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ho.shxzukj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fg.gzmigu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dj.szxytkj.cn

[D11] 反转数组
来源：http://rm.asd995.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ai.bookmarksfly.cn

PHP:  array_reverse($arr);
来源：http://xd.szxytkj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ne.huixiangedu.cn

TS:   [...arr].reverse();
来源：http://jp.hahajie.cn

Java: Collections.reverse(list);
来源：http://ly.nicolike.cn

Go:   slices.Reverse(arr)
来源：http://uu.bookmarksfly.cn

Ruby: arr.reverse
来源：http://pa.hahajie.cn

C#:   list.Reverse();
来源：http://gz.shxzskj.cn

[D12] 查找元素下标
来源：http://vs.yuntaijiaju.cn

Py:   arr.index(x);  x in arr
来源：http://wy.huanxung.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://yy.huanxung.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vl.asd995.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mh.shxzskj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cz.nicolike.cn

Go:   slices.Index(arr, x)
来源：http://pu.gzmigu.cn

Ruby: arr.index(x)
来源：http://or.colortex.cn

C#:   list.IndexOf(x);
来源：http://sc.shxzskj.cn

[D13] 过滤（保留满足条件的）
来源：http://qi.colortex.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xi.asd995.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xn.yuexingan06.cn

JS:   arr.filter(x => x > 3)
来源：http://gj.asd995.cn

TS:   arr.filter(x => x > 3)
来源：http://xd.huanxung.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://kn.newstarts.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ue.bookmarksfly.cn

Ruby: arr.select { |x| x > 3 }
来源：http://dq.wgjwhj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://sr.shtwfgs.cn

[D14] 映射转换（每个元素变形）
来源：http://jn.nszjky.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://pm.colortex.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wh.wgjwhj.cn

JS:   arr.map(x => x * 2)
来源：http://kf.jctech888.com.cn

TS:   arr.map(x => x * 2)
来源：http://zm.panjiajie.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://mj.521024.cn

Go:   // 手写循环
来源：http://dr.wgjwhj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://vv.yuexingan06.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://zx.chemitech.net.cn

[D15] 去重
来源：http://pb.lnxyls.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hs.jctech888.com.cn

PHP:  array_unique($arr);
来源：http://kc.shtwfgs.cn

JS:   [...new Set(arr)]
来源：http://lp.wgjwhj.cn

TS:   [...new Set(arr)]
来源：http://kt.huixinmuqiang.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://th.shxzukj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://hk.szsharing.cn

Ruby: arr.uniq
来源：http://pg.asd995.cn

C#:   list.Distinct().ToList()
来源：http://ns.huanxung.cn

[D16] 求和与平均值
来源：http://lx.jctech888.com.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dz.asd995.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wd.yuexingan06.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bq.shxzskj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://he.hahajie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ku.nicolike.cn

Go:   // 手写循环累加
来源：http://kv.yuntaijiaju.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vs.521024.cn

C#:   list.Sum();  list.Average()
来源：http://ob.yuexingan06.cn

[D17] 最大值与最小值
来源：http://sc.hnjuh.cn

Py:   max(arr);  min(arr)
来源：http://rf.colortex.cn

PHP:  max($arr);  min($arr);
来源：http://jh.szxytkj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zk.nicolike.cn

TS:   Math.max(...arr);
来源：http://qg.gzmigu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ij.jctech888.com.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wq.huanxung.cn

Ruby: arr.max;  arr.min
来源：http://xa.haigaiapp.cn

C#:   list.Max();  list.Min()
来源：http://qd.chemitech.net.cn

[D18] 扁平化嵌套数组
来源：http://ye.shtwfgs.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bs.huixiangedu.cn

PHP:  array_merge(...$nested);
来源：http://uh.szsharing.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xk.shtwfgs.cn

TS:   nested.flat();
来源：http://wh.yuntaijiaju.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xr.asd995.cn

Go:   // 手写双层循环
来源：http://la.chemitech.net.cn

Ruby: nested.flatten
来源：http://gl.hahajie.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://um.panjiajie.cn

[D19] 按字段分组
来源：http://zf.bookmarksfly.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ab.huixinmuqiang.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://iw.shtwfgs.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xp.chemitech.net.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://sr.jctech888.com.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://id.hnjuh.cn

Go:   // 手写 map[string][]T
来源：http://kw.newstarts.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://al.jctech888.com.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fw.jctech888.com.cn

[D20] 统计每个元素出现次数
来源：http://vj.hahajie.cn

Py:   Counter(arr)
来源：http://fo.gzmigu.cn

PHP:  array_count_values($arr);
来源：http://bd.yuexingan06.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ny.bjjhwx.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xv.521024.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rl.huixiangedu.cn

Go:   // 手写 map[T]int
来源：http://ot.huixiangedu.cn

Ruby: arr.tally
来源：http://lf.shxzskj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jk.szsharing.cn

[D21] 判断是否包含某元素
来源：http://dv.colortex.cn

Py:   x in arr
来源：http://sm.nicolike.cn

PHP:  in_array($x, $arr, true);
来源：http://kc.bookmarksfly.cn

JS:   arr.includes(x)
来源：http://zb.gzmigu.cn

TS:   arr.includes(x)
来源：http://cj.yuntaijiaju.cn

Java: list.contains(x)
来源：http://rc.nicolike.cn

Go:   slices.Contains(arr, x)
来源：http://lk.shtwfgs.cn

Ruby: arr.include?(x)
来源：http://fi.newstarts.cn

C#:   list.Contains(x)
来源：http://sn.yuntaijiaju.cn

[D22] 复制数组（避免共享引用）
来源：http://qq.jianghongdianzi.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vk.shxzskj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://su.colortex.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wo.9csxet.cn

TS:   [...arr];
来源：http://dp.jctech888.com.cn

Java: new ArrayList<>(list);
来源：http://vt.muxihuayi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://kj.lnxyls.cn

Ruby: arr.dup;  arr.clone
来源：http://at.nicolike.cn

C#:   new List<int>(list);
来源：http://ym.huixiangedu.cn

[D23] reduce 累积计算
来源：http://we.hnjuh.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ml.521024.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ma.shxzukj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uz.jianghongdianzi.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://iy.shtwfgs.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://gj.asd995.cn

Go:   // 手写循环
来源：http://yw.szxytkj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://re.hahajie.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ve.hnjuh.cn

[D24] 字典 / Map 基本操作
来源：http://lk.yuntaijiaju.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jm.9csxet.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wn.haigaiapp.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://lk.newstarts.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ug.jianghongdianzi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ya.muxihuayi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ut.haigaiapp.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://tf.nszjky.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vl.9csxet.cn

[D25] Set 集合去重与交并差
来源：http://nm.shxzskj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ew.newstarts.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ls.hnjuh.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fo.gzmigu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ef.colortex.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tl.asd995.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qg.szsharing.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xv.shxzskj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jp.panjiajie.cn

[D26] 数组转字符串
来源：http://bo.nszjky.cn

Py:   ", ".join(map(str, arr))
来源：http://gp.yuexingan06.cn

PHP:  implode(", ", $arr);
来源：http://tg.jianghongdianzi.cn

JS:   arr.join(", ")
来源：http://gv.hnjuh.cn

TS:   arr.join(", ")
来源：http://nq.haigaiapp.cn

Java: String.join(", ", list)
来源：http://yo.haigaiapp.cn

Go:   strings.Join(strs, ", ")
来源：http://if.wgjwhj.cn

Ruby: arr.join(", ")
来源：http://hr.huixiangedu.cn

C#:   string.Join(", ", list)
来源：http://nf.shtwfgs.cn

================================================================================
来源：http://ht.huanxung.cn

E. 字符串处理
来源：http://ac.asd995.cn

================================================================================
来源：http://fm.yuexingan06.cn

[E01] 拼接字符串
来源：http://tb.hahajie.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ur.nicolike.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dm.shxzskj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://kq.shxzukj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wp.shxzukj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://dv.panjiajie.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hc.jianghongdianzi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://by.521024.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://se.haigaiapp.cn

[E02] 重复字符串
来源：http://ff.panjiajie.cn

Py:   "ab" * 3
来源：http://hx.shxzskj.cn

PHP:  str_repeat("ab", 3);
来源：http://eu.yuexingan06.cn

JS:   "ab".repeat(3)
来源：http://gj.muxihuayi.cn

TS:   "ab".repeat(3)
来源：http://zw.panjiajie.cn

Java: "ab".repeat(3)
来源：http://ml.wgjwhj.cn

Go:   strings.Repeat("ab", 3)
来源：http://ge.nicolike.cn

Ruby: "ab" * 3
来源：http://ab.9csxet.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gl.lnxyls.cn

[E03] 截取子串
来源：http://zs.wgjwhj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://pn.hahajie.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://cq.nszjky.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wm.huanxung.cn

TS:   s.slice(1, 4)
来源：http://zi.nicolike.cn

Java: s.substring(1, 4)
来源：http://rr.asd995.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mr.bookmarksfly.cn

Ruby: s[1, 3];  s[1..3]
来源：http://di.chemitech.net.cn

C#:   s.Substring(1, 3)
来源：http://ah.jianghongdianzi.cn

[E04] 查找子串位置
来源：http://kq.wgjwhj.cn

Py:   s.find("x");  s.index("x")
来源：http://dx.huanxung.cn

PHP:  strpos($s, "x");
来源：http://gs.nszjky.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://pk.wgjwhj.cn

TS:   s.indexOf("x")
来源：http://fw.haigaiapp.cn

Java: s.indexOf("x")
来源：http://oh.huixiangedu.cn

Go:   strings.Index(s, "x")
来源：http://mb.bookmarksfly.cn

Ruby: s.index("x")
来源：http://re.shtwfgs.cn

C#:   s.IndexOf("x")
来源：http://fu.bjjhwx.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://gm.huanxung.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xc.gzmigu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qk.szxytkj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gt.yuexingan06.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ec.521024.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qw.jianghongdianzi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kx.nszjky.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xf.9csxet.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kq.panjiajie.cn

[E06] 替换子串
来源：http://ti.huixinmuqiang.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://lk.lnxyls.cn

PHP:  str_replace("a", "b", $s);
来源：http://ip.huanxung.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gi.nicolike.cn

TS:   s.replaceAll("a", "b")
来源：http://ma.colortex.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://eh.haigaiapp.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://uo.panjiajie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://bv.szxytkj.cn

C#:   s.Replace("a", "b")
来源：http://kf.jctech888.com.cn

[E07] 按分隔符拆分
来源：http://gg.hahajie.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://up.asd995.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://md.yuexingan06.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://px.colortex.cn

TS:   s.split(",")
来源：http://ne.nicolike.cn

Java: s.split(",");  s.split("\\s+")
来源：http://xk.szxytkj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ha.huixiangedu.cn

Ruby: s.split(",");  s.split
来源：http://xu.jctech888.com.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dl.huixiangedu.cn

[E08] 数组按分隔符合并
来源：http://eo.haigaiapp.cn

Py:   ",".join(items)
来源：http://mp.wgjwhj.cn

PHP:  implode(",", $items);
来源：http://ab.bjjhwx.cn

JS:   items.join(",")
来源：http://qt.shxzskj.cn

TS:   items.join(",")
来源：http://du.hahajie.cn

Java: String.join(",", items)
来源：http://ox.bjjhwx.cn

Go:   strings.Join(items, ",")
来源：http://cx.nicolike.cn

Ruby: items.join(",")
来源：http://su.haigaiapp.cn

C#:   string.Join(",", items)
来源：http://kv.shxzskj.cn

[E09] 去除所有空白字符
来源：http://lk.bjjhwx.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nm.haigaiapp.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://sr.hahajie.cn

JS:   s.replace(/\s+/g, "")
来源：http://ix.haigaiapp.cn

TS:   s.replace(/\s+/g, "")
来源：http://eo.hnjuh.cn

Java: s.replaceAll("\\s+", "")
来源：http://md.jctech888.com.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://oi.jctech888.com.cn

Ruby: s.gsub(/\s+/, "")
来源：http://tp.wgjwhj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://um.huixiangedu.cn

[E10] 左侧补零 / 定长填充
来源：http://uf.shxzskj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ni.szsharing.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bg.szsharing.cn

JS:   "7".padStart(3, "0")
来源：http://qm.chemitech.net.cn

TS:   "7".padStart(3, "0")
来源：http://sw.huanxung.cn

Java: String.format("%03d", 7)
来源：http://zr.bjjhwx.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://zu.huixiangedu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://cj.muxihuayi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://im.yuntaijiaju.cn

[E11] 反转字符串
来源：http://fj.newstarts.cn

Py:   s[::-1]
来源：http://ge.hahajie.cn

PHP:  strrev($s);
来源：http://mc.yuexingan06.cn

JS:   [...s].reverse().join("")
来源：http://rw.jianghongdianzi.cn

TS:   [...s].reverse().join("")
来源：http://dw.hnjuh.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://sa.wgjwhj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://si.panjiajie.cn

Ruby: s.reverse
来源：http://cn.colortex.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ut.jctech888.com.cn

[E12] 统计某字符出现次数
来源：http://bw.szsharing.cn

Py:   s.count("a")
来源：http://hx.hahajie.cn

PHP:  substr_count($s, "a");
来源：http://tr.bookmarksfly.cn

JS:   s.split("a").length - 1
来源：http://jz.panjiajie.cn

TS:   s.split("a").length - 1
来源：http://fv.wgjwhj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://aw.huixiangedu.cn

Go:   strings.Count(s, "a")
来源：http://fo.hahajie.cn

Ruby: s.count("a")
来源：http://uo.jctech888.com.cn

C#:   s.Count(c => c == 'a')
来源：http://bu.nicolike.cn

[E13] 逐字符遍历
来源：http://lp.szxytkj.cn

Py:   for ch in s: print(ch)
来源：http://co.newstarts.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vf.szsharing.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ko.shxzukj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://me.newstarts.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ot.szsharing.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vu.nszjky.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://py.colortex.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://uo.bjjhwx.cn

[E14] URL 编码与 Base64
来源：http://sd.haigaiapp.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ld.gzmigu.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://yi.colortex.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xx.szsharing.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bg.nszjky.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ak.shxzukj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qc.yuexingan06.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qn.panjiajie.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mn.asd995.cn

[E15] HTML 转义 / 反转义
来源：http://sf.yuntaijiaju.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://fe.szsharing.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ri.hnjuh.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ua.haigaiapp.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://na.shxzukj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zq.newstarts.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://kq.shtwfgs.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://sn.newstarts.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bm.nicolike.cn

[E16] 数字千分位
来源：http://lq.newstarts.cn

Py:   f"{1234567:,}"
来源：http://el.muxihuayi.cn

PHP:  number_format(1234567);
来源：http://lw.yuexingan06.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://iy.gzmigu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ao.newstarts.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://aw.colortex.cn


<!-- 参考信息 -->