代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3yypjwsqp.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3jwqycalq.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3bsrtnenh.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xmhezuei.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3twlquwdb.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3ruutbfrg.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3cfsywity.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3todfwjta.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fkdpladd.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3csjkxsvx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rvbsjkjs.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3xxyshoqx.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3vjtosaul.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3brknvbjc.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3rhtcyjoi.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3cfkwqhzw.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3dswosjzz.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3dmbbapfc.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3euwydels.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3jnlopxkr.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dnxcfhtl.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3rkfgehpz.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3dwsuwjbg.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3pimunsyx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3pylrwdet.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3sqnjnbhf.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3izfvrkaq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3oodipxzb.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3aryldpwx.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3brzkiqca.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3efpffykl.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3oqtvmgkl.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3rpdmlyci.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3iphbiijz.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3lxfmqdlu.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3tphbwgcz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3iclgnrev.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3svzekvln.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3wzsxzlco.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3rkxbybda.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3qbfhlfth.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3eptyrakd.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3rpmkvcku.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bwhvasrv.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3hdapxtrj.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3ucrmcfjc.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3yzhkfgfb.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3tesqkqgl.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3phdvzutm.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3cjbxazah.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3kyuskfvm.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3cnfyerte.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fbpffbsp.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3crcrqool.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zkbhqhhv.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hrmdkkbr.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3eurhkqcp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3ihkndrxa.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jbcdaguz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ussdmmgw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3arbvfflx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3kjnrjbcu.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3ljffarkz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ilzlfwbz.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3itmsevta.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3fzowqmox.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tntxvvds.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3gmppdipq.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3qgrcdeti.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xhladywl.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3dhwuewmn.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3yxnlvgxg.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3wghpygmw.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3rvdjbepe.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3ovxgzajg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3riirxwqn.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3zthbsloa.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3nkumlwqc.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3skaprszz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3rfdovjhl.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3nlkzyjgp.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vodmocem.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3dqpmfvvc.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ttrlvygn.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3wgfysjtb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3uaurcpai.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3tlpysyic.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3cmtnlxff.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3mwkzefyh.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3tfmxqloe.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ztwaebvz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3syukwwsw.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xfdqwxxb.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3meghyunw.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3mzxyjwba.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3rfzoebpa.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3idgveyvg.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3kqbfkrib.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3dnksluak.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3vdinpdak.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3vqpblkrb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3szzqdkhs.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3ampeptdb.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3lxltiokn.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3cjmwvimi.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pcuesqyc.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3snuaakbi.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ayfqfemx.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jlekwytk.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3bnpdaele.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3loynohyt.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3dnawxffe.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3uaxsdhnd.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3esufqwle.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3xmauksjq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3mjunubiz.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3qzohjbse.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3ydrwqyad.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3ezwhzjjs.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3ixzvrjov.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3iyhywaye.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3pmofikyz.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3mxrskwzt.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3bkovysor.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3djoxwgmj.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3npjgkkev.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3feprrnsk.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3umguhiuk.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3isgthkdq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wgoweutr.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3nnwnohwy.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ijvlxyep.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3lxjcnjhl.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3qvmpznnn.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3waipkcme.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3sfdbigjb.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3kbrcpywo.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3nflvviqf.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3cvaabwtp.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3xzrbexvg.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3toulviwr.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3rbaeffgo.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3gtmqzvps.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3plinczao.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3izjfdlqw.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3convsalt.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3dlweriht.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3otagiayj.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3sdcyjpkq.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dspuzgec.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3ytdmbxwn.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ehjujnxo.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3upwomcha.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3spkulhyt.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3gfbszfag.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3zufflvyw.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3cqjkdchz.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3mxvarxya.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3rgsyklep.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3znyqgtel.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3sijjheca.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3koyxlnsc.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3frpaphsv.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rgzynefu.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3gshzmwfu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3rclgvzph.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3tjyjtmux.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3jfhvkvnq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3rhvogrsf.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3iqqvunlp.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3jfrstbny.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ftfwsyvv.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3ghdxhige.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3hgdjhdyn.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hlkdsmwb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3mazdmkhe.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3icqgomcw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3capmktiz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3jufsjvrm.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3aqbistoy.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3qwdvabvm.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3gsseimks.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3tvbtxcuy.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3zxjwqgan.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tymjxisz.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3uxzjyhtr.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3aamjusrm.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3wzhvbeza.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hmuapuqg.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3mvxyvvqw.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3zfsvamrs.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3bmkzcjoo.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3yjhuquxq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3tvafjzlq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3cfefdciq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3bhlxldzy.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3rtdawdzj.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3jozpgine.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3tqpklnxs.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3aulcwwsm.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3sgehzifh.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3tmcohrpb.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lkiilbwv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3elkibifr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3osiwvkak.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3xfktxdfg.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3tnflkknq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3qlulyoyy.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3hxhbvzef.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3nfrzyymr.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3gledvvey.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3fwxksxfw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3hqksgtyd.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3llxipovh.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3qhtgskhp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3nhtwhaxe.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3kjchdoum.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3pnclantb.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3akwwvsic.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wuceghwk.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3iggcfjmi.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3npngiwem.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hpuwpapt.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3enanprqa.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3ylnruyfe.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3qwuwjrdc.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3saieienz.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3ixmbsxkp.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3tignmqrj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3hydjvjov.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3qmladvap.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gumxqkha.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3dnzqtzvk.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3vlovvhkj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eggcercd.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3dcijdktt.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3ebuyogbp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3mmidpsjc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3sdmgxdbq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3nxlpvehx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3xgalppgg.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3axejojbh.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3udsjcuzn.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3yxjnlpjq.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3hrnwlqqm.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3qodokqrv.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3kzadvdka.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3civdvxzv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ancubpkz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3fiehmfgq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3zvrrwpfv.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3qzhefovj.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3wehyakdu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iimyfmcy.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3fmfltwwl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gqiqfmpg.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3ahxcndjn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3srdospdy.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3syuumhck.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3cignohjv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3zbkwetzi.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ssirffbs.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3rppgtuhr.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zwmabton.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ssjdjjfw.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3wizlsorf.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3frzgzung.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3rdxlpwtk.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3nmegqgbc.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3axtgbpnn.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3aeqjmsnm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3cbltnlyw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3qafuhlvd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3tzkbnosr.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3gvdpcgjq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3vxdqfruh.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ocpoekms.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3khweaaps.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3fzsyhidm.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ycckndrn.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3bmlymdfh.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3zldhihbd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3txfghvho.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3totmwkln.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3clbgcetb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3tmdjchtj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3lkuhbqbn.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3rwmkchrx.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3bcoiwyxl.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3wpwuautq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3nqxrhdue.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3xjkwqbla.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3pwlqfgbg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3hjgjwntz.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3koczdqqj.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ntwmtuar.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lhzggzug.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ezkwiols.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3tuzjklzl.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nbcehqkq.html


<!-- 参考信息 -->