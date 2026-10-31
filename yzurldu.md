代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rz.jctech888.com.cn

Ruby: arr.select { |x| x > 3 }
来源：http://mt.huixinmuqiang.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://cv.huixinmuqiang.cn

[D14] 映射转换（每个元素变形）
来源：http://aa.chemitech.net.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xl.lnxyls.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://nd.haigaiapp.cn

JS:   arr.map(x => x * 2)
来源：http://vj.wgjwhj.cn

TS:   arr.map(x => x * 2)
来源：http://rx.muxihuayi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://vy.huixinmuqiang.cn

Go:   // 手写循环
来源：http://yp.shxzukj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://at.hnjuh.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://wx.nszjky.cn

[D15] 去重
来源：http://qj.asd995.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hb.asd995.cn

PHP:  array_unique($arr);
来源：http://uv.szxytkj.cn

JS:   [...new Set(arr)]
来源：http://kl.newstarts.cn

TS:   [...new Set(arr)]
来源：http://bz.shxzukj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qd.szxytkj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://vl.szxytkj.cn

Ruby: arr.uniq
来源：http://jy.lnxyls.cn

C#:   list.Distinct().ToList()
来源：http://bg.bjjhwx.cn

[D16] 求和与平均值
来源：http://pg.bookmarksfly.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qu.bookmarksfly.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ok.newstarts.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dx.szsharing.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qu.hahajie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gc.yuntaijiaju.cn

Go:   // 手写循环累加
来源：http://qq.yuexingan06.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nj.9csxet.cn

C#:   list.Sum();  list.Average()
来源：http://id.chemitech.net.cn

[D17] 最大值与最小值
来源：http://pv.jctech888.com.cn

Py:   max(arr);  min(arr)
来源：http://fy.jctech888.com.cn

PHP:  max($arr);  min($arr);
来源：http://tl.newstarts.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://uv.shxzukj.cn

TS:   Math.max(...arr);
来源：http://my.nicolike.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://vu.newstarts.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yn.huixiangedu.cn

Ruby: arr.max;  arr.min
来源：http://mt.bjjhwx.cn

C#:   list.Max();  list.Min()
来源：http://pj.huanxung.cn

[D18] 扁平化嵌套数组
来源：http://fe.wgjwhj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wt.huixinmuqiang.cn

PHP:  array_merge(...$nested);
来源：http://qq.nicolike.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pi.muxihuayi.cn

TS:   nested.flat();
来源：http://an.521024.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ew.huanxung.cn

Go:   // 手写双层循环
来源：http://hw.9csxet.cn

Ruby: nested.flatten
来源：http://ny.newstarts.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://mq.yuexingan06.cn

[D19] 按字段分组
来源：http://tu.jctech888.com.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rn.9csxet.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lj.jctech888.com.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jo.wgjwhj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://oh.yuexingan06.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yl.shxzskj.cn

Go:   // 手写 map[string][]T
来源：http://ul.bjjhwx.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://bw.szsharing.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://pd.jianghongdianzi.cn

[D20] 统计每个元素出现次数
来源：http://kg.haigaiapp.cn

Py:   Counter(arr)
来源：http://kv.jctech888.com.cn

PHP:  array_count_values($arr);
来源：http://zb.9csxet.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pg.huanxung.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qe.shxzukj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://eh.shxzukj.cn

Go:   // 手写 map[T]int
来源：http://iq.panjiajie.cn

Ruby: arr.tally
来源：http://ty.szsharing.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ep.haigaiapp.cn

[D21] 判断是否包含某元素
来源：http://nv.colortex.cn

Py:   x in arr
来源：http://zt.shxzskj.cn

PHP:  in_array($x, $arr, true);
来源：http://hz.shxzukj.cn

JS:   arr.includes(x)
来源：http://eh.lnxyls.cn

TS:   arr.includes(x)
来源：http://oj.hnjuh.cn

