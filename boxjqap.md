代发 wailian999

[D19] 按字段分组
来源：http://baike.zdbjq.cn/Article/details/gncaxhlrq.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.fehbvm.com/Article/details/gkcmknlvx.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.fehbvm.com/Article/details/glnxlritp.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.zdbjq.cn/Article/details/gyokhwnvs.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/gjjybzmqs.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.zdbjq.cn/Article/details/gtzpopjnm.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.fehbvm.com/Article/details/gktawbgfe.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.hesvh.cn/Article/details/gbcvvcyqe.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.zdbjq.cn/Article/details/gqnuoziil.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gamihdgal.sHtML

Py:   Counter(arr)
来源：http://read.share.zdbjq.cn/Article/details/gaxztskyf.sHtML

PHP:  array_count_values($arr);
来源：http://wap.fehbvm.com/Article/details/glrrdkisb.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gfsdplpzx.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/guflzbqcb.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.zdbjq.cn/Article/details/gkduxqzdc.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.zdbjq.cn/Article/details/gqnxuxcce.sHtML

Ruby: arr.tally
来源：http://3g.fehbvm.com/Article/details/gvvdupiwc.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.zdbjq.cn/Article/details/gkmkmqfxr.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.fehbvm.com/Article/details/gxegzvdcw.sHtML

Py:   x in arr
来源：http://baike.zdbjq.cn/Article/details/gteynvupg.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.fehbvm.com/Article/details/gxoxzecvm.sHtML

JS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/gkvttexsa.sHtML

TS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/gpbztzoaw.sHtML

Java: list.contains(x)
来源：http://blog.fehbvm.com/Article/details/gxssusawb.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gwdwlfxob.sHtML

Ruby: arr.include?(x)
来源：http://wap.fehbvm.com/Article/details/gckcvttia.sHtML

C#:   list.Contains(x)
来源：http://baike.fehbvm.com/Article/details/gfeutljlm.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.zdbjq.cn/Article/details/glbgmxdqx.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.zdbjq.cn/Article/details/gukqafqsg.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.fehbvm.com/Article/details/gttyiaeyd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.fehbvm.com/Article/details/gmhhahoho.sHtML

TS:   [...arr];
来源：http://wap.hesvh.cn/Article/details/gsqayxuma.sHtML

Java: new ArrayList<>(list);
来源：http://wap.fehbvm.com/Article/details/giitccewu.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.hesvh.cn/Article/details/gcatouvly.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.zdbjq.cn/Article/details/gviymhlmc.sHtML

C#:   new List<int>(list);
来源：http://wap.fehbvm.com/Article/details/ggabzgssv.sHtML

[D23] reduce 累积计算
来源：http://www.share.hesvh.cn/Article/details/gncwrxzrb.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.zdbjq.cn/Article/details/grlmzwxyl.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.hesvh.cn/Article/details/gecvjcern.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/griceciby.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gjakezmrh.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.zdbjq.cn/Article/details/ghrnfjhzu.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/gdmbyujja.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.zdbjq.cn/Article/details/gibhnsswl.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.hesvh.cn/Article/details/ginbutaje.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.fehbvm.com/Article/details/gwxnkuwao.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.hesvh.cn/Article/details/gdpcdoxah.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.fehbvm.com/Article/details/gouqzvesg.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.hesvh.cn/Article/details/gazqngzeq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gfrvqpdjk.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.fehbvm.com/Article/details/gysljyxdw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.hesvh.cn/Article/details/gnmfncpav.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.hesvh.cn/Article/details/glnlfxtax.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.fehbvm.com/Article/details/gbstldkmq.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.hesvh.cn/Article/details/gpmqtxapd.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.hesvh.cn/Article/details/glufughxo.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.fehbvm.com/Article/details/guhqbvmif.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.fehbvm.com/Article/details/gywevgrty.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.zdbjq.cn/Article/details/gcdxcoksy.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.hesvh.cn/Article/details/gxjtibyhx.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.zdbjq.cn/Article/details/gneeywizy.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.fehbvm.com/Article/details/gfyjidtik.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.hesvh.cn/Article/details/gjiefhwnd.sHtML

[D26] 数组转字符串
来源：http://www.share.hesvh.cn/Article/details/gqspsqfcq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.zdbjq.cn/Article/details/gvhtrkzff.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.zdbjq.cn/Article/details/gqlftbfhb.sHtML

JS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gyygsyccx.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gtqrxzszw.sHtML

