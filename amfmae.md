代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2fzapomcz.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2elejatbp.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2gwvsadrg.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jocaosfo.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2nkbomlhk.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2xxvqvmtd.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2helgkrqc.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2qaogaucm.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2rnnkrtje.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2pfahfweo.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2miequzzb.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2wqxzuivq.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2hnoroxzs.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2beduoykf.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tnuilgbz.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qrfbfuhx.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ficefxzw.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ztetoeex.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2zbigsrik.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2ueiengkw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2hyhknblp.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2iqhainja.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2guehdodk.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2uvghymzv.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2xnxqamop.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2ucpnifbz.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2wgsuoirb.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2aqtsnzlt.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2naechyxk.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wbmqagsh.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tnkobslk.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2yiowryga.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2lfmyrdza.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2fkrqormz.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2sahjhngh.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2bimywwwx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2rsgoraqd.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2bzwzwtqt.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2ugsfzrzt.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2muhfutxo.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2boqonvzy.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2echiwthn.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2dpbemqst.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2iufcdwrp.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2umwszrjt.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2kvgaanyj.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2cgmwshte.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2cllzotrv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2rxwqvfmw.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2fetvgymp.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2zvjmvkjd.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2tifzxyre.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2yqoyyxlz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2kaxpjdrl.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kvruxgfr.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jfuxnmum.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2riejflaj.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2aevxernb.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2stdcfucy.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2lvjdzfgf.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2eajkloki.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2pepjsfxr.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2zonhwkvs.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2himykelx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2okzifhib.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2qtneksbn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ujxaqmmi.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2lgergzjc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2mtpeaucw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ayusqrqf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jyvlhcdk.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xwxtqkos.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2jihpsyig.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2bywngiah.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2ycowekyu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qgmnedru.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lvoyslzp.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2laypdzgr.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ktzhopim.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2owgpohrm.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2wjvnyvkt.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2qcyvfvxw.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2lphobyag.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2hlkmgxwp.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2mfeekmdo.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2kzikwkgv.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2dtnjfecu.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2pwnmanti.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2jezpvhoi.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2buurqbuw.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2yzvjngof.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2ngkrhpvi.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2awjmyezi.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2kuayrzgs.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2tnyfsbcn.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2vlokldos.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2oginxhms.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2rymipawd.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2pntwkazd.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2evwuphrv.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2wjydujzr.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ofbgyqel.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ligtbtiz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2wpixispt.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2oagrkala.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2wuicngwx.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2wzddqrtx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2lojzejjx.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2hxrcyhuq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2iebvdzcj.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2jzmxlewp.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2musxydhr.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2iuxmtmng.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2chlffpxz.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2uhluapsc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ufcitqzt.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2fnxvysrd.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hoffcnez.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2sfncurbq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nrvfuuin.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2waijowff.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2rajkdmwq.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2zpjsaccu.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2zqyegyhg.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2qqdwlbkv.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2yokakhpb.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2mtppeote.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2evfwplpj.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2urikdjra.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2bvcktaax.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2tiqvuuij.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2bwyospkx.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2yzrzbxfq.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2zamfbiwt.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2lpmcxxfy.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2vagimplk.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2zhfknvfs.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2tcrvtqqu.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2zzketlka.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2nnuzpsdj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ywzwytan.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2cpcgylkd.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2zqhcmqnp.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2zaulsowl.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2rqobhfsb.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2uzediwqt.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2irrwetol.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ashmjuos.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2qhwrflfx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ilrbbqae.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2fsdyxckp.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2gmhdxskt.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2qbmdqbpu.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2hchonpft.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2rwctmqha.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2powhczfb.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2dpxfoguz.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2bicmnvcj.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2fcszzefo.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qmapafuy.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vsjqdcoc.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wsazdsxq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2vuiskbtn.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2rqtietsf.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2lpyztgnk.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2kzxvfzbz.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2oofspsaw.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2dkzgevne.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2foargzde.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2asusjisx.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2xmwizqro.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2bpwcsine.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2ohnuuzxe.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2sacfahrq.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2wsddcjjd.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2yorwxgdf.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2jsnwqnvb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2uiewleex.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2mdkkydzi.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2vqzyavan.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2zltcqlyz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bpkkmhjc.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2snphkssh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2pcaepklp.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2vqgpnsna.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2quxmoyjo.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2nfplqepu.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2muoyqsbw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nfagprie.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ckbzkgtr.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2tnexpdxq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2stvktiih.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2kyblxgyx.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2xjiqlqhd.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pdjqqzwf.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2enkkdhfz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dedbjphc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2hiceyjiu.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2xdpbubsb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cxzozlih.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2tyczxkhc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2bsbyqxet.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2lhtdumhp.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2tjrsryxl.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2amslegwh.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2rofayysi.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2ufzrlpog.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2wdgvrxlo.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2sdsqhpcu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2rppmufdh.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2zddvvbsf.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2qkjkrvbi.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2zloblkoz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2jlbtsbhw.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2wfkenuwn.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bqinzjkc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ntkxyhsr.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2qtaibahb.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2culbniea.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2jckvzgjg.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2ehhhzmdy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2oyblqbcy.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2vdqygorn.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2pnjitglv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2yjsslctw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2pzpaehhm.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hyrlynja.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2hpbelyiy.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2oovjutqr.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2kuxhgzet.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2wbrxuegk.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2mvxftvpl.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2lebxzrer.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2rzqigksj.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2pzfnstuw.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2atbuoiti.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2nffjcpld.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2toxkcjsp.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2pvjlaobv.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2fgmozmuj.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2nhaojxbe.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2rcybtcuf.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2cwljvvsj.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2psaullud.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2yhchxhab.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2fthsyvru.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dnicytwb.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2riywjxye.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2bbyguqrp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ayhledmm.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2lrabpxgm.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2hziobnnv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2wcfxbruk.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2gnsbicha.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vnjdhdwc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ujjauqbg.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2onnapyrs.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2ridfwxub.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2lcwssxnp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2oaxyjvzz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2llqkfkkx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2nbnygmxa.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2tblzxsrq.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2oyinasqd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2rljwfvaa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fhfeteqe.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2nrreaydn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dlmipnho.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2othukbxn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2mpkdwfqm.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vclmgwpv.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2zikejyfl.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2mqlxgerg.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2awpotgpe.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2xtjnjhci.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ovggvnfe.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ednvzqwd.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2cwwvwhrc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2brierksv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2uguhyjwp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kyrzcbxw.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bfosoywp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2xbmvawuw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2xqtchwht.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2prrbiarr.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2anpleybv.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2uzzyhadi.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2abemeoun.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2mbxqlcil.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2dfgfkitb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2detberph.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2cpqdtplj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2vapmwfvp.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2xpnuzufb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2nwkcbxls.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2mlfprjxi.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2dqetmyya.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2omsahqcy.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2scjeniqq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2osqaplcd.html


<!-- 参考信息 -->