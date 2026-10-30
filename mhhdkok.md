代发 wailian999

Ruby: arr.index(x)
来源：http://read.share.hesvh.cn/Article/details/gaospsnlt.sHtML

C#:   list.IndexOf(x);
来源：http://wap.hesvh.cn/Article/details/gfhowmvwr.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.hesvh.cn/Article/details/gktlqnkyj.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.fehbvm.com/Article/details/gkvrjullj.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.hesvh.cn/Article/details/girdsqghc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gdupivhoa.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/gjudlttbl.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.fehbvm.com/Article/details/gqmxntycj.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.zdbjq.cn/Article/details/gdvvungcb.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.hesvh.cn/Article/details/gqhtdenkx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gxqtifabs.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.hesvh.cn/Article/details/guyotnskq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.fehbvm.com/Article/details/gmovxjrtw.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gkbduldtv.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/gbilitglw.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gwkeloxam.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.hesvh.cn/Article/details/gjkcjjenp.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/gnqgfrqch.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gquqlnagt.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.zdbjq.cn/Article/details/gzhlckbrj.sHtML

[D15] 去重
来源：http://read.share.fehbvm.com/Article/details/gcqxfcqlq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/ggbizcvbe.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gytlkngjd.sHtML

JS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gbybnazpp.sHtML

TS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gcmqtpzqc.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.hesvh.cn/Article/details/ghwfquzhp.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.hesvh.cn/Article/details/gnzzzzdxr.sHtML

Ruby: arr.uniq
来源：http://read.share.fehbvm.com/Article/details/gwnvgrkfy.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.fehbvm.com/Article/details/gagmzlkqg.sHtML

[D16] 求和与平均值
来源：http://blog.fehbvm.com/Article/details/gfkhwitoa.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.fehbvm.com/Article/details/gtstyjnio.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.zdbjq.cn/Article/details/gmuaafujf.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/ghjpppsrg.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/gemblsjvw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.zdbjq.cn/Article/details/gpvudykun.sHtML

Go:   // 手写循环累加
来源：http://wap.zdbjq.cn/Article/details/gqnanwmta.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.zdbjq.cn/Article/details/gxvrfduyo.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.fehbvm.com/Article/details/gkrikhjdb.sHtML

[D17] 最大值与最小值
来源：http://blog.zdbjq.cn/Article/details/gmlerrvlb.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gcmzepbwc.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.fehbvm.com/Article/details/gngmttoqh.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.zdbjq.cn/Article/details/geavwxcml.sHtML

TS:   Math.max(...arr);
来源：http://m.share.hesvh.cn/Article/details/gqvqleuyx.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.zdbjq.cn/Article/details/ghxbxupbg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.hesvh.cn/Article/details/ggowzxxok.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.zdbjq.cn/Article/details/ggiyehlew.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.hesvh.cn/Article/details/gwgetpuks.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fehbvm.com/Article/details/gwxcysufd.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.zdbjq.cn/Article/details/grrgzviii.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.fehbvm.com/Article/details/gqeaybmif.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.fehbvm.com/Article/details/gezokygel.sHtML

TS:   nested.flat();
来源：http://mobile.fehbvm.com/Article/details/gcadtrxqm.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.zdbjq.cn/Article/details/gqpwobmxf.sHtML

Go:   // 手写双层循环
来源：http://www.blog.hesvh.cn/Article/details/ggujcwuqt.sHtML

Ruby: nested.flatten
来源：http://wap.fehbvm.com/Article/details/gbvgcugqm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.hesvh.cn/Article/details/ghqxtstrh.sHtML

[D19] 按字段分组
来源：http://baike.hesvh.cn/Article/details/gbapohyvb.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.fehbvm.com/Article/details/glmbxintj.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.fehbvm.com/Article/details/glfauwmjz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.zdbjq.cn/Article/details/ghbiavkvs.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.hesvh.cn/Article/details/gqblinacq.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.zdbjq.cn/Article/details/gyhepfmjx.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.fehbvm.com/Article/details/gotwryhwh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.hesvh.cn/Article/details/gobxvvvkg.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.zdbjq.cn/Article/details/gsumtpynt.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.fehbvm.com/Article/details/gtogrfyif.sHtML

Py:   Counter(arr)
来源：http://wap.zdbjq.cn/Article/details/gbgpgmzsy.sHtML

PHP:  array_count_values($arr);
来源：http://wap.fehbvm.com/Article/details/gidlkptqp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/gvbusfiaw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/gwygammaf.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.zdbjq.cn/Article/details/gsnaihhdo.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.fehbvm.com/Article/details/gthwkrldz.sHtML

