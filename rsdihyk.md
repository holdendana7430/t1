代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://hx.nicolike.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ax.huixiangedu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://if.huixinmuqiang.cn

[D06] 数组长度
来源：http://gi.shxzukj.cn

Py:   len(arr)
来源：http://eo.panjiajie.cn

PHP:  count($arr);
来源：http://zz.yuntaijiaju.cn

JS:   arr.length
来源：http://fh.muxihuayi.cn

TS:   arr.length
来源：http://fr.jctech888.com.cn

Java: list.size();
来源：http://ou.asd995.cn

Go:   len(arr)
来源：http://fd.huanxung.cn

Ruby: arr.length; arr.size
来源：http://vn.haigaiapp.cn

C#:   list.Count;
来源：http://no.nicolike.cn

[D07] 切片 / 取子数组
来源：http://sg.szsharing.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://st.yuexingan06.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ap.chemitech.net.cn

JS:   arr.slice(1, 4);
来源：http://vv.szsharing.cn

TS:   arr.slice(1, 4);
来源：http://cr.yuexingan06.cn

Java: list.subList(1, 4);
来源：http://bi.panjiajie.cn

Go:   arr[1:4]
来源：http://nt.bookmarksfly.cn

Ruby: arr[1, 3]
来源：http://mc.bookmarksfly.cn

C#:   list.GetRange(1, 3);
来源：http://er.yuexingan06.cn

[D08] 合并两个数组
来源：http://qz.yuntaijiaju.cn

Py:   a + b;  a.extend(b)
来源：http://iz.huixinmuqiang.cn

PHP:  array_merge($a, $b);
来源：http://ld.haigaiapp.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://do.gzmigu.cn

TS:   [...a, ...b];
来源：http://iq.chemitech.net.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://eh.nszjky.cn

Go:   append(a, b...)
来源：http://dv.huixiangedu.cn

Ruby: a + b;  a.concat(b)
来源：http://hy.chemitech.net.cn

C#:   a.Concat(b).ToList()
来源：http://qj.newstarts.cn

[D09] 排序（升序）
来源：http://kr.hnjuh.cn

Py:   sorted(arr);  arr.sort()
来源：http://vc.newstarts.cn

PHP:  sort($arr);
来源：http://gz.newstarts.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://go.asd995.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://bn.szsharing.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ja.szsharing.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gn.szxytkj.cn

Ruby: arr.sort
来源：http://gw.nszjky.cn

C#:   list.Sort();
来源：http://gj.shtwfgs.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://jq.521024.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://on.szxytkj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jy.colortex.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://lf.yuexingan06.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://cn.gzmigu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://lw.shxzskj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ka.colortex.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wf.hahajie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://sk.nszjky.cn

[D11] 反转数组
来源：http://pr.yuexingan06.cn

Py:   arr[::-1];  arr.reverse()
来源：http://qo.huixinmuqiang.cn

PHP:  array_reverse($arr);
来源：http://qd.shxzskj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zi.shxzskj.cn

TS:   [...arr].reverse();
来源：http://fd.nszjky.cn

Java: Collections.reverse(list);
来源：http://ah.muxihuayi.cn

Go:   slices.Reverse(arr)
来源：http://xq.huixiangedu.cn

Ruby: arr.reverse
来源：http://ci.szsharing.cn

C#:   list.Reverse();
来源：http://jq.haigaiapp.cn

[D12] 查找元素下标
来源：http://sm.gzmigu.cn

Py:   arr.index(x);  x in arr
来源：http://ck.newstarts.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vo.chemitech.net.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zo.hnjuh.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kd.huixiangedu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://up.hahajie.cn

Go:   slices.Index(arr, x)
来源：http://by.huanxung.cn

Ruby: arr.index(x)
来源：http://po.panjiajie.cn

C#:   list.IndexOf(x);
来源：http://wg.521024.cn

[D13] 过滤（保留满足条件的）
来源：http://sq.shxzukj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bc.bookmarksfly.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://cf.szxytkj.cn

JS:   arr.filter(x => x > 3)
来源：http://nr.huanxung.cn

