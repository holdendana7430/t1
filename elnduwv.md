代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://be.colortex.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ud.huixinmuqiang.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hk.bookmarksfly.cn

Go:   slices.Index(arr, x)
来源：http://vq.shxzskj.cn

Ruby: arr.index(x)
来源：http://ut.jctech888.com.cn

C#:   list.IndexOf(x);
来源：http://cx.haigaiapp.cn

[D13] 过滤（保留满足条件的）
来源：http://ri.asd995.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cp.yuntaijiaju.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://su.shxzskj.cn

JS:   arr.filter(x => x > 3)
来源：http://lu.muxihuayi.cn

TS:   arr.filter(x => x > 3)
来源：http://hy.shxzskj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://cy.jianghongdianzi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://pi.nicolike.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ec.nszjky.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://hm.bjjhwx.cn

[D14] 映射转换（每个元素变形）
来源：http://lm.wgjwhj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ix.colortex.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ls.gzmigu.cn

JS:   arr.map(x => x * 2)
来源：http://yv.521024.cn

TS:   arr.map(x => x * 2)
来源：http://hu.jianghongdianzi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ik.jianghongdianzi.cn

Go:   // 手写循环
来源：http://qy.hahajie.cn

Ruby: arr.map { |x| x * 2 }
来源：http://el.asd995.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ld.hahajie.cn

[D15] 去重
来源：http://dn.shtwfgs.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zr.hahajie.cn

PHP:  array_unique($arr);
来源：http://cv.wgjwhj.cn

JS:   [...new Set(arr)]
来源：http://ze.yuntaijiaju.cn

TS:   [...new Set(arr)]
来源：http://pu.9csxet.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://df.muxihuayi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ue.yuntaijiaju.cn

Ruby: arr.uniq
来源：http://nk.bjjhwx.cn

C#:   list.Distinct().ToList()
来源：http://ve.jianghongdianzi.cn

[D16] 求和与平均值
来源：http://eq.521024.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wu.521024.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ep.newstarts.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bs.9csxet.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://pi.huanxung.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zc.jctech888.com.cn

Go:   // 手写循环累加
来源：http://qt.wgjwhj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hm.haigaiapp.cn

C#:   list.Sum();  list.Average()
来源：http://iz.panjiajie.cn

[D17] 最大值与最小值
来源：http://sd.colortex.cn

Py:   max(arr);  min(arr)
来源：http://ak.hahajie.cn

PHP:  max($arr);  min($arr);
来源：http://pk.521024.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gd.asd995.cn

TS:   Math.max(...arr);
来源：http://vk.asd995.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://fb.yuexingan06.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yq.yuntaijiaju.cn

Ruby: arr.max;  arr.min
来源：http://hs.newstarts.cn

C#:   list.Max();  list.Min()
来源：http://ma.shxzskj.cn

[D18] 扁平化嵌套数组
来源：http://gk.shtwfgs.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://cd.huanxung.cn

PHP:  array_merge(...$nested);
来源：http://xi.521024.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://cz.colortex.cn

TS:   nested.flat();
来源：http://lg.chemitech.net.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fm.shxzskj.cn

Go:   // 手写双层循环
来源：http://ob.9csxet.cn

Ruby: nested.flatten
来源：http://yc.yuntaijiaju.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://hu.hahajie.cn

[D19] 按字段分组
来源：http://vj.shxzskj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ap.yuexingan06.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jn.hahajie.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lu.muxihuayi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ey.szsharing.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://uy.shxzukj.cn

Go:   // 手写 map[string][]T
来源：http://ry.hahajie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://bi.jctech888.com.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rt.wgjwhj.cn

[D20] 统计每个元素出现次数
来源：http://ve.huanxung.cn

Py:   Counter(arr)
来源：http://wp.huanxung.cn

PHP:  array_count_values($arr);
来源：http://be.hahajie.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ip.szsharing.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pb.hahajie.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://uu.shtwfgs.cn

Go:   // 手写 map[T]int
来源：http://jv.colortex.cn

Ruby: arr.tally
来源：http://ml.gzmigu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ph.9csxet.cn

[D21] 判断是否包含某元素
来源：http://nv.shxzukj.cn

Py:   x in arr
来源：http://ke.yuntaijiaju.cn

PHP:  in_array($x, $arr, true);
来源：http://aj.shxzukj.cn

JS:   arr.includes(x)
来源：http://fr.bookmarksfly.cn

TS:   arr.includes(x)
来源：http://ee.huanxung.cn

Java: list.contains(x)
来源：http://po.chemitech.net.cn

Go:   slices.Contains(arr, x)
来源：http://fn.bookmarksfly.cn

Ruby: arr.include?(x)
来源：http://ra.hahajie.cn

C#:   list.Contains(x)
来源：http://fq.chemitech.net.cn

[D22] 复制数组（避免共享引用）
来源：http://li.gzmigu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ll.shxzukj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ip.shxzukj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bb.jianghongdianzi.cn

TS:   [...arr];
来源：http://dr.hahajie.cn

Java: new ArrayList<>(list);
来源：http://sd.shtwfgs.cn

