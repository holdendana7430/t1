代发 wailian999

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3kvlpibjr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3vnxsekxw.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3iotribnt.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3lsaoifda.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3pkzotmlx.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3pusmazuq.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3luvctpqj.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ymzcnxpz.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3awxshnzq.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ahgwfeoi.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hxcyesda.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3xjtyndiw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3gbxwzlkc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3bgygfksk.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3sujrohbl.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3qmnzpcxc.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ghycclfd.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3cuiszswk.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3kjktinqf.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3niyggrss.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3otgwktml.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hzaaczzn.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hljgjuup.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3izswbszh.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3raoeheyn.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3ffhhlwsb.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3bxcomgez.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3yewudhba.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3akeuaspp.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3oceoejuf.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3xcxshedz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jwogisvy.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xculaxim.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3lnqfkonv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3xxycrugp.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3rxdrtgrx.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ncshxiyn.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3qdfuaxaq.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3inxitjsb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3pjxcjgwh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3tbaxpdvk.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3qyecvbpt.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3jxrlljoi.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rhylpufm.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3bjikfcnt.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3espcntqv.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3fsfkvrit.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kyfnqhng.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3boqaqmcb.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3omjlfkcz.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3yubmuffk.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3aopdvuel.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3kqvconbx.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3kowtejrr.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3wusrbcxm.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3ublnqpfq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xdgxzskc.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3owvrwbcf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3esnttpvw.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zlfurvcn.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3ealrfivs.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3lgdwuxcg.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cguabmbt.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ueeonpeh.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3smuscvad.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3jibfazra.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3ttghwfoq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zhdxvshf.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3ntsifwsk.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3dmdpxfyr.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3elvxmusw.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3etknoegy.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3awzikiyd.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3yzpwlfci.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rvkzfehk.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3qycrjjuk.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3rfkvhtbw.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3pfhufxvw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3vibpbhlz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3zpsybfwq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3aftrllnz.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3uwcorgba.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ilvttugb.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3pycsatbo.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3kdjskqdy.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3peemeugw.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3hoafjtep.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ulpfjrws.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3icdksjyb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3ivnpksai.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3rabdbhnf.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3oucpnelk.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3wmsgrxpi.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ukzaonjw.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3evgdqccg.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3cxyxzegb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3dfwplpsp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3wrpucyht.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3kmjhdqsv.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ydjqebuw.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3dpacrbis.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3nuvhbxis.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3coixxqfe.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3qcskvsos.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3krbvxgls.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dbfnvpdj.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xidepvjf.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3epjqjlpv.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3efejgxxx.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bsufgfyh.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3bkqxigkp.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tshjohmv.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vtvgshds.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3tevbqbci.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3gmpvjhsb.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3msbrovjj.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3udmkkhzq.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3ulujqfxl.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3mreblfpc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3gnxaujij.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3jxewpujo.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3gcjllgdh.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3chwrtrgx.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3zstawhgr.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3utngkihs.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3agjgkmkf.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3mjwhpazd.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3atdmqdbj.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3fxdpewgu.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3mwhmazft.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3yercsvtw.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3jrarflht.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3cultwpxf.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3teowevcu.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3twehzqng.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3efcbcxtw.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3einoipuw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3nnvawubq.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3bjxleqql.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3kyqoqkmt.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3yjrpueap.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3roynknkc.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3rxmjjiwz.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3mhlutpik.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3nmaqangc.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3oziqnfgt.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3amakgrsq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3pazlkoun.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3sfykfhxx.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3ktnmeoqf.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3lyymswly.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3unbsekpf.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3obcxgpnz.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3upcghvtj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3cicvlfeu.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3phxwmpcy.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3lwbxzfnr.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3jgfgekqx.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ulvvklwn.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3kjzjpawo.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3ndkbgeax.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3iphwppzf.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3fmvtyhis.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3cqdbkopy.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3egmniuwo.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3bvuswski.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3klywwydd.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3qaizvjog.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3wptdjzml.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3scvrxwws.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3tegvzhqz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3lyjnsrdk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3xqtczvst.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3mfnfujyh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3bztaglxt.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3hdpnioxy.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3jxmckysv.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3adwgwbph.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3gzflkkos.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3bjwbnfvl.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cmbkilra.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ohkrhffl.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3htiyilah.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3ryxkxvgm.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3vvmykvep.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3shsdifhv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ezfdggug.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3spzklsbg.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mtwgirby.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ewvwnbgp.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3uxcfgauf.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kjhyezbi.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3ohpeftdb.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bzqhnbgl.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3lafnanif.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3anvpqmmv.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3tslibfbo.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3ektodbkj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3qhfjeedm.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3gvhudwjl.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3niawhwxd.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3hzqmvmfz.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3lnpekroh.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3ocdnuvfn.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3dkiwdqdo.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3uajakcqv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3yvwuczqk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3szkobhns.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hijgvkgk.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3zpygwkqh.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3ztdlsxme.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3htecntoq.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3uywbaaui.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3yuywarna.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3aayhstes.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3jrfiqxhk.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3eazhgydw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3hfahsgxb.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3qrkwlfca.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3uiriqsco.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3itdmvaxp.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3hpybwycl.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3zmeycgxv.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3nyigwztt.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3kvjrqtbd.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3mnntxskv.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3szjfotuw.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3iyvedpsm.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3zwhagjqj.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3buhnlnnr.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3fpejmdti.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3apxabwjf.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3dyqevwve.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dwzfffcg.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3tadgpwax.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bczswjny.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3hijeidvw.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3ttiirnzs.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3zdfqcvgx.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3ittixgza.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3yxxjhorr.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3wxefeotj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3akeumulh.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3wcjkqblt.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ubqfqwpg.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3ypzoyjwv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3okgbhnsm.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3smrszcfd.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3vblzubzr.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3ierzdnii.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ppsdsjmk.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3eevmkbml.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3etranbil.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3aiouexhw.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3etvuviyr.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3gtwqpbup.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3vdzjkcno.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oflpgyai.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3rjkwctai.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jwjbgyzv.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3scptdsqm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3dflnedyl.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pfgkidld.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3leicxlhx.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3tjllipat.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3fvgikhuw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3cqqmibke.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ferkwnuo.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ulnbojxl.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3osgcnthr.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3swcawqzf.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3kwnugyjd.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3odwxfbku.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yyyxzuvn.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3bzfofuih.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3hpjjjksc.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3hnpzacmr.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3waersyzg.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3vmqgmzqc.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ervvofld.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3pyfttwjg.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3vdplkfjj.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3zejiopty.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3ucgpsmoo.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3vefhqqwf.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3nmpeslnd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3vahmjzke.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3jvzyuaka.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3uyweqegz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3ujwiswjh.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xuslpihu.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ylzlbbck.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3dtmqzutd.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3ghchrrue.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3yqdxhokx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3qmcferxm.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3hchvikdj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3aybxmhji.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qnxpdqiq.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3arxatbnx.html


<!-- 参考信息 -->