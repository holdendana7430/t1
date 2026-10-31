代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vk.chemitech.net.cn

JS:   arr.filter(x => x > 3)
来源：http://jh.muxihuayi.cn

TS:   arr.filter(x => x > 3)
来源：http://fd.lnxyls.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mg.hahajie.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ox.huanxung.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ku.shxzukj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ly.panjiajie.cn

[D14] 映射转换（每个元素变形）
来源：http://ex.bookmarksfly.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ct.bookmarksfly.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tf.haigaiapp.cn

JS:   arr.map(x => x * 2)
来源：http://hc.bookmarksfly.cn

TS:   arr.map(x => x * 2)
来源：http://rv.jianghongdianzi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://si.9csxet.cn

Go:   // 手写循环
来源：http://fo.jianghongdianzi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://li.jctech888.com.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://sd.hnjuh.cn

[D15] 去重
来源：http://hl.shxzskj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qr.szxytkj.cn

PHP:  array_unique($arr);
来源：http://fb.shtwfgs.cn

JS:   [...new Set(arr)]
来源：http://hk.jctech888.com.cn

TS:   [...new Set(arr)]
来源：http://ca.hahajie.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wg.asd995.cn

Go:   // 用 map[T]struct{} 手写
来源：http://kt.szxytkj.cn

Ruby: arr.uniq
来源：http://uy.nicolike.cn

C#:   list.Distinct().ToList()
来源：http://mk.hnjuh.cn

[D16] 求和与平均值
来源：http://oj.hahajie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zh.muxihuayi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://th.521024.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://tr.nszjky.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tm.shtwfgs.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xr.huanxung.cn

Go:   // 手写循环累加
来源：http://ks.colortex.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xi.chemitech.net.cn

C#:   list.Sum();  list.Average()
来源：http://lt.bookmarksfly.cn

[D17] 最大值与最小值
来源：http://ni.bjjhwx.cn

Py:   max(arr);  min(arr)
来源：http://ix.521024.cn

PHP:  max($arr);  min($arr);
来源：http://fs.panjiajie.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vx.shxzukj.cn

TS:   Math.max(...arr);
来源：http://xp.nicolike.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://mr.panjiajie.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://oz.huixiangedu.cn

Ruby: arr.max;  arr.min
来源：http://mm.huixinmuqiang.cn

C#:   list.Max();  list.Min()
来源：http://mb.huixiangedu.cn

[D18] 扁平化嵌套数组
来源：http://pq.hnjuh.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://iv.9csxet.cn

PHP:  array_merge(...$nested);
来源：http://ks.colortex.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://bi.szsharing.cn

TS:   nested.flat();
来源：http://oq.panjiajie.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://im.newstarts.cn

Go:   // 手写双层循环
来源：http://sr.hahajie.cn

Ruby: nested.flatten
来源：http://cn.521024.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://qd.asd995.cn

[D19] 按字段分组
来源：http://jz.9csxet.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://lg.nicolike.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ki.jianghongdianzi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://up.jctech888.com.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://sd.521024.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wq.haigaiapp.cn

Go:   // 手写 map[string][]T
来源：http://gj.shtwfgs.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://hq.colortex.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://on.gzmigu.cn

[D20] 统计每个元素出现次数
来源：http://ne.9csxet.cn

Py:   Counter(arr)
来源：http://mi.newstarts.cn

PHP:  array_count_values($arr);
来源：http://gk.newstarts.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://aw.szsharing.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ta.huanxung.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ow.shtwfgs.cn

Go:   // 手写 map[T]int
来源：http://be.muxihuayi.cn

Ruby: arr.tally
来源：http://wo.shxzukj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ar.huixinmuqiang.cn

[D21] 判断是否包含某元素
来源：http://lu.shxzukj.cn

Py:   x in arr
来源：http://pi.bookmarksfly.cn

PHP:  in_array($x, $arr, true);
来源：http://if.szxytkj.cn