Go:   copied := append([]int(nil), arr...)
来源：http://by.nicolike.cn

Ruby: arr.dup;  arr.clone
来源：http://nt.lnxyls.cn

C#:   new List<int>(list);
来源：http://pc.wgjwhj.cn

[D23] reduce 累积计算
来源：http://fk.newstarts.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rq.shtwfgs.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wn.chemitech.net.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://im.jctech888.com.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yc.shxzskj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://rt.haigaiapp.cn

Go:   // 手写循环
来源：http://ue.asd995.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lq.521024.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://vg.szsharing.cn

[D24] 字典 / Map 基本操作
来源：http://ia.shtwfgs.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gl.hahajie.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bm.yuexingan06.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fd.szsharing.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ag.lnxyls.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hh.chemitech.net.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qm.huixiangedu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rz.521024.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ve.nszjky.cn

[D25] Set 集合去重与交并差
来源：http://hc.nicolike.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tr.asd995.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://et.bjjhwx.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://yp.panjiajie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ed.newstarts.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xy.haigaiapp.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ln.hahajie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://sl.muxihuayi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wv.hnjuh.cn

[D26] 数组转字符串
来源：http://ii.shxzskj.cn

Py:   ", ".join(map(str, arr))
来源：http://ch.yuexingan06.cn

PHP:  implode(", ", $arr);
来源：http://sc.panjiajie.cn

JS:   arr.join(", ")
来源：http://lb.521024.cn

TS:   arr.join(", ")
来源：http://pz.haigaiapp.cn

Java: String.join(", ", list)
来源：http://rl.9csxet.cn

Go:   strings.Join(strs, ", ")
来源：http://hs.wgjwhj.cn

Ruby: arr.join(", ")
来源：http://ug.jianghongdianzi.cn

C#:   string.Join(", ", list)
来源：http://rh.haigaiapp.cn

================================================================================
来源：http://zm.yuexingan06.cn

E. 字符串处理
来源：http://kj.jctech888.com.cn

================================================================================
来源：http://ij.yuexingan06.cn

[E01] 拼接字符串
来源：http://qv.jianghongdianzi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zh.muxihuayi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vh.chemitech.net.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vx.jctech888.com.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hb.bookmarksfly.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xx.szsharing.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tp.nszjky.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ei.szxytkj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fm.muxihuayi.cn

[E02] 重复字符串
来源：http://fx.huixiangedu.cn

Py:   "ab" * 3
来源：http://vs.huanxung.cn

PHP:  str_repeat("ab", 3);
来源：http://xc.newstarts.cn

JS:   "ab".repeat(3)
来源：http://ei.9csxet.cn

TS:   "ab".repeat(3)
来源：http://se.szsharing.cn

Java: "ab".repeat(3)
来源：http://cs.panjiajie.cn

Go:   strings.Repeat("ab", 3)
来源：http://km.bookmarksfly.cn

Ruby: "ab" * 3
来源：http://al.lnxyls.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jz.muxihuayi.cn

[E03] 截取子串
来源：http://hr.521024.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ye.shxzukj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ut.newstarts.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://px.szsharing.cn

TS:   s.slice(1, 4)
来源：http://gr.wgjwhj.cn

Java: s.substring(1, 4)
来源：http://te.wgjwhj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ib.hnjuh.cn

Ruby: s[1, 3];  s[1..3]
来源：http://qk.yuntaijiaju.cn

C#:   s.Substring(1, 3)
来源：http://tg.panjiajie.cn

[E04] 查找子串位置
来源：http://qa.shtwfgs.cn

Py:   s.find("x");  s.index("x")
来源：http://wk.yuntaijiaju.cn

PHP:  strpos($s, "x");
来源：http://ib.szxytkj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tl.haigaiapp.cn

TS:   s.indexOf("x")
来源：http://kt.yuntaijiaju.cn

Java: s.indexOf("x")
来源：http://gp.521024.cn

Go:   strings.Index(s, "x")
来源：http://mg.asd995.cn

Ruby: s.index("x")
来源：http://hq.colortex.cn

C#:   s.IndexOf("x")
来源：http://ca.jianghongdianzi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://kj.lnxyls.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://oo.yuntaijiaju.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hn.huixinmuqiang.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gp.huixinmuqiang.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://zg.chemitech.net.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vs.yuexingan06.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tp.hnjuh.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mi.panjiajie.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dm.jctech888.com.cn

[E06] 替换子串
来源：http://ve.huixinmuqiang.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zo.shxzskj.cn

PHP:  str_replace("a", "b", $s);
来源：http://rf.newstarts.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ue.shtwfgs.cn

TS:   s.replaceAll("a", "b")
来源：http://qe.jctech888.com.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pu.huixinmuqiang.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://aj.shtwfgs.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://tl.szxytkj.cn

C#:   s.Replace("a", "b")
来源：http://za.bjjhwx.cn

[E07] 按分隔符拆分
来源：http://ae.521024.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://la.bookmarksfly.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ya.hnjuh.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://af.szsharing.cn

TS:   s.split(",")
来源：http://na.muxihuayi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://cr.huixinmuqiang.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://si.haigaiapp.cn