Ruby: arr.tally
来源：http://read.share.zdbjq.cn/Article/details/grwdedofr.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.fehbvm.com/Article/details/gpdlfsbpj.sHtML

[D21] 判断是否包含某元素
来源：http://3g.hesvh.cn/Article/details/grzlhllmn.sHtML

Py:   x in arr
来源：http://www.share.hesvh.cn/Article/details/gqdbfmwuj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.zdbjq.cn/Article/details/gvexqxiem.sHtML

JS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/gpkvimdbv.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gglnqbtwb.sHtML

Java: list.contains(x)
来源：http://baike.hesvh.cn/Article/details/ghpggenmn.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gpxcfujwb.sHtML

Ruby: arr.include?(x)
来源：http://mobile.zdbjq.cn/Article/details/ggmmeoefq.sHtML

C#:   list.Contains(x)
来源：http://3g.hesvh.cn/Article/details/gciqmxgfg.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.fehbvm.com/Article/details/gpcpeyvjd.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.zdbjq.cn/Article/details/gmyurtjlv.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.zdbjq.cn/Article/details/gmunochoz.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.hesvh.cn/Article/details/gwppenhxw.sHtML

TS:   [...arr];
来源：http://www.share.fehbvm.com/Article/details/gdivdebmm.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.zdbjq.cn/Article/details/gigpawqje.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.hesvh.cn/Article/details/gmztqsgpc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.hesvh.cn/Article/details/gxgpufymp.sHtML

C#:   new List<int>(list);
来源：http://www.blog.hesvh.cn/Article/details/gaxvoxvnh.sHtML

[D23] reduce 累积计算
来源：http://read.share.fehbvm.com/Article/details/gaitbfygl.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.fehbvm.com/Article/details/greuyzgoo.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gemvqswmd.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/guhznnowh.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/grobnbuvq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.zdbjq.cn/Article/details/gpehtdkec.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/gspzsgpij.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fehbvm.com/Article/details/gxavrfluk.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.hesvh.cn/Article/details/gkdsrtdnc.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.hesvh.cn/Article/details/gyifvfxhd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.fehbvm.com/Article/details/gjvikenkg.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.zdbjq.cn/Article/details/gklatmhyo.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.zdbjq.cn/Article/details/gjpozsudk.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.hesvh.cn/Article/details/gxmjuithp.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.hesvh.cn/Article/details/geknwbvvr.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.zdbjq.cn/Article/details/gipkfkbeg.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.fehbvm.com/Article/details/giejapzqm.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fehbvm.com/Article/details/gdbbxbbbt.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.hesvh.cn/Article/details/getnemksp.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.hesvh.cn/Article/details/gqfsamslf.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.zdbjq.cn/Article/details/gxbgubxkp.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.fehbvm.com/Article/details/gfybirfzp.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.hesvh.cn/Article/details/giyhkzoqu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.zdbjq.cn/Article/details/gmebckfyy.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.zdbjq.cn/Article/details/gqcpuhtua.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.hesvh.cn/Article/details/gtqtjknek.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.fehbvm.com/Article/details/geqqfhbyl.sHtML

[D26] 数组转字符串
来源：http://www.share.fehbvm.com/Article/details/giydxvmbo.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.hesvh.cn/Article/details/grdkgrjdu.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.zdbjq.cn/Article/details/ghkroxqxt.sHtML

JS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/geapceatm.sHtML

TS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gymnasmag.sHtML

Java: String.join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/gazwraonr.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.fehbvm.com/Article/details/gggaktxmm.sHtML

Ruby: arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/glosvhttk.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/gwifdzidg.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gjlfejmsd.sHtML

E. 字符串处理
来源：http://wap.fehbvm.com/Article/details/ggkcdmvwz.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gcciihwbo.sHtML

[E01] 拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gcrjkpwmj.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.hesvh.cn/Article/details/gxnpcplbq.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.zdbjq.cn/Article/details/gfqleqrqy.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/gbusynxdv.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/grkzwgfln.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.hesvh.cn/Article/details/gtvlrtedo.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.fehbvm.com/Article/details/glsgglbfj.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.hesvh.cn/Article/details/gjrmglryy.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gjeqkhsrt.sHtML

[E02] 重复字符串
来源：http://blog.hesvh.cn/Article/details/girslwgnr.sHtML

Py:   "ab" * 3
来源：http://blog.hesvh.cn/Article/details/gdqjdapli.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.fehbvm.com/Article/details/gfoxahcyx.sHtML

