代发 wailian999

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2kllyhvay.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2peemnbeq.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2ctifdtne.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2zgevmwpu.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2bxgsgsmq.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2fwonateu.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2eooqskvz.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2efakmgqu.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fcztylzq.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dksyqiwm.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tqfswzsk.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2tidlleet.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ssdmgbun.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2siadacgl.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kpzmwelj.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2tiviazba.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2dcgrsvnw.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2uxngqibv.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2cyrafefr.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2zordxhcs.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2ykekubge.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2gljnwpha.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2viwocqnk.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2upjpnjxj.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2abqnojwd.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2knradrit.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2bqplnebw.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2ynnfyjqk.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2lnvsuwsk.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2mpvivipa.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2lgxjjrle.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2imlgwken.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hlhldtjx.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ceburfxo.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2grhpshbs.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2pldnjbsm.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2zfyrbnbn.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2fuoeazqm.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2stcuqzwg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2srtzrflq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2lkjegvzp.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zcgnzfbm.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2xlykrzbl.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2warsopsy.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2ywiiflfs.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2dyygernx.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lgjsrasq.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2wkweotbo.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2wbkompxf.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bhiwbehl.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2xetyduhg.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2pkafkfyp.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2gszfhftu.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2uoeddiwh.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2prefvihx.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2lbyddlsy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yivxwfsq.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2frehqowk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fycijjqa.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lmytcerz.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2lquflcic.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2wjdunumw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2eiddfyfg.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2oxijndgs.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2beaxzjah.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2lrkgapwg.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2ybhomebu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dpnozboq.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2yppnfote.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2eklycnqj.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2drewwtws.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jqawugxx.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2oxmynfwr.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2aotzrkyt.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2gdljqewe.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ajinavxu.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2epijhxds.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ywecgrot.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2gunklrhc.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2fddptasy.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2wgsiytdy.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2oavojhsd.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2sxwlawiw.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2kasellna.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2jhyeytrm.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2pruiquzl.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2fubgxsnr.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ugiehyre.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2uudimdww.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2nyayhkxz.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2puuavjxe.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ntkexehb.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2igzjwtoq.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2pviyvalx.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bjwvulbc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2iarimihk.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2yjamcysd.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2jlbfxsir.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2lcczwmkw.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2oywvgmuz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2jqznnndn.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2vrvzqujq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2kwvcurpi.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2gnztbmpb.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2oojipoyl.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2pbuzqzyo.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2swuduehe.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ffnzmqsk.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qtlrcytv.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zmtetzhf.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qquwxmxi.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ojiaqryg.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bdsitxae.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2oouprmeg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2hqgoucha.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ujddkslo.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2csaiyzsh.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2xxzqrvbb.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2tmzjxsiz.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2bhppgpud.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2ficwtssr.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2sxcbhqbq.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2rcbpkdtk.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2uagtifmd.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2wtwvtcxl.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2udnmxcea.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2dhchkchi.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2dwbqcbqa.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2krdjtrrt.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ytkdsmbs.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2louanrvm.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2rewrkift.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2ojmswucf.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2opxwenpq.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2xauzrpou.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2qniimoon.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2btbuccqd.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2skhzfsko.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2veiodvkm.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2trjepnoc.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2wzqugrkd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2xvcqmrbf.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2hrrgbsew.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2byhzfmuv.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2sdthbhfg.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2wcawosto.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2odziwbyj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ujediort.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2cxyythhi.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2bqrafamm.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2kwsqjrzi.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2sgsxsyjf.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2qffqeovv.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2cpnhrrnx.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2gxgasbpt.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2eijwuimp.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ypxhhyft.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2rcsraiie.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2bfelmalk.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2iwiwlisz.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2pvmhqxcm.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2jdwksxsc.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2tymosppf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2yponfvdi.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2pvfaawvs.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2obmstzdy.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2yzrfykdd.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2lkmnjzbz.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2frqoelzm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2kfzvdavb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2esfebzhy.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2hqpsfbdi.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2bhilqdet.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2exuwfpzc.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2qyefdats.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2kwwvdosm.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2bjxsxywf.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2lzsuyfjn.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2jclqqdvw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2azwrmfqp.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ldhovket.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2vpmejqbk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2nrpzxaco.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2lnlfzirr.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ivchoach.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2zxehrnda.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2jnhnueaj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2frtyigvy.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2qokmzlzz.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2ixmaukar.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2nsnlbnjt.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cqpvxnfd.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mqeocaxk.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lhooiref.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2wrzibloc.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2bzonjkru.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2cvrqicbb.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2eyhcpgzb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2jvvbujhs.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2jhisadwz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2bstomfzs.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2urluzgiv.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2lbhgbckx.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2gccsfgiv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2kgcaovkj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2xqbmozrw.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2xbjepygt.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ktanfugs.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gwtwelzh.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2kajfhdch.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2gaofpkbv.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2tpiqztsk.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2qdlazref.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2ovyoijcz.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2akfhjvgp.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2icpdmtss.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2khprwpdq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2sjyrmraw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2hdqgbklv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2svyifxkq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2fmjxxqxz.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2icxmngab.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2jfyumuat.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2kcdpweju.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2uhcuspox.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ccftvyws.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xkbcdhxp.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2fspvuzbc.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2camkloov.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2cyyzqddr.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2nvnhsggp.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2ruwmngda.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2sjfpbyow.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nuuwhskm.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2hvfrdsym.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lslovrev.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2kedaabkd.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2adsrbrhj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lwbdchfd.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2ltnviukl.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2cmhprnct.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2qoubnxjd.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2zamkldaj.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2uisknpcj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2sjnvaygj.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2kdmjoahl.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2yzakeydu.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ekxjphvk.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2yqxphmse.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2qktsdvzl.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2bcuocbvb.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2lvnkcupo.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2gtwfyinf.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2cbqrdckr.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2xzclyuuy.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2aqipmafi.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2kscqdjpi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fwahpmiz.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2rhbkhcgb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tvqrberk.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2gcdjyxix.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2fitlglfx.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dsxrcots.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2phbunckg.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2plsujifc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2titbvetf.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2rztxubfv.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wtdzgift.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dhkrdxlu.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2sdxqypvb.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2nunqdquy.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2jfvikjgi.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2hnydteka.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ddcsqswx.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2tteefusg.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2xpmiojjg.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2wxivpuhr.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2mqbxoupq.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2jcbffiwc.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2bkxztpom.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2iufelupy.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2kbvrscri.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2xwxkahks.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2vaibgvnn.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2fpzwsmqc.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2qsmoxhrv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2vyrnqbfl.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2soxpdhmc.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ekvqyfwp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2hzllrajo.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xzhqmqwk.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2xygcnwag.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2ekyixoed.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2clkhrfcs.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2dbtjyelu.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2lnekffez.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2jzgbqxmy.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2urpnuoky.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bwmodjzz.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vnmruspv.html


<!-- 参考信息 -->