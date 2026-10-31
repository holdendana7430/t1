代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://js.gzmigu.cn

Ruby: arr.sort
来源：http://ij.huixinmuqiang.cn

C#:   list.Sort();
来源：http://ge.jctech888.com.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://hm.jianghongdianzi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://bw.huixinmuqiang.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://br.chemitech.net.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gw.hahajie.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ir.muxihuayi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xx.bjjhwx.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://te.yuntaijiaju.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cx.hnjuh.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ba.nicolike.cn

[D11] 反转数组
来源：http://ec.chemitech.net.cn

Py:   arr[::-1];  arr.reverse()
来源：http://sy.jctech888.com.cn

PHP:  array_reverse($arr);
来源：http://je.yuntaijiaju.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ha.haigaiapp.cn

TS:   [...arr].reverse();
来源：http://xo.newstarts.cn

Java: Collections.reverse(list);
来源：http://br.shxzukj.cn

Go:   slices.Reverse(arr)
来源：http://sb.shxzskj.cn

Ruby: arr.reverse
来源：http://ak.colortex.cn

C#:   list.Reverse();
来源：http://su.wgjwhj.cn

[D12] 查找元素下标
来源：http://nz.521024.cn

Py:   arr.index(x);  x in arr
来源：http://mx.chemitech.net.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hi.huixiangedu.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://je.bookmarksfly.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qh.bjjhwx.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://py.nszjky.cn

Go:   slices.Index(arr, x)
来源：http://nn.yuntaijiaju.cn

Ruby: arr.index(x)
来源：http://oc.yuexingan06.cn

C#:   list.IndexOf(x);
来源：http://cd.bjjhwx.cn

[D13] 过滤（保留满足条件的）
来源：http://js.newstarts.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wk.9csxet.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://nq.huanxung.cn

JS:   arr.filter(x => x > 3)
来源：http://yu.nicolike.cn

TS:   arr.filter(x => x > 3)
来源：http://gq.yuexingan06.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ok.szxytkj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://sw.gzmigu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://yj.nicolike.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://hr.szsharing.cn

[D14] 映射转换（每个元素变形）
来源：http://pq.panjiajie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xi.jianghongdianzi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ak.9csxet.cn

JS:   arr.map(x => x * 2)
来源：http://hs.bookmarksfly.cn

TS:   arr.map(x => x * 2)
来源：http://hw.lnxyls.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://fe.nszjky.cn

Go:   // 手写循环
来源：http://at.haigaiapp.cn

Ruby: arr.map { |x| x * 2 }
来源：http://lp.panjiajie.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://pl.colortex.cn

[D15] 去重
来源：http://sb.jianghongdianzi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://do.hnjuh.cn

PHP:  array_unique($arr);
来源：http://fm.huixinmuqiang.cn

JS:   [...new Set(arr)]
来源：http://sv.nszjky.cn

TS:   [...new Set(arr)]
来源：http://jl.shxzukj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ge.9csxet.cn

Go:   // 用 map[T]struct{} 手写
来源：http://te.szxytkj.cn

Ruby: arr.uniq
来源：http://ly.newstarts.cn

C#:   list.Distinct().ToList()
来源：http://ok.bjjhwx.cn

[D16] 求和与平均值
来源：http://uq.bjjhwx.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://uz.hnjuh.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://my.huixiangedu.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://au.wgjwhj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zi.yuexingan06.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ca.nszjky.cn

Go:   // 手写循环累加
来源：http://el.chemitech.net.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gu.wgjwhj.cn

C#:   list.Sum();  list.Average()
来源：http://qk.huixinmuqiang.cn

[D17] 最大值与最小值
来源：http://ct.hnjuh.cn

Py:   max(arr);  min(arr)
来源：http://mj.newstarts.cn

PHP:  max($arr);  min($arr);
来源：http://vd.jianghongdianzi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ud.shxzskj.cn

TS:   Math.max(...arr);
来源：http://rq.huixinmuqiang.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://bp.szsharing.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nr.hnjuh.cn

