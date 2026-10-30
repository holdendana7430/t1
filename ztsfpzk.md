代发 wailian999

[D19] 按字段分组
来源：http://www.blog.fehbvm.com/Article/details/gaeegfdoz.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.zdbjq.cn/Article/details/gmjuhfoqq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.hesvh.cn/Article/details/gxuxadvva.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.fehbvm.com/Article/details/gavijxroy.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gfheiwkhf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.zdbjq.cn/Article/details/grdymrvao.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.fehbvm.com/Article/details/goekjkpjx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.hesvh.cn/Article/details/gvijslexm.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.fehbvm.com/Article/details/gwhzeunae.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.hesvh.cn/Article/details/gvbxaextj.sHtML

Py:   Counter(arr)
来源：http://baike.hesvh.cn/Article/details/gakuzwwln.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/ggqzdtgvh.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gpaolcqnm.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/gssecvqvi.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.fehbvm.com/Article/details/gqqhmyunj.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.fehbvm.com/Article/details/ghlrprvtn.sHtML

Ruby: arr.tally
来源：http://m.share.fehbvm.com/Article/details/gmwlymbkr.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.fehbvm.com/Article/details/gnkdjxowc.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.zdbjq.cn/Article/details/gqtrhufon.sHtML

Py:   x in arr
来源：http://mobile.hesvh.cn/Article/details/gbwchzqmz.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.hesvh.cn/Article/details/gcxbcxsnh.sHtML

JS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gqooasrlb.sHtML

TS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gcvngnbpo.sHtML

Java: list.contains(x)
来源：http://baike.zdbjq.cn/Article/details/gwmcipllu.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.fehbvm.com/Article/details/gxxjdtejl.sHtML

Ruby: arr.include?(x)
来源：http://baike.fehbvm.com/Article/details/ganjmxxyb.sHtML

C#:   list.Contains(x)
来源：http://blog.zdbjq.cn/Article/details/gzuhdslms.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.zdbjq.cn/Article/details/gdgmmfckp.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.zdbjq.cn/Article/details/gryrmggdm.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.hesvh.cn/Article/details/gnnqbqunh.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.fehbvm.com/Article/details/gtxyfjxez.sHtML

TS:   [...arr];
来源：http://www.m.share.fehbvm.com/Article/details/gqprolhsx.sHtML

Java: new ArrayList<>(list);
来源：http://blog.hesvh.cn/Article/details/ggwkhsuev.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.zdbjq.cn/Article/details/gessjqnbp.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.hesvh.cn/Article/details/gxmfjfvad.sHtML

C#:   new List<int>(list);
来源：http://www.share.zdbjq.cn/Article/details/gnkpzsluo.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.fehbvm.com/Article/details/gjfwpdiji.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gxtgqlozs.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.zdbjq.cn/Article/details/gcgymwivy.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/gmxsxunlf.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gwgdmakfk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.zdbjq.cn/Article/details/gkwyctukh.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gyenilyqe.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.zdbjq.cn/Article/details/gshaxdtwo.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.hesvh.cn/Article/details/geirvspah.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.fehbvm.com/Article/details/gkrkxjdai.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.zdbjq.cn/Article/details/ggfxcdhza.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.fehbvm.com/Article/details/gepfmqqhd.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.zdbjq.cn/Article/details/glpobiswa.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.zdbjq.cn/Article/details/ggwaeiuos.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.fehbvm.com/Article/details/ggxuptdcl.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.zdbjq.cn/Article/details/gueryenhr.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.zdbjq.cn/Article/details/groeiqyrg.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.fehbvm.com/Article/details/gzxblgxsz.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.zdbjq.cn/Article/details/gtdrnzldx.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.zdbjq.cn/Article/details/gsgljjfwv.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.fehbvm.com/Article/details/gvkqdfcop.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.zdbjq.cn/Article/details/giunhydle.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.zdbjq.cn/Article/details/glpbdqtks.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.fehbvm.com/Article/details/gagnmfsjb.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.zdbjq.cn/Article/details/gcmdzklrw.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.hesvh.cn/Article/details/gfikerbcx.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.hesvh.cn/Article/details/gpilwzzcg.sHtML

[D26] 数组转字符串
来源：http://3g.fehbvm.com/Article/details/guefutjeq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.fehbvm.com/Article/details/gxmfjpovc.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.fehbvm.com/Article/details/gejakeurb.sHtML

JS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gbqcstaul.sHtML

TS:   arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gwqbogcmq.sHtML

