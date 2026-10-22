代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2ddzwtugw.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2frbcvgza.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ayjvmefc.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2bxuimvvh.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2gmncvznq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2ipzzmyxm.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2bvjshsjo.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2ctscrptg.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2lcfriyts.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2tbulpxol.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2mhmizkvq.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2ioncvnaa.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2qrrlcbgs.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pmlveuwq.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ruaslhgk.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rsxcfhpj.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2geptyzxs.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2celofyvp.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ovgeqjqy.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2uknjoeuh.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mgaaqtnj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2pteuqgxc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2snqqigjz.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2gglxhpbx.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2nkxbsydq.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2jjfnxayb.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2entjvacv.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2cknplzsd.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2xldjlfgx.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2arojgyag.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jodusxor.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2csjlckce.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2zplbyaar.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2vizmonqj.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2tlnzthde.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2dhtwgdvt.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2dnsuxwol.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2akcnphvl.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2wtpghtvu.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2llzxrwtk.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jvgterli.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2sdkfmtek.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2okpyplmq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2xylesdzu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2sqahxghx.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2ccfphwwh.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2ihpptmme.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2nrrnseha.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2ywlyollf.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2coowshhd.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2djiimfea.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2znqvgjbc.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2hffpncdv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2sskamddo.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2yxlrilbs.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2owdzpnci.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2gzuwjczp.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2umgggggf.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2nbofcvdz.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2gyxbgtwd.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2icxfniyt.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2znxilzvf.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2tplplwis.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2gutinvqt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2skiubnll.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2lwheoxcs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mhrwtthy.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vekhnauy.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2bdsvncbr.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2jfzaluvh.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bjjiwjaz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2jjlihxfi.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2pntsdehy.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2frpsjzen.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2txflaxqx.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2osfqiyrs.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2crzijdxy.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2njiphmbu.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2sphkhbht.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2hknnlspp.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2fmnezyfe.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fssuviza.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2bwxrpxbn.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2srdvyytb.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2zhjcqsar.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2dtohzqgm.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2wsimjnvo.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2gsvdywsq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2nsfeujbm.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2xxtszcah.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2lftrckrm.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2lmlsmuzh.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2qxiozidk.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2huukgrzj.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2fbpsxxho.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ulodnjvi.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2krkofiuj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2tvtfviwn.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lzmaeiag.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2pynepuit.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2devuyvzk.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2nzflkioo.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zvmtoxld.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2oecktbiw.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2udwjgmrg.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2dskzgsum.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2qavsiool.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2xiwrbifb.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2hqcgtxvc.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2gbmzulpg.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2hubhllcl.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2bmewwfvs.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2rsqrwkxe.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2sjtxisba.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2tzyoboqw.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wxjmbshg.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ayxwghdt.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fzpvyhyk.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2bqvybskh.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2waichqjv.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jezdsfpu.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2maubtjfn.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2ahhtsrnj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2qzdgheip.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2gexpmkpa.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ebafnqrh.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2rmpklhbc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ydxhshee.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2wzxtewjf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2gfcnkpjw.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2jjjbjoni.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2atxqukss.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2vxkqviyi.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2bvuyvpyr.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2mfopzkyl.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2uoqonfhy.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2alxsynla.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2tyyjbbwe.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2iqumbbzy.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2rnxhmrmu.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2poorxtgn.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2sxkgplky.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2mmkwuuuv.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ntttpusr.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2qjdjwtdg.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2augdjukl.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2yxilicbw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2lebhabfu.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2intsbjrw.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2znnghzme.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2xtgyatjh.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2xpgldwqe.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2vlhwnowf.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2rinpyoyh.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2klrepspb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2kumujqqq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2stmmqqpn.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zeoeprne.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ibpgyayi.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2obudzton.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2cwlknent.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2gxxmiuzu.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2irbjjzon.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2tifwtrgw.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2qoaikoer.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2xbpvcreb.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2ltzeiuth.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2efokcvcd.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2bafrnhdp.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2laofjqif.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2vhbtzgno.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2sulwuuua.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2wnpqthvz.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2dhlheomf.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2ticmizzp.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rdoggujq.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2lnzrbjrh.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2lhjpzdsc.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2pqtpvnln.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2hygakkys.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2lyrjhjor.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2nlacyzbf.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2tvqzqxps.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2umaonkbm.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2yjsqmtqc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2hrueisls.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2aibthxzt.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2bhsjgrnb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pkqnhyag.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2dypuxtew.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2dcoayldl.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2oncuaqbk.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2iwvxvfaw.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2zsjvhrif.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fzckdjya.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2snhgleuu.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2srooqxcw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2dupiosbp.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2rqsvyryb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ucizniht.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zqtyrjiz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2uzjstmhr.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2zjeczvqw.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2rldguhmf.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2gktzyugp.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2jpgueruv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2icwsxybo.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2vemumqbg.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2sfphpzjq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2wgkjqnew.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2jihxhfnz.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2ksyjvxaw.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2kgyysyxt.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2uedjyddh.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2phuktaeo.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zlzvqygc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zdqscfoi.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2rxhhyfwt.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2llchmwdb.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2gqwzfbdt.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2rzehxanx.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2digiylxq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2qwmfwtku.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2huolrsnv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2wlddifps.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2drqddeqr.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2bzhhlinv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2doekhcib.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2lzezcbrh.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2rncjfnqd.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2kynqxlnz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2tjlxpoos.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2ccjgsgvs.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2kprmyxke.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2injedjez.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2poarvpep.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2spcyazni.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2kntxvejm.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2iwrjumtc.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2pbbprivh.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2hlsexyhp.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2vsjdakhe.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2hmyvvzql.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hqobwkfd.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2kzgzykmf.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2rbbqqfpn.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2qgunynpz.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2vuuyvpmm.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2eamxqubf.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2rkahgpdi.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2jqlyjzbi.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2cgjtxtjl.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2zlpvvhbs.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2kwoxdabe.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2bkqvhhsk.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2rekprrrg.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2ftlvwwcd.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2xlhtyalf.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2kgdhchps.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2fwkjevfd.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2upwtqxtl.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2wgypyior.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2pzsfpemi.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2qunxqnzq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2vperpfqg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dlemirnm.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2yybhlqsm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sldcbegg.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ntoivrlx.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2pdqymubh.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bvgtnbif.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2wporzahc.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ykgctbtz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2seacthey.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2idczkrbn.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2givgqtio.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vnqhsfrg.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2phbrowal.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2wixtgong.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2hiaisqns.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aouaqfik.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ovxcvgkt.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2draootwh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2xoftmgmu.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2aacgzcza.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2bdqtydrs.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2acltthqk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2huspkiwm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2rnxfsqyq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2bbpdjlyf.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2jcaaggsp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2ooxnrsdv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2bvgpoeos.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2xhwawedk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2cfefcytq.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2pthufmot.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xoiezyua.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2pcqlvcrj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jfmoitkm.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2nfnljhly.html


<!-- 参考信息 -->