Java: list.contains(x)
来源：http://ag.521024.cn

Go:   slices.Contains(arr, x)
来源：http://sn.hnjuh.cn

Ruby: arr.include?(x)
来源：http://tp.colortex.cn

C#:   list.Contains(x)
来源：http://el.shxzskj.cn

[D22] 复制数组（避免共享引用）
来源：http://vo.huixiangedu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://be.lnxyls.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zc.shtwfgs.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ls.huanxung.cn

TS:   [...arr];
来源：http://jy.colortex.cn

Java: new ArrayList<>(list);
来源：http://pi.huixinmuqiang.cn

Go:   copied := append([]int(nil), arr...)
来源：http://qw.szxytkj.cn

Ruby: arr.dup;  arr.clone
来源：http://zr.haigaiapp.cn

C#:   new List<int>(list);
来源：http://aa.9csxet.cn

[D23] reduce 累积计算
来源：http://ys.huixiangedu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ky.colortex.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wh.colortex.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mp.jctech888.com.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cp.szsharing.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://jw.wgjwhj.cn

Go:   // 手写循环
来源：http://xb.shxzskj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://uc.chemitech.net.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hu.yuexingan06.cn

[D24] 字典 / Map 基本操作
来源：http://yz.gzmigu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://lj.huixiangedu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pd.panjiajie.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://nt.nicolike.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xk.shtwfgs.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ge.shxzukj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qw.bookmarksfly.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rb.haigaiapp.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zu.shxzukj.cn

[D25] Set 集合去重与交并差
来源：http://cn.lnxyls.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://re.shtwfgs.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ij.muxihuayi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://cq.gzmigu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://js.newstarts.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jl.yuexingan06.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jj.yuntaijiaju.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ko.bookmarksfly.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ao.bjjhwx.cn

[D26] 数组转字符串
来源：http://vo.szsharing.cn

Py:   ", ".join(map(str, arr))
来源：http://cl.yuntaijiaju.cn

PHP:  implode(", ", $arr);
来源：http://ti.wgjwhj.cn

JS:   arr.join(", ")
来源：http://hk.huixiangedu.cn

TS:   arr.join(", ")
来源：http://kp.huixinmuqiang.cn

Java: String.join(", ", list)
来源：http://wb.huixiangedu.cn

Go:   strings.Join(strs, ", ")
来源：http://nt.hnjuh.cn

Ruby: arr.join(", ")
来源：http://wv.shxzukj.cn

C#:   string.Join(", ", list)
来源：http://na.yuntaijiaju.cn

================================================================================
来源：http://di.panjiajie.cn

E. 字符串处理
来源：http://ue.hnjuh.cn

================================================================================
来源：http://su.jctech888.com.cn

[E01] 拼接字符串
来源：http://pt.szsharing.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qj.jianghongdianzi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://za.yuexingan06.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fx.szxytkj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://bv.jianghongdianzi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tq.hahajie.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tf.huanxung.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://sc.hnjuh.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vb.hahajie.cn

[E02] 重复字符串
来源：http://po.szxytkj.cn

Py:   "ab" * 3
来源：http://dy.haigaiapp.cn

PHP:  str_repeat("ab", 3);
来源：http://wz.haigaiapp.cn

JS:   "ab".repeat(3)
来源：http://up.shxzukj.cn

TS:   "ab".repeat(3)
来源：http://ru.9csxet.cn

Java: "ab".repeat(3)
来源：http://ll.haigaiapp.cn

Go:   strings.Repeat("ab", 3)
来源：http://fk.yuntaijiaju.cn

Ruby: "ab" * 3
来源：http://qo.newstarts.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://of.panjiajie.cn

[E03] 截取子串
来源：http://wt.hnjuh.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ar.shtwfgs.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://lb.yuexingan06.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mr.haigaiapp.cn

TS:   s.slice(1, 4)
来源：http://pm.jctech888.com.cn