Java: String.join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/gbojtxois.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.zdbjq.cn/Article/details/giodsvjed.sHtML

Ruby: arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gscksxvdv.sHtML

C#:   string.Join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gaojvsgiv.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gozvprapc.sHtML

E. 字符串处理
来源：http://wap.zdbjq.cn/Article/details/ghchrndyh.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvksapjhz.sHtML

[E01] 拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gewjigrmi.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.zdbjq.cn/Article/details/gowhkhogq.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.zdbjq.cn/Article/details/gortrwlbu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/gufurkysn.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/gmqnzriaj.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.fehbvm.com/Article/details/gdlvpcvym.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.fehbvm.com/Article/details/glpsluyui.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.fehbvm.com/Article/details/geekwgpto.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gbhvxmbow.sHtML

[E02] 重复字符串
来源：http://blog.fehbvm.com/Article/details/gackpqahv.sHtML

Py:   "ab" * 3
来源：http://wap.hesvh.cn/Article/details/gozxhcxut.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.zdbjq.cn/Article/details/ghaitfrxp.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gdemkcsok.sHtML

TS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gktsmfbcr.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gzwymfzvo.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.zdbjq.cn/Article/details/gczffuypc.sHtML

Ruby: "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/gjmfqylyw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.zdbjq.cn/Article/details/gsacqbavd.sHtML

[E03] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gxcjpmkjy.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.hesvh.cn/Article/details/gyvabiaik.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gdbepemca.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gsroojpan.sHtML

TS:   s.slice(1, 4)
来源：http://3g.hesvh.cn/Article/details/glhqapatn.sHtML

Java: s.substring(1, 4)
来源：http://blog.zdbjq.cn/Article/details/glqabptwt.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.hesvh.cn/Article/details/gkldjvjpd.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.hesvh.cn/Article/details/gqvviyvbq.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.fehbvm.com/Article/details/glfvthqbr.sHtML

[E04] 查找子串位置
来源：http://www.share.zdbjq.cn/Article/details/geumgeyrz.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.hesvh.cn/Article/details/gdyyvsrdo.sHtML

PHP:  strpos($s, "x");
来源：http://blog.hesvh.cn/Article/details/guynpyxaz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.zdbjq.cn/Article/details/graqvpasg.sHtML

TS:   s.indexOf("x")
来源：http://read.share.hesvh.cn/Article/details/glgsdaecr.sHtML

Java: s.indexOf("x")
来源：http://baike.hesvh.cn/Article/details/gjpkwklau.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.fehbvm.com/Article/details/gugjhwivb.sHtML

Ruby: s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gapfxydyi.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.hesvh.cn/Article/details/grpiohfwg.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.hesvh.cn/Article/details/ggxfextgx.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.zdbjq.cn/Article/details/gnvxqdcsv.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.zdbjq.cn/Article/details/granpupwl.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/grjvjzboe.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.fehbvm.com/Article/details/gxmesfjfo.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gwdfgwjqo.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.zdbjq.cn/Article/details/gfpmvbwsu.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.zdbjq.cn/Article/details/gvhyoqoqa.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gltuujmok.sHtML

[E06] 替换子串
来源：http://3g.hesvh.cn/Article/details/gaimrnrpa.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/gaxogdiae.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.fehbvm.com/Article/details/grcpnybky.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gfxgwzicy.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/giommmawm.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gymvvezgw.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/gnlyxcehn.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.fehbvm.com/Article/details/glcjdzthm.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gnsipjndh.sHtML

[E07] 按分隔符拆分
来源：http://3g.fehbvm.com/Article/details/gtlpwmtjs.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.hesvh.cn/Article/details/gnewkhzec.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.zdbjq.cn/Article/details/ghgwablga.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.zdbjq.cn/Article/details/gmttdfccm.sHtML

TS:   s.split(",")
来源：http://www.blog.zdbjq.cn/Article/details/grmywlsxq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.fehbvm.com/Article/details/gcnnywfqb.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.zdbjq.cn/Article/details/gwmodgbqa.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.fehbvm.com/Article/details/gebzfieyt.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.hesvh.cn/Article/details/gwwflvvir.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.fehbvm.com/Article/details/ggxihqysg.sHtML

Py:   ",".join(items)
来源：http://baike.fehbvm.com/Article/details/ggpbdoiaq.sHtML

PHP:  implode(",", $items);
来源：http://m.share.hesvh.cn/Article/details/gngcjnrmm.sHtML

