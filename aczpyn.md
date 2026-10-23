代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3fndfrfia.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3cujxwjcj.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3czkschrf.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3qrslodnt.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3qnrpmlur.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3arljhvhk.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3qfzlsoxz.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ihvdiqbo.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ggqravpz.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3lisbfjba.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3njxdfqvr.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3nuoauljn.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3jiibteze.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3drdiuozy.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3uhhuonqq.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3mgryzfpp.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3qgmtvfaa.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3iqhwpuiu.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3yfloscmw.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vgtvvagy.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ahgayrrn.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3huixnhfa.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3hyahzkxc.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3qcellpaw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hbcspfps.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3ybmyoypr.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cmhhssbr.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3lwyhfrqm.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3ejdjiokn.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3nbyvnxyv.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3qdocthmr.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3nnncnqul.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3tlnskwqi.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3chtqyugq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dgzsuevm.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wjewdnlh.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nsqoflks.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3eebtuywf.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3tohatfxx.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3xufinibi.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3cktbaqaj.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3ukczadcv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3weephjrs.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3lluzwpix.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dqcbrowi.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3tsptrtaa.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3xkjglzeo.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3aekggpbk.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3kfqkxfwv.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3uakouadk.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3xzhqbzbe.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3sywlnadr.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3zquaresp.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3mjzsssch.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3gobmytad.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mothbixe.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3vugmalpk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zsalliyn.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3znwsjmfa.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3dowhcwdm.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qlvhleqh.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kqfmanxk.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3shpphcfw.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3wofjjbug.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3shdwxdyi.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3twgrfhyz.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3useqnceg.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3fiveplto.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3smffdsqf.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3kccrccoz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3abuylxen.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3yamgciem.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3cgqvyhlz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3tijqlxkc.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3vynzfskg.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3wmtzbjnc.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3mahvanms.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3aeizsqzc.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3hpythzym.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pktcciff.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3gtgpbkkw.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3rvfhqzcj.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qokptoyw.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ryzggqtq.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ztdwcwyf.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3atrnwvku.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3jznrkagt.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3ixpjbdzf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3vgelpzaw.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3lrhilgas.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3usckxekx.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3mvoxxwji.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3wdbkreta.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3xyjizrrg.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3lvsyzurk.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3rdzndscn.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3jcywxreq.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hhnvnbzb.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3uxbebvdh.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3voilmrzc.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3vigkeyan.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3viuwmsfz.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3pjlkokxt.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3sgpafblu.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3eyhnyjwz.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3faphpyvv.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3izpeamgf.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3zbjfhadc.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3zwmgwntj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3znbdvgxn.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3dwjpnzkt.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ooqatlhi.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3uogvpfdf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3rtjfmqsr.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3omjdyqua.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3dsnwxxia.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3yswxrflp.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3jeqipnxr.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3njfjbucf.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3siajubep.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3scwctovc.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ymqlgemm.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3svivxurc.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ompztgvo.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3yekicfky.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3hrowodqz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3mhcawnqg.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3grzsflze.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3kquydnex.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3ztdqeeqq.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3oegjperp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3iggiosfj.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3btvwgjxe.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3dkyaqbjb.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3xxvcqwha.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3fnmndzgj.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3zwnewdxl.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3dogbbakf.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3kxtrxmkg.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3awgoirfa.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3cjpsdosk.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3mwcvpsly.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3zwgbwhhz.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3jeqtzmyv.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3hoayokli.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3kzclqdhy.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3kxmfxxpm.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3yzzizisk.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3nmmyanii.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3edoojjjs.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3vcwxhgjc.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3dmvxrahc.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3kutkjoxa.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3qxhjxlkn.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3gafihxyc.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3wqjpbhpn.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3qlysxggz.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3hvogjkrn.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3kaxalmjj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3jsxuzxtg.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3hkxvjufb.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rqmzspfw.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3tudugtmx.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3yxaxxuww.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3cxmpluin.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ebnevwax.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3pdmzcael.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3cqtqdolj.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3txkrcdic.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3oiqlfdjh.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3bssuwmeb.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3fkmipemy.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3fxrdrztx.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3moepdrlq.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3tfvpnvof.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3wcbkyxcl.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3lzuhguzm.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3nmwcbapo.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3mnnjwsdy.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3uxtrbkge.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3yllnkwok.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3qatyecxg.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3dfmkjtlh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3zexfujnd.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3igpuuykg.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hyaygowd.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3rvkfjnqe.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3kaisqiri.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3eawcznvm.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3chjeomxc.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jirczkgo.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3xxzpiiaa.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mmifkfob.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3nxnxzytn.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3mthtocrr.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3labijzaa.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3pgozcizj.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3ysfbmaai.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3bblbyyzb.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3ofbwovgy.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3xktniihv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3urhrvsxz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3ztovsixu.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zasthqkj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fixzhcct.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3odwgxsjy.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3wffohyzw.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3zkfgjgwb.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3kaixphqi.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3pwmjgatq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3fbpqwfzm.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3hnghyzmw.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3ldjfwgyu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3pmbudkpn.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3cwqygpyh.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3hjewsuyt.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3vabgdver.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3dnhryjnn.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ktfafdze.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fucjhgye.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3alyahiuo.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3nutwmjuu.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3zkgplofv.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3ziceuyng.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3jhrvivnn.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3pqyrhpio.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3ogbhqkib.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xltjzvlo.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3qmhuoces.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3plsxhjuh.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3yzwmksxz.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3chxkcble.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3qduzysuc.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3afmwdzsn.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3kdsbrkhy.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3jnoxmpbn.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3azphfvmf.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ovvcjswb.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3itpykwhw.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3avqvwtgo.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3vqnkrzno.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3zrpkcdae.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3cdtyhmrg.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3mckfcjeb.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3remnscil.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3bshzeeyd.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3dyjritme.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3nonedrcr.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3hzlmebeo.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3earvrvve.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ljqlqetf.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3ypothsmj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3vnklsstb.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3nqezgfwk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3bkvchaye.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3qbtdrbcy.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3wrfovwan.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3qwebwuyj.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3wfmhfhlr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3zdrzrsgu.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3bjegpiau.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ihrkwzsu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3hrqhbcyf.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3bdgssylj.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3kjfujxcq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3imbksvmy.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3byznnsbj.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3zypmaunz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3nsjcugpi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nenzugnf.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3yivwfezb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qxgzenep.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3loqjgotn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3iralfjjh.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rsmhofyw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3peyqmuhp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3kfejtmmf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3lcvydxww.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3vpkqbghp.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ywbbfrfd.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rxotxrtn.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3qjyvrsjj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3mrheygoo.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3ssuapwsv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3midbhuay.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3getfpyqm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3qgrdtldu.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3vgbzjvmi.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3rkudbngs.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3yeimhtqn.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3qyceqayl.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3wlhfvqqm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3kktwphpt.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3cxbkazgw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3fgpddsea.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3nzhpgytl.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3jrqizrzz.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3zztnpsdc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3dtzlndgc.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3ubfdcpdd.html


<!-- 参考信息 -->