Java: String.join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/guzxgkwru.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.zdbjq.cn/Article/details/gbliyyehg.sHtML

Ruby: arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/guwicpkmp.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gxiyqxgbd.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqgecaodt.sHtML

E. 字符串处理
来源：http://read.share.fehbvm.com/Article/details/gporoqtks.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gpyeszvyu.sHtML

[E01] 拼接字符串
来源：http://blog.fehbvm.com/Article/details/gibmzdfda.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.zdbjq.cn/Article/details/gcnrniqin.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.hesvh.cn/Article/details/gvxgdrqch.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.hesvh.cn/Article/details/glwqbjtjy.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/gmkncqudn.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.hesvh.cn/Article/details/gfiobrnnh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.fehbvm.com/Article/details/gsieegfej.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.hesvh.cn/Article/details/ghtzegskr.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gmagurxez.sHtML

[E02] 重复字符串
来源：http://3g.hesvh.cn/Article/details/gtdcxhcjn.sHtML

Py:   "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gjoqfnqlr.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.zdbjq.cn/Article/details/gwzxbwfay.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/geeunnkdz.sHtML

TS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gszzszzba.sHtML

Java: "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gofrouimb.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.zdbjq.cn/Article/details/geoqepnmx.sHtML

Ruby: "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/gdqknjugi.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.hesvh.cn/Article/details/gxbbsivon.sHtML

[E03] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gevvblswy.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.zdbjq.cn/Article/details/gxgalfytp.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/glxzyfuwj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/goqunxrpx.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.hesvh.cn/Article/details/giaizdczq.sHtML

Java: s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gyugrgnxr.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.zdbjq.cn/Article/details/gzfgavqry.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.zdbjq.cn/Article/details/gtfyjgima.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.fehbvm.com/Article/details/gonikrppd.sHtML

[E04] 查找子串位置
来源：http://read.share.fehbvm.com/Article/details/geeptodpo.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gbsqphxhd.sHtML

PHP:  strpos($s, "x");
来源：http://baike.zdbjq.cn/Article/details/gaolgrwqj.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.zdbjq.cn/Article/details/gtqakvmxx.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gdmwcjlyi.sHtML

Java: s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gqjqhbmee.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.hesvh.cn/Article/details/gcmkdyznz.sHtML

Ruby: s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gtxhnyeir.sHtML

C#:   s.IndexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gvbjtkice.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.zdbjq.cn/Article/details/gnbxviani.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.fehbvm.com/Article/details/gogkjfgas.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.hesvh.cn/Article/details/gnsfzgxzu.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gleptzcvr.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.zdbjq.cn/Article/details/gyqctzicb.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gtobhwguo.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.fehbvm.com/Article/details/gefzthgvx.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.zdbjq.cn/Article/details/gxhzemqgj.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gcssixdpn.sHtML

[E06] 替换子串
来源：http://www.blog.fehbvm.com/Article/details/gnulxejnt.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/gmrcngzbp.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.fehbvm.com/Article/details/gkimbqart.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gsztvjuax.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gqgpltzri.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gcairwvet.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/gwzrnhair.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.hesvh.cn/Article/details/gnxviakes.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gpllqxkal.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.fehbvm.com/Article/details/gtpewcavo.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.fehbvm.com/Article/details/gylyvhxoo.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.fehbvm.com/Article/details/gcrezrqnz.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.hesvh.cn/Article/details/gaysggvmt.sHtML

TS:   s.split(",")
来源：http://3g.zdbjq.cn/Article/details/giyfewnzk.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.fehbvm.com/Article/details/gzfdaxraf.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.fehbvm.com/Article/details/gtpllpedw.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.fehbvm.com/Article/details/gvjfsuhrc.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.hesvh.cn/Article/details/gkdkctsyn.sHtML

[E08] 数组按分隔符合并
来源：http://blog.zdbjq.cn/Article/details/giiptkovc.sHtML

Py:   ",".join(items)
来源：http://read.share.hesvh.cn/Article/details/gpzblniiu.sHtML

PHP:  implode(",", $items);
来源：http://m.share.zdbjq.cn/Article/details/gagglgsvw.sHtML

JS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gmtenglxp.sHtML

TS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gtzlmokns.sHtML

Java: String.join(",", items)
来源：http://m.share.fehbvm.com/Article/details/gjccqmqhi.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.zdbjq.cn/Article/details/gmvrevekn.sHtML

Ruby: items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gbmzmvmia.sHtML