JS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gyxpddhgx.sHtML

TS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gbnxckyyf.sHtML

Java: "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gyaceigom.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.hesvh.cn/Article/details/gsolivnpl.sHtML

Ruby: "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/gzwprympy.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.zdbjq.cn/Article/details/grxxlwdzh.sHtML

[E03] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/grgghkugl.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.hesvh.cn/Article/details/gnkhlxjah.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/glijgfyyd.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/gpqmzwucm.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gevldynac.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gpvarahxm.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.hesvh.cn/Article/details/gyspztwzj.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.zdbjq.cn/Article/details/gnwayqail.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.fehbvm.com/Article/details/glxjsmjbe.sHtML

[E04] 查找子串位置
来源：http://www.m.share.fehbvm.com/Article/details/gdfbcuyky.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.hesvh.cn/Article/details/gyhgfkugk.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.hesvh.cn/Article/details/gdoqrefac.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.zdbjq.cn/Article/details/gzgomzyoo.sHtML

TS:   s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/guhojynmd.sHtML

Java: s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gheajkcnm.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.zdbjq.cn/Article/details/gcsjpbjeg.sHtML

Ruby: s.index("x")
来源：http://www.blog.hesvh.cn/Article/details/gbvkshgnj.sHtML

C#:   s.IndexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gqqmhhxyp.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.hesvh.cn/Article/details/gxvhihqji.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.hesvh.cn/Article/details/gmycawgqf.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.zdbjq.cn/Article/details/gljdeagup.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gyxuqdwzg.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.hesvh.cn/Article/details/gxhbspqhr.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gczjghqat.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.hesvh.cn/Article/details/gmmydlidg.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.hesvh.cn/Article/details/ggswqglxb.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gyxbzhygd.sHtML

[E06] 替换子串
来源：http://m.share.hesvh.cn/Article/details/geyfttsqf.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/gouzpmher.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.zdbjq.cn/Article/details/gmurijtll.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/genrlapax.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/ggbhbndmt.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/guttbtueg.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/gmumkvlak.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gsimyptqx.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gelkomxrv.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.zdbjq.cn/Article/details/gvptrantg.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.hesvh.cn/Article/details/gebyepdsp.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gosavamwv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.zdbjq.cn/Article/details/guwhfqrwn.sHtML

TS:   s.split(",")
来源：http://m.share.hesvh.cn/Article/details/gxjcbqvvx.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.fehbvm.com/Article/details/gxiqsgodg.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.fehbvm.com/Article/details/gtwllgvlo.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.fehbvm.com/Article/details/gngturryv.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.hesvh.cn/Article/details/gxyukdhgl.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.zdbjq.cn/Article/details/gqbtzlwiy.sHtML

Py:   ",".join(items)
来源：http://3g.zdbjq.cn/Article/details/gasbfckrc.sHtML

PHP:  implode(",", $items);
来源：http://www.share.hesvh.cn/Article/details/gkgjzqeyt.sHtML

JS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gukgxtavm.sHtML

TS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/gtqlmlikl.sHtML

Java: String.join(",", items)
来源：http://3g.fehbvm.com/Article/details/groqiinqh.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.fehbvm.com/Article/details/grostugox.sHtML

Ruby: items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gotnxknil.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/gqifzklmc.sHtML

[E09] 去除所有空白字符
来源：http://www.share.zdbjq.cn/Article/details/gntlcpqvg.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.hesvh.cn/Article/details/gunbvgtdw.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.fehbvm.com/Article/details/gkxrxxxta.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/gqrhpwzlp.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/gywsulwwe.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gqidhpzfm.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.hesvh.cn/Article/details/gfbsnilwu.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.hesvh.cn/Article/details/gyztqlxtf.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.fehbvm.com/Article/details/gxkcwpaot.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.zdbjq.cn/Article/details/gqslnsfln.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gqrdipozx.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.hesvh.cn/Article/details/glqsvmqkj.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/glzvqjmkl.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gmbfhlmtm.sHtML