TS:   arr.filter(x => x > 3)
来源：http://xn.shxzukj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dr.bjjhwx.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ez.jianghongdianzi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://pb.shxzskj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://gj.bjjhwx.cn

[D14] 映射转换（每个元素变形）
来源：http://kk.yuexingan06.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xh.lnxyls.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xi.panjiajie.cn

JS:   arr.map(x => x * 2)
来源：http://ip.hnjuh.cn

TS:   arr.map(x => x * 2)
来源：http://jh.wgjwhj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://jo.shtwfgs.cn

Go:   // 手写循环
来源：http://bz.shxzskj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ot.newstarts.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ra.nszjky.cn

[D15] 去重
来源：http://kw.panjiajie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bf.jctech888.com.cn

PHP:  array_unique($arr);
来源：http://xk.lnxyls.cn

JS:   [...new Set(arr)]
来源：http://rh.nicolike.cn

TS:   [...new Set(arr)]
来源：http://er.shxzukj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jr.wgjwhj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://kz.bjjhwx.cn

Ruby: arr.uniq
来源：http://rg.haigaiapp.cn

C#:   list.Distinct().ToList()
来源：http://th.lnxyls.cn

[D16] 求和与平均值
来源：http://xv.hahajie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://se.shtwfgs.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://id.haigaiapp.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://nk.jctech888.com.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kj.jctech888.com.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fh.nszjky.cn

Go:   // 手写循环累加
来源：http://sy.newstarts.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://la.hahajie.cn

C#:   list.Sum();  list.Average()
来源：http://px.nszjky.cn

[D17] 最大值与最小值
来源：http://cq.shxzskj.cn

Py:   max(arr);  min(arr)
来源：http://vi.nicolike.cn

PHP:  max($arr);  min($arr);
来源：http://ke.shtwfgs.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xw.9csxet.cn

TS:   Math.max(...arr);
来源：http://rn.asd995.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://lh.bjjhwx.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://cy.yuexingan06.cn

Ruby: arr.max;  arr.min
来源：http://yg.shxzskj.cn

C#:   list.Max();  list.Min()
来源：http://pa.jianghongdianzi.cn

[D18] 扁平化嵌套数组
来源：http://qp.hnjuh.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pe.asd995.cn

PHP:  array_merge(...$nested);
来源：http://qh.huanxung.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://bk.9csxet.cn

TS:   nested.flat();
来源：http://wy.yuntaijiaju.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ux.szxytkj.cn

Go:   // 手写双层循环
来源：http://qf.panjiajie.cn

Ruby: nested.flatten
来源：http://uk.wgjwhj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://xf.szxytkj.cn

[D19] 按字段分组
来源：http://oj.colortex.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://yx.huixinmuqiang.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://gx.shtwfgs.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ct.nicolike.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ix.yuntaijiaju.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://pc.huixinmuqiang.cn

Go:   // 手写 map[string][]T
来源：http://gl.521024.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ml.szxytkj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nr.huixiangedu.cn

[D20] 统计每个元素出现次数
来源：http://dg.panjiajie.cn

Py:   Counter(arr)
来源：http://ok.nicolike.cn

PHP:  array_count_values($arr);
来源：http://mt.shtwfgs.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ny.colortex.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pk.shtwfgs.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://no.bjjhwx.cn

Go:   // 手写 map[T]int
来源：http://vv.szxytkj.cn

Ruby: arr.tally
来源：http://fa.szxytkj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vy.lnxyls.cn

[D21] 判断是否包含某元素
来源：http://wt.hahajie.cn

Py:   x in arr
来源：http://zk.haigaiapp.cn

PHP:  in_array($x, $arr, true);
来源：http://jm.huixinmuqiang.cn

JS:   arr.includes(x)
来源：http://rd.bookmarksfly.cn

TS:   arr.includes(x)
来源：http://wr.nszjky.cn

Java: list.contains(x)
来源：http://fv.nicolike.cn

Go:   slices.Contains(arr, x)
来源：http://kg.9csxet.cn

Ruby: arr.include?(x)
来源：http://bz.521024.cn

C#:   list.Contains(x)
来源：http://ep.asd995.cn