Ruby: arr.max;  arr.min
来源：http://yv.bjjhwx.cn

C#:   list.Max();  list.Min()
来源：http://lc.huixiangedu.cn

[D18] 扁平化嵌套数组
来源：http://gt.newstarts.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://yw.521024.cn

PHP:  array_merge(...$nested);
来源：http://zc.szxytkj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kv.hnjuh.cn

TS:   nested.flat();
来源：http://gk.nszjky.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fg.newstarts.cn

Go:   // 手写双层循环
来源：http://ya.gzmigu.cn

Ruby: nested.flatten
来源：http://fo.lnxyls.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ji.haigaiapp.cn

[D19] 按字段分组
来源：http://ru.chemitech.net.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://sq.wgjwhj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dl.9csxet.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tz.panjiajie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://is.panjiajie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jb.shxzskj.cn

Go:   // 手写 map[string][]T
来源：http://fy.hahajie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ws.wgjwhj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://eu.bjjhwx.cn

[D20] 统计每个元素出现次数
来源：http://yz.haigaiapp.cn

Py:   Counter(arr)
来源：http://yt.nicolike.cn

PHP:  array_count_values($arr);
来源：http://jo.hnjuh.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bq.bjjhwx.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zc.gzmigu.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ia.bookmarksfly.cn

Go:   // 手写 map[T]int
来源：http://rx.huanxung.cn

Ruby: arr.tally
来源：http://wz.jctech888.com.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://pn.haigaiapp.cn

[D21] 判断是否包含某元素
来源：http://xo.panjiajie.cn

Py:   x in arr
来源：http://hz.nszjky.cn

PHP:  in_array($x, $arr, true);
来源：http://ad.jianghongdianzi.cn

JS:   arr.includes(x)
来源：http://qg.hnjuh.cn

TS:   arr.includes(x)
来源：http://ov.521024.cn

Java: list.contains(x)
来源：http://ew.panjiajie.cn

Go:   slices.Contains(arr, x)
来源：http://xl.newstarts.cn

Ruby: arr.include?(x)
来源：http://ck.bookmarksfly.cn

C#:   list.Contains(x)
来源：http://vb.colortex.cn

[D22] 复制数组（避免共享引用）
来源：http://ur.shxzukj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ar.szsharing.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vj.jianghongdianzi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xr.huixiangedu.cn

TS:   [...arr];
来源：http://de.bjjhwx.cn

Java: new ArrayList<>(list);
来源：http://rt.panjiajie.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ur.szsharing.cn

Ruby: arr.dup;  arr.clone
来源：http://jh.bjjhwx.cn

C#:   new List<int>(list);
来源：http://xm.shxzskj.cn

[D23] reduce 累积计算
来源：http://fo.nicolike.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hu.szxytkj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://uu.shxzukj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gk.newstarts.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wd.shxzukj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://si.9csxet.cn

Go:   // 手写循环
来源：http://tw.chemitech.net.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xd.huanxung.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mc.chemitech.net.cn

[D24] 字典 / Map 基本操作
来源：http://ft.hnjuh.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://yp.nicolike.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mj.nszjky.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jo.9csxet.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bv.bjjhwx.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hc.huanxung.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vd.asd995.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://tn.wgjwhj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://uv.panjiajie.cn

[D25] Set 集合去重与交并差
来源：http://ke.huixinmuqiang.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://iz.bjjhwx.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pi.yuexingan06.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fq.jctech888.com.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fs.gzmigu.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://gk.jianghongdianzi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ly.huanxung.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ch.bookmarksfly.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nf.huixiangedu.cn

[D26] 数组转字符串
来源：http://nu.huanxung.cn

Py:   ", ".join(map(str, arr))
来源：http://vi.asd995.cn

PHP:  implode(", ", $arr);
来源：http://mx.yuntaijiaju.cn

JS:   arr.join(", ")
来源：http://jg.nszjky.cn

