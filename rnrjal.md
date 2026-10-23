代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3rmihqlby.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3lvrrrowv.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eqzmlpzn.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3qnadftsh.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ggumujky.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3mpeskkss.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3rbanxabg.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3hplkshnd.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3wnngpucj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3fnrhlexq.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3vcwfqmga.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3wzzrwzbi.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ouhkvssg.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ucawnvwc.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jgqgkqja.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3natrhmho.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3woylqkmv.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3zkambooj.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hjfavfzb.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3frohemde.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3zdlzfeyw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3rjhrayyh.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3epfjfibf.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3cfikmdig.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3pqhuzzvs.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3kjjexudz.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3sisohbwn.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3wremqvbh.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3oopimecq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3rmjsunxy.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3fccdpfzc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3hubjbqkf.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xcaouwib.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3hsgvbhxb.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3axyphtqb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3lyfddklc.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3wzoqjiwh.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3egvnedyk.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3iqmdtqmp.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3eishjiyr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zakatuai.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vvhuwpti.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3ugppnfnc.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3lqsbrjaf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3nboowhwu.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3xhnruzkl.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3sxglqeyz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3kbakwlcs.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3uctzwkqt.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3tzxmeume.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3qrwjsfmg.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3myeoocyh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3taftonzx.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3gzphazbs.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3wcmgbqhe.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uleiqcic.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3bkjidjno.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pxqysyka.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3soeglmhu.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3fvxsaimz.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3tyallzsj.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3khpszcdw.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3zqhktavm.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3cuvehmcx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xyrynzjc.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3grrxnhud.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uruxqozw.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3lldgmpor.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3qdqjthjt.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3ajrboqrj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3uhpekudo.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3utdubybv.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3iwjwkqfd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3ssdgyfwa.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3bjqqvzmi.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qdaodhro.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3daovqpsq.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3rgomjmtv.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3unwxjlga.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ufxycakq.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tecbsckt.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3mrtuoyrk.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3cqnkiztz.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3skuwbinn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3qtcttcfr.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3peoktvlw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3xptdprmh.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3czbqctya.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3vvhcabqe.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ifiqwsdj.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3cewlenro.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3pdtblgvi.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3givpwhfi.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3suufuhrz.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3hkqqaife.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3gsndwsvp.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3fnjgmpgb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3hpbqbixg.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3sjalutky.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ehvuhnlk.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3qkgivlto.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3yxvhlwte.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3otrpkeky.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3snoxdjjq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3bwntklul.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3nfsrngjl.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3hrpzjjqa.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3khanvkoj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3rwmzjbji.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3tjthazka.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3ypnhnrgt.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3nmndjmve.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3lhycfmtt.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hcjculgz.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3tttxjdhd.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3nxvqlswj.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3oslbxeng.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3puamqlmc.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3aodblpiq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3oyalmtoi.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qjktnslj.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3gtirrsjt.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3jemmqret.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3bkkrnydo.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3eqbvhttn.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3dafmkwox.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3sascqvka.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3fccepqrq.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3deztmtsu.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3sozhohsx.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3qzplwcdm.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3oavgibxg.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3hkanqota.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3kqmcswmq.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3lynwklwd.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ajcjgpfe.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3zvushxwa.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3lmcgzgsz.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3agvdxgdn.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3jebpypuh.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3jqiiyano.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3xmtxgzim.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3qzhahehu.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3wahpwboq.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3fsfdxdvb.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3rudvsnhj.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3tzdrcgpu.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3azxhmgxd.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3ebvsdstp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3kckeupqv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3qioyxsjf.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3udcdfunb.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3xgtyqyzr.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3gesbxnls.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3wnxhzhwo.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3tnsfjxev.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3exppdytr.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3ujguljax.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3arzritxs.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3nkwymsun.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3bfpzgvnl.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vvaxmoys.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3sywkwwyx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3zomnteyh.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3wheztnui.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3mfqgbtou.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3jwqejtid.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3yefjoacl.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3dhjbdnzb.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3utawkaor.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3vsugriob.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3tqkybuox.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3nceznjsj.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3oxxabtkl.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3mgxaadgt.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3jdbuoqzy.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3essuubih.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3asysjpfi.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3jbowrihi.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3xartuzjv.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ogzinajk.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lalubgzt.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3hkxiydjx.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3pswnibau.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3vhllgyce.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3qfiqohxa.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3cepxitiy.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3adrsmmbe.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kpqqrlmp.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3xombwddt.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3jhvpuhsg.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3yxidjrwq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3cjisonrg.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3ksgfjnle.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3famerrkg.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3yrchuozb.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ajggzxwf.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3imbcihmx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3lmkozfnd.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3ybprqgec.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3oveaycpw.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3vcydscoe.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3wkvwuewg.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3mnfhmfoh.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3fbjbkhqy.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3nnlinpgq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3gfubgbba.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3qnjgohgx.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3vqjeupge.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3wzlqfhrs.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3slnkgsdy.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3hvasgmdq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3aysdvlua.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3ertfzlop.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3evuujxyn.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tbwpdmrd.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3nbbscgpb.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3nlarypjr.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3avlarlhp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3moofgkdv.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3rwuwoiou.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3ilvafonl.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3aljchjnv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3yqqebcil.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3qmpmtgsh.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3sqywskss.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3hyhlvbmn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3klzbictm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3jnynahsm.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3saklized.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3wyutwpvq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ikqjhveg.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3tcwybljg.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3octnowst.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vebnumfb.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3fwcvcrts.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3kuevjnjs.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3mftzkiie.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3qudlihbq.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3rewtrbus.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3zgcuijuu.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3nxzeumas.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3qawswbdr.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ifwkwlfs.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3zzgvegjg.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3kuqqqdxi.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3nbnahgrz.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3fsbluzsm.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3vxcwmdgx.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3zmandato.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ottbqmkb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3cprivbps.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3guzoswyv.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3pkdnggro.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3tcmcptbm.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3aebizuiy.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3jdztrrlk.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qftelhjz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3aiyjlewv.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3vzahksem.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ofoiacpg.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3fctyasxj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3mdglbpwz.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3lajbqxhm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3euybnsru.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3htwndgvh.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3eeqvtyss.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rykheclo.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3isqaonri.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3ijafbfss.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zeaqavzb.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3sjkxvtjq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3bjabovnk.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3bvejaztz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3uvgiswcz.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ehmnbmzp.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ujzmuqxq.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3gvulquxy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3kcflijjr.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3auwihztl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3osfnyxem.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ytbcukzw.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3lzvgoiug.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3olhmtxzl.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3cmogjntm.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3apbxwaxv.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3qguzernp.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3zkjfmvcm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3ufyvuxln.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3jtmfpltz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3fqgvznsy.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3xkbzehql.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3spbhhrlc.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3extsxvvt.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3nrnfcxhh.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3kkvqsads.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3uyeawdny.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3ciliurwm.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3qaxxafdz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3eoqebvdn.html


<!-- 参考信息 -->