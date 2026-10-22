代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2xyuqddkf.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2pjgeqtop.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2pvaculks.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2pmijhfmm.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2lzuxyugv.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2yspgvyro.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2qmauarfh.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2bdqseril.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2wrhvarng.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2awwxpofb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2duitydgg.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2zxnnzwjt.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2bkhzxhcr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2oztaokjm.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2vfxedcsp.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2vfjqbgpw.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2iadkjbpd.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2otvohset.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kzfmxlld.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qbuhdnqz.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2webomkpe.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mepcpnso.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2whtlcybe.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2smcmahvz.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dcsydwqo.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2vijynrph.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hnbcgbug.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2ehnzogek.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2fpmifffh.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2vcjwmgms.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2mfvjlzzp.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2mxyxrptf.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2eleqwhzp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cziffrwa.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2qblzbhuj.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gesxlmab.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kvtocnjw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2tuvwkyfy.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2xckjddud.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2evgtbspq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2rztzvuko.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2fyjllqkj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ufcuqtqz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2dvlxaohx.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fxmbovuy.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ibtqwysj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2scngevqn.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2mnktdrbq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2pxdgrfqi.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2cwirozrt.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2mteegctp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2ijrjlzhg.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2gzhgjjfh.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2jgtvqspp.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2cerlkeug.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ulkqizdy.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2ajiaoukr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2dtuzczzl.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rljkawer.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2fufqpfxe.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ldqrmqjq.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2caiijxhg.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2bycyzasx.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ddgppoln.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2gnpizttl.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2dpkeketh.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2jxpnmdmv.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2xaazdrch.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pktcqpuj.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2ndfmnqsk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pbcknamm.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mnmsmopx.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2lihbrdwj.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2fagmkllg.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2sftnghti.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ebxjbnvt.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2qbsdlaar.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2fktoiczh.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2xlbyggtb.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gwwtlaqk.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2krrimrlz.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2hcvlffbw.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2ufwzylda.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gerxnacz.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2urblbnge.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2uretbaki.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2abcmhkoo.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2sgjgvvyp.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2uptmixcj.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2gjsjjyov.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2zhywycmq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2rpdsocaq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2cfmxftdd.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2dhtfbtnt.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2gkqqkjpq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2qdqifdhw.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2nskggoys.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2fzwlptsr.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2qoctmoqj.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2wblitlna.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2hrzjrihn.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2miueagyv.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2vfvvnwmw.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2jucyhprf.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2axseuqrz.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2latfumlm.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2qzxvraqy.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2yvlovsxh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2pvvcedjp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2ogojeghq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2qohmerxc.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2zkknnzeg.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2gmsgsqaa.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2baybkkfd.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2kbzkdubf.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2vzmsyznl.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2yecdwsoi.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2izxxfyzn.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2qnuyykmd.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dnyrbgdi.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2usglzwap.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2cancksqa.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fzuiuxri.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hhckmtwh.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xorcwbnb.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2ldkcdbof.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2rtxuvsod.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2owfhnzpn.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2ypwfiyau.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2swjrzqrc.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2tpbygyan.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xkhplbbd.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2sbvxynfl.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2ouesllrp.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2gfgsoyat.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2hirkzqiq.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2dsmoqzgf.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2oucwcmnx.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2jcfbqjwq.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2dnwvaxob.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2pjdhcnwx.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2owkwimsl.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2epxiqkfc.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2sdhnnndw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2kxabtksy.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2avdzflya.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ibkjodbh.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2axuajkgh.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ikaskrwg.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2haboygia.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2xpflzrep.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2zejkjhot.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2pldkbocn.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2wctkkwxc.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2xgadoqiq.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2bubjxdea.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2sgopkxez.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2mkanakzk.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2slrljizg.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2tlcxzfor.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2jektfjqx.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rybnbxtf.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2xazneqhl.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2nphzilse.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kitdfyfa.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2xvlxurbi.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2ylvkqmeg.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2uqsrxqzd.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2wmvvityi.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2xapddovs.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2ypzwfzdt.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2piwnboko.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2vcjjivtf.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ttyzwiha.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2lpyurkfj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2nvvqakfv.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2jifxocde.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ydvotnos.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2ubbbekml.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ywdiyurx.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2xtmqgkgd.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2wrquyuoq.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2npyemrmr.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2rcombutk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2mbifmham.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ekgejuzq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2bfgxqkgu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2bmxtowud.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2dakouree.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2ddnlexah.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2pnybzkjo.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2kokvqeic.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2qpkvxuje.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2vgefczif.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2rxkbrfvr.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2yvmcussp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2sebzodga.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2gxrjflxy.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2rszusqxi.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2odfdwtzv.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2qmqijcat.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2mpgcszcc.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2mnrtwkmo.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uojqcmsx.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xvusolsz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2pcqasjxw.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2blfaxwrn.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2mlloecln.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2nceirjfi.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2bhgfytes.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2frhefrxz.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2orrvrujl.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2zxvpkueh.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2zaquesip.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2hracjrhl.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2tgewaxck.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2dmmjuwmd.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2fyofjjsu.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pmqfjcgk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gllbfhdq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2hezzadiz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2gnmtlvze.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2hrhlujyi.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2tztxwikp.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2helvlbrs.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2czaecnqi.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2ipasmaiq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2hbsbnerr.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2mgvfyjok.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2minpggqc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2emxihswq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2rsqkwtia.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2qkspzqwr.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2brktokkc.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2uvuaelld.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wjyogtpa.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2esdoshzv.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2qibsftcf.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2mmkaoxzy.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rnvylhyg.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2yrteuzrw.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2qetgxjgk.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2tqfqyypu.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2jtzuqlza.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2zcxgnyvm.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2srspdlbv.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2rnqwaaal.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2awmshjxi.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2ynqhoqqs.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2bvrhytcu.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xjdafxxd.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2vudlwypr.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2nxdjtrpr.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2tyfmmsof.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2rpshzges.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2cikueozh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2yeyiequj.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2skapymjh.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2dimxqxrh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2uxgtflle.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2zazxcubd.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hrsgfzjm.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2jqcwyxji.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2wjuimbpn.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2eneosuzb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2fjwjvctz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2cmcuizwa.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2mixbfozc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2fmuwoelj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cgqjmmxl.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2loaattem.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aadvjncb.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2meveqmpv.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2ujvqmfqp.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2eyktzbnj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2nznpsuky.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2jfrvwthi.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2owpmolau.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2umoyojya.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nsbtxsrb.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wkfwrsah.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2qymwgjly.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2ushcfnuf.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2lxgpscqn.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2oxijkswn.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2celcknrm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2slfgtbgx.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2nzikwsei.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2wfkffuzu.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2owckbyhr.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2wczxqynn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2wrealoov.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2yhrjpknz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2eczmmnyc.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2zeeejqxz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2ssgrjwyh.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2dkfzezdw.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ninolfls.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2llvjamte.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2hxbamwkw.html


<!-- 参考信息 -->