TS:   arr.join(", ")
来源：http://jq.bjjhwx.cn

Java: String.join(", ", list)
来源：http://jj.shxzskj.cn

Go:   strings.Join(strs, ", ")
来源：http://hx.wgjwhj.cn

Ruby: arr.join(", ")
来源：http://iz.shxzskj.cn

C#:   string.Join(", ", list)
来源：http://wf.shxzskj.cn

================================================================================
来源：http://va.szxytkj.cn

E. 字符串处理
来源：http://ed.hnjuh.cn

================================================================================
来源：http://nv.muxihuayi.cn

[E01] 拼接字符串
来源：http://au.shtwfgs.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cc.yuntaijiaju.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jd.shxzskj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wh.nicolike.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xw.bookmarksfly.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://be.wgjwhj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ax.jianghongdianzi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vc.haigaiapp.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ok.bjjhwx.cn

[E02] 重复字符串
来源：http://cl.hahajie.cn

Py:   "ab" * 3
来源：http://ua.huanxung.cn

PHP:  str_repeat("ab", 3);
来源：http://rr.shxzukj.cn

JS:   "ab".repeat(3)
来源：http://kc.bjjhwx.cn

TS:   "ab".repeat(3)
来源：http://qf.shxzskj.cn

Java: "ab".repeat(3)
来源：http://xj.wgjwhj.cn

Go:   strings.Repeat("ab", 3)
来源：http://nz.szxytkj.cn

Ruby: "ab" * 3
来源：http://rn.panjiajie.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hd.nszjky.cn

[E03] 截取子串
来源：http://wx.haigaiapp.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ap.newstarts.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vu.yuntaijiaju.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dg.panjiajie.cn

TS:   s.slice(1, 4)
来源：http://vy.gzmigu.cn

Java: s.substring(1, 4)
来源：http://xr.jctech888.com.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://yg.asd995.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ef.shtwfgs.cn

C#:   s.Substring(1, 3)
来源：http://ab.haigaiapp.cn

[E04] 查找子串位置
来源：http://ic.huixiangedu.cn

Py:   s.find("x");  s.index("x")
来源：http://in.yuntaijiaju.cn

PHP:  strpos($s, "x");
来源：http://uv.haigaiapp.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://az.panjiajie.cn

TS:   s.indexOf("x")
来源：http://va.huixiangedu.cn

Java: s.indexOf("x")
来源：http://mw.szxytkj.cn

Go:   strings.Index(s, "x")
来源：http://tw.panjiajie.cn

Ruby: s.index("x")
来源：http://qu.huixinmuqiang.cn

C#:   s.IndexOf("x")
来源：http://ct.szsharing.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://zh.huanxung.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gt.colortex.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mt.nszjky.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bk.asd995.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://xr.bookmarksfly.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zy.jctech888.com.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://km.colortex.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://cf.muxihuayi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://sk.huanxung.cn

[E06] 替换子串
来源：http://og.hnjuh.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://js.nszjky.cn

PHP:  str_replace("a", "b", $s);
来源：http://or.gzmigu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bn.nicolike.cn

TS:   s.replaceAll("a", "b")
来源：http://ja.bookmarksfly.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dz.bjjhwx.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://to.wgjwhj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://po.bjjhwx.cn

C#:   s.Replace("a", "b")
来源：http://fv.nicolike.cn

[E07] 按分隔符拆分
来源：http://tf.521024.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mr.bookmarksfly.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://lf.asd995.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://rz.panjiajie.cn

TS:   s.split(",")
来源：http://vx.shtwfgs.cn

Java: s.split(",");  s.split("\\s+")
来源：http://kg.wgjwhj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ca.shtwfgs.cn

Ruby: s.split(",");  s.split
来源：http://eh.colortex.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pi.muxihuayi.cn

[E08] 数组按分隔符合并
来源：http://yz.521024.cn

Py:   ",".join(items)
来源：http://dx.jianghongdianzi.cn

PHP:  implode(",", $items);
来源：http://jb.wgjwhj.cn

