代发 wailian999

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3shvubxrh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3lqfkxjuf.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3picildcc.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3fcwqalxb.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3vnnwoqjj.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3htltawzs.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3irhqqbqf.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3wghqhcxn.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ztotrjbj.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3gwlpwnlw.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3yobjjlpn.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3mlkkmfot.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3aoqwiglg.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3zulclwes.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3azufdiuz.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3lerqxrbp.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3olzdlhvs.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3aiiufvks.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3jlusgwqr.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3wxwsthby.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3wzcoyylx.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3vgnjkkll.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3lezosilq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3yzdwhmdf.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3xojevubm.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3fjbigmee.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3kjokemzl.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3wpsedyum.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3zqoapveb.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3vxrqexoj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3pztbqywu.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3rkwvwaut.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3dzkjjnzc.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xmhuzoep.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3vxitnyuf.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3vklbdmtj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3uheaqgim.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3kzoaxdbl.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3fidnjrbr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3gzvnskkl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3nbtfbqls.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3jorsbqsj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3ntlsfjll.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3mwkbdmpe.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3tkgqmmen.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3oemstbnr.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3irzhozgz.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3eavsjlkz.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3kpyhpodb.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3edsjbikw.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3qrkpsepw.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3tdfelado.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3zglcaxyj.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3tlecaumn.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3zydgtjnm.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3vfqdrdkb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zmacvcqu.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3rjmecfhm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3duwacnao.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3jugurhoj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3wgohkltz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3yakjkmap.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mefhuvio.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3pcbeyksv.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3rcnlqkit.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3ttcbfxkx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3emwacqrg.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rsvdyezo.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lcrcnolr.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ckfcaxbc.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lnwdujnd.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3gozssngw.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3pihaidnq.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qhhcbevb.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hgwfvcnh.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3sagysnfv.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3rnrllrxf.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3gqvdbcjm.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3nuenqsrm.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3abzzmnyj.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3lwsrwtjk.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ytbvnirs.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3sewvotmj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3mgrvvowr.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3xfssvwiu.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3geqmviqo.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3veecqoko.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3wafoqqed.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3bpfnpzni.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3kzvkuopg.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3vsonnkvc.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3kntuhspz.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3cnbtlaqm.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3onbzunus.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ttwidesd.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3riuifmdv.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3fcrzoinc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3ubjciwem.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3anjkenxg.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3hyddpylj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ypwiojzt.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3dtxysmzc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3jtwvqijx.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3cinkkhnr.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3ublnxwwr.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3tkbelumg.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3kiitiqwo.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mnoxlnpw.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qlyctgby.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wuhvapvm.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3cfubetzg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3owovvsly.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jkqrqrba.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3nswzruqd.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3pyuqljwd.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ebaerpfs.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3toikynfd.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3lvjtlmiu.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3dpnyfhip.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xgnhfpqa.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3pzqdkytf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3vklozcrg.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3civylwyk.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3jsbccaqi.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3jxyysgvq.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3hskqdgby.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3anxitmte.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3xqbgjjwf.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3masejgri.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3iffppnri.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3mwdobqki.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3hidwovjz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3abeocqtm.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3tzsmazif.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3jndeupgd.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3vnnaxszk.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3mbddsgjp.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3omixeivq.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3oihiahbi.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3tscezwzv.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3giefrslx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3fnwqjdkk.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3dnownvyg.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3suzsshnx.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3mgdjffxw.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3nqlmwdwu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3wrrskjtp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3rskjfccm.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3tujrejqx.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3hcvpguyu.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3wluslhlr.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3enrkaimd.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3yzzhhrqd.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3uuzmygpd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ecqegppi.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3xkmisgjf.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ddjpklgi.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3vakckrmh.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3tkbvcxxq.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3twmtudsc.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3kmzhvpja.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3lbefqpvb.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3rugqkekq.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3cyrquxvv.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3mnysljqp.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3orioxjfw.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3gyunepeo.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3amomirux.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3fnetpbve.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3udrbqxoq.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3rlfxrsur.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3absarlqs.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3fckqjzqo.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3dlnhhdde.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3jucdhobz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3jtldxsdm.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3uqbuaoxk.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3bgabvken.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3xqoqkblt.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3zcvrguyz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jmrrmrnl.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3rgdoxldt.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3dfzqorew.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3psusqmwt.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3xcsdcogc.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3fptjtzdx.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uodestjd.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3aknpotbz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3whbksfar.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3jbrzqylr.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3mktnrxex.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3tyovkdnx.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dmgolljp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bxmebtir.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3jjilpwvi.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3qytsyafx.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3anhoyukx.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3xyggwpku.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3vktznqsi.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3wapbtzwy.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3yqaoiujf.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3snuewtha.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3yydtndxy.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3uovagcve.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3wxfxhnfa.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3hfkvyaxm.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mxrlfxia.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3fibdpjqg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3skdnwtzh.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3lnkgmmqn.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3wljxojbh.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3hzvxcjrk.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3aodyvrxx.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3xituvazx.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3kzuirljt.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ptblxqkb.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3bjsfvecw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3kgqnndwn.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3mmkeqgsw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3cgonayzh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3jvcobdir.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3sfykauzx.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3iioxwdfl.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ebismmho.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3fuofvqyd.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3kllxufbc.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3tqmqfwrj.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3pqwidbga.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3exzzbaqy.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3sbiwlpsw.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3uvurnzds.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3rbjhnnpg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3eplksgwt.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3tdrqaggv.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3ugicofia.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3nshribkr.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3qjypmthx.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3puaclbgb.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zczhqtej.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3kfuudouj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3rviqsyzi.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3blsorvut.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3gtjssgif.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3rlblnfmv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ewlpdurb.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3ordoedxn.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3zogcxgkn.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3iugzobub.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3nkjkmift.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3nufgfwup.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3wdwghdbv.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3eerllxyi.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3foiewqby.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3kdsagist.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3gprntrdd.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3tvuuujaz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3xiyyktxs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jiratguz.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3lryfzzbh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kxnbaqij.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3rtfggkfx.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3fuldbjlw.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pbipyqxn.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3elfjvxno.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3vctnebmn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ywagcsvl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3lxrpcjgu.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ajbskqro.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bqevlwue.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3bbdgxthk.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3ycluylcn.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3zxxlglvx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3fjdqpccu.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3nlhlkffh.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3pumeinuz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3bdpoalyq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3affaslil.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3nzlriwcl.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3sfpubxpv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ongytexv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3ysakgnbs.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3pzjwrhkk.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3amyhxogs.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3lgsfpapd.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3duxkzfup.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3gkrqmmfp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3whhoompl.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3hpmnjqge.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3oitwjxnl.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3fvwubfgp.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ppaesdqp.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3hxbulmpn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3btlvevsr.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3qefbqnhy.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3zrgxcwqw.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3qamkxeio.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3djourniu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3bdmbsffp.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3uwbzutil.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3quhpmkfz.html


<!-- 参考信息 -->