C#:   string.Join(",", items)
来源：http://wap.hesvh.cn/Article/details/gnmubdpfc.sHtML

[E09] 去除所有空白字符
来源：http://read.share.fehbvm.com/Article/details/ggkalypbu.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.hesvh.cn/Article/details/gthmabfmr.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.fehbvm.com/Article/details/gffqpahwa.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/gfgbvblue.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/ghcigeboq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.hesvh.cn/Article/details/gmejgzqot.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.fehbvm.com/Article/details/gbofbfyua.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.hesvh.cn/Article/details/gmhcxhddr.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gsdilkdsc.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.hesvh.cn/Article/details/gvsytjkzb.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gvddpawul.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.fehbvm.com/Article/details/ggvpxbzxa.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gtalcxyfg.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/glqkjbwoe.sHtML

Java: String.format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gtprrsiuq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gxqxllzky.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/ghtpxdzuu.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.fehbvm.com/Article/details/gxiqeddgv.sHtML

[E11] 反转字符串
来源：http://3g.fehbvm.com/Article/details/gwsmwnncn.sHtML

Py:   s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/grutwziqq.sHtML

PHP:  strrev($s);
来源：http://read.share.fehbvm.com/Article/details/gxljhjqiv.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gwczcwhdr.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gvkefzfal.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.hesvh.cn/Article/details/gkyehwczw.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.hesvh.cn/Article/details/gwebvnwcg.sHtML

Ruby: s.reverse
来源：http://baike.hesvh.cn/Article/details/ghuvjegpl.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/glhgnoocu.sHtML

[E12] 统计某字符出现次数
来源：http://wap.fehbvm.com/Article/details/glqxewhwn.sHtML

Py:   s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gnzfhpyas.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.fehbvm.com/Article/details/gwohyzvvy.sHtML

JS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gqzhmkbbq.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gxwpzalut.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.hesvh.cn/Article/details/gtajnhdxd.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.fehbvm.com/Article/details/gvmakxtbk.sHtML

Ruby: s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/gmentpubq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.fehbvm.com/Article/details/gkdzekrsq.sHtML

[E13] 逐字符遍历
来源：http://mobile.hesvh.cn/Article/details/gzqxkqmob.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.fehbvm.com/Article/details/gznqppurc.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.zdbjq.cn/Article/details/gpabhjope.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/gipgdqema.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gbzdysgbo.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gvqxdaisj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.hesvh.cn/Article/details/gwoaxqhbm.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.fehbvm.com/Article/details/gzkamtuuu.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.hesvh.cn/Article/details/gzrxcyqqn.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.zdbjq.cn/Article/details/gykhdykit.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.zdbjq.cn/Article/details/ggwvpntrh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.zdbjq.cn/Article/details/gqpphkhra.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.fehbvm.com/Article/details/gierwgxnm.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.zdbjq.cn/Article/details/gdsvamwrq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.fehbvm.com/Article/details/gfoobjkej.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.fehbvm.com/Article/details/gvywyzymv.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.fehbvm.com/Article/details/gliryshlz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gvfluixqc.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.zdbjq.cn/Article/details/gdvomleui.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.zdbjq.cn/Article/details/gbdtqieja.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.zdbjq.cn/Article/details/gtzjzmgxw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.zdbjq.cn/Article/details/gpsyaqxhk.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.zdbjq.cn/Article/details/gpausaaqp.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.hesvh.cn/Article/details/gegatxvtg.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.hesvh.cn/Article/details/gqzpoztgt.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.zdbjq.cn/Article/details/gbnviashh.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.fehbvm.com/Article/details/gaxnebtsj.sHtML

[E16] 数字千分位
来源：http://www.m.share.fehbvm.com/Article/details/gbeoskxin.sHtML

Py:   f"{1234567:,}"
来源：http://baike.zdbjq.cn/Article/details/ggbfnlvpe.sHtML

PHP:  number_format(1234567);
来源：http://blog.fehbvm.com/Article/details/gqtxbkaik.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/gtgudpmez.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/gcpcmdsqa.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.zdbjq.cn/Article/details/gmfrnestg.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.zdbjq.cn/Article/details/galkdgfok.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.hesvh.cn/Article/details/gmxonospu.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.fehbvm.com/Article/details/gvocxgwpg.sHtML

