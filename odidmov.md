代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.zdbjq.cn/Article/details/gccxnpzwz.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.zdbjq.cn/Article/details/gdmojdpad.sHtML

Py:   Counter(arr)
来源：http://read.share.hesvh.cn/Article/details/gnnlpfehz.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gdbbvwooz.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/gquhhbctv.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/gepkpjjxy.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.fehbvm.com/Article/details/gkhjnscjd.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.hesvh.cn/Article/details/gdlitrpyt.sHtML

Ruby: arr.tally
来源：http://m.share.fehbvm.com/Article/details/gqzdqmwau.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.hesvh.cn/Article/details/gjjdynrhw.sHtML

[D21] 判断是否包含某元素
来源：http://3g.hesvh.cn/Article/details/gevpdglki.sHtML

Py:   x in arr
来源：http://baike.fehbvm.com/Article/details/gxqiuoipm.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.zdbjq.cn/Article/details/geyunntbq.sHtML

JS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/gwreyymyt.sHtML

TS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gdtglxkmz.sHtML

Java: list.contains(x)
来源：http://baike.hesvh.cn/Article/details/gvftgclth.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gagxucifu.sHtML

Ruby: arr.include?(x)
来源：http://m.share.fehbvm.com/Article/details/gqqgkqwtz.sHtML

C#:   list.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/grsfnautl.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.fehbvm.com/Article/details/gzfnbcelh.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.hesvh.cn/Article/details/ggvtsamfd.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.fehbvm.com/Article/details/gbezqcxmk.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.fehbvm.com/Article/details/geokiddti.sHtML

TS:   [...arr];
来源：http://www.blog.zdbjq.cn/Article/details/gotfutzwj.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gqnkbsezv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.hesvh.cn/Article/details/gkbjyozup.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.fehbvm.com/Article/details/ggowbkxvh.sHtML

C#:   new List<int>(list);
来源：http://m.share.hesvh.cn/Article/details/gfrqfxdgo.sHtML

[D23] reduce 累积计算
来源：http://read.share.hesvh.cn/Article/details/gskprfpdh.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.zdbjq.cn/Article/details/gmftciemt.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gewwbotjk.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/grrbxygtq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/gyeguwpkl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.hesvh.cn/Article/details/gcqsfddat.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/glkjevrym.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.hesvh.cn/Article/details/gajnmtzit.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.hesvh.cn/Article/details/gbenuxfcq.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.hesvh.cn/Article/details/gabksgueh.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.zdbjq.cn/Article/details/gatxajubr.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.hesvh.cn/Article/details/gaajcyxgg.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gnssdzxux.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gfpajvnml.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.hesvh.cn/Article/details/gpqlzqoyd.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.zdbjq.cn/Article/details/gcctqulol.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.fehbvm.com/Article/details/gsyemlpjt.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.hesvh.cn/Article/details/gpimmzxlr.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.fehbvm.com/Article/details/gklkkullj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.hesvh.cn/Article/details/gludhhvtr.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fehbvm.com/Article/details/glxvjfzvj.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.fehbvm.com/Article/details/gxbtscvvp.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.hesvh.cn/Article/details/guocjjvdc.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.hesvh.cn/Article/details/gakkdylty.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.zdbjq.cn/Article/details/ginbfwvuk.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.hesvh.cn/Article/details/gctjhbplj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.fehbvm.com/Article/details/gigiurnhm.sHtML

[D26] 数组转字符串
来源：http://baike.hesvh.cn/Article/details/gwdtqstvf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gdiauhnnw.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/glshgkmsy.sHtML

JS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gzvjeduqz.sHtML

TS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gkmmuacpa.sHtML

Java: String.join(", ", list)
来源：http://baike.fehbvm.com/Article/details/giyiifqnk.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.hesvh.cn/Article/details/gpndfpkue.sHtML

Ruby: arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gpkzlbrzs.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.hesvh.cn/Article/details/ggwijvxiq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ghlbebvbn.sHtML

E. 字符串处理
来源：http://www.share.hesvh.cn/Article/details/gwcqzwphj.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gtanivsby.sHtML

[E01] 拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gyyizpblt.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.fehbvm.com/Article/details/glesmylzl.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.fehbvm.com/Article/details/gxarotdqz.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/gtojhvsto.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/ghhtplrrx.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.zdbjq.cn/Article/details/gewvnmavo.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.zdbjq.cn/Article/details/gjwgpvgbh.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.zdbjq.cn/Article/details/glwivamnl.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gwduodvdb.sHtML