JS:   arr.includes(x)
来源：http://nb.haigaiapp.cn

TS:   arr.includes(x)
来源：http://cu.nszjky.cn

Java: list.contains(x)
来源：http://bs.gzmigu.cn

Go:   slices.Contains(arr, x)
来源：http://ac.newstarts.cn

Ruby: arr.include?(x)
来源：http://du.huixiangedu.cn

C#:   list.Contains(x)
来源：http://jx.muxihuayi.cn

[D22] 复制数组（避免共享引用）
来源：http://mk.nszjky.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jr.asd995.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gz.yuntaijiaju.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://oj.muxihuayi.cn

TS:   [...arr];
来源：http://bg.bookmarksfly.cn

Java: new ArrayList<>(list);
来源：http://nl.haigaiapp.cn

Go:   copied := append([]int(nil), arr...)
来源：http://xl.521024.cn

Ruby: arr.dup;  arr.clone
来源：http://er.szxytkj.cn

C#:   new List<int>(list);
来源：http://dp.panjiajie.cn

[D23] reduce 累积计算
来源：http://jd.shtwfgs.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://uq.hahajie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://br.nicolike.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sx.chemitech.net.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fd.bookmarksfly.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://yi.haigaiapp.cn

Go:   // 手写循环
来源：http://tr.9csxet.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bx.9csxet.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://fq.bookmarksfly.cn

[D24] 字典 / Map 基本操作
来源：http://rl.chemitech.net.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://fe.wgjwhj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://oc.jctech888.com.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fv.wgjwhj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dc.huixinmuqiang.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wy.wgjwhj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://nw.shxzukj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ep.szsharing.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://yi.nicolike.cn

[D25] Set 集合去重与交并差
来源：http://wi.jctech888.com.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ps.hahajie.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fw.nszjky.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://td.szxytkj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qq.panjiajie.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mx.9csxet.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ix.hahajie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qy.huixinmuqiang.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fe.nszjky.cn

[D26] 数组转字符串
来源：http://uz.shxzukj.cn

Py:   ", ".join(map(str, arr))
来源：http://kf.bjjhwx.cn

PHP:  implode(", ", $arr);
来源：http://fs.asd995.cn

JS:   arr.join(", ")
来源：http://ro.muxihuayi.cn

TS:   arr.join(", ")
来源：http://vf.shxzskj.cn

Java: String.join(", ", list)
来源：http://da.jctech888.com.cn

Go:   strings.Join(strs, ", ")
来源：http://xd.bookmarksfly.cn

Ruby: arr.join(", ")
来源：http://eg.yuexingan06.cn

C#:   string.Join(", ", list)
来源：http://ow.asd995.cn

================================================================================
来源：http://uy.nicolike.cn

E. 字符串处理
来源：http://xe.colortex.cn

================================================================================
来源：http://ip.newstarts.cn

[E01] 拼接字符串
来源：http://ix.shxzskj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cg.muxihuayi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://we.muxihuayi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ij.shtwfgs.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fb.huixiangedu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ea.szxytkj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://iu.shxzskj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vi.9csxet.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qb.bookmarksfly.cn

[E02] 重复字符串
来源：http://yc.nszjky.cn

Py:   "ab" * 3
来源：http://po.bjjhwx.cn

PHP:  str_repeat("ab", 3);
来源：http://pp.asd995.cn

JS:   "ab".repeat(3)
来源：http://wj.521024.cn

TS:   "ab".repeat(3)
来源：http://fy.lnxyls.cn

Java: "ab".repeat(3)
来源：http://dm.haigaiapp.cn

Go:   strings.Repeat("ab", 3)
来源：http://og.huixinmuqiang.cn

Ruby: "ab" * 3
来源：http://dm.colortex.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ay.huixiangedu.cn

[E03] 截取子串
来源：http://bk.9csxet.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://bb.szsharing.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tt.gzmigu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://nx.521024.cn

