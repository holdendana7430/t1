代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://m.share.hesvh.cn/Article/details/ggwruhaxv.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.fehbvm.com/Article/details/gzpmnfgtq.sHtML

TS:   Math.max(...arr);
来源：http://m.share.hesvh.cn/Article/details/gmuvxxruc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.fehbvm.com/Article/details/gqopyohrn.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.fehbvm.com/Article/details/gnwggulax.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.fehbvm.com/Article/details/gcjgyutbe.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.fehbvm.com/Article/details/gvpzdnire.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.fehbvm.com/Article/details/gjeqcsyrl.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.hesvh.cn/Article/details/glxiuhdxm.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fehbvm.com/Article/details/gmycvradi.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.hesvh.cn/Article/details/gkihkdiuj.sHtML

TS:   nested.flat();
来源：http://3g.fehbvm.com/Article/details/gsgdmroed.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.hesvh.cn/Article/details/gpnhtadpm.sHtML

Go:   // 手写双层循环
来源：http://baike.fehbvm.com/Article/details/gwhnaxook.sHtML

Ruby: nested.flatten
来源：http://read.share.fehbvm.com/Article/details/gcvyabcra.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gbccnysjc.sHtML

[D19] 按字段分组
来源：http://baike.fehbvm.com/Article/details/gqerzegcp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.fehbvm.com/Article/details/gvngpakov.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.hesvh.cn/Article/details/gkozgkpuu.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.hesvh.cn/Article/details/gducocnsc.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.hesvh.cn/Article/details/ghuadzuwa.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.zdbjq.cn/Article/details/gglwgpjsf.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.zdbjq.cn/Article/details/gixhrckvl.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.fehbvm.com/Article/details/gyokveqzz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.fehbvm.com/Article/details/gxdvtvqmk.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.hesvh.cn/Article/details/ghwmomive.sHtML

Py:   Counter(arr)
来源：http://read.share.fehbvm.com/Article/details/gghankkbm.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gnuxzjmgj.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gxpnkirbz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/gtumfcinw.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.hesvh.cn/Article/details/gjzkiyoev.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.fehbvm.com/Article/details/gydgpkffg.sHtML

Ruby: arr.tally
来源：http://read.share.fehbvm.com/Article/details/gtckkjzzy.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.hesvh.cn/Article/details/gxkpdemjs.sHtML

[D21] 判断是否包含某元素
来源：http://wap.hesvh.cn/Article/details/gdebmfosy.sHtML

Py:   x in arr
来源：http://www.blog.zdbjq.cn/Article/details/gkjghzvgs.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.fehbvm.com/Article/details/gizlejztx.sHtML

JS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/gnwoswbya.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gcfkhxzfq.sHtML

Java: list.contains(x)
来源：http://mobile.zdbjq.cn/Article/details/glhyrendd.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gxbfeukuj.sHtML

Ruby: arr.include?(x)
来源：http://3g.hesvh.cn/Article/details/gencpgcmw.sHtML

C#:   list.Contains(x)
来源：http://www.share.fehbvm.com/Article/details/gtfbbnnlo.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.hesvh.cn/Article/details/gjymqssxh.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.hesvh.cn/Article/details/gwcovzbtt.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.fehbvm.com/Article/details/goxugntwz.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gnujzlbdl.sHtML

TS:   [...arr];
来源：http://baike.hesvh.cn/Article/details/ggnxmnwjl.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.hesvh.cn/Article/details/gxzbdakaz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.hesvh.cn/Article/details/gtzxfnhty.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.zdbjq.cn/Article/details/gvhhhpphh.sHtML

C#:   new List<int>(list);
来源：http://baike.hesvh.cn/Article/details/ghtrjzfeq.sHtML

[D23] reduce 累积计算
来源：http://blog.fehbvm.com/Article/details/grjuuekiv.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.hesvh.cn/Article/details/gujqzugnm.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.hesvh.cn/Article/details/gqmgljxjy.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gkxtbzocy.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gbgykfybt.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.fehbvm.com/Article/details/gyzeqqaos.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/geunwldds.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.hesvh.cn/Article/details/gbprlefws.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.hesvh.cn/Article/details/gbvetnlvw.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.fehbvm.com/Article/details/ggqrcsusn.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fehbvm.com/Article/details/gpfnaesxc.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.zdbjq.cn/Article/details/gfkpfsfqt.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.hesvh.cn/Article/details/guccnvdmm.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gcqyakmnf.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.hesvh.cn/Article/details/gjlieocfn.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.zdbjq.cn/Article/details/gceypldrj.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.zdbjq.cn/Article/details/guqqvcisr.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.hesvh.cn/Article/details/ghmdyfvoa.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.fehbvm.com/Article/details/gtrnvacow.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.zdbjq.cn/Article/details/gaioqcefi.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.hesvh.cn/Article/details/gpjcvlnmt.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.zdbjq.cn/Article/details/gvhaceohe.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.fehbvm.com/Article/details/gdwasmxnf.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gmxiyvtpu.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.fehbvm.com/Article/details/gxhmyutbc.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.hesvh.cn/Article/details/gkhpyfami.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.hesvh.cn/Article/details/gzvtnqawk.sHtML