[D22] 复制数组（避免共享引用）
来源：http://hl.szxytkj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wh.yuntaijiaju.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://js.haigaiapp.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fe.huixiangedu.cn

TS:   [...arr];
来源：http://gi.yuntaijiaju.cn

Java: new ArrayList<>(list);
来源：http://fu.shxzukj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://vk.shxzukj.cn

Ruby: arr.dup;  arr.clone
来源：http://cf.gzmigu.cn

C#:   new List<int>(list);
来源：http://yy.huanxung.cn

[D23] reduce 累积计算
来源：http://lo.chemitech.net.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jc.haigaiapp.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ww.jctech888.com.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://no.gzmigu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://oy.colortex.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://eq.huanxung.cn

Go:   // 手写循环
来源：http://fj.bjjhwx.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gl.newstarts.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qj.shxzukj.cn

[D24] 字典 / Map 基本操作
来源：http://wv.bjjhwx.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zr.521024.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ap.colortex.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xu.wgjwhj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ab.haigaiapp.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mm.hnjuh.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://pe.lnxyls.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ar.lnxyls.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ho.jianghongdianzi.cn

[D25] Set 集合去重与交并差
来源：http://re.jianghongdianzi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://et.bjjhwx.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ju.chemitech.net.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://sf.huixinmuqiang.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://nz.haigaiapp.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tz.9csxet.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://de.nszjky.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://we.shxzskj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qq.szsharing.cn

[D26] 数组转字符串
来源：http://ww.colortex.cn

Py:   ", ".join(map(str, arr))
来源：http://ib.jianghongdianzi.cn

PHP:  implode(", ", $arr);
来源：http://qb.nicolike.cn

JS:   arr.join(", ")
来源：http://bw.yuntaijiaju.cn

TS:   arr.join(", ")
来源：http://yi.bookmarksfly.cn

Java: String.join(", ", list)
来源：http://lx.nicolike.cn

Go:   strings.Join(strs, ", ")
来源：http://or.szxytkj.cn

Ruby: arr.join(", ")
来源：http://xv.szxytkj.cn

C#:   string.Join(", ", list)
来源：http://lu.szsharing.cn

================================================================================
来源：http://vl.shtwfgs.cn

E. 字符串处理
来源：http://px.shtwfgs.cn

================================================================================
来源：http://gr.panjiajie.cn

[E01] 拼接字符串
来源：http://zp.9csxet.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ec.shtwfgs.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://su.9csxet.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dh.huixinmuqiang.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://kd.szxytkj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ii.521024.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rn.hahajie.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ej.shxzukj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vh.yuexingan06.cn

[E02] 重复字符串
来源：http://iy.haigaiapp.cn

Py:   "ab" * 3
来源：http://xc.9csxet.cn

PHP:  str_repeat("ab", 3);
来源：http://ue.haigaiapp.cn

JS:   "ab".repeat(3)
来源：http://bz.yuntaijiaju.cn

TS:   "ab".repeat(3)
来源：http://nw.szxytkj.cn

Java: "ab".repeat(3)
来源：http://we.yuntaijiaju.cn

Go:   strings.Repeat("ab", 3)
来源：http://vj.wgjwhj.cn

Ruby: "ab" * 3
来源：http://re.hnjuh.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://pj.huanxung.cn

[E03] 截取子串
来源：http://id.jctech888.com.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ho.jctech888.com.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wq.521024.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zd.newstarts.cn

TS:   s.slice(1, 4)
来源：http://tv.bookmarksfly.cn

Java: s.substring(1, 4)
来源：http://ss.lnxyls.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://il.huixinmuqiang.cn

Ruby: s[1, 3];  s[1..3]
来源：http://fu.gzmigu.cn

C#:   s.Substring(1, 3)
来源：http://qz.muxihuayi.cn

[E04] 查找子串位置
来源：http://ni.huixinmuqiang.cn

Py:   s.find("x");  s.index("x")
来源：http://yb.gzmigu.cn

PHP:  strpos($s, "x");
来源：http://rq.521024.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://oj.jctech888.com.cn

TS:   s.indexOf("x")
来源：http://rn.nicolike.cn