Java: s.substring(1, 4)
来源：http://lf.yuexingan06.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rw.colortex.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ui.shtwfgs.cn

C#:   s.Substring(1, 3)
来源：http://kl.hnjuh.cn

[E04] 查找子串位置
来源：http://rr.panjiajie.cn

Py:   s.find("x");  s.index("x")
来源：http://rp.wgjwhj.cn

PHP:  strpos($s, "x");
来源：http://bb.bjjhwx.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://by.lnxyls.cn

TS:   s.indexOf("x")
来源：http://dr.shxzukj.cn

Java: s.indexOf("x")
来源：http://zn.jianghongdianzi.cn

Go:   strings.Index(s, "x")
来源：http://ua.muxihuayi.cn

Ruby: s.index("x")
来源：http://uy.jctech888.com.cn

C#:   s.IndexOf("x")
来源：http://uw.wgjwhj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://zk.jianghongdianzi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://pt.wgjwhj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qz.huixiangedu.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vk.asd995.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://qr.huixiangedu.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qn.colortex.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pb.asd995.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://cj.wgjwhj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zw.gzmigu.cn

[E06] 替换子串
来源：http://kl.asd995.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xi.szsharing.cn

PHP:  str_replace("a", "b", $s);
来源：http://xa.hnjuh.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jx.gzmigu.cn

TS:   s.replaceAll("a", "b")
来源：http://ql.lnxyls.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fy.shxzskj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hw.hahajie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://cm.muxihuayi.cn

C#:   s.Replace("a", "b")
来源：http://jx.huixinmuqiang.cn

[E07] 按分隔符拆分
来源：http://sk.9csxet.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://na.bjjhwx.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://lg.yuntaijiaju.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://sd.yuexingan06.cn

TS:   s.split(",")
来源：http://xw.wgjwhj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://pd.huanxung.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ke.bookmarksfly.cn

Ruby: s.split(",");  s.split
来源：http://es.shxzskj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://em.szxytkj.cn

[E08] 数组按分隔符合并
来源：http://vy.szxytkj.cn

Py:   ",".join(items)
来源：http://oh.szsharing.cn

PHP:  implode(",", $items);
来源：http://pl.colortex.cn

JS:   items.join(",")
来源：http://ew.nszjky.cn

TS:   items.join(",")
来源：http://lg.panjiajie.cn

Java: String.join(",", items)
来源：http://hm.shxzukj.cn

Go:   strings.Join(items, ",")
来源：http://xd.muxihuayi.cn

Ruby: items.join(",")
来源：http://ae.huixinmuqiang.cn

C#:   string.Join(",", items)
来源：http://ag.haigaiapp.cn

[E09] 去除所有空白字符
来源：http://en.hahajie.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xm.newstarts.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://pf.yuntaijiaju.cn

JS:   s.replace(/\s+/g, "")
来源：http://et.colortex.cn

TS:   s.replace(/\s+/g, "")
来源：http://gv.shxzukj.cn

Java: s.replaceAll("\\s+", "")
来源：http://jm.asd995.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://mt.shxzskj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://qa.jctech888.com.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lt.colortex.cn

[E10] 左侧补零 / 定长填充
来源：http://au.shxzskj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lk.newstarts.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://an.hnjuh.cn

JS:   "7".padStart(3, "0")
来源：http://cy.shxzukj.cn

TS:   "7".padStart(3, "0")
来源：http://br.colortex.cn

Java: String.format("%03d", 7)
来源：http://jz.huixinmuqiang.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://bx.bjjhwx.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wa.yuexingan06.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://au.hnjuh.cn

[E11] 反转字符串
来源：http://yi.hnjuh.cn

Py:   s[::-1]
来源：http://gr.521024.cn

PHP:  strrev($s);
来源：http://nk.shxzskj.cn

JS:   [...s].reverse().join("")
来源：http://kq.gzmigu.cn

TS:   [...s].reverse().join("")
来源：http://gp.nszjky.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ru.colortex.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://qy.bookmarksfly.cn

Ruby: s.reverse
来源：http://lw.huixiangedu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://aq.huanxung.cn

[E12] 统计某字符出现次数
来源：http://jp.9csxet.cn

Py:   s.count("a")
来源：http://ve.shxzukj.cn

PHP:  substr_count($s, "a");
来源：http://jb.bookmarksfly.cn

JS:   s.split("a").length - 1
来源：http://rk.shtwfgs.cn

TS:   s.split("a").length - 1
来源：http://yn.haigaiapp.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yl.szsharing.cn

Go:   strings.Count(s, "a")
来源：http://bg.lnxyls.cn

Ruby: s.count("a")
来源：http://vo.9csxet.cn

C#:   s.Count(c => c == 'a')
来源：http://da.shxzskj.cn

[E13] 逐字符遍历
来源：http://te.muxihuayi.cn

Py:   for ch in s: print(ch)
来源：http://nq.szsharing.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kn.9csxet.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://md.bookmarksfly.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://xb.521024.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://sp.szsharing.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hd.muxihuayi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://rh.newstarts.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ba.hahajie.cn

[E14] URL 编码与 Base64
来源：http://nn.chemitech.net.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gc.nicolike.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ds.shtwfgs.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zy.newstarts.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vg.szsharing.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wj.nszjky.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://kj.jctech888.com.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://nu.chemitech.net.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ux.yuntaijiaju.cn

[E15] HTML 转义 / 反转义
来源：http://jy.szxytkj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://bc.bjjhwx.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://sn.chemitech.net.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ts.shtwfgs.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://kz.9csxet.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ir.lnxyls.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://sf.asd995.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qe.gzmigu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fh.szsharing.cn

[E16] 数字千分位
来源：http://tl.huixinmuqiang.cn

Py:   f"{1234567:,}"
来源：http://so.jianghongdianzi.cn

PHP:  number_format(1234567);
来源：http://pf.szsharing.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://yp.newstarts.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ou.9csxet.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qm.yuntaijiaju.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://tl.asd995.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://rk.chemitech.net.cn

C#:   1234567.ToString("N0")
来源：http://su.chemitech.net.cn

[E17] 首字母大写
来源：http://rq.nszjky.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://kh.chemitech.net.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://sr.huixiangedu.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vf.gzmigu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pv.shxzukj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ib.huixinmuqiang.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://dq.szsharing.cn

Ruby: s.capitalize
来源：http://zu.nszjky.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://bw.jianghongdianzi.cn

[E18] 模板占位符替换
来源：http://vw.bjjhwx.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.haigaiapp.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mx.yuntaijiaju.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://tz.panjiajie.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://rv.haigaiapp.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pa.wgjwhj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ih.521024.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ee.bjjhwx.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rj.huanxung.cn

[E19] 多行文本按行拆分
来源：http://mp.colortex.cn

Py:   s.splitlines()
来源：http://lf.huixiangedu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://sk.huanxung.cn

JS:   s.split(/\r?\n/)
来源：http://yn.bookmarksfly.cn

TS:   s.split(/\r?\n/)
来源：http://hw.jctech888.com.cn

Java: s.lines().toList()
来源：http://mq.jctech888.com.cn

Go:   strings.Split(s, "\n")
来源：http://uk.yuntaijiaju.cn

Ruby: s.lines
来源：http://mb.huixiangedu.cn

C#:   s.Split('\n')
来源：http://xt.panjiajie.cn

[E20] 判断字符串是否为空
来源：http://ox.wgjwhj.cn

Py:   if not s:
来源：http://pf.szxytkj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vv.yuntaijiaju.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ho.panjiajie.cn

TS:   if (s === "") {}
来源：http://zw.nszjky.cn

Java: if (s.isEmpty()) {}
来源：http://ht.haigaiapp.cn


<!-- 参考信息 -->