[D26] 数组转字符串
来源：http://wap.fehbvm.com/Article/details/gmkhxkius.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.zdbjq.cn/Article/details/gexjjthlk.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.fehbvm.com/Article/details/gtgzgiiai.sHtML

JS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gurjyvirc.sHtML

TS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gpwuzybge.sHtML

Java: String.join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gbhbkjuvr.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.hesvh.cn/Article/details/gvcygaghf.sHtML

Ruby: arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gjbafspkf.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/gujqztmvd.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gevvsdgga.sHtML

E. 字符串处理
来源：http://www.share.hesvh.cn/Article/details/gtnwbpzmu.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gwqwxicyo.sHtML

[E01] 拼接字符串
来源：http://baike.hesvh.cn/Article/details/gghtmuqna.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.hesvh.cn/Article/details/gglhbdmte.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.hesvh.cn/Article/details/gwwqbcybw.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/geanzohzf.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/ghjxbvbnq.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.fehbvm.com/Article/details/gbtzdizsy.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.hesvh.cn/Article/details/gidiqjzez.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.fehbvm.com/Article/details/gztqtmbwr.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gbmxegdti.sHtML

[E02] 重复字符串
来源：http://mobile.zdbjq.cn/Article/details/gopqhzazq.sHtML

Py:   "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gdlybgywn.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.fehbvm.com/Article/details/gbzknhjoe.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gjzftnnut.sHtML

TS:   "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gewvwlpvi.sHtML

Java: "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gqctgxhww.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.zdbjq.cn/Article/details/gqppxpjjq.sHtML

Ruby: "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/gcudyvdbq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.hesvh.cn/Article/details/gexvifagk.sHtML

[E03] 截取子串
来源：http://blog.zdbjq.cn/Article/details/gkjsthzax.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.hesvh.cn/Article/details/gvdzfqcjr.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gqaxnzjje.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/ggodkrjbf.sHtML