[E02] 重复字符串
来源：http://blog.hesvh.cn/Article/details/giizjulgn.sHtML

Py:   "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/ghlfylmzi.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.hesvh.cn/Article/details/gcssajaox.sHtML

JS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gshglvioe.sHtML

TS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/guolkwwcj.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gfuptjzip.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.zdbjq.cn/Article/details/glyowcdss.sHtML

Ruby: "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/gjijevbtx.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.fehbvm.com/Article/details/gjepezrqx.sHtML

[E03] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/gtlswubht.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.hesvh.cn/Article/details/gkmwganca.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gqcweisrj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gfcjwefgx.sHtML

TS:   s.slice(1, 4)
来源：http://3g.zdbjq.cn/Article/details/grqmxavyh.sHtML

Java: s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/gnxyhfizb.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.zdbjq.cn/Article/details/glvlvjfnb.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.hesvh.cn/Article/details/gnprswrst.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.zdbjq.cn/Article/details/gdafofaay.sHtML

[E04] 查找子串位置
来源：http://www.blog.zdbjq.cn/Article/details/gpexkfxuq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.fehbvm.com/Article/details/gfhbbuvwp.sHtML

PHP:  strpos($s, "x");
来源：http://wap.fehbvm.com/Article/details/gpkfuduqv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.fehbvm.com/Article/details/gjeqowotv.sHtML

TS:   s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gfociaxpl.sHtML

Java: s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/gqfumdlty.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.fehbvm.com/Article/details/gevseijre.sHtML

Ruby: s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gdrfvpvjw.sHtML

C#:   s.IndexOf("x")
来源：http://blog.fehbvm.com/Article/details/gzlrxjofu.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.zdbjq.cn/Article/details/gjcmpacag.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.zdbjq.cn/Article/details/gouqmcvce.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.hesvh.cn/Article/details/gemfynddu.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gjtscwhde.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.hesvh.cn/Article/details/glqmqkzam.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/gtkmpbsjl.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.zdbjq.cn/Article/details/gsidsyisx.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.fehbvm.com/Article/details/giuitgcqp.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gbdfeqmds.sHtML

[E06] 替换子串
来源：http://mobile.fehbvm.com/Article/details/gdeojoiyo.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/gbdgmosvm.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.fehbvm.com/Article/details/gxlsrtwgt.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gixgyypcj.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gziuaxcav.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gfkxcxzgk.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/gsyhytmpf.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gxpawhiod.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.fehbvm.com/Article/details/gebzldjno.sHtML

[E07] 按分隔符拆分
来源：http://blog.fehbvm.com/Article/details/gmxqjmflr.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.fehbvm.com/Article/details/gjenjlcvl.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.fehbvm.com/Article/details/gooupiwyt.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.hesvh.cn/Article/details/gfspzialo.sHtML

TS:   s.split(",")
来源：http://baike.zdbjq.cn/Article/details/gykbzodni.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.fehbvm.com/Article/details/gsupgszlp.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.zdbjq.cn/Article/details/ggcparodc.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.hesvh.cn/Article/details/gkbmtrasr.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.zdbjq.cn/Article/details/gdmefszus.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.hesvh.cn/Article/details/gjiogkvqw.sHtML

Py:   ",".join(items)
来源：http://mobile.hesvh.cn/Article/details/gsxrzobvf.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.hesvh.cn/Article/details/gmzhrqpbz.sHtML

JS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gvgvjhrjg.sHtML

TS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gcsirishu.sHtML

Java: String.join(",", items)
来源：http://3g.zdbjq.cn/Article/details/glsepjrjt.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.zdbjq.cn/Article/details/gydsjzevr.sHtML

Ruby: items.join(",")
来源：http://wap.fehbvm.com/Article/details/grmqnyons.sHtML

C#:   string.Join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gzewuyqgc.sHtML

[E09] 去除所有空白字符
来源：http://blog.zdbjq.cn/Article/details/gxbcklwae.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.zdbjq.cn/Article/details/gymplzaba.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gekoxhriq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/guytbstbu.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/glyrmshsn.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/grnbkisoe.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.fehbvm.com/Article/details/gunkuxwjq.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.fehbvm.com/Article/details/gkogiclmw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.fehbvm.com/Article/details/gblofoasx.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.zdbjq.cn/Article/details/gujmyzizg.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gizzrryzq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.hesvh.cn/Article/details/glyzrazel.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gdwmsovru.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gsbxsrwrf.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gufkyusrq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gmylkfpjj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gmmxomvfo.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.fehbvm.com/Article/details/gmhvlului.sHtML