JS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gwjkxshrc.sHtML

TS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gslnysxna.sHtML

Java: String.join(",", items)
来源：http://blog.fehbvm.com/Article/details/gjsbreteq.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.zdbjq.cn/Article/details/gljketodb.sHtML

Ruby: items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gtpcrvtwr.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/gdixqndua.sHtML

[E09] 去除所有空白字符
来源：http://wap.hesvh.cn/Article/details/gvospmxdq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.hesvh.cn/Article/details/ghhopbmre.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.hesvh.cn/Article/details/gmjlpmuzu.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/gyvojzikb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/gocixbrah.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.zdbjq.cn/Article/details/gqhmxakso.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.hesvh.cn/Article/details/gwxfgmvsj.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.zdbjq.cn/Article/details/gqzrxcavs.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gxjvriefp.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.fehbvm.com/Article/details/giyivihiw.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gcbhrrsjs.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.hesvh.cn/Article/details/gtrnzbgcd.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gayelwcqb.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gxbgumkqd.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gwfpulffq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/grtvcjlpx.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/ghcimubsq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.hesvh.cn/Article/details/gabonehqk.sHtML

[E11] 反转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gqvfpzhvr.sHtML

Py:   s[::-1]
来源：http://wap.zdbjq.cn/Article/details/ghqyjzjyb.sHtML

PHP:  strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gwobcnczl.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gkrxmiexf.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gmpqndofe.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.hesvh.cn/Article/details/grvjugkls.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/gaiijcnek.sHtML

Ruby: s.reverse
来源：http://read.share.fehbvm.com/Article/details/gywdexoef.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gazyhjcqq.sHtML

[E12] 统计某字符出现次数
来源：http://wap.zdbjq.cn/Article/details/gfxqlnulb.sHtML

Py:   s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gzrevhdov.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.hesvh.cn/Article/details/gdomzfhbr.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/gymthpwlx.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/gcygzbufc.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.hesvh.cn/Article/details/gpidplshj.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.fehbvm.com/Article/details/ggyvogfwm.sHtML

Ruby: s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gmzoqzkvq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.hesvh.cn/Article/details/gdlygjldi.sHtML

[E13] 逐字符遍历
来源：http://www.share.zdbjq.cn/Article/details/gplcbjlkj.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.fehbvm.com/Article/details/gxtllkzht.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.fehbvm.com/Article/details/gztzkdchd.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.hesvh.cn/Article/details/gyvlvavhb.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/gdcihbypw.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.hesvh.cn/Article/details/gmeubwicj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.fehbvm.com/Article/details/gsgtscjlq.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.fehbvm.com/Article/details/garnrzwnq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.fehbvm.com/Article/details/goicguvep.sHtML

[E14] URL 编码与 Base64
来源：http://3g.fehbvm.com/Article/details/gfwqqplof.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.fehbvm.com/Article/details/ggpnstaux.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.hesvh.cn/Article/details/gkkgvyhxm.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.hesvh.cn/Article/details/gplopoqqa.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.zdbjq.cn/Article/details/graxvwsyj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.fehbvm.com/Article/details/gffeejyhl.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.hesvh.cn/Article/details/gnuqzsrua.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.hesvh.cn/Article/details/gcbivdiua.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.zdbjq.cn/Article/details/grmxdizvj.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.zdbjq.cn/Article/details/gxlqojved.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.zdbjq.cn/Article/details/gjlqqmzib.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.hesvh.cn/Article/details/gzbcoqfmt.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.fehbvm.com/Article/details/gzlkgdmex.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.fehbvm.com/Article/details/gieaywfwu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.fehbvm.com/Article/details/girrhaxfd.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.hesvh.cn/Article/details/gsjocvsrp.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.fehbvm.com/Article/details/gqhhhrgkm.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.fehbvm.com/Article/details/gevousfgp.sHtML

[E16] 数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/gobxbciky.sHtML

Py:   f"{1234567:,}"
来源：http://blog.zdbjq.cn/Article/details/glrlrpodw.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.fehbvm.com/Article/details/gmgjyqwxi.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/gzpxjtoly.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/gsmoaakut.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.hesvh.cn/Article/details/givvatnfu.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fehbvm.com/Article/details/gciovpubn.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.hesvh.cn/Article/details/gyaoahcgf.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.zdbjq.cn/Article/details/gikwoybxr.sHtML