Java: s.indexOf("x")
来源：http://og.gzmigu.cn

Go:   strings.Index(s, "x")
来源：http://jw.jctech888.com.cn

Ruby: s.index("x")
来源：http://bi.yuexingan06.cn

C#:   s.IndexOf("x")
来源：http://rv.521024.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://du.hnjuh.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fq.9csxet.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hk.newstarts.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fn.hahajie.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ve.muxihuayi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bs.muxihuayi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fc.asd995.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ps.hahajie.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://je.hnjuh.cn

[E06] 替换子串
来源：http://bx.haigaiapp.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jk.huixiangedu.cn

PHP:  str_replace("a", "b", $s);
来源：http://fk.hahajie.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ft.hnjuh.cn

TS:   s.replaceAll("a", "b")
来源：http://hw.huanxung.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kz.9csxet.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ye.nicolike.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hu.szxytkj.cn

C#:   s.Replace("a", "b")
来源：http://jx.wgjwhj.cn

[E07] 按分隔符拆分
来源：http://os.jctech888.com.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://yw.szsharing.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nz.muxihuayi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://rp.521024.cn

TS:   s.split(",")
来源：http://ib.nszjky.cn

Java: s.split(",");  s.split("\\s+")
来源：http://st.szsharing.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://me.shtwfgs.cn

Ruby: s.split(",");  s.split
来源：http://pn.shxzukj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qi.bjjhwx.cn

[E08] 数组按分隔符合并
来源：http://bk.9csxet.cn

Py:   ",".join(items)
来源：http://ka.szsharing.cn

PHP:  implode(",", $items);
来源：http://nu.hnjuh.cn

JS:   items.join(",")
来源：http://tf.jianghongdianzi.cn

TS:   items.join(",")
来源：http://gd.jianghongdianzi.cn

Java: String.join(",", items)
来源：http://tm.yuntaijiaju.cn

Go:   strings.Join(items, ",")
来源：http://xm.shxzukj.cn

Ruby: items.join(",")
来源：http://pq.hnjuh.cn

C#:   string.Join(",", items)
来源：http://fb.huixinmuqiang.cn

[E09] 去除所有空白字符
来源：http://uj.szsharing.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qs.521024.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ov.yuexingan06.cn

JS:   s.replace(/\s+/g, "")
来源：http://kj.jctech888.com.cn

TS:   s.replace(/\s+/g, "")
来源：http://qi.gzmigu.cn

Java: s.replaceAll("\\s+", "")
来源：http://xj.huixinmuqiang.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://uk.szxytkj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ou.shxzukj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xp.yuexingan06.cn

[E10] 左侧补零 / 定长填充
来源：http://vl.nszjky.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fn.yuntaijiaju.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xg.asd995.cn

JS:   "7".padStart(3, "0")
来源：http://ph.gzmigu.cn

TS:   "7".padStart(3, "0")
来源：http://cs.nicolike.cn

Java: String.format("%03d", 7)
来源：http://ki.bjjhwx.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://yg.hnjuh.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://nb.nszjky.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://nd.szsharing.cn

[E11] 反转字符串
来源：http://ys.muxihuayi.cn

Py:   s[::-1]
来源：http://eg.shtwfgs.cn

PHP:  strrev($s);
来源：http://qm.bjjhwx.cn

JS:   [...s].reverse().join("")
来源：http://pi.muxihuayi.cn

TS:   [...s].reverse().join("")
来源：http://op.bjjhwx.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ie.chemitech.net.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://th.asd995.cn

Ruby: s.reverse
来源：http://le.bookmarksfly.cn

C#:   new string(s.Reverse().ToArray())
来源：http://hh.yuexingan06.cn

[E12] 统计某字符出现次数
来源：http://dv.haigaiapp.cn

Py:   s.count("a")
来源：http://kr.huixinmuqiang.cn

PHP:  substr_count($s, "a");
来源：http://af.wgjwhj.cn

JS:   s.split("a").length - 1
来源：http://vw.asd995.cn

TS:   s.split("a").length - 1
来源：http://fe.shxzskj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dx.bookmarksfly.cn


<!-- 参考信息 -->