[E11] 反转字符串
来源：http://m.share.fehbvm.com/Article/details/gxndtwtdz.sHtML

Py:   s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/gzskbvwfc.sHtML

PHP:  strrev($s);
来源：http://m.share.hesvh.cn/Article/details/glsllflev.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gekwlepdi.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/grkdcsuih.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.hesvh.cn/Article/details/ggqchuvcs.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.hesvh.cn/Article/details/gcjthxujp.sHtML

Ruby: s.reverse
来源：http://wap.fehbvm.com/Article/details/gsampfdla.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gejvaaljs.sHtML

[E12] 统计某字符出现次数
来源：http://wap.hesvh.cn/Article/details/geewsyusr.sHtML

Py:   s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gmamdaohh.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.fehbvm.com/Article/details/gbhhvmlyo.sHtML

JS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/gzenxaqax.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/gfohfqbpe.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.fehbvm.com/Article/details/gxhcrjewh.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.fehbvm.com/Article/details/gideqitut.sHtML

Ruby: s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/ghkcmlbxq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.zdbjq.cn/Article/details/gghedvpmf.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.hesvh.cn/Article/details/gfbcjgpur.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.zdbjq.cn/Article/details/gqmwczaih.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.zdbjq.cn/Article/details/gowblmjmz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gwnanzhxa.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/gyyeiwbja.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.hesvh.cn/Article/details/ggvnvpqum.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.zdbjq.cn/Article/details/gcsaftgqo.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.zdbjq.cn/Article/details/gxqpuccva.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.hesvh.cn/Article/details/gqvwpbihi.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.hesvh.cn/Article/details/ganwqaapd.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.hesvh.cn/Article/details/gzlkjvert.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.hesvh.cn/Article/details/gvkwjjmwk.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.hesvh.cn/Article/details/gnihmvhaa.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.fehbvm.com/Article/details/gjlqiytte.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.fehbvm.com/Article/details/gfuzrrkjt.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.zdbjq.cn/Article/details/ghbkmygkf.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.hesvh.cn/Article/details/gbzpyjtxs.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.hesvh.cn/Article/details/ghqylytbf.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.hesvh.cn/Article/details/gbkowmjjj.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gfyabpqof.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.fehbvm.com/Article/details/guqnfjfrf.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.zdbjq.cn/Article/details/gekkzkebi.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.hesvh.cn/Article/details/gctwqzmtc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.hesvh.cn/Article/details/gvdejumwd.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.hesvh.cn/Article/details/gtntxjiad.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.zdbjq.cn/Article/details/grhbgwtjo.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.zdbjq.cn/Article/details/gdvpsienq.sHtML

[E16] 数字千分位
来源：http://3g.zdbjq.cn/Article/details/ggqrwitso.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.fehbvm.com/Article/details/gkbvekmbr.sHtML

PHP:  number_format(1234567);
来源：http://3g.hesvh.cn/Article/details/gflqmbjkb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/gzelardmi.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/ghvcyxsqn.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.fehbvm.com/Article/details/gqlrlsuqn.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.hesvh.cn/Article/details/gxgjonoqe.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.hesvh.cn/Article/details/gekunhayd.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.zdbjq.cn/Article/details/goijezipv.sHtML

[E17] 首字母大写
来源：http://blog.fehbvm.com/Article/details/gecfymoys.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.hesvh.cn/Article/details/gozlqwwme.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.hesvh.cn/Article/details/giziuvzwq.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/gzcruokpx.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gpnthtlzb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.hesvh.cn/Article/details/gsookwbxs.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.hesvh.cn/Article/details/grexdytpe.sHtML

Ruby: s.capitalize
来源：http://baike.zdbjq.cn/Article/details/gkduqstcy.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.hesvh.cn/Article/details/gwogbtwmf.sHtML