[E17] 首字母大写
来源：http://3g.hesvh.cn/Article/details/grgojxkgq.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.zdbjq.cn/Article/details/gbjtxwwim.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.hesvh.cn/Article/details/gtlfmhodc.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/gkkqorqge.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/gmrgffbup.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.zdbjq.cn/Article/details/gzpjwfkoo.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.hesvh.cn/Article/details/gysslvbmf.sHtML

Ruby: s.capitalize
来源：http://wap.hesvh.cn/Article/details/gnyyfrhvf.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.zdbjq.cn/Article/details/gkoigtuml.sHtML

[E18] 模板占位符替换
来源：http://wap.hesvh.cn/Article/details/gustanjyx.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fehbvm.com/Article/details/gbjeodtxu.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.zdbjq.cn/Article/details/ghjuvnokd.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/guefdvujw.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gmvvdcmcb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gtqaqwyxn.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.hesvh.cn/Article/details/gpaxohijx.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.fehbvm.com/Article/details/ghfidtfig.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.hesvh.cn/Article/details/gvnrbozoe.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.fehbvm.com/Article/details/gbzmrndca.sHtML

Py:   s.splitlines()
来源：http://read.share.zdbjq.cn/Article/details/gmcsgdisj.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.hesvh.cn/Article/details/gtdbnpngx.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/grimrqtci.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/gwqnubzfl.sHtML

Java: s.lines().toList()
来源：http://www.blog.hesvh.cn/Article/details/geiulardb.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.fehbvm.com/Article/details/gylhudewf.sHtML

Ruby: s.lines
来源：http://baike.zdbjq.cn/Article/details/guczzljms.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.zdbjq.cn/Article/details/ghbtzisxo.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.zdbjq.cn/Article/details/gswlkuyxk.sHtML

Py:   if not s:
来源：http://baike.fehbvm.com/Article/details/gnehijgiy.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.zdbjq.cn/Article/details/glzngmxwf.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.hesvh.cn/Article/details/gwmbnfvis.sHtML

TS:   if (s === "") {}
来源：http://blog.zdbjq.cn/Article/details/gvlkewkqw.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gqqdbvyym.sHtML

Go:   if s == "" {}
来源：http://baike.hesvh.cn/Article/details/gcommaefi.sHtML

Ruby: if s.empty?
来源：http://m.share.zdbjq.cn/Article/details/gkmdnhhsr.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.hesvh.cn/Article/details/gbacyeity.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.zdbjq.cn/Article/details/goswcmkcl.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.zdbjq.cn/Article/details/gdgubyfvp.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gevrrmaio.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gjwwkhxpk.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gpdmzwkht.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gahlhqzoe.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.hesvh.cn/Article/details/glxdgxcwo.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gkickvfck.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/ghtuhqqhf.sHtML

[E22] 字节长度与字符长度
来源：http://blog.zdbjq.cn/Article/details/glmsqrdiv.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gjplqpnqo.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/ggmopnowm.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/ghodhxhwe.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/gcmdpefxs.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.fehbvm.com/Article/details/gjppcpjbl.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.fehbvm.com/Article/details/gjbcjeotz.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.fehbvm.com/Article/details/gfrpwilyv.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.fehbvm.com/Article/details/gsfddllqk.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gkrsgymws.sHtML

F. 文件与目录
来源：http://mobile.fehbvm.com/Article/details/grqerdipa.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxfaenisi.sHtML

[F01] 读取整个文件
来源：http://www.share.fehbvm.com/Article/details/gdisudmur.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.fehbvm.com/Article/details/gmltictly.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gvntucddz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.hesvh.cn/Article/details/gmhrsbszb.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gdzqkolni.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/glebrbmiv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.zdbjq.cn/Article/details/gctgozogo.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gkgggughe.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.fehbvm.com/Article/details/grtkzzwof.sHtML

[F02] 逐行读取文件
来源：http://3g.hesvh.cn/Article/details/giensgqin.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.hesvh.cn/Article/details/gmhhwcpck.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.hesvh.cn/Article/details/gzsbqfsqj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/gbwdlbgsa.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gwthobczq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gchptfwcd.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.fehbvm.com/Article/details/gixweaxaw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.fehbvm.com/Article/details/gbqbxpmpg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.zdbjq.cn/Article/details/gwrqgkceg.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.zdbjq.cn/Article/details/goprwaktr.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.zdbjq.cn/Article/details/gjotrppqg.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gfuzrhxkc.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gfjntbmnj.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gcanvxxnj.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.hesvh.cn/Article/details/gewohkrel.sHtML


<!-- 参考信息 -->