TS:   s.slice(1, 4)
来源：http://rz.panjiajie.cn

Java: s.substring(1, 4)
来源：http://pb.gzmigu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kv.yuexingan06.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ku.huanxung.cn

C#:   s.Substring(1, 3)
来源：http://gb.huixiangedu.cn

[E04] 查找子串位置
来源：http://ko.haigaiapp.cn

Py:   s.find("x");  s.index("x")
来源：http://bv.jctech888.com.cn

PHP:  strpos($s, "x");
来源：http://jw.shxzskj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://lq.yuntaijiaju.cn

TS:   s.indexOf("x")
来源：http://os.shxzskj.cn

Java: s.indexOf("x")
来源：http://mq.hahajie.cn

Go:   strings.Index(s, "x")
来源：http://ep.chemitech.net.cn

Ruby: s.index("x")
来源：http://xq.haigaiapp.cn

C#:   s.IndexOf("x")
来源：http://zv.hahajie.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://nw.bookmarksfly.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hu.muxihuayi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://rr.hnjuh.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://na.szsharing.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://mz.shxzukj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://db.panjiajie.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hs.asd995.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pp.shxzukj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://sx.bookmarksfly.cn

[E06] 替换子串
来源：http://au.huixiangedu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://sb.hahajie.cn

PHP:  str_replace("a", "b", $s);
来源：http://xa.jctech888.com.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bv.szxytkj.cn

TS:   s.replaceAll("a", "b")
来源：http://ua.bookmarksfly.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mg.yuexingan06.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rj.shxzukj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://du.shxzskj.cn

C#:   s.Replace("a", "b")
来源：http://dz.hnjuh.cn

[E07] 按分隔符拆分
来源：http://sf.shxzskj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xx.szsharing.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gd.haigaiapp.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://qh.chemitech.net.cn

TS:   s.split(",")
来源：http://fj.lnxyls.cn

Java: s.split(",");  s.split("\\s+")
来源：http://lo.nszjky.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vd.panjiajie.cn

Ruby: s.split(",");  s.split
来源：http://tm.lnxyls.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://eo.lnxyls.cn

[E08] 数组按分隔符合并
来源：http://ht.jctech888.com.cn

Py:   ",".join(items)
来源：http://vr.bjjhwx.cn

PHP:  implode(",", $items);
来源：http://fs.lnxyls.cn

JS:   items.join(",")
来源：http://kj.newstarts.cn

TS:   items.join(",")
来源：http://gx.nszjky.cn

Java: String.join(",", items)
来源：http://dp.haigaiapp.cn

Go:   strings.Join(items, ",")
来源：http://vu.bjjhwx.cn

Ruby: items.join(",")
来源：http://du.bookmarksfly.cn

C#:   string.Join(",", items)
来源：http://xm.asd995.cn

[E09] 去除所有空白字符
来源：http://gk.wgjwhj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kp.lnxyls.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ip.jctech888.com.cn

JS:   s.replace(/\s+/g, "")
来源：http://tj.shxzukj.cn

TS:   s.replace(/\s+/g, "")
来源：http://za.bookmarksfly.cn

Java: s.replaceAll("\\s+", "")
来源：http://bx.jianghongdianzi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://rz.panjiajie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://qe.muxihuayi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rl.bookmarksfly.cn

[E10] 左侧补零 / 定长填充
来源：http://lt.lnxyls.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zb.jctech888.com.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://re.huanxung.cn

JS:   "7".padStart(3, "0")
来源：http://cf.hnjuh.cn

TS:   "7".padStart(3, "0")
来源：http://ax.haigaiapp.cn

Java: String.format("%03d", 7)
来源：http://lm.hahajie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://mk.bookmarksfly.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://me.521024.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mv.hnjuh.cn

[E11] 反转字符串
来源：http://ei.colortex.cn

Py:   s[::-1]
来源：http://vb.lnxyls.cn

