代发 wailian999

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3lkiigxhm.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3mizrijzi.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3iwlprran.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3slominlw.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3yykcqoak.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3younpzvf.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3izfagmzu.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3ngngkqfc.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3hqpoqszi.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3mcjmvzid.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3maofoxld.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3iifbghcy.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3jkimrwyk.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3keyabcza.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3toeimtoq.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3haqdotda.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3ncycbyzd.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3zytmreeu.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3pevkamvv.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3sckgjqxv.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3krjapbsy.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mzlyejhk.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3cjvtsokp.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3mmmkxvlj.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hvoddooo.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3wewroqbu.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3exdioixs.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3gubwqpcm.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3gqjihcuw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3vnltvdxn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lmwqtnzr.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3gngmcxpy.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3cxzobowd.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3vjvibahd.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3ipyzzwxu.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3ridthkha.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3dgkrkdkw.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3niavaltb.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3pkwpspra.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3opfczrmh.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3sfpjlatx.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3sjugzruq.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3byblkbvl.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3dzdyhsih.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3icubbent.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3xooxnxeq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3occspiba.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3gppudhak.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ewckkscs.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3iqcvxobd.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3xfcqnmcc.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3pmxsjeuq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3otlcdrob.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3zplrastd.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3lbebcamq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3yigyxwam.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3tnwppynp.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3vrfnrqzp.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3rolwiytw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zkrvmmcg.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3zcfphoot.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3baqvhinc.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jacoarnm.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wuywomfa.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3lhypildy.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3ehtxwcjy.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3nknfztdf.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3gkykvjjz.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3jqrjcqqm.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3rblpccvd.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3lashzcvg.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3ptklzyxm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3smijbrrk.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3wdspxlis.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ueezvnpf.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3zqtlemjp.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3djhjazuc.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ihmzgzhq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qtlycfxm.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3edfpgsec.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3mkhmlzgb.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3ovsjdrzo.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3bybqbsuw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3uahlgpfp.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3vmpirces.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3vupuvjty.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3rjdutxkk.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3aomrurbw.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3durfkubn.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mcwupndl.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3pnvsdryi.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3movlwfus.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3lsemtukh.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3juzebvss.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3aacwupmp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3kcwsumqy.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3fsqtdkiz.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3vfyyzpul.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3rmlgpfjv.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3krpnkiay.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3zimumemg.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3qphkzdra.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3ljneiczl.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3wznmdoev.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3jycotwcs.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3gpuhsmja.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3nqzqwsgg.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3izqwhabs.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3isxhzjjk.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3kmpfmvio.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zrqolssh.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3wgoyzwcm.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3uqbplyqr.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3hcitepvi.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3utgmmkeo.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3oemavsob.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3pvldihju.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3iywidrfh.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3siksoxll.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3palcpyrk.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3gjczkqbz.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xtvsmxzb.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fiohgufg.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mqvxvnzy.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3veenhqte.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pjaurnzk.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dvrhiitn.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3aiaysywe.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3aiqjugwy.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3nhbzmqwz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3hxjgfilg.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3apfmuczo.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3qmjrjkqy.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3ieijadwn.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3njtqftlf.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3oaskfgmy.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3bjmbfueb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3qxnevyjk.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3cdwwjvhm.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3bnwuttiz.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3efhoyzyh.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3kvqkktzx.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3wwmxuprf.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3zbyzadxw.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3fgszhweb.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3bglqjlcf.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3qzdrhqoj.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3npdguinx.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ditabrwb.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3cxrnmqei.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3eeqjnsot.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3axwmwfdu.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3lqndrcar.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3gtscpptw.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3wryyimld.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ndbcfcuy.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3gmrygrls.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3nzgitzkn.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3shbuflxi.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3wcbsmvqt.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3sbdwwdpk.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3uqcfbzsm.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3wmykpobl.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3lahuoxcf.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3vencmmin.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3waurxlaw.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3vrqpecyd.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hpztqlxr.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3whmfcqyw.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3rzzmwbhq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3bbkwvmqt.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3igefobmu.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ksgiweeg.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3gpepanza.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3hddodtmc.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3rufwinsw.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3ngvcrdsv.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3bjsbzqfn.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3regczpir.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3lfucmzaa.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3bdefcsje.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3wdefavlf.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3ertfybvn.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3unmjenke.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3gblxyeoq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3lkiwkyzm.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3gvptttln.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3dwopwaik.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3euxssaos.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rkerxyit.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3nuodsojy.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3yrbykzpx.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3puprdnxo.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3uscucrps.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3iloettha.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3oyzccdzu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pxgagghc.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3lqcnjyud.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3gjfptzce.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3jkgepejt.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3oastwlcl.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3cynggppx.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3nehajrjm.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3gujidjid.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pwkymdkx.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3rrwkwwev.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3qbegkfxz.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3bddsmubr.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oitylhty.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3evrgpyda.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3bomhatyd.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3czhbedbl.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3zpnbbmiv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3rmgpmgjm.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3vqxffrib.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3nxayxsrz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3sndrtwef.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3vezwxqnj.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3jyvgkfzg.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3smodjexy.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3elqxmykc.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3ylfkmzdh.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3afzcrzny.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3wrhjjqjr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3watjrqsi.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3icoaiggs.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3vzbpnfly.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3zlzpuqbv.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3xvaunbpx.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3epaobpvj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3gckngefe.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xjnkmoke.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3wmgqavhh.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3haeolcsl.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3jebgdbjm.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3bcgrqxwz.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3zwzsfpis.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3zvfjqefb.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3kyycfkyd.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3imhmsayl.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3hjitycla.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ykeixicj.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3atwqfddj.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3pysbvuvt.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3dshqcnof.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3tsgffgqh.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3dtgdlvqk.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3yurdtjsa.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3rrxbmlbw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3tahqymce.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3ftamkroo.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vaqwsjct.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3ymjjhcsi.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3nzhpevdp.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3fsjdqfbl.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3jrclkjva.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3ofbarnju.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3vjtlfcuf.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3tjanfsjd.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3vakcujeg.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3huoazrco.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3qewyfuaj.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ykxhgohk.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3hheelsgt.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3fnrjrlpq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3miezviku.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3xvaukzty.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3sbgkwlin.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3jzbquirr.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3yqbszxzd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3gzzughoe.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3gocqnbcu.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3misdorno.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gbkjuweh.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3pcingwxf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wipovcmn.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3zwbkydoe.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3pulyjnja.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3npqflddt.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3gutuymbf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3vnjvjrau.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3zpqvtcig.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3fxvteyhx.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hizphqiy.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rfquqcdy.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3xowpospw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3rbpnohqu.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3dxxwkvwd.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3vrtqgidi.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3kggfydrn.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3pxznpdod.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3qzztksti.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3iywyerzu.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3vwtxudws.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3ierqtmog.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3hpcceknl.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3vvbjjjlk.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3mqqkvfui.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3kdzumpqe.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3pccaaykb.html


<!-- 参考信息 -->