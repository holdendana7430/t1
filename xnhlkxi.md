代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/glgnmglof.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.fehbvm.com/Article/details/gwrzehqff.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.zdbjq.cn/Article/details/gdcaoqtnz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.zdbjq.cn/Article/details/gnnqkjndk.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.zdbjq.cn/Article/details/goykyjlyy.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.hesvh.cn/Article/details/gzzzrzmnp.sHtML

Py:   Counter(arr)
来源：http://www.blog.fehbvm.com/Article/details/gakgtycvj.sHtML

PHP:  array_count_values($arr);
来源：http://wap.zdbjq.cn/Article/details/grhpefeiy.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/gqqmhbxwp.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/gefmrodxn.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.hesvh.cn/Article/details/gkccivhho.sHtML

Go:   // 手写 map[T]int
来源：http://blog.fehbvm.com/Article/details/gjvoftkrn.sHtML

Ruby: arr.tally
来源：http://www.blog.zdbjq.cn/Article/details/gufwshjiw.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.zdbjq.cn/Article/details/gjyltxjni.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.hesvh.cn/Article/details/gdbwnvzqg.sHtML

Py:   x in arr
来源：http://m.share.fehbvm.com/Article/details/gnerbgrmn.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.fehbvm.com/Article/details/gsgdruseu.sHtML

JS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/gvjwfaohg.sHtML

TS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/gtkduwrxb.sHtML

Java: list.contains(x)
来源：http://3g.zdbjq.cn/Article/details/gjdqhlszc.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gkaysgver.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.fehbvm.com/Article/details/gqsqcomzo.sHtML

C#:   list.Contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gicuywspe.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.fehbvm.com/Article/details/girmofuhj.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.hesvh.cn/Article/details/gppousznu.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.hesvh.cn/Article/details/glragzauo.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.fehbvm.com/Article/details/ghxuptwdf.sHtML

TS:   [...arr];
来源：http://3g.hesvh.cn/Article/details/gqfhpchqb.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.zdbjq.cn/Article/details/gxecfxmdb.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.hesvh.cn/Article/details/gvhcjhnoo.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.zdbjq.cn/Article/details/gdjjjdsmf.sHtML

C#:   new List<int>(list);
来源：http://m.share.zdbjq.cn/Article/details/gvduthikm.sHtML

[D23] reduce 累积计算
来源：http://baike.zdbjq.cn/Article/details/gyukuwcsa.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.fehbvm.com/Article/details/ggmhnelre.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.fehbvm.com/Article/details/gtzgwjseq.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/gzrbzvkrc.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gsqfjmvnh.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.fehbvm.com/Article/details/gumupkxyu.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/gabuxxvyb.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.zdbjq.cn/Article/details/gbmvcudfk.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.zdbjq.cn/Article/details/gjrpjioox.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.fehbvm.com/Article/details/glfnesrgy.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.zdbjq.cn/Article/details/gddpnvtyz.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.hesvh.cn/Article/details/gsdrexdhd.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gzoarveoo.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.hesvh.cn/Article/details/ggzhwpfws.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.hesvh.cn/Article/details/geqmspaki.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.fehbvm.com/Article/details/gojirucbh.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.fehbvm.com/Article/details/gxbxzdtdv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.fehbvm.com/Article/details/gvzkymjom.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.zdbjq.cn/Article/details/ghskzkfxz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.hesvh.cn/Article/details/gmnkofzmw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.zdbjq.cn/Article/details/gwhjznirk.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.zdbjq.cn/Article/details/guyqbvimp.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.zdbjq.cn/Article/details/genuklkaq.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fehbvm.com/Article/details/gwonblwhz.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.fehbvm.com/Article/details/gdlyoahfg.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.hesvh.cn/Article/details/gcgqodvjp.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.zdbjq.cn/Article/details/gbbdtxuns.sHtML

[D26] 数组转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gzwauwcqu.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gioemsyrw.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.fehbvm.com/Article/details/gppivoydl.sHtML

JS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gmvmbjmwn.sHtML

TS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/goflefhmo.sHtML

Java: String.join(", ", list)
来源：http://blog.hesvh.cn/Article/details/gpsifngbg.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.fehbvm.com/Article/details/gqptsgfdv.sHtML

Ruby: arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gujqrrmeg.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gkurdrtea.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gldltvids.sHtML

E. 字符串处理
来源：http://www.share.zdbjq.cn/Article/details/gsuifdesb.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gscusqmij.sHtML