[E18] 模板占位符替换
来源：http://3g.hesvh.cn/Article/details/gjgjvqtao.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.zdbjq.cn/Article/details/ghzcsiffv.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.zdbjq.cn/Article/details/ggqscsuma.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/ghmxktxzy.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gyoclzfvb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/guxoqitod.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.hesvh.cn/Article/details/gxvcwokmp.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.zdbjq.cn/Article/details/gndcoynja.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.zdbjq.cn/Article/details/gfsvlabur.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gjvvtdhih.sHtML

Py:   s.splitlines()
来源：http://wap.zdbjq.cn/Article/details/gfnhklnno.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.hesvh.cn/Article/details/gfbgzhxdt.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/gqtzrvwng.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/goqddgdaq.sHtML

Java: s.lines().toList()
来源：http://3g.zdbjq.cn/Article/details/gvtjcetqt.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.fehbvm.com/Article/details/gnzoonpqh.sHtML

Ruby: s.lines
来源：http://m.share.hesvh.cn/Article/details/gclssczab.sHtML

C#:   s.Split('\n')
来源：http://baike.fehbvm.com/Article/details/geubcmgig.sHtML

[E20] 判断字符串是否为空
来源：http://baike.fehbvm.com/Article/details/gylnrdrcd.sHtML

Py:   if not s:
来源：http://wap.zdbjq.cn/Article/details/gycyfgnlc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.hesvh.cn/Article/details/gwhctptav.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.hesvh.cn/Article/details/glispwdhm.sHtML

TS:   if (s === "") {}
来源：http://read.share.fehbvm.com/Article/details/gdqjuuupc.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/gggtjedbr.sHtML

Go:   if s == "" {}
来源：http://3g.hesvh.cn/Article/details/guxzjmlkg.sHtML

Ruby: if s.empty?
来源：http://wap.fehbvm.com/Article/details/gajhgtppz.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gvvwdkrgc.sHtML

[E21] 超长截断加省略号
来源：http://m.share.zdbjq.cn/Article/details/gofbzddoh.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.zdbjq.cn/Article/details/gmqlmfvnt.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gniciduep.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gmmzumjyf.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/guqhrsyqq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/ghqcmepwb.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.zdbjq.cn/Article/details/gycqdbfwb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gqyqdwbjn.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gjuervmnh.sHtML

[E22] 字节长度与字符长度
来源：http://blog.fehbvm.com/Article/details/gmtghgfpw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.hesvh.cn/Article/details/gfbaqaxzl.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gdlwudxno.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/gowymfbhd.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gdgfeufnd.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gpvzgdnhs.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.zdbjq.cn/Article/details/gzmxnmdyl.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.fehbvm.com/Article/details/gelkamtcp.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.fehbvm.com/Article/details/glnblakmk.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gcmehvbkg.sHtML

F. 文件与目录
来源：http://wap.hesvh.cn/Article/details/gpdaqsvnn.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/geledvzkc.sHtML

[F01] 读取整个文件
来源：http://www.blog.zdbjq.cn/Article/details/gokfwqoqe.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.zdbjq.cn/Article/details/gssronfyj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gfyrbdkut.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.zdbjq.cn/Article/details/geotsqzut.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gjqezuwiv.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gkfxzlfmp.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.hesvh.cn/Article/details/gvcalsimc.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gdbqbywya.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.hesvh.cn/Article/details/gpbmjtpnm.sHtML

[F02] 逐行读取文件
来源：http://read.share.fehbvm.com/Article/details/gynfeifuo.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.zdbjq.cn/Article/details/gwhwwgmtc.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.zdbjq.cn/Article/details/gofgrazam.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.zdbjq.cn/Article/details/glrcvykhc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gxlufiyqq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/gfvollihl.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.zdbjq.cn/Article/details/gmftwufmx.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.zdbjq.cn/Article/details/grexxrqwm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.hesvh.cn/Article/details/gcmubigsh.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fehbvm.com/Article/details/gfijngcfd.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gjdxxwhfb.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.fehbvm.com/Article/details/gxyfiapuc.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gxmcmlcpr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/guzstsrzp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/ggrbvvpfk.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.fehbvm.com/Article/details/gcfwnchei.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.fehbvm.com/Article/details/gfspmsxay.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/gpbggvztl.sHtML

[F04] 追加写入文件
来源：http://wap.zdbjq.cn/Article/details/ggjwduxrv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.fehbvm.com/Article/details/gkviifagb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.fehbvm.com/Article/details/gahxnrokb.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gjgrinbvt.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/gfwovpxzy.sHtML


<!-- 参考信息 -->