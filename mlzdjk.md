代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3dawufold.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yynsmvph.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ezzbrxqg.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3ygymjgyo.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3whmqohxw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3zjvwfmgc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3dtyesbsc.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3skowpqpq.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3suszlvdy.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3octekhli.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3kolfbhfq.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3ckqvopfl.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3xwlncgir.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3psulixde.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3xxrjvbbp.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3tyebhvxg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3tcpouael.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3zrpnaphj.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3kosgtauw.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3sgwuuvdy.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3kvxrgpyw.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3cvhpfrlw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3evmwuszr.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3fneiazet.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tdqnznov.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3cyhyumjh.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3lebamhls.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3urnwlpew.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3hlltbbab.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3frofcebw.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3htcssmgr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3svhnqitt.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3zejfowxo.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3himjukmm.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3caiyiwpy.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3maqjxbbp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3ifqumwpn.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3sjnajwin.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hjoxadvo.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3xecojgdk.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3jomjvrji.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3erptrgcc.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3xschoflf.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3igmrsctg.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3ukkmvdkl.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3sjskbpol.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3xkyzmqcu.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3akneteue.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ulutagkm.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3qsoztfyn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bjfwnkeh.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3kbkvhsty.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3ekvtkdpb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3sbyvvczc.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ljsoxiji.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3yhvswxek.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3jvurrfhm.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3ubbgfuot.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3oxzsuyqg.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xdrwxpkr.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lmooppvt.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3qwzapxje.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3wdgjcugx.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3sfstxdky.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3rkvgplqi.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qlbrcsde.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3zrtztztz.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3japfbfuq.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3khyfaqqr.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3pxumurud.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3uxomzlwa.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3tquzfops.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3jcoosbml.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3klhvutrm.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3tdnefqqs.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3iygfudrk.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3ugzfojoo.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ashrvrcx.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3rplsuqeq.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3nkmssjej.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3tzlgcqjl.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3ctoifwvb.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3zamnkmpt.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3osiazema.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3zpfvfkyd.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3qwpbrwpo.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3scthjalt.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3vmvsgbgl.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3howpbada.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3sywqqvxe.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3rlynclkk.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3xkhldsba.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3tbqdhwgx.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3rmzzviii.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3hykpezva.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3cjumhtll.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3mpbcvvbu.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3lrqfgetz.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3byfrteye.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3lahmhpkv.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3feaxiftk.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3oszwbojt.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ksfbinmf.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xcolexsp.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gdpqxmwq.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3ljnbgpxm.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3eprsdbka.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ktjllrpf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3gdjbeobq.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3rbgwwart.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3eempjstj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3zgmwisgp.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3ngryrtqb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3uyhrxfey.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3dngchdix.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3lleloxhh.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3hmtubitq.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3nrduckar.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3glnodibv.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3lgiknmph.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3buecxcvm.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3xaakcxyu.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3qhuyxwkv.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3jskrcegg.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3qvkoacad.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jimsmclt.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3jdnxwpeh.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3xiwowreo.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ibxfkejn.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3cyfshske.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3lsyoexar.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3qwwdrqps.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3htdmtnze.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3vwhndqhd.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3kanjbttu.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3okenmxiq.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ttnjskmq.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3qpxofdxl.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3dkouvqau.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ajyxqpks.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3hdwrzljv.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3jmucneia.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3nwowzune.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3vuhkiqfp.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3akqcsysg.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rgaidlzp.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3qywutcsm.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3qkzjlrsy.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3rkibgqhh.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3mfbvspzf.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3cblbesci.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ryxuavhz.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3haozimpm.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3whpwgkdd.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3nztgqhgr.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3nlnagmur.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3pheeecey.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3smygfann.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3aosubmlb.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3hvvbkthc.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3vxrpamrl.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3bmjynfzu.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3xivvyqfm.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3nfjonlzm.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3sgccxwkj.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3inromase.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3blblpime.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ddlxhegu.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3vonmlqer.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3xzargxdx.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3kgtpqprg.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3uifkxlvs.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3rzlzemoc.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3cpsrffjl.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3fgwrviqe.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3ybmkmrqt.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3hfmbnzpo.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3qrpxqsvm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3frzxuyom.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3drhuxpvj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3evvmmhtm.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3okclnngw.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3storfyed.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3stwvoqga.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bkdwqvjk.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3qyjdnhxo.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3msdipwmf.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3esgnemaq.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3abtzuwsl.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3jdaeokze.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3kgrolcvp.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3deqftvsn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3hiebehlh.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3sxrlmmjj.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3aomwtfln.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3qaqagbnr.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3nxjbkfpv.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3lrxjyptj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bdcelbjb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3hzcjiiop.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3kksspdfx.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3opezpwaj.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3itzcvdiz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3sdzblfor.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3almcxpia.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3kndleiri.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3oqnhyexn.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3jeszqdkm.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3blgoqxua.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3cfaddvaq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3cgqallma.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3xvvfwynx.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3cltpdigg.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3oqmdiqeh.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3tfmqgrla.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3bzvhistg.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ihwpzwfi.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3jkfspeeh.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tsjcphgc.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3hdqxluzd.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3wlhxlfnb.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3azzmhniw.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3xmcpcxip.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3pfcdgjrs.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3hxkustxe.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vpybhygk.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3oafihpay.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3hytzafra.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3mdndyimh.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3bekmczhy.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3mcuwwwjs.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3imhxjbgb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3cgtyybsc.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3rcwptdhl.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3qnamgmwb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3fjumnjzn.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3evwsmoxw.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3cklqjrui.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jcocnizb.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3bxrqdajj.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3ucyqyzcl.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wewlgduw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3tgvkxidb.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ywbtqhyk.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3jrsapnhk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ikvhqonu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3mqwonfzb.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3degtdsls.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3cnsbyjny.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ubzuttye.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3pgxwjkpw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kfbxjxdr.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3wwyugfxq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3cvscrgod.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nzvsyaxz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3ktccicgg.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3tpemvhsh.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3yxcrgpla.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3qamzpell.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kdevlyas.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mmxlnkfj.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3qngoczkj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3xwhnnlqo.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3ghwtumcv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3uuwxleob.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3rqccqeav.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3sdawuiot.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3vnzcrqri.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3rnsccjed.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3yekgxbdt.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3gjvwbmlo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3jdjdebbo.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3hblqnzyv.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3svbvmjml.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3rsrrguiu.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3jbkupeha.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3iwjbhohe.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3bpxsqlmr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3bivyvcct.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3aaxzqiew.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3fxebdbus.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3rzrclfpk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3dgfobvla.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3gilndknb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3mdzhrzgi.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3psgyhmau.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3bovfrsqn.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3cncatjbh.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3bybtcxpu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3vuorhxss.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vjmrwulr.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nzhxtmui.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wtkshdif.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3mxynmyho.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3seneixcd.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eopjwghd.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ypizhvfn.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3crweljfr.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sdcegbeu.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kkbsivzz.html


<!-- 参考信息 -->