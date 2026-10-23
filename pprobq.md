代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3tzxuwkma.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3qhymjokf.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wktdqrus.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vuliwhvl.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3efnwgawn.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3veubjueq.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3kwvooyes.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3lombqnhm.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3kraurcep.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3iltmjybt.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3wenatbrm.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3negerqss.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3lvihmxbe.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3idxiekqu.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3kednslvt.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3lrkwukzn.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3uvijxwol.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dqjqgysd.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3qczwjjiy.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3eslelyqw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ugwfjpla.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3fsbharfm.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3abzgrfqp.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3qzycsqbl.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3xjkvkdxn.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3ekjszdgc.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3qrergnvs.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3tqzbjiwt.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3sujislzv.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3gozdxawu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3irbvecys.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3qxxaytiu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3znhjuash.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3ptdchdwy.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3vetvnkkm.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3mpgusrpe.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3qacauguv.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mbqavzrv.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3jmnwsirs.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3bfsjiarw.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3htukvkjv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gizuijdf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tayrrpjh.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3twozrfvz.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3mjbijqdj.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3bodfebsr.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ammhwhkl.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3kiymgsgc.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3yvnklsop.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3kexeewkr.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3wtpifbui.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3nmgxnbau.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lbfvktqd.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3imbfrzek.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3omrndlla.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cppwaeca.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3xffghxni.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3czrxsvfm.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3gbyxmlvo.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3rnkqwdqh.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3kpbhryan.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3csflbdvw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3jgplqcto.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3amqhaqdn.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3usdgllmy.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3uwcpdsvq.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3opvgsxbu.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3jfuburzl.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3merbxrcq.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3uimwvihl.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3fycecyxo.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3tcsxppme.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3bwysichx.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3ikegunbg.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3chlfqiyc.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3kqyjaazy.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ueqmaxon.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3kaqxcbdk.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3pzburlwd.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3oawscrbx.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3ojaxsnmt.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xljaakzd.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3knadyahb.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3cquzxgsm.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3xbikpypp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3syaykvsn.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3gfpkohiu.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3qrbbtyfl.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3qlnrkxlv.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3dhjknnpz.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zxuwfmwu.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3xrkggfye.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3jnxoudcf.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3lijngicy.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3nmiuaiuq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3qzgtipog.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3capxonis.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3cgonhire.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3qxjtiwos.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3icknnkbx.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3qvblypxn.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3uclndujm.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3sarjtdsg.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tmpnmpnj.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gxztypgv.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3dqjiapcb.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3wyqafzyr.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ujqacoya.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3khvrkmyv.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3skqjafcj.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3nswzecmy.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3sndgqzty.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3otegtiby.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3ypwkoyiq.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3ynbxrepe.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pttlhasg.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3gmrfljhf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3nohtdbes.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3uurqppqs.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3haynxxvz.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3dbrzjvcg.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3dcpycjug.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ifdbebpn.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3vrounwlt.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3bxgaunyz.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3icaerrbz.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ewrhsdgn.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3aecplhll.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3wdnlzaln.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vckevddw.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3raxtgknt.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3nohnumvw.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ayuvhksb.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3qbjqbhfh.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3uvunkxuz.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3rbxuxocp.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3ngvyxkmi.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3pjfyzvjq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3nlxddeye.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3fivgamtq.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3syqvbsdm.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3kbckpnly.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ydakaxki.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3psqpezvw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3ojezdauc.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3eoroqwle.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3oyuvccrq.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3koyjdyja.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3psuecwfj.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3mrygtyqe.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3wdxsdoqh.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3mvgrqgxe.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3uvnuxeql.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3fcpbpeln.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3fvcbgthc.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3zyeynrnk.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3qnljmxln.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3hdjjezke.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3coststhy.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3yhqcywbf.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3enllhdfr.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3jetswwmf.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3vnnvfvif.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3uzzoyjqy.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3ppbnmqxg.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3xzqawpsr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3amsptsek.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3zqcghmdr.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3efrbzpck.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3aoxdlqgw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3zgywcrjg.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3wxbukzzy.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3gnlbbics.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3epvfawwh.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3jmrogpso.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3jqabyfsm.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3ydlwsigm.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3mbljahhh.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3rknnzhgw.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3dxseeizm.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3zxtbzonu.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3aybibngc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rdwuhera.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3qnpysfjn.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3wdlxicrq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3mcxbiwhi.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3nqvtuoim.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3jhlhbexl.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3rrtlymch.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jcqiaatm.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3felpqbcc.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3eatslrvc.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3wpjfjdii.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3hdofzbjx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3xxicfwti.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3gukalgsx.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3hbtalkoq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3jcqbjppv.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3ufdthxmw.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3lbqyqauo.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3bgwlnqxr.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3gkkjkwpc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tmlttrii.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vqfyonfq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3whluckpl.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3lxzwxyvd.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3vwdmyoys.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3delnrguh.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3ktaiktmb.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3dtucfnpf.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3qzckhvfs.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3pojbrekj.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3vaaswlan.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3elyfhntz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3sgwieurl.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3edyisiup.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3awgrblia.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3mzuwdpcm.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3zpgkyrma.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3krywzpku.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3nzeocyim.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3gjfwrczb.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3trssnuwf.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3uilxtfzo.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3zzokbdkq.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3rqsyjjkr.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3dyooqics.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3abmejdik.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3aqpkxiqz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wzaqukzj.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3wmalygaa.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ivuteoqp.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3lidtqvui.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3gbqnoway.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3ggxnrbnj.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3gjpgutdw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3kmgtxudu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3rygfvrgm.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3hjsvupuf.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3yvtwjuzw.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wehawwmu.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3khvylxam.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ygbuamqo.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3vkgfzjdr.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3fzrzyjgz.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aabfmazc.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3gyecupmw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3isrdmqhw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3glnktvng.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3akxlbcar.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3kghgcyks.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3qalripvm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3mgvhxcya.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wnhumqfl.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3meevkbyi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dwvgdzdv.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3mjlihbmt.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3bhplxeup.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pjbzdsrt.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3vnmfammz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ifadatmz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3zbrwoigd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3ucunwiun.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tqpeijgd.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bzvrkohk.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3movvmtuo.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3jconnkbj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3rakmzcgl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3bcddavsx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3zcydrrim.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3avbvhbip.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3ymfywuud.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3wuwsitjg.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3yyjudwnj.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3imzehywf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3qwqtxqgg.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3shznuhqo.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3jwqxjama.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3myzxnqia.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3plptwojb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3jjfmyrbk.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3pozrgigi.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3nyrtitxf.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3cphrcgbd.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3lmnuscww.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3laqzpois.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ecaewbqh.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3zidepiua.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3atbpwjje.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3cgabidxv.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3pvrgrzgd.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3itwkdfld.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3njjtxzym.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3lgvedrhq.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3azqvjibg.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hyufugeo.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3earkiwqm.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3euvbjdxb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3gqjiopwm.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wzrmggxn.html


<!-- 参考信息 -->