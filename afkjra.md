代发 wailian999

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2gcpvkllj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2itrluofx.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2plgtudnb.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2tcjktmfa.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2cgnuhzcn.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yqavuzen.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tpdsahmr.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2lxcihtfk.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jdvvvoeo.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2plqzvnjk.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2evirrazx.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2jnvxshwl.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2hzjfkoxh.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2ylyvpnmg.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2imedohyy.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2jsdydktn.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2hltgjexx.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2pgcvuyrr.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2efohjgqd.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2knxyzzuz.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2sbuapqmy.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2uoldhbro.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2jgcfdiqp.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2wrarpuga.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2qayltixn.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2tqcbownt.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2tvecqfti.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2qixooucg.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2cfwhacoe.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2mygohspn.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2tghqatto.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jrsgxkuo.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ltvwjtda.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ewonsmvr.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2yaryfalz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2pwvzttms.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2rdhhnufc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2iirpypig.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2vcppujtm.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2gqzzbnvl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2xizbivtl.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bhbgdyny.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2kdlzxrfg.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ctgnchtp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2ieogxino.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yuagwwvp.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jmonyqdc.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2klhzezug.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2royjpxip.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wophjwsm.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2qqiokeqd.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2nziwslpq.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2wwajbsrd.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2meddrman.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ugreplhv.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2tkmeoxua.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fzfovsgh.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2jbpmtsiu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wxwyblhd.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2rjuuysns.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2wgseecox.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ojmmfhvh.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2gcwdrixy.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tkzbbrqp.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2wxooumzj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2fpfuqloy.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2qyjkqjfw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2cukqpfdc.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2qgfsnwkd.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2dpxwayqv.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ajsvpdof.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gyvigxbg.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2nlgvxiks.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jsskhvis.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2lrxrywkp.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2ghmtcdva.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2uewtajcu.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2yodghkbu.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2xjmnuomw.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2xqxbddpq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2jweysgll.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2qfyoqaoj.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ulgdbdyb.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2xzwrkbgg.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2ozuaaytm.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2fmdjycge.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2utulaezd.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lxqtlgdq.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2xaehpiou.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2lasmiqho.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2dsvwchcf.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ldumrbeh.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2rpqophcj.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2rrmlpifd.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ddmeaaki.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2upuuihft.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jnfejtdq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2friyygid.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2hfilvtrc.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2amuqsdts.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2hqadwnza.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2hwyheibk.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2ftxlrodc.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2bkectrqy.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2fsreybex.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2ujwdsyyp.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2wrvhqgnq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2npszlhiw.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gkakzvte.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xksingww.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vvdkeuww.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2sxuxvaox.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2esugnfih.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2czefzppq.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2enhatiij.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2xhmuyiqo.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2nhtmdktv.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2dudcmaoy.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2rpynrrrf.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2ferostud.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2cxyeqntg.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2uhuwlkvs.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2fldylcts.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2padkryiu.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2yahughxy.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2eksjdfgb.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2vqurtcrv.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2avilbmvt.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2iizltfyo.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ylefnabo.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2xubqblsv.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2hfyiyvzw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2cbpsusnj.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2xgjbnznp.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2lcerpcej.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2xgximntu.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2khprykas.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2lqammukc.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2sjdsleav.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2wtwhxopc.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2ihlafxvg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2pampxtix.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2kjnxgfyj.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2oyuyybzg.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2yoqxqvsg.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2zyoxopob.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2fhtrjzoy.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2qionyxts.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2upgflhgv.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dpovhkhu.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2iuccupad.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2efiyxoiu.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2hppixjze.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2urmtewuc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2enwrxlym.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2odkuuehp.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2iabyljcb.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ldsujqtn.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2reelsjwm.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2estngrut.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2eyhfelns.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2bfdmnbmj.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2bqagvisx.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2hgllgjeg.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2iqpjwppa.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ncyxvhwn.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2jglnwrnu.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rmframpp.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2qjisxcsy.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2tkltznpe.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2sjtmgplr.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2dijxnggl.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2dzuvzsko.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2sgbmbbyc.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2ullfhwhd.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2vextvjhe.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2huvpwbbg.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2fzwxpzrs.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2lbkewbcu.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2digsdtim.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zjwpluee.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2enaespdn.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2nvbepoze.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2chkzaoqe.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2fofyybmb.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2sjiufyct.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oywkcoqz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2eyfbncgu.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zqapmrvg.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2kjkeiszb.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2fawmxemy.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2updpvlus.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2evnjyfxf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2xvtkcaof.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2enuozvoy.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2hcujjnya.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2kdzxxwzi.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2qtuoaswu.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2lfuyqtac.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2rdpdajmj.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2vviliawy.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2kxzcopiq.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2iaiimryh.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2hnvbelih.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2xcymljtz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2cyctispo.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2svapcuvb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2eqyqvxso.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2kbgcnucn.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2rpgoykhy.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2atrfizat.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2cbycmlsl.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2jcfymqns.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2qgnlyeiu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2wodcrqtx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2vevnlfzw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hfsiidat.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2mejljtns.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2bdltuzwo.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2nadmjwmi.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2gxuluorn.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ipzfzhgl.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2qoldoamn.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2eessnacx.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2iqhjxmen.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2oksaqqyh.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2werufegi.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2edylhwwv.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2ychacywr.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2ojbvxjou.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2hjtdcsit.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2cwwxiyrt.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2rhdjgevt.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ejahskkt.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2nqbyabyb.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wnbbknye.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2mngqlcrb.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2fltzepbj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2nyoynqdr.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2eqajzsbu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2fqwohapa.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2frqcuaol.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2nequaayr.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2kyljrygx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2jcccavtp.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2fmhgkium.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2iyqkhfom.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2gcljqjab.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2ibpmforq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2oopdvjry.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2oxppaoky.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2omjzqmrs.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2snbvruft.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2spdemrcm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2olsrgctb.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2sphwfltv.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ywswxsuw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yxcbmpcp.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2eamgbrpu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tiysfeoi.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2uocbayai.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2xyjumhts.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lhtqdoha.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2kpcsthwa.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2mkookage.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2txqruihl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2msvtvhxv.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rnxndyyo.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2sbzsbbck.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2ecdzhqni.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2kcvwiujk.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2sojswlkv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ozuzvejo.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2svuieidh.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2baubjlca.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2ypcurttz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2zadkachn.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2pwenebvo.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2hpsygcql.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2mkqwedzh.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2gtwtetms.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2hnovvutb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2bfuewkcj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2wlnaycdn.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2gbhllqdz.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2gfasnngs.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2ooyriakb.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2xqlztipp.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xvolwdto.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2mkjkdbdr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2uuazjtba.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2qcpofgtg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2xfvzdrhr.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2tthbamla.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2vsexblao.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ukxlyizk.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ekphzqjl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2mgrsoysb.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zvtjpuxf.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nuyqiwxt.html


<!-- 参考信息 -->