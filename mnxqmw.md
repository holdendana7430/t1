代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3rniwaqhc.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3mkikrzku.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3felcadtg.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3tlskukra.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3htpsbjqw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3uygstung.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3ofwirbum.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3ethtbuhy.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3rkrjtufn.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oqxlokeb.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3bhtccyfg.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vqkialxj.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xvyeqgsl.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3wunvnilk.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3bpokciki.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3ltzzqsxj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3vwcyapmo.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3wonpddfd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3ygrioopx.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3mwskkhux.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3fchkpoax.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ouxrmuji.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3bpixrzrg.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3clrwibfg.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3jkhwydwk.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wuoskufv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ywgtylub.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3goioxlom.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lpapyalv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3nxdgdhaq.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3yslbfwes.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3poerwqva.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3jgvnxpio.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3wxjtgems.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3portbpqc.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3poupfhmm.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3sffmagvl.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3tpsxgnhj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3jahrhuxn.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3behppxef.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3sxvnhwjv.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3wqfdntza.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3kjkyilgw.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3fckxiuap.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3xsahsocs.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3vcerbucd.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3hmwngazc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3nesysluq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3ieruteli.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3wshjffmw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3xthcralk.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3riwufdhs.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3bzxxxdzx.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nzerktdy.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3dlswqsba.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ctjjoebm.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3wqfjcute.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3hzvvennf.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ifeyhvko.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3uojeviah.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ykhmjvpg.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3emleonab.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nvejafpg.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wqpcsjuy.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3jwaldkhh.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3fvtxursl.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3zxysxbqk.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3sfjvwamn.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3trqlyntx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3mwbewoai.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3btwhxhms.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bormcbfc.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bjtjsapv.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3zuwrtrwr.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3anccenvo.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3artgnpmc.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3wwgvswwk.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3pqogxpfm.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3lqicpsxp.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3zljtmilv.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3jeswjuzo.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3zfrpxjsq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3xflqelsy.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3puybmqeo.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3jkwqbqta.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3zhlcucgy.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3xtyxhkdi.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3hhhwoukl.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3xccxqtuh.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3oollisuz.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3xouqxwbe.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ymhmexsm.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3brnzpxaf.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3nuioivog.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3yuhywfuq.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3kpoynqhy.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3ftzjwnvx.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3pyjtlzsp.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3faizjcnv.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3gnvxhatb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3oyvvdlbj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3zrwusklf.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3cdigmepi.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3xnekciku.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ymclrmuh.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3fqbaodal.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3midqekpq.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3uwfycdwk.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3tprdelvd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3kgaelzlj.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3zqjblyxr.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3pixgkncq.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vkigfzsy.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3fpsxvhdl.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zyuvwyuz.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3euopxytf.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3imxklzem.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3pzxgvbam.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3vrmowekh.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3zmzztsga.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3amwlfqas.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3izqcjwft.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3jhdhvnft.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3brpxjdtn.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3tuyehdvp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3gnmolyyq.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3fnevjykp.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3lvreojyt.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3paewqhyr.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3mynrslgi.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3nhtymcal.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3eqlbnpqi.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3kvpsdcty.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3vwgzksys.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3aaajiwue.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3xtazkfcw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3gblxtsxi.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vvgkhkzh.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3txyjdrek.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3citkzfku.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ukixsyqd.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3jesseihv.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ahtiqsgw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3nzbgobcm.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3nhaogkch.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3gylgcyoy.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3bcslifhi.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ccxhwwse.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3gveruhxj.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ayduuayw.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3apzjsgsw.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3qdmjcobg.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3mhbwwnad.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3epoxdlcs.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3marmytoy.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3zwiuqybi.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tbsnmnyl.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3oujmdddo.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3lvwrqtvl.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3tkpopquz.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3qlbvfxtj.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3fohawlmz.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3tzidjtmg.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3uibclljc.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3iutdfqgo.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3qrnzrkhy.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3ppgdigkq.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3ofzveiam.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3lgqbolhr.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3hhwiudkb.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3vudyandx.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jbtavfkq.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3yuqjdaga.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3zpsqeujh.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3kklpmght.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3rbscjrzv.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3kwffkqyp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3pgyaweuj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3aepcumgo.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3otzzkypu.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3gritkkyj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3tmjdwzkt.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3gmydfzwb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3fxatfjrx.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3wmicjdpy.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3xyhiyrsc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3rypzttua.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3wzckvish.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3yyfembwt.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3qhjjddvb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3mjlaizzb.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mzvvpbnr.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dhxsccxl.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3rolbbgwc.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3ggyizgxl.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3knqmgsoe.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3teurqgtc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3oibksntl.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3zsevslko.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3maroiylu.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3weogyxwq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3qzkqjwrs.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3hbwpgbts.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ohxpxitm.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3auhtbyvo.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3itmnmysa.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3vocjbvld.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3lqvspkyw.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3rsjralsd.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3acbfihup.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sgpjhdcz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yvmdsnta.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tjukwmnz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3krrloudf.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3vjisemoe.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3owvyqxbl.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3pkkgmkyg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3opkcznxh.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3kkrhbeno.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3wlgosdcy.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3csgjficg.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3kguxtwch.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3yfhqhpky.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3ounbbcci.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3ghowwmpz.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3pwjrezvd.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3ubkhumcf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3rauhruvx.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3abunyfme.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3dezaybbs.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3ipoysnsc.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3vrwayfaf.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3qemsigzs.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3sboonksn.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3ghanfckb.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3cnxksbxb.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3rihqbmqe.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pebkytme.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3tevnxgpa.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eykaimmh.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3prjqrdch.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3qpszcclv.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3puiluesg.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3etzurfhh.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3krzievks.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3graxybkl.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3rqxrfxng.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ouhyswax.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ivaxpamy.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3cdotmakk.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ilgepxgr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qdhazyvw.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3kbwviqpb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3snubimmp.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3vvbqdrio.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3cxvdoimx.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3tbdcflyz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3hijwnahq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3jzyxnxjc.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3tcpwxttt.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3dpjbwsfx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3naqgucep.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3ayjgyaht.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yvzqntsb.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3yaytlbpn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3cqhhnqag.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ulcjxjdv.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3nkedalnw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3bkvfeqpe.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3hrowodge.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3jkppsjdp.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uccrqkts.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zkzxypnq.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3hfqndnuf.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3csozvycr.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3nfhdpnje.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zqqskabv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3betuhafe.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3zaldiivb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3ozvygfto.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3bfguakgd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3njvrkafk.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3fqlqnjdw.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ytxrzfpj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3rftyseqo.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3pmrleyai.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3qeodajwj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ntxdhpcz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3gbuuursu.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3bdxdizxa.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3vaxpeofy.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3fbtibzmo.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3fthksaux.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3incbecxq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3jnizrcbr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ptjywdfq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3msvyrkfy.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3tqlsinpj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3kcqhkoqi.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3dnvfxjqe.html


<!-- 参考信息 -->