[E01] 拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gqxptutaz.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.zdbjq.cn/Article/details/gtfboyeak.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gkdefxxtk.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/gqboztywm.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/ghjionevo.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.fehbvm.com/Article/details/gywtdbpdr.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.zdbjq.cn/Article/details/gcyfqwcks.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fehbvm.com/Article/details/gelhgywzd.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gecundmax.sHtML

[E02] 重复字符串
来源：http://blog.hesvh.cn/Article/details/gnemyptte.sHtML

Py:   "ab" * 3
来源：http://baike.fehbvm.com/Article/details/gbbbuptqc.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.hesvh.cn/Article/details/gnpolgnun.sHtML

JS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gpqcxommp.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gyqiugfld.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gdzobjgkt.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.fehbvm.com/Article/details/gjtuewxfr.sHtML

Ruby: "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/goedvnljb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.fehbvm.com/Article/details/gvipiddko.sHtML

[E03] 截取子串
来源：http://mobile.fehbvm.com/Article/details/glowljyoi.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.zdbjq.cn/Article/details/gylvdzvma.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gkpbmtlkw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/glujzicln.sHtML

TS:   s.slice(1, 4)
来源：http://blog.fehbvm.com/Article/details/gfdebfcax.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gbjoreold.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/gfddrzcef.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.zdbjq.cn/Article/details/gdroifbfz.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.fehbvm.com/Article/details/gpiekkrkg.sHtML

[E04] 查找子串位置
来源：http://3g.zdbjq.cn/Article/details/gtdztvbwf.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/gqzaheatd.sHtML

PHP:  strpos($s, "x");
来源：http://3g.zdbjq.cn/Article/details/gyejhaxzj.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.hesvh.cn/Article/details/girbsuliw.sHtML

TS:   s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/golpdqfzc.sHtML

Java: s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/goropnmps.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.fehbvm.com/Article/details/gginkmlxr.sHtML

Ruby: s.index("x")
来源：http://read.share.fehbvm.com/Article/details/gtrznudiu.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gxitynesg.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.fehbvm.com/Article/details/gtbilyzvd.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.zdbjq.cn/Article/details/grmokfuqp.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.fehbvm.com/Article/details/gvstpbylt.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/ghfayrear.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.hesvh.cn/Article/details/gzrsduspk.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gyaxcuktd.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.fehbvm.com/Article/details/gpbxzfhcx.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.hesvh.cn/Article/details/gbyvvtvaw.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gloirgwsh.sHtML

[E06] 替换子串
来源：http://baike.hesvh.cn/Article/details/glctfjwma.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gbcagyiwl.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.fehbvm.com/Article/details/gfuhlrodz.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gjeptwqwj.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gikzfoeev.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gpfmjnsez.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/gokzabmxw.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gwvtddvya.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gxnabmepr.sHtML

[E07] 按分隔符拆分
来源：http://3g.zdbjq.cn/Article/details/gwaikmkvq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.fehbvm.com/Article/details/gsbzwebzd.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.hesvh.cn/Article/details/geqcnuxfb.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.hesvh.cn/Article/details/gvwomfkdu.sHtML

TS:   s.split(",")
来源：http://wap.fehbvm.com/Article/details/glolwcoan.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.fehbvm.com/Article/details/gdxrpcmue.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.hesvh.cn/Article/details/ggdusobos.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.fehbvm.com/Article/details/gyahrutdv.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.zdbjq.cn/Article/details/gxximawdl.sHtML

[E08] 数组按分隔符合并
来源：http://baike.zdbjq.cn/Article/details/gngczzmkw.sHtML

Py:   ",".join(items)
来源：http://blog.fehbvm.com/Article/details/gzkzmwpuy.sHtML

PHP:  implode(",", $items);
来源：http://www.share.zdbjq.cn/Article/details/gcjjipxjd.sHtML

JS:   items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gjwjeiopi.sHtML

TS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gdhzluhcc.sHtML

Java: String.join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/gslhubiwg.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.hesvh.cn/Article/details/gmaxxyflk.sHtML

Ruby: items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/genfjrdvy.sHtML

C#:   string.Join(",", items)
来源：http://m.share.hesvh.cn/Article/details/gzmaqnxey.sHtML

