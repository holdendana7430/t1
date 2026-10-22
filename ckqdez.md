代发 wailian999

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2ybuheqcg.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2xumkikyi.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2qrsqsnvr.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2svzvunhh.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2vdoxurwv.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2cafvpxly.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2meftkrdi.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2cpiqabxz.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lqkfdzjq.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2snwdevei.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jmdqtirc.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2rhdeqkls.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ddozebhc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2pzkqrofp.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2sgpdvftm.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2tcakvadt.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2kviwmjbr.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2vxqlmryq.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2ptbdcnij.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2sruoolgf.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2sazlfqca.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2erzmptlf.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xkhtbnrs.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2llgshiyc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fkjjamzh.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2lfzicddg.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2lmcaoonj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2fdeyxoau.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2mlcupuvt.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2xbgogtff.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ktgdktcu.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2kwfnxyaq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2pyevuiro.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2thnuwmkx.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2efrevmrh.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2offuacfz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2gltdvtjn.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2nhxxckkh.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2gfoptiek.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2gaeblgsx.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2fhazbwek.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rgvkffuc.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2rcpjbeft.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2mywgjgku.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2gfchkwrs.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ylepspsa.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zdbwbzvv.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xdobbzgh.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2mvjvodtj.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2egpavhoy.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2aymirhan.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2mikoxrnn.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2gdjffvdf.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2sayosbvd.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2qkbkfxti.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2hgjjxfgd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jxqunhqx.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2iucgzzbe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qbarfnxr.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2zpnbuqis.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2wdgzqbew.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2pgrugtks.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2elouiloj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2zmyahuxn.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2rfurdeok.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2giuhsclv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2qstykblm.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2twhxoxlf.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2fexqjbti.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2jahgqkjl.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2cnvqqbmv.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2zqilpuvw.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vosbofxp.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zmrpvwdr.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2icghjayu.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2npdhxszx.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2vcouysup.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2xisximbi.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2upqowhyo.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2zjnfhpne.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ixztyapy.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2rddkhspc.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2sgfmmwcj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2txgyvgki.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2ttnzzhzk.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2dsbrsufn.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2jaglhlkh.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ygviqrgl.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2lnywrfee.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2hjajwlxs.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ewyiwbac.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2tatirjxd.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2byxvqzbg.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2fgumelop.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2tnzshbvy.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2njzzupvi.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xqylreuo.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2irpnyjcj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2rtmmeqid.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2xskodwtn.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2mqevxodc.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2fhhporxx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2gkfsivst.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2nftjngje.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2duyujtwb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2sglctsra.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bmpgwsmj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2yomjqlyi.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2iwpaokqn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xydrltzy.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bkunssru.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2otqepoql.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2yrkghqsi.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2chyypzde.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2smcnoeio.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2qtrqwsma.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2sjehttti.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2bkjnfhfv.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2fgayxlws.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2xcpbyhjo.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2iggiqzdf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2afnhbvvi.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2tdbdgnku.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2lgabdcke.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2awubiqaj.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2nsvjlyyf.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2swvpjmeb.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2doguppkp.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2seftrafq.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2hdcgdvha.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2pqvecbmi.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2hrgyfjpm.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2tesmrbar.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nsikevzx.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2gnmjczqz.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2bkdjpfek.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2kcltfdjh.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2osxcvrsu.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2torsjsyg.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2wuemevcn.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2hgevmqyi.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ygltvtjw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2ilyxjxno.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2nsrabsbj.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2vzfxtros.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2yffziudi.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2tyeuzzpx.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ujxyblno.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2uxsfjfdf.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2clyqryhe.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2moawuwqo.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2vajnzgfg.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2bofsatnf.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cuhcwntg.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2bizixczo.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2tuzokemb.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2mixojcdn.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2epwzxdtw.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2yrcsmeey.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2whgxohnd.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2yeapuwuq.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2akxkrnqp.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2mzxahgra.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2sruybnvg.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2oinhyftw.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2nsswppqn.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2hdxvyjvy.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2qrclfubr.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2gojnjgwt.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2mlhwhqti.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2amdzphsw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2flulciew.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2wrewwule.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2uqkuysje.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2dofidwdy.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2hquihrvh.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2yrkkurzb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2yovaiakp.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2avrmjarj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2xxuxemux.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ouhomtgw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2xjakvxxb.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2bmhjganw.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2lgmlvzbz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2wsqsposy.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2nuqpfkvy.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2osswjjvm.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dvxdzckj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oreenqjp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2veyohtcu.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2xvhvlwug.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2myqahcjo.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2wvapdbom.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2fyejtesx.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2pppzxoha.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2alpinkwa.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2ewynqfov.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2qkovurlk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2noqkvkbu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2swhlgriq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2qfcmuust.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2olkcqjjq.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2rfhpdydm.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2sgppcqlv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2lugqfxuu.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2dpohsmig.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xssdtfuj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2juigpmeb.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2spgkqowm.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2xnneehle.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2yhhinjzx.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2ljsogpim.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2lnnsmuhr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2lziiuteg.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2khwuyovh.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2uunhozop.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2qtkmulkx.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2qeeiuqqp.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2bumpzrmu.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2lazifjjl.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2wnmmhlqs.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ewnoybir.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2tvdytmkv.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2zkmerckj.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2knzvubgy.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2txmcyrum.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xgcpgzlv.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2ovdwsukp.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2dviiqsaf.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2qlncypor.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2vnpuhgzt.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2oktjhnzp.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2jnlscjdj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2rurzikgq.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2dlpjjvtg.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ztfkkkxd.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2uyxlxbgm.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2xfeqpdtx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wsfmmiyu.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2rstdodej.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2wlgmdzav.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2djhslsrg.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ewxeafou.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xvgdwfwk.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2tnfypgzr.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2vtmizfyb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2keojjdur.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qlzwriuu.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2xkadxluy.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2oahpifzz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2svfbfxmf.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2asipgzug.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2himzxnvy.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2zvidbwph.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2qsvnfoww.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2dxudystq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2omuwmvjy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2osjkvzab.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2wxorvgxi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2panwbiqh.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2yxzgmfvg.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2jnczdtko.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2reipnxdr.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2slhllpbz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2tqdibkwg.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2yznorkpa.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2kzebvvfp.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iqpxeqxl.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hacxucge.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2ihhuvefw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2aziciepo.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2jadxrvhk.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2whfdvdvm.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2nijtaqvv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2saypvxry.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2pakhinss.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2fqhxhfxi.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2kzqjghny.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2usoodpoi.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2zxzxprvd.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2aqmehgyt.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2utbvlimh.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2imzmiebb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2azezgpzv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2gktdnvrv.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2allpqovr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2ywknohra.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2mcesxgvq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2oxgahjaq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2avcvgxar.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2msbeislq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2mhltmncn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2xbdpdjwq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2gnwjdjfy.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2hbsqlkwx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2twyayxkp.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2oxsftsqy.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2cjpnsznn.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fkirbgbo.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cwquwtyo.html


<!-- 参考信息 -->