PHP:  strrev($s);
来源：http://qp.yuexingan06.cn

JS:   [...s].reverse().join("")
来源：http://mz.yuntaijiaju.cn

TS:   [...s].reverse().join("")
来源：http://ai.bjjhwx.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://rx.muxihuayi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ip.panjiajie.cn

Ruby: s.reverse
来源：http://kg.huanxung.cn

C#:   new string(s.Reverse().ToArray())
来源：http://sj.shxzskj.cn

[E12] 统计某字符出现次数
来源：http://mj.yuexingan06.cn

Py:   s.count("a")
来源：http://nk.bookmarksfly.cn

PHP:  substr_count($s, "a");
来源：http://vl.shxzskj.cn

JS:   s.split("a").length - 1
来源：http://ny.szsharing.cn

TS:   s.split("a").length - 1
来源：http://dh.yuntaijiaju.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mf.newstarts.cn

Go:   strings.Count(s, "a")
来源：http://ag.521024.cn

Ruby: s.count("a")
来源：http://so.chemitech.net.cn

C#:   s.Count(c => c == 'a')
来源：http://ka.bjjhwx.cn

[E13] 逐字符遍历
来源：http://so.gzmigu.cn

Py:   for ch in s: print(ch)
来源：http://cb.nicolike.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://sh.newstarts.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://yc.gzmigu.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://wy.jianghongdianzi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ni.9csxet.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://sd.gzmigu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://xh.szsharing.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://rg.shxzukj.cn

[E14] URL 编码与 Base64
来源：http://ui.hahajie.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://dz.colortex.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://fw.shtwfgs.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://sw.muxihuayi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hk.hnjuh.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://pp.huixiangedu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hi.szsharing.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bo.huanxung.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://kq.haigaiapp.cn

[E15] HTML 转义 / 反转义
来源：http://gn.yuexingan06.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://tw.shxzukj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hs.yuntaijiaju.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wu.shxzskj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ye.panjiajie.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gm.colortex.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wb.nszjky.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ai.shxzskj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://to.jctech888.com.cn

[E16] 数字千分位
来源：http://cy.jctech888.com.cn

Py:   f"{1234567:,}"
来源：http://hi.chemitech.net.cn

PHP:  number_format(1234567);
来源：http://cu.colortex.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://wf.jianghongdianzi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ee.lnxyls.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jx.521024.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rw.shxzskj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://os.shtwfgs.cn

C#:   1234567.ToString("N0")
来源：http://rb.wgjwhj.cn

[E17] 首字母大写
来源：http://rp.nszjky.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://iv.521024.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://tq.jianghongdianzi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ea.newstarts.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yo.9csxet.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vj.nszjky.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fy.jctech888.com.cn

Ruby: s.capitalize
来源：http://ak.haigaiapp.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ev.wgjwhj.cn

[E18] 模板占位符替换
来源：http://sf.hnjuh.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kz.yuntaijiaju.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://pp.colortex.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ew.gzmigu.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://sw.jianghongdianzi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mw.panjiajie.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://sy.lnxyls.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ss.hahajie.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://aa.shxzskj.cn

[E19] 多行文本按行拆分
来源：http://ts.jctech888.com.cn

Py:   s.splitlines()
来源：http://wd.gzmigu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rx.colortex.cn

JS:   s.split(/\r?\n/)
来源：http://gw.huanxung.cn

TS:   s.split(/\r?\n/)
来源：http://hi.bjjhwx.cn

Java: s.lines().toList()
来源：http://qo.nszjky.cn

Go:   strings.Split(s, "\n")
来源：http://fe.szxytkj.cn

Ruby: s.lines
来源：http://ri.szxytkj.cn

C#:   s.Split('\n')
来源：http://qv.huanxung.cn

[E20] 判断字符串是否为空
来源：http://ka.muxihuayi.cn

Py:   if not s:
来源：http://gj.9csxet.cn


<!-- 参考信息 -->