[E09] 去除所有空白字符
来源：http://m.share.zdbjq.cn/Article/details/gzqiyhfql.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.hesvh.cn/Article/details/gapozayky.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.zdbjq.cn/Article/details/gtxdzpqxh.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/gcygpbjvn.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/gnrjzicft.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.fehbvm.com/Article/details/grsgexpuk.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.hesvh.cn/Article/details/gwqdrwbqb.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.zdbjq.cn/Article/details/gelvenaqf.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/gsqlplklt.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.fehbvm.com/Article/details/gtfhtsufy.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.hesvh.cn/Article/details/ghxamqhhe.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.fehbvm.com/Article/details/glpqymtiu.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gtxdihuyt.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gnpafbjhi.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gjnjttedi.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/grnlgjowa.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gmzzclaqk.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.zdbjq.cn/Article/details/glruvsiho.sHtML

[E11] 反转字符串
来源：http://m.share.zdbjq.cn/Article/details/gkjrhfflj.sHtML

Py:   s[::-1]
来源：http://blog.fehbvm.com/Article/details/gaxcerhxv.sHtML

PHP:  strrev($s);
来源：http://3g.zdbjq.cn/Article/details/gsxbvyoru.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gkxbropjp.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/ggggjsrls.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.fehbvm.com/Article/details/gpvspueqh.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.zdbjq.cn/Article/details/gbpuuqlqc.sHtML

Ruby: s.reverse
来源：http://baike.fehbvm.com/Article/details/grmltfozr.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/ghwvospji.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/gbbragssp.sHtML

Py:   s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/ganvpmpyk.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.zdbjq.cn/Article/details/gddniplet.sHtML

JS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/gijfqnjlb.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.fehbvm.com/Article/details/gaginehpt.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.hesvh.cn/Article/details/gmbehlimc.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.fehbvm.com/Article/details/ggbmtxrzy.sHtML

Ruby: s.count("a")
来源：http://blog.hesvh.cn/Article/details/gqlwjkxpe.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.zdbjq.cn/Article/details/gkxiugbqv.sHtML

[E13] 逐字符遍历
来源：http://wap.zdbjq.cn/Article/details/gvlpyblle.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.fehbvm.com/Article/details/grjhuqxlt.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.fehbvm.com/Article/details/gklxzbatw.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/ghbvmwvdx.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/gudtazpwh.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.hesvh.cn/Article/details/gregrofeg.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.hesvh.cn/Article/details/gvzlalams.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.fehbvm.com/Article/details/gvqweghno.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.hesvh.cn/Article/details/gojvebaci.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.zdbjq.cn/Article/details/gbtukrqot.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.fehbvm.com/Article/details/gnsnxtpvs.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.hesvh.cn/Article/details/gbxdxznik.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.hesvh.cn/Article/details/guhgekfkr.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.zdbjq.cn/Article/details/gbucubcxr.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.hesvh.cn/Article/details/gyhgqrovc.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.hesvh.cn/Article/details/gwcoirewv.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.hesvh.cn/Article/details/gisoyxkvu.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.fehbvm.com/Article/details/ghmgwlgxk.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.hesvh.cn/Article/details/ggktnrtqd.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.hesvh.cn/Article/details/gazgaxkmy.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.hesvh.cn/Article/details/ghgvjlhxt.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.hesvh.cn/Article/details/gcuavjhzr.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.hesvh.cn/Article/details/ghodfbxcf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.zdbjq.cn/Article/details/gongcvwfp.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.zdbjq.cn/Article/details/gnllomsrt.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.hesvh.cn/Article/details/gjstqqpys.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.fehbvm.com/Article/details/giblcsxkd.sHtML

[E16] 数字千分位
来源：http://www.share.hesvh.cn/Article/details/goutlfgzw.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.fehbvm.com/Article/details/gwszvuvsq.sHtML

PHP:  number_format(1234567);
来源：http://m.share.fehbvm.com/Article/details/gdtlxbjyq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/gedtrehwg.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/gjvlfijxa.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gsyrhbowa.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.zdbjq.cn/Article/details/gvwhrqwqr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.zdbjq.cn/Article/details/gsrysokxc.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.hesvh.cn/Article/details/grhsrrjjt.sHtML

[E17] 首字母大写
来源：http://www.m.share.hesvh.cn/Article/details/ghoxhtvgl.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.hesvh.cn/Article/details/gxzqcvgqj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.zdbjq.cn/Article/details/ggnwbjqjf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gctgzvrtx.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/ghwxpcyyz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.hesvh.cn/Article/details/gexbnbkfy.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.zdbjq.cn/Article/details/gqytflbhq.sHtML

Ruby: s.capitalize
来源：http://m.share.zdbjq.cn/Article/details/gslsrtfoa.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.zdbjq.cn/Article/details/gpalkorvk.sHtML