Ruby: s.split(",");  s.split
来源：http://fd.hahajie.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xc.shxzskj.cn

[E08] 数组按分隔符合并
来源：http://us.jctech888.com.cn

Py:   ",".join(items)
来源：http://jd.jianghongdianzi.cn

PHP:  implode(",", $items);
来源：http://wn.bookmarksfly.cn

JS:   items.join(",")
来源：http://ca.bookmarksfly.cn

TS:   items.join(",")
来源：http://uk.muxihuayi.cn

Java: String.join(",", items)
来源：http://gr.panjiajie.cn

Go:   strings.Join(items, ",")
来源：http://ku.yuntaijiaju.cn

Ruby: items.join(",")
来源：http://tk.yuexingan06.cn

C#:   string.Join(",", items)
来源：http://gj.szsharing.cn

[E09] 去除所有空白字符
来源：http://qz.huixinmuqiang.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ew.9csxet.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://gy.yuntaijiaju.cn

JS:   s.replace(/\s+/g, "")
来源：http://hc.yuexingan06.cn

TS:   s.replace(/\s+/g, "")
来源：http://dh.chemitech.net.cn

Java: s.replaceAll("\\s+", "")
来源：http://li.colortex.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ys.haigaiapp.cn

Ruby: s.gsub(/\s+/, "")
来源：http://qm.9csxet.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ua.panjiajie.cn

[E10] 左侧补零 / 定长填充
来源：http://su.521024.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ai.wgjwhj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fn.nicolike.cn

JS:   "7".padStart(3, "0")
来源：http://oq.nszjky.cn

TS:   "7".padStart(3, "0")
来源：http://kr.521024.cn

Java: String.format("%03d", 7)
来源：http://bs.colortex.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://op.bjjhwx.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://sc.hnjuh.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://gz.9csxet.cn

[E11] 反转字符串
来源：http://wo.szsharing.cn

Py:   s[::-1]
来源：http://oa.shxzukj.cn

PHP:  strrev($s);
来源：http://he.bjjhwx.cn

JS:   [...s].reverse().join("")
来源：http://sr.wgjwhj.cn

TS:   [...s].reverse().join("")
来源：http://xu.wgjwhj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://us.jctech888.com.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://iz.521024.cn

Ruby: s.reverse
来源：http://ve.yuexingan06.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ss.bookmarksfly.cn

[E12] 统计某字符出现次数
来源：http://kk.panjiajie.cn

Py:   s.count("a")
来源：http://mu.shxzukj.cn

PHP:  substr_count($s, "a");
来源：http://ye.huanxung.cn

JS:   s.split("a").length - 1
来源：http://ff.panjiajie.cn

TS:   s.split("a").length - 1
来源：http://ir.nszjky.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ba.huixiangedu.cn

Go:   strings.Count(s, "a")
来源：http://xt.521024.cn

Ruby: s.count("a")
来源：http://ji.chemitech.net.cn

C#:   s.Count(c => c == 'a')
来源：http://vn.bookmarksfly.cn

[E13] 逐字符遍历
来源：http://cu.chemitech.net.cn

Py:   for ch in s: print(ch)
来源：http://av.huixiangedu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rr.szxytkj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://en.huanxung.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ox.asd995.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://sf.hahajie.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://lw.muxihuayi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://tl.haigaiapp.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ri.gzmigu.cn

[E14] URL 编码与 Base64
来源：http://re.szsharing.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kq.chemitech.net.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://st.shxzukj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://du.hnjuh.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ei.shxzskj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://uh.hnjuh.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ds.yuntaijiaju.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ad.hnjuh.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ni.nicolike.cn

[E15] HTML 转义 / 反转义
来源：http://ok.521024.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://io.9csxet.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ed.newstarts.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zr.yuntaijiaju.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://aq.9csxet.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ql.huanxung.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jz.shxzskj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jy.asd995.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://tu.521024.cn

[E16] 数字千分位
来源：http://ei.chemitech.net.cn

Py:   f"{1234567:,}"
来源：http://zh.colortex.cn

PHP:  number_format(1234567);
来源：http://wc.szsharing.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://wv.shtwfgs.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ei.chemitech.net.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://im.wgjwhj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rk.bjjhwx.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zk.szsharing.cn

C#:   1234567.ToString("N0")
来源：http://br.bookmarksfly.cn

[E17] 首字母大写
来源：http://ng.hahajie.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xg.hahajie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://kf.huixinmuqiang.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mz.hnjuh.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://io.colortex.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zs.nicolike.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://dq.gzmigu.cn

Ruby: s.capitalize
来源：http://sk.asd995.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://om.hnjuh.cn

[E18] 模板占位符替换
来源：http://bo.newstarts.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kj.huixiangedu.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://dz.huixiangedu.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://jl.huanxung.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ec.huixinmuqiang.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://us.huixinmuqiang.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://pe.bookmarksfly.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mz.szxytkj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bg.colortex.cn

[E19] 多行文本按行拆分
来源：http://vz.muxihuayi.cn

Py:   s.splitlines()
来源：http://kt.hahajie.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://da.huanxung.cn


<!-- 参考信息 -->