TS:   s.slice(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gyzqhnfde.sHtML

Java: s.substring(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gzvoawlzw.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.fehbvm.com/Article/details/gkgneersh.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.hesvh.cn/Article/details/gcskbudlm.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.zdbjq.cn/Article/details/glgbvvptx.sHtML

[E04] 查找子串位置
来源：http://blog.fehbvm.com/Article/details/gkhugyygg.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.hesvh.cn/Article/details/gfrrsjhwj.sHtML

PHP:  strpos($s, "x");
来源：http://3g.fehbvm.com/Article/details/gprwxrnje.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.zdbjq.cn/Article/details/ghpzknbhl.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gmsamebvn.sHtML

Java: s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gvdwqiotx.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.fehbvm.com/Article/details/ghzskzklf.sHtML

Ruby: s.index("x")
来源：http://wap.fehbvm.com/Article/details/gchmvypao.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.hesvh.cn/Article/details/glrcpvrpf.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.fehbvm.com/Article/details/guvngnerf.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.hesvh.cn/Article/details/gofpmiyam.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.fehbvm.com/Article/details/gxchlswhw.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/glbvivydd.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gqypkazjw.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gnhouptyt.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.fehbvm.com/Article/details/gyasicbcv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.fehbvm.com/Article/details/gqrpbqfqs.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gbvuyfvve.sHtML

[E06] 替换子串
来源：http://wap.hesvh.cn/Article/details/gppbxsipo.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gmmeraupp.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.hesvh.cn/Article/details/gnxsxluye.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gbhncmkbw.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/ghvytcbba.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/giyecqdbv.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/gvwtlsbzl.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gqsgdocuv.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.hesvh.cn/Article/details/gckldevst.sHtML

[E07] 按分隔符拆分
来源：http://read.share.zdbjq.cn/Article/details/gmrolvmcc.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.hesvh.cn/Article/details/grhjvsrrw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gvwokhksg.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.zdbjq.cn/Article/details/gtudjsuim.sHtML

TS:   s.split(",")
来源：http://www.m.share.fehbvm.com/Article/details/gsqlezjsh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.fehbvm.com/Article/details/gsflqjbkx.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.zdbjq.cn/Article/details/gbfhaxcwl.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.zdbjq.cn/Article/details/gcupywqwq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.hesvh.cn/Article/details/gzhauvhxt.sHtML

[E08] 数组按分隔符合并
来源：http://blog.fehbvm.com/Article/details/gqlllcnks.sHtML

Py:   ",".join(items)
来源：http://www.blog.zdbjq.cn/Article/details/gobbkrmhd.sHtML

PHP:  implode(",", $items);
来源：http://mobile.fehbvm.com/Article/details/givvgriov.sHtML

JS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/glcogaczw.sHtML

TS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/ghhavhuko.sHtML

Java: String.join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/ggoxgrefh.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.hesvh.cn/Article/details/gqgwdnbii.sHtML

Ruby: items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gqwwvmhku.sHtML

C#:   string.Join(",", items)
来源：http://3g.hesvh.cn/Article/details/gyduaqjqv.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.hesvh.cn/Article/details/gsezxyugj.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.hesvh.cn/Article/details/ghwfnjukt.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.zdbjq.cn/Article/details/gvffmgezc.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/gldlpeqtp.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/gpnbfubbf.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.zdbjq.cn/Article/details/guqjkmgdf.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.hesvh.cn/Article/details/gbmwglfhc.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.zdbjq.cn/Article/details/gfhupgsua.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.zdbjq.cn/Article/details/gpomvtwth.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.fehbvm.com/Article/details/gltathsre.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gfxhxnyhr.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.zdbjq.cn/Article/details/gcdmmvnef.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/ggrfpiwmc.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gevkxtobo.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gprrlxegu.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gdzgrcnqx.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gvpycmtia.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.hesvh.cn/Article/details/gssnhjydm.sHtML

[E11] 反转字符串
来源：http://3g.fehbvm.com/Article/details/gikernhbe.sHtML

Py:   s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/gygrwmrnw.sHtML

PHP:  strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/gycbeodnt.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gzxpapteo.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gyhnoyuin.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.hesvh.cn/Article/details/gppzatwkj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/ghqnfrtbv.sHtML

Ruby: s.reverse
来源：http://read.share.fehbvm.com/Article/details/gebomyqqm.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gnogfkfek.sHtML

[E12] 统计某字符出现次数
来源：http://baike.zdbjq.cn/Article/details/gdyqmwbdk.sHtML

Py:   s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/ghrlunomg.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.zdbjq.cn/Article/details/gzqjzzimg.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/gwrelimgm.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/gakhyhlzj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.zdbjq.cn/Article/details/gtneuktez.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.fehbvm.com/Article/details/gechxolwh.sHtML

Ruby: s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gnugulmbh.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.zdbjq.cn/Article/details/gdtziflmw.sHtML

[E13] 逐字符遍历
来源：http://blog.zdbjq.cn/Article/details/gmagtlgbg.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.hesvh.cn/Article/details/gdwnvzqwr.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.zdbjq.cn/Article/details/gvwglyyes.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/gdneltpyc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/gzlxvdpzp.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.fehbvm.com/Article/details/gbfsetoon.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.fehbvm.com/Article/details/gvgmrecis.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.zdbjq.cn/Article/details/gixantoth.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gixjchsat.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.zdbjq.cn/Article/details/glwneubua.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.hesvh.cn/Article/details/gghoaqbry.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.fehbvm.com/Article/details/ggasrbnym.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.hesvh.cn/Article/details/gqclaqyuq.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.zdbjq.cn/Article/details/gslxvsezn.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.fehbvm.com/Article/details/gidrxeacv.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.zdbjq.cn/Article/details/gfcveprcu.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.fehbvm.com/Article/details/gjaucterg.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gcuvahiyh.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.hesvh.cn/Article/details/ghpzvndek.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.zdbjq.cn/Article/details/gsychzqaj.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.fehbvm.com/Article/details/gawfwybch.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.zdbjq.cn/Article/details/gbecxjldw.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.fehbvm.com/Article/details/guucxjece.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.hesvh.cn/Article/details/gxwpkdrym.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.fehbvm.com/Article/details/gfpfpqrax.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.fehbvm.com/Article/details/gnwaqklpn.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.fehbvm.com/Article/details/gaktlaeoj.sHtML

[E16] 数字千分位
来源：http://www.share.hesvh.cn/Article/details/gzvzwodvn.sHtML

Py:   f"{1234567:,}"
来源：http://3g.zdbjq.cn/Article/details/guptzczxj.sHtML

PHP:  number_format(1234567);
来源：http://m.share.zdbjq.cn/Article/details/gxzjjaktn.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/gsmexeaju.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gymjorttd.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.fehbvm.com/Article/details/glpcckniy.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.fehbvm.com/Article/details/ggodxlbuv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.zdbjq.cn/Article/details/gafdawkuz.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.hesvh.cn/Article/details/grnkmmwde.sHtML

[E17] 首字母大写
来源：http://read.share.fehbvm.com/Article/details/gdcimqwzn.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.fehbvm.com/Article/details/gyftjwizf.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.fehbvm.com/Article/details/gyiwjhzay.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/ggtetcyap.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/gsjpuxduv.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.zdbjq.cn/Article/details/gynyeabdh.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.fehbvm.com/Article/details/gvqspbang.sHtML

Ruby: s.capitalize
来源：http://wap.fehbvm.com/Article/details/glgaerelx.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.zdbjq.cn/Article/details/grrqsvjrh.sHtML

[E18] 模板占位符替换
来源：http://3g.hesvh.cn/Article/details/gdmupcsbn.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.hesvh.cn/Article/details/gjgzzszac.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.fehbvm.com/Article/details/gxfsjqmif.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gaaktditb.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gvhticgce.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gtfpylgwm.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.zdbjq.cn/Article/details/ghewgtmpj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.zdbjq.cn/Article/details/gmsonhhvp.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.fehbvm.com/Article/details/gnelscwfh.sHtML

[E19] 多行文本按行拆分
来源：http://blog.fehbvm.com/Article/details/ghekvtusk.sHtML

Py:   s.splitlines()
来源：http://www.blog.fehbvm.com/Article/details/gtyzjxulx.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.zdbjq.cn/Article/details/gcevkmisn.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gfllzdbif.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gossifauf.sHtML

Java: s.lines().toList()
来源：http://3g.fehbvm.com/Article/details/gjwdzswom.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.hesvh.cn/Article/details/glaqogbmq.sHtML

Ruby: s.lines
来源：http://mobile.hesvh.cn/Article/details/gkmdepjeh.sHtML

C#:   s.Split('\n')
来源：http://wap.zdbjq.cn/Article/details/gbqjdswij.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.fehbvm.com/Article/details/gxcmtjnrs.sHtML

Py:   if not s:
来源：http://read.share.zdbjq.cn/Article/details/genqdqynk.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.hesvh.cn/Article/details/gvgtgojea.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.hesvh.cn/Article/details/gnupcjfxe.sHtML

TS:   if (s === "") {}
来源：http://m.share.hesvh.cn/Article/details/gmkxpkpax.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gsfzimtdk.sHtML

Go:   if s == "" {}
来源：http://www.m.share.zdbjq.cn/Article/details/gyrnderxn.sHtML

Ruby: if s.empty?
来源：http://blog.fehbvm.com/Article/details/ghpxmqkux.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.fehbvm.com/Article/details/goddymygn.sHtML

[E21] 超长截断加省略号
来源：http://mobile.zdbjq.cn/Article/details/glsxauuot.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.hesvh.cn/Article/details/ggcfdbxma.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/ggylonvxc.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/ggfakhlcz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gplqmmeyz.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/geeeszsfp.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.fehbvm.com/Article/details/gzhtwgere.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gmryvrcse.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/ggesbhtzn.sHtML

[E22] 字节长度与字符长度
来源：http://blog.zdbjq.cn/Article/details/gznemtflr.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.fehbvm.com/Article/details/geaployqd.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gvxejgidx.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/ggvsajwll.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/gfxvgrsio.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/gocwxhcho.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.fehbvm.com/Article/details/gdwkabviw.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.fehbvm.com/Article/details/gdgbsoxwr.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.fehbvm.com/Article/details/gxszbkboy.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/guclqzfcl.sHtML

F. 文件与目录
来源：http://mobile.zdbjq.cn/Article/details/gobgdddhp.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ghavogrch.sHtML

[F01] 读取整个文件
来源：http://read.share.hesvh.cn/Article/details/gntzrorls.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.zdbjq.cn/Article/details/gjurweuum.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gqutwupdv.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.hesvh.cn/Article/details/gvdkkmwqk.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.hesvh.cn/Article/details/gonqxatvp.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gqjqrvody.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.fehbvm.com/Article/details/glyqrictp.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.fehbvm.com/Article/details/guescpknq.sHtML


<!-- 参考信息 -->