代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.zdbjq.cn/Article/details/ghnpotrea.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.hesvh.cn/Article/details/gfrtezwag.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.hesvh.cn/Article/details/gzjynhdfu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.hesvh.cn/Article/details/glyqqmogs.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.fehbvm.com/Article/details/gdbezpoje.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.fehbvm.com/Article/details/gflzpxlye.sHtML

Py:   Counter(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gacfsixog.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/ghcvlvrvx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gglnrqiaf.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/gwcsjdojl.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.hesvh.cn/Article/details/gcczhzqfp.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.zdbjq.cn/Article/details/gfmbbblpa.sHtML

Ruby: arr.tally
来源：http://read.share.fehbvm.com/Article/details/gheruykss.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.zdbjq.cn/Article/details/gvsxalmyx.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.fehbvm.com/Article/details/gggvrqjuz.sHtML

Py:   x in arr
来源：http://wap.fehbvm.com/Article/details/gosvpitqw.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.hesvh.cn/Article/details/gkfpkxrzp.sHtML

JS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gixnofmhb.sHtML

TS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gcjhvxcmo.sHtML

Java: list.contains(x)
来源：http://read.share.fehbvm.com/Article/details/groqgcssh.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gtrjjmldp.sHtML

Ruby: arr.include?(x)
来源：http://read.share.zdbjq.cn/Article/details/gjztzbcib.sHtML

C#:   list.Contains(x)
来源：http://wap.zdbjq.cn/Article/details/gbwmouzap.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.hesvh.cn/Article/details/gdprnjlcf.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.hesvh.cn/Article/details/ghckkwinc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.hesvh.cn/Article/details/ggwnizshs.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.hesvh.cn/Article/details/ggsawxtkh.sHtML

TS:   [...arr];
来源：http://blog.hesvh.cn/Article/details/gxkkdibbz.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.fehbvm.com/Article/details/gejqagfhg.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.hesvh.cn/Article/details/gtrvjjajx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.zdbjq.cn/Article/details/gngavicam.sHtML

C#:   new List<int>(list);
来源：http://m.share.hesvh.cn/Article/details/gzyvgvszo.sHtML

[D23] reduce 累积计算
来源：http://3g.fehbvm.com/Article/details/gmojrvdxe.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.fehbvm.com/Article/details/gsmxokhgp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.zdbjq.cn/Article/details/gqtlouvov.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/gjbczddfl.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/gwocctpic.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.zdbjq.cn/Article/details/ggfzocotz.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/gyttdoshi.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.hesvh.cn/Article/details/gwfyogzjm.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.hesvh.cn/Article/details/glwrhsdub.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.zdbjq.cn/Article/details/ggayvbcwo.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.fehbvm.com/Article/details/gpldlwogb.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.hesvh.cn/Article/details/gatmsshxm.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.fehbvm.com/Article/details/gjfsocdit.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gtcgcqqpn.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.zdbjq.cn/Article/details/gypktvmea.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.hesvh.cn/Article/details/gwhjjaflz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.hesvh.cn/Article/details/gmlqjccan.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.hesvh.cn/Article/details/glgwsiwpl.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fehbvm.com/Article/details/gcmvfnaoa.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.zdbjq.cn/Article/details/gvsczumag.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.hesvh.cn/Article/details/grwwflufg.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.fehbvm.com/Article/details/gvbgvnujt.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.fehbvm.com/Article/details/glrizovqi.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.fehbvm.com/Article/details/gzrlztkcp.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.fehbvm.com/Article/details/gdenaxnmc.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.fehbvm.com/Article/details/gcsdnsisz.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gzwdalewr.sHtML

[D26] 数组转字符串
来源：http://www.share.zdbjq.cn/Article/details/gztilufdg.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.fehbvm.com/Article/details/glqrqefkv.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.hesvh.cn/Article/details/guumgarwq.sHtML

JS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gkfhjpyml.sHtML

TS:   arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/guwfbedtv.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/gryaiyuqp.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.hesvh.cn/Article/details/gkemqynhz.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gstsglnxc.sHtML

C#:   string.Join(", ", list)
来源：http://blog.hesvh.cn/Article/details/gpcghixdt.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gbtohkmfw.sHtML

E. 字符串处理
来源：http://blog.zdbjq.cn/Article/details/gwvxrudsz.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxoiabvhi.sHtML

[E01] 拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gooetkafk.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.hesvh.cn/Article/details/gstwfvwwh.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.zdbjq.cn/Article/details/goqiujaby.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/gpaqqzuum.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/graadtfgh.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.fehbvm.com/Article/details/ghfgsfpju.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.fehbvm.com/Article/details/gjrsaqyru.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.zdbjq.cn/Article/details/gdtdkunre.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gizrzwhdf.sHtML

[E02] 重复字符串
来源：http://www.blog.zdbjq.cn/Article/details/ggfvavgdr.sHtML

Py:   "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gxxdvflqz.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.hesvh.cn/Article/details/gtezjvdsa.sHtML

JS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/ggjpkgiof.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gjvtjhecv.sHtML

Java: "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gsiicecnv.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.fehbvm.com/Article/details/grhnzujoc.sHtML

Ruby: "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/gbookuyxn.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.fehbvm.com/Article/details/gbuwgdqou.sHtML

[E03] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/gfwficnjh.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.hesvh.cn/Article/details/gffbdkdwv.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gsnvgbaxy.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gzwnmvozq.sHtML

TS:   s.slice(1, 4)
来源：http://3g.fehbvm.com/Article/details/ggqxuknyl.sHtML

Java: s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gyqomjxiz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.hesvh.cn/Article/details/gahhtqlel.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.hesvh.cn/Article/details/gljpmiwtc.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.hesvh.cn/Article/details/gbdhydsxr.sHtML

[E04] 查找子串位置
来源：http://3g.hesvh.cn/Article/details/gqxnsmloj.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gynykxzfr.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.fehbvm.com/Article/details/gowmazpzn.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.hesvh.cn/Article/details/ghumurkmg.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gthiremzi.sHtML

Java: s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/gvpihzikz.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.zdbjq.cn/Article/details/golzuyzbx.sHtML

Ruby: s.index("x")
来源：http://www.share.fehbvm.com/Article/details/gflawzcsg.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gsfxrlupm.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fehbvm.com/Article/details/gaxmpgchn.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.zdbjq.cn/Article/details/gqdefkyde.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.hesvh.cn/Article/details/gujtxrsqi.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/grzchwooo.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.zdbjq.cn/Article/details/gtuidvzkv.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/grzeqppsb.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.fehbvm.com/Article/details/gcsrmhvly.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.hesvh.cn/Article/details/gpcqcqmys.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gbmcrzmlr.sHtML

[E06] 替换子串
来源：http://www.m.share.hesvh.cn/Article/details/gvdyetwrl.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/gqwhcnmsb.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.hesvh.cn/Article/details/gdluiisuf.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gomeponcu.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gpsejhjme.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gjchmxvzn.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/gfhepartp.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.hesvh.cn/Article/details/gohamaypy.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gzcwdprlj.sHtML

[E07] 按分隔符拆分
来源：http://3g.hesvh.cn/Article/details/gvkemsxhb.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.fehbvm.com/Article/details/gnqjmyjdr.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gzytujmow.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.hesvh.cn/Article/details/giiedqviw.sHtML

TS:   s.split(",")
来源：http://read.share.zdbjq.cn/Article/details/gzschulbc.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.zdbjq.cn/Article/details/gbipgzkel.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.hesvh.cn/Article/details/gzkyovdjt.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.fehbvm.com/Article/details/ghhvizkkc.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.hesvh.cn/Article/details/gfynozwxs.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.fehbvm.com/Article/details/gcmkilcgl.sHtML

Py:   ",".join(items)
来源：http://blog.zdbjq.cn/Article/details/gzffvchiz.sHtML

PHP:  implode(",", $items);
来源：http://www.share.fehbvm.com/Article/details/glopmgauu.sHtML

JS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/grrkiftxn.sHtML

TS:   items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gbacekyuq.sHtML

Java: String.join(",", items)
来源：http://read.share.fehbvm.com/Article/details/gwhvplrxq.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.zdbjq.cn/Article/details/gbplplphp.sHtML

Ruby: items.join(",")
来源：http://www.share.fehbvm.com/Article/details/guzedynoq.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gmviiyijy.sHtML

[E09] 去除所有空白字符
来源：http://3g.hesvh.cn/Article/details/grnrakjge.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.fehbvm.com/Article/details/gytzmucbw.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.zdbjq.cn/Article/details/gmstlutpv.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/gwwmjzvey.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/ghytextib.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/gzficfiye.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.zdbjq.cn/Article/details/gdepdobrv.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.fehbvm.com/Article/details/gwpqtalmj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.fehbvm.com/Article/details/gjxiavdbg.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.hesvh.cn/Article/details/gxmupzmpo.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gbnllpgzf.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.hesvh.cn/Article/details/gekgkkewg.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gpvtkpjxy.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gdaxhcopw.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/glymtlieo.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gjpltwdpn.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/ggitpqvzd.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.fehbvm.com/Article/details/gzogvasbw.sHtML

[E11] 反转字符串
来源：http://read.share.zdbjq.cn/Article/details/gbcrcrdxn.sHtML

Py:   s[::-1]
来源：http://wap.fehbvm.com/Article/details/gdmpmmvmp.sHtML

PHP:  strrev($s);
来源：http://wap.hesvh.cn/Article/details/ggwahkujl.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gwbfwarfq.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gfgjygdso.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/girlwflsl.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gokngjmms.sHtML

Ruby: s.reverse
来源：http://www.share.hesvh.cn/Article/details/gbxyedxtl.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gyozpogsk.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.fehbvm.com/Article/details/giiotvdoe.sHtML

Py:   s.count("a")
来源：http://wap.hesvh.cn/Article/details/gqciefeaq.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.zdbjq.cn/Article/details/gywslkkud.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/gexhobreq.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gznyrzrvc.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.hesvh.cn/Article/details/gvlviqbls.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.zdbjq.cn/Article/details/gvlfvsqyh.sHtML

Ruby: s.count("a")
来源：http://blog.hesvh.cn/Article/details/gzzhabwmn.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.zdbjq.cn/Article/details/gtvrvwtfe.sHtML

[E13] 逐字符遍历
来源：http://blog.hesvh.cn/Article/details/gcgezhdjb.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.hesvh.cn/Article/details/gzztepltl.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.hesvh.cn/Article/details/ggeoyanif.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gxiepikmw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gtgfgbriu.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.zdbjq.cn/Article/details/gvxgpydet.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.fehbvm.com/Article/details/gxpxooeqm.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.zdbjq.cn/Article/details/gmqlxxavw.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.zdbjq.cn/Article/details/gmxijzwdo.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.zdbjq.cn/Article/details/gszudlhfr.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.hesvh.cn/Article/details/gfwskzgxl.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.fehbvm.com/Article/details/gfrosjibs.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.zdbjq.cn/Article/details/gmyuarbdb.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.fehbvm.com/Article/details/gcasnigzo.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.fehbvm.com/Article/details/gjkgrwytp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.hesvh.cn/Article/details/gttkmxbdy.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.hesvh.cn/Article/details/goomzhltl.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/glhrnkimk.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.hesvh.cn/Article/details/gyhlwumcq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.hesvh.cn/Article/details/gptbmfilh.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.fehbvm.com/Article/details/goktcjtcc.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.hesvh.cn/Article/details/geajbyyjj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.fehbvm.com/Article/details/gttuhquhg.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.zdbjq.cn/Article/details/ggbihqtaa.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.hesvh.cn/Article/details/gyoqlhbjs.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.zdbjq.cn/Article/details/giwclqibm.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.fehbvm.com/Article/details/gwlhclnvj.sHtML

[E16] 数字千分位
来源：http://m.share.zdbjq.cn/Article/details/gatfnzygo.sHtML

Py:   f"{1234567:,}"
来源：http://baike.zdbjq.cn/Article/details/grmspvjgw.sHtML

PHP:  number_format(1234567);
来源：http://m.share.hesvh.cn/Article/details/gztjrqkmx.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/guqdnseiq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/gcnjrwbpu.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/gsjrdwyhv.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.hesvh.cn/Article/details/gqllvbfso.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.zdbjq.cn/Article/details/gkbnyuucc.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.hesvh.cn/Article/details/gkcsbejkr.sHtML

[E17] 首字母大写
来源：http://wap.hesvh.cn/Article/details/gmwjocvbq.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.hesvh.cn/Article/details/gfuwchyeo.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.zdbjq.cn/Article/details/ggpfjktmi.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.hesvh.cn/Article/details/godnqffyv.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/gcfmyaigm.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.fehbvm.com/Article/details/gvavinati.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.hesvh.cn/Article/details/grjzqebcp.sHtML

Ruby: s.capitalize
来源：http://www.share.fehbvm.com/Article/details/gkyacpapy.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.fehbvm.com/Article/details/guicwzxfh.sHtML

[E18] 模板占位符替换
来源：http://baike.zdbjq.cn/Article/details/gwnousomh.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.hesvh.cn/Article/details/giemakoac.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.hesvh.cn/Article/details/gbkodipeo.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gsrwrqntf.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gmovtwenj.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gvbojnydn.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gscmiqeig.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.fehbvm.com/Article/details/gjzjztoep.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.fehbvm.com/Article/details/ggdmwfujg.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.fehbvm.com/Article/details/ggngepaos.sHtML

Py:   s.splitlines()
来源：http://baike.fehbvm.com/Article/details/gwgbvikcp.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/giaihhjug.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/gdhmygjyx.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/gvrndjkdx.sHtML

Java: s.lines().toList()
来源：http://read.share.fehbvm.com/Article/details/gagadrhys.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.hesvh.cn/Article/details/galwqfngl.sHtML

Ruby: s.lines
来源：http://wap.hesvh.cn/Article/details/gmhuvgtao.sHtML

C#:   s.Split('\n')
来源：http://baike.zdbjq.cn/Article/details/gkmnuqlcx.sHtML

[E20] 判断字符串是否为空
来源：http://wap.zdbjq.cn/Article/details/gakqhwqmm.sHtML

Py:   if not s:
来源：http://m.share.hesvh.cn/Article/details/gvvcyvfil.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.fehbvm.com/Article/details/gbxkbptjk.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fehbvm.com/Article/details/gtxeydpfm.sHtML

TS:   if (s === "") {}
来源：http://3g.hesvh.cn/Article/details/glqzeclfi.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/gqrbyttxm.sHtML

Go:   if s == "" {}
来源：http://3g.hesvh.cn/Article/details/gnicondkc.sHtML

Ruby: if s.empty?
来源：http://www.share.fehbvm.com/Article/details/geodvgipk.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.fehbvm.com/Article/details/glajebfpw.sHtML

[E21] 超长截断加省略号
来源：http://mobile.hesvh.cn/Article/details/gosdnhzmf.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.zdbjq.cn/Article/details/guykhzdoh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/getqpajgn.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gmleeeoqg.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gevnflvys.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gkysvnbcy.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.hesvh.cn/Article/details/gfiiwljwi.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/ghyxlamou.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gtuaajiif.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.zdbjq.cn/Article/details/gamnjvoba.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.zdbjq.cn/Article/details/gypgzgzhu.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gparuijei.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gdntabarz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gjcjdfokn.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.zdbjq.cn/Article/details/glvtdsvxz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.fehbvm.com/Article/details/gjwupeabc.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.fehbvm.com/Article/details/gpxyvmflb.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.fehbvm.com/Article/details/grbwnrdau.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gubwqysto.sHtML

F. 文件与目录
来源：http://wap.zdbjq.cn/Article/details/gsdgktjxm.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmogwwzwb.sHtML

[F01] 读取整个文件
来源：http://www.share.hesvh.cn/Article/details/gtiarofuh.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.hesvh.cn/Article/details/ggtugcdhn.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gbyplvdtt.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.fehbvm.com/Article/details/gnvszdtui.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.zdbjq.cn/Article/details/guzuxjmgb.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gleekkpgo.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.fehbvm.com/Article/details/gjmbuymjj.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gqcfhivor.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gqiinfcnq.sHtML

[F02] 逐行读取文件
来源：http://mobile.fehbvm.com/Article/details/gohoiryxo.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.fehbvm.com/Article/details/gozqbrmqd.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.hesvh.cn/Article/details/gukhpfmwm.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/gpdezxvdt.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/grlquiyah.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gqppqjqrk.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.fehbvm.com/Article/details/gdostvzfv.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.zdbjq.cn/Article/details/gdprimaxd.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.fehbvm.com/Article/details/gtsfrejqc.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.hesvh.cn/Article/details/gmczhurva.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fehbvm.com/Article/details/gljxxajyw.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gorladmru.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/gefucnaju.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gfoheltxb.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.hesvh.cn/Article/details/giqmtxzcy.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.zdbjq.cn/Article/details/gctrqefhd.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.fehbvm.com/Article/details/geljbcvuv.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/ghoxhfhis.sHtML

[F04] 追加写入文件
来源：http://www.blog.zdbjq.cn/Article/details/gtmdbwlsz.sHtML


<!-- 参考信息 -->