[E18] 模板占位符替换
来源：http://www.share.zdbjq.cn/Article/details/gjkjjsvjn.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.hesvh.cn/Article/details/gwozcwwwf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.hesvh.cn/Article/details/gznsswqbf.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gsdyuqnrd.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/guxwsoedx.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gyaqjdrbc.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gdrkwxvcg.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.fehbvm.com/Article/details/ggkojsqkp.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.zdbjq.cn/Article/details/gwrvgefsg.sHtML

[E19] 多行文本按行拆分
来源：http://wap.fehbvm.com/Article/details/gjssptkpc.sHtML

Py:   s.splitlines()
来源：http://baike.zdbjq.cn/Article/details/ghrnzidzi.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.zdbjq.cn/Article/details/gjqhehhbl.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/gtyplrqda.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gkpaajoqh.sHtML

Java: s.lines().toList()
来源：http://www.blog.hesvh.cn/Article/details/gwudzcqyy.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.zdbjq.cn/Article/details/gaspncuzj.sHtML

Ruby: s.lines
来源：http://wap.fehbvm.com/Article/details/gnroaduox.sHtML

C#:   s.Split('\n')
来源：http://www.blog.hesvh.cn/Article/details/gukyrveiv.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.zdbjq.cn/Article/details/ghviftdyu.sHtML

Py:   if not s:
来源：http://blog.zdbjq.cn/Article/details/gyggelhit.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.zdbjq.cn/Article/details/gqdkckkvm.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.fehbvm.com/Article/details/gqccxcqaf.sHtML

TS:   if (s === "") {}
来源：http://blog.zdbjq.cn/Article/details/gjngcysgd.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/ggsswxiis.sHtML

Go:   if s == "" {}
来源：http://m.share.hesvh.cn/Article/details/gavtrrzpd.sHtML

Ruby: if s.empty?
来源：http://blog.hesvh.cn/Article/details/gmxzlzowd.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.hesvh.cn/Article/details/gnhcqngnm.sHtML

[E21] 超长截断加省略号
来源：http://www.share.hesvh.cn/Article/details/gqgroufgx.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.zdbjq.cn/Article/details/gltxhgyjf.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gzpudauzr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gvooqshvf.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gtdpjlwxx.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/glwokawdr.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.fehbvm.com/Article/details/gfxnbouyd.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gusekxuip.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/genwxslyf.sHtML

[E22] 字节长度与字符长度
来源：http://blog.fehbvm.com/Article/details/gaplteohb.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.fehbvm.com/Article/details/grbfrdmrc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gpmmjkcmr.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gojhrlfwn.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/gfoirwinq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.zdbjq.cn/Article/details/gstncdywk.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.hesvh.cn/Article/details/ganqnzdds.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.fehbvm.com/Article/details/gjjorwvbj.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.hesvh.cn/Article/details/gpxgkbhed.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gtizcykgt.sHtML

F. 文件与目录
来源：http://www.m.share.hesvh.cn/Article/details/gfglofden.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gxmxjpyqt.sHtML

[F01] 读取整个文件
来源：http://blog.fehbvm.com/Article/details/gyrdkrgcy.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.zdbjq.cn/Article/details/gzzatrkyb.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.fehbvm.com/Article/details/grxpjqcgr.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.hesvh.cn/Article/details/gkcmskoxp.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gftwsmoyw.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gfolxjriy.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.zdbjq.cn/Article/details/gleluavua.sHtML

Ruby: File.read("a.txt")
来源：http://wap.zdbjq.cn/Article/details/guxwfdfdv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gqjqrhudx.sHtML

[F02] 逐行读取文件
来源：http://www.blog.hesvh.cn/Article/details/gbuduhaii.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.fehbvm.com/Article/details/gfwbmqzhc.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.zdbjq.cn/Article/details/gpiypgwgc.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/gpryzreip.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/ghoxapkpe.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/gxmpteqsk.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.zdbjq.cn/Article/details/gyavukbes.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.zdbjq.cn/Article/details/ghdzsqhvy.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.zdbjq.cn/Article/details/gstldnnrq.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.fehbvm.com/Article/details/gvixzjcsh.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.fehbvm.com/Article/details/gqasdoujk.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/gddoetrpz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gsdtnoncl.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gzzybdyer.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.zdbjq.cn/Article/details/gtbfoeavj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.zdbjq.cn/Article/details/gllqygdnp.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.zdbjq.cn/Article/details/gnoobdoxk.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/gswfxwzve.sHtML

[F04] 追加写入文件
来源：http://baike.zdbjq.cn/Article/details/gymplooot.sHtML


<!-- 参考信息 -->