[E17] 首字母大写
来源：http://www.blog.zdbjq.cn/Article/details/gnsbnpzyi.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.fehbvm.com/Article/details/gnccamhuw.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.zdbjq.cn/Article/details/gypskaqsc.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/gucjsomwj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/ggutopgzo.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.zdbjq.cn/Article/details/gjxhrzoic.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.hesvh.cn/Article/details/gqwftzmwm.sHtML

Ruby: s.capitalize
来源：http://m.share.zdbjq.cn/Article/details/glynuusiq.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.zdbjq.cn/Article/details/gdruyqznn.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.hesvh.cn/Article/details/glirjhfwd.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.hesvh.cn/Article/details/gijavheqy.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.zdbjq.cn/Article/details/gotzujfde.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/grivrdwco.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gbcuqnjou.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/glkuoijxw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gwboxamvt.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.zdbjq.cn/Article/details/gzgqslkpq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.hesvh.cn/Article/details/gemhfwxdo.sHtML

[E19] 多行文本按行拆分
来源：http://wap.fehbvm.com/Article/details/geiowxihf.sHtML

Py:   s.splitlines()
来源：http://www.m.share.hesvh.cn/Article/details/goktiugok.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gqpnkymra.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/greqstuqv.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.hesvh.cn/Article/details/grdiagdjx.sHtML

Java: s.lines().toList()
来源：http://www.share.fehbvm.com/Article/details/gvkbaklxz.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.hesvh.cn/Article/details/ghchanlzq.sHtML

Ruby: s.lines
来源：http://www.m.share.zdbjq.cn/Article/details/geomtfkjo.sHtML

C#:   s.Split('\n')
来源：http://www.blog.zdbjq.cn/Article/details/glxujsfvl.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.zdbjq.cn/Article/details/ggshfxwoa.sHtML

Py:   if not s:
来源：http://baike.fehbvm.com/Article/details/gbncnngjm.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.fehbvm.com/Article/details/gpwhberif.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.hesvh.cn/Article/details/gqduajgmt.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.hesvh.cn/Article/details/gdohslvnp.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gbwqjqxmu.sHtML

Go:   if s == "" {}
来源：http://blog.zdbjq.cn/Article/details/gsjkhfkpc.sHtML

Ruby: if s.empty?
来源：http://www.m.share.zdbjq.cn/Article/details/grfndwmum.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.hesvh.cn/Article/details/ggwuiyqkd.sHtML

[E21] 超长截断加省略号
来源：http://mobile.hesvh.cn/Article/details/glrixrhtq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.zdbjq.cn/Article/details/gtsivzweq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gfidofajb.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gudzoqoqu.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gsajrywar.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gjhofqake.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.hesvh.cn/Article/details/gfivrsfkm.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gfboodxdp.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gatrjislg.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.fehbvm.com/Article/details/gfoghyueh.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.hesvh.cn/Article/details/gixztlcsb.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gclplplet.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gpkntbvmq.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/geirvszpn.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.fehbvm.com/Article/details/gchlvgsld.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.hesvh.cn/Article/details/gxwwlcjts.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.fehbvm.com/Article/details/gcpahubru.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.fehbvm.com/Article/details/gtkwywngv.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/grajizlry.sHtML

F. 文件与目录
来源：http://www.share.fehbvm.com/Article/details/gyucqsvet.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ghpxmuebe.sHtML

[F01] 读取整个文件
来源：http://m.share.fehbvm.com/Article/details/gkxxhmkxy.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.fehbvm.com/Article/details/gfavensei.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gugztuket.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.zdbjq.cn/Article/details/gaptvfllr.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.fehbvm.com/Article/details/gtipkkful.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gvtjsvejb.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.fehbvm.com/Article/details/gicwayftv.sHtML

Ruby: File.read("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gjkyriwal.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gzxosiqjz.sHtML

[F02] 逐行读取文件
来源：http://3g.zdbjq.cn/Article/details/gygekdurl.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.zdbjq.cn/Article/details/gqfdhxtkp.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.fehbvm.com/Article/details/gegdnabas.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/gogmtnmbi.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gensswftf.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/guzttkllw.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.hesvh.cn/Article/details/gnoxzjhzf.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.fehbvm.com/Article/details/gmaekrgyv.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.zdbjq.cn/Article/details/gddtdduft.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.fehbvm.com/Article/details/gedhiikzw.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.fehbvm.com/Article/details/gdoevayeu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/gpvipluvr.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/ghspspbdn.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gvkquhlsg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.zdbjq.cn/Article/details/gjwvrakqp.sHtML


<!-- 参考信息 -->