JS:   items.join(",")
来源：http://ar.lnxyls.cn

TS:   items.join(",")
来源：http://sa.muxihuayi.cn

Java: String.join(",", items)
来源：http://ue.panjiajie.cn

Go:   strings.Join(items, ",")
来源：http://az.yuexingan06.cn

Ruby: items.join(",")
来源：http://lb.yuntaijiaju.cn

C#:   string.Join(",", items)
来源：http://ys.asd995.cn

[E09] 去除所有空白字符
来源：http://yf.gzmigu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ty.newstarts.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wf.shtwfgs.cn

JS:   s.replace(/\s+/g, "")
来源：http://nx.gzmigu.cn

TS:   s.replace(/\s+/g, "")
来源：http://sl.lnxyls.cn

Java: s.replaceAll("\\s+", "")
来源：http://ca.huanxung.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://tt.colortex.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ik.yuexingan06.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qd.szxytkj.cn

[E10] 左侧补零 / 定长填充
来源：http://gs.huixinmuqiang.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://km.bookmarksfly.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://po.nszjky.cn

JS:   "7".padStart(3, "0")
来源：http://ve.chemitech.net.cn

TS:   "7".padStart(3, "0")
来源：http://uo.hahajie.cn

Java: String.format("%03d", 7)
来源：http://gl.asd995.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://iq.newstarts.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zm.521024.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kv.nszjky.cn

[E11] 反转字符串
来源：http://yh.huixinmuqiang.cn

Py:   s[::-1]
来源：http://rw.wgjwhj.cn

PHP:  strrev($s);
来源：http://fw.hahajie.cn

JS:   [...s].reverse().join("")
来源：http://fh.hnjuh.cn

TS:   [...s].reverse().join("")
来源：http://uj.lnxyls.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://un.yuntaijiaju.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://hp.yuntaijiaju.cn

Ruby: s.reverse
来源：http://ig.lnxyls.cn

C#:   new string(s.Reverse().ToArray())
来源：http://qc.huanxung.cn

[E12] 统计某字符出现次数
来源：http://nj.asd995.cn

Py:   s.count("a")
来源：http://ml.jianghongdianzi.cn

PHP:  substr_count($s, "a");
来源：http://rs.shxzskj.cn

JS:   s.split("a").length - 1
来源：http://gq.lnxyls.cn

TS:   s.split("a").length - 1
来源：http://wf.gzmigu.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://pl.bjjhwx.cn

Go:   strings.Count(s, "a")
来源：http://jw.colortex.cn

Ruby: s.count("a")
来源：http://rn.haigaiapp.cn

C#:   s.Count(c => c == 'a')
来源：http://ft.jctech888.com.cn

[E13] 逐字符遍历
来源：http://dy.nicolike.cn

Py:   for ch in s: print(ch)
来源：http://ge.shxzskj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rz.shtwfgs.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://gd.shtwfgs.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://zc.shxzukj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://yq.hahajie.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gt.nszjky.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ie.asd995.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://rw.muxihuayi.cn

[E14] URL 编码与 Base64
来源：http://pc.muxihuayi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ig.newstarts.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://en.lnxyls.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bs.chemitech.net.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ej.gzmigu.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jf.huixiangedu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://un.panjiajie.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bf.nszjky.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bv.newstarts.cn

[E15] HTML 转义 / 反转义
来源：http://xn.szxytkj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://lm.yuexingan06.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ah.szsharing.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vf.shxzukj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://gc.haigaiapp.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://nn.haigaiapp.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ow.521024.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://kl.chemitech.net.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hs.nicolike.cn

[E16] 数字千分位
来源：http://ib.gzmigu.cn

Py:   f"{1234567:,}"
来源：http://un.jianghongdianzi.cn

PHP:  number_format(1234567);
来源：http://gn.bookmarksfly.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://xh.chemitech.net.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://xe.shtwfgs.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bt.colortex.cn


<!-- 参考信息 -->