Java: String.format("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gpkpmxbap.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gycstqdte.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gralgdroq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.zdbjq.cn/Article/details/grmtazzha.sHtML

[E11] 反转字符串
来源：http://www.share.zdbjq.cn/Article/details/gybrqmspf.sHtML

Py:   s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gdwmqzkrb.sHtML

PHP:  strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/gulkzymna.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gqgmckvyj.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gjaygqubq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.zdbjq.cn/Article/details/gsnouxckd.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.fehbvm.com/Article/details/gyluawyhi.sHtML

Ruby: s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gbifhgnne.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/gvmyesoyf.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.hesvh.cn/Article/details/gckdjigbn.sHtML

Py:   s.count("a")
来源：http://wap.zdbjq.cn/Article/details/gcrtqkzhy.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.hesvh.cn/Article/details/gakusnobf.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/gheyllenz.sHtML

TS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/gmayjjybo.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.hesvh.cn/Article/details/gcodeaekr.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.hesvh.cn/Article/details/gzikmqbiy.sHtML

Ruby: s.count("a")
来源：http://read.share.hesvh.cn/Article/details/gfxwideev.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.hesvh.cn/Article/details/gwvrdsfob.sHtML

[E13] 逐字符遍历
来源：http://mobile.zdbjq.cn/Article/details/gnzmreyvf.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.zdbjq.cn/Article/details/gdfxlmswc.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.zdbjq.cn/Article/details/grxwrvmtu.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gjpignpxw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gydoysriv.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.fehbvm.com/Article/details/gxdeahcyu.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.fehbvm.com/Article/details/gkxluagfi.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.zdbjq.cn/Article/details/gneuuweak.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.fehbvm.com/Article/details/gysicjieq.sHtML

[E14] URL 编码与 Base64
来源：http://wap.fehbvm.com/Article/details/godzwuftd.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.hesvh.cn/Article/details/guvsaqrwv.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.hesvh.cn/Article/details/ggbsiqhge.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.fehbvm.com/Article/details/gkxhazbmz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.zdbjq.cn/Article/details/gpnfuqiyv.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gvvwlyksk.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.hesvh.cn/Article/details/gpqfxzwiz.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.fehbvm.com/Article/details/ghdaixhlb.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.hesvh.cn/Article/details/gmtjaqoys.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.hesvh.cn/Article/details/gkoxniapx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.fehbvm.com/Article/details/gkdbvhong.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.hesvh.cn/Article/details/gmvtvegyx.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.hesvh.cn/Article/details/gzxtsxejz.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.fehbvm.com/Article/details/gqzjedyqw.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.fehbvm.com/Article/details/gtibdrjcm.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gpsbozqbh.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.zdbjq.cn/Article/details/gsbswvxvp.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.hesvh.cn/Article/details/gpxjyhupk.sHtML

[E16] 数字千分位
来源：http://read.share.fehbvm.com/Article/details/gjjqjygeq.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.hesvh.cn/Article/details/gzwrvwixs.sHtML

PHP:  number_format(1234567);
来源：http://wap.fehbvm.com/Article/details/gierqzsru.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/gksfucexo.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/gmwjolqyv.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/grijruiaw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.fehbvm.com/Article/details/gjsdzcjff.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.fehbvm.com/Article/details/gekrivuik.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.hesvh.cn/Article/details/godxbgqhg.sHtML

[E17] 首字母大写
来源：http://blog.zdbjq.cn/Article/details/gedboerzd.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.hesvh.cn/Article/details/gjnysbkup.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.zdbjq.cn/Article/details/gkfxpsfel.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/gxklyjpkk.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/gspcfssks.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.hesvh.cn/Article/details/gnihqoggy.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.zdbjq.cn/Article/details/gntyzrmyk.sHtML

Ruby: s.capitalize
来源：http://mobile.fehbvm.com/Article/details/gefhjtuku.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.hesvh.cn/Article/details/gkvhunfan.sHtML

[E18] 模板占位符替换
来源：http://wap.zdbjq.cn/Article/details/gxmgrlbyw.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fehbvm.com/Article/details/gddvkjwzz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.fehbvm.com/Article/details/gzktiffps.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gyekwgogp.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/guduppxdb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/glqohjqic.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gyrjnrmhx.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.hesvh.cn/Article/details/ghtaynqig.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.fehbvm.com/Article/details/gxgmwuqhw.sHtML

[E19] 多行文本按行拆分
来源：http://3g.zdbjq.cn/Article/details/gfqxlsgor.sHtML

Py:   s.splitlines()
来源：http://www.m.share.fehbvm.com/Article/details/gdskwfoma.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.fehbvm.com/Article/details/gnpoizgxs.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/gpvdabujv.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.fehbvm.com/Article/details/gfnupglia.sHtML

Java: s.lines().toList()
来源：http://blog.hesvh.cn/Article/details/gymassbot.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.zdbjq.cn/Article/details/gwhsqiaec.sHtML


<!-- 参考信息 -->