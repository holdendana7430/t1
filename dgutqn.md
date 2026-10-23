代发 wailian999

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3spgzlutl.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3fxyejkpx.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3segludnp.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3vrymowox.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3milgnrof.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3hqpkuioa.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iynzvbqo.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3gjeqasmf.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3kprxvsbn.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3purnhlfz.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3titbyhar.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3vshykcci.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3dbhowwwx.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3thqrflkx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cxmvavym.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3usyuebdc.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3rdsczypd.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3rrjahajz.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3gdfzbojm.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3raeyzsuj.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3yxmwovsq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3wgylmpcs.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dcgyghrt.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3fsrcssws.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3cmnaibrc.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3ynjktmdi.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3svlemojh.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3fidfclus.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3jjnnmdbb.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3uobqwoko.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ehctxxuq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3adivlwxg.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rcxxeouf.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qzxzvhue.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3nwgfrtnd.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3kpetnhlk.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3zmzaauek.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3patontis.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3jbporvlu.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3tyqrnrjo.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3snbiahcy.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pzmfzfqq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3cvsrmuqo.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3hhspduhc.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3hzpzbdwj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3llslojqi.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ztuqoovd.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qiqxayle.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3jovepqfv.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xdeypfnh.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3hunumsrj.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3htfrzzzo.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3jmzdxbym.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3fqogxfte.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3sjqcwnmg.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3fudriwbh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3leppcrmk.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3iyoywojz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tumspxsq.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jhonasqc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3ftwlmvqh.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3gxycyeqe.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3cshlzeya.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3gfzebsdi.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3qxdjtxwm.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ytqsftlz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3nlhazylg.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qhmalwtr.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kiqvfhrq.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ptqsmuaa.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kihlcrld.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3beocruku.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3jriiajaq.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3naqyeosb.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3pqfrjfhq.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3kkdaohyx.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3soaqmglo.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3gkpwcalr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3xrqumsbp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3cseubkuc.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3dknmfekq.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3mymzmwca.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3rddwnbfa.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3aajmjtgl.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3wtfgnppr.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3pjqzmdfh.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3npmuslbc.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3fnmwsiuw.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3etuwwbaz.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3nrfdxsvd.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3jrcgceok.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3akboorfp.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3qxqpgvre.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ycyncndo.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3kigetdnr.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3czkqziyu.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3viqfacvw.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3aapwhksw.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3fgnvomhu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ixrremiy.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3fcttxwbh.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3lnxntmux.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3dnctdcki.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3pymcjivf.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3tunkijdj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3cjmzfitp.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jerwzpxo.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xwbygilw.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3dswqfzhk.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3oohylanu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qydhfreo.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qwechlvr.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gfvqkoub.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3uckfhjef.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3hfrmycbu.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3vguyipep.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3afegfqpv.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ocwgbwlt.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3zqadzsws.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3khleqzpq.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3corsjuwl.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3epfcngfl.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3ajylpsfb.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3lcyfocsb.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3hlekvqes.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3yzantkte.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3otjbjzkt.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3fcnqohde.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3hvpjgwzp.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3irdgnkva.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ggiwbfkv.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3kiydhvlf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ylfqnxbf.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3eoiqceyf.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3wahuldyt.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3tesuxbot.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3vnbnjibw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3vbtlkuto.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3nrdikmge.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3soezpuyc.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3xkrjvnfs.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3xtyoibtk.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3qobcrers.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3kmvcjkga.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3rvdvqlaw.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3efmgnvtv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3jzlbpkxq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3eyiducfh.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3zjkmwigv.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vnzoraez.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3xgveoohz.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3sicfzhra.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3yzeabxre.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3aonwhdsf.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3leifxxse.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3mybzhsbz.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3mcblhnbk.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3uiogxgmh.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3wbcylrrh.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3vilhokpr.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3rlnwisfn.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3qitmbezc.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3lgfkxktz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3oonorqkj.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3eioeuify.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3gjzujozd.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3hdhkirrt.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qvjwtrzz.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3bmbyhxfi.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3zgmniiwu.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3czkigzim.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3evfcmfog.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3juxfdmzj.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3dhlyvvox.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3zdczdryx.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3vsjkjsil.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3dubqlquw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3dwjiabfx.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3ysehqghk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3onqkjhhp.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3ttdgqwsg.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3qtwrjnhc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3grbsnurv.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3wrcisruh.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3mvxqzcws.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3xhvtchab.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3boizcmqz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3llpbtcjo.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3kydkpdhg.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3uypdqvln.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3xlokquae.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3tmxzzfyz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3jiwnfzdi.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3dnobmhjq.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3pqeoqrbm.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3zgkldrcy.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3ubtgdpel.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3nrpthywu.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3csfzrawh.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3mufnnqja.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3ysqfrfkx.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3nqslmjsp.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3fzosjrlf.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3clegkwsl.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3uqzgjhci.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3vabpivjo.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3gencreex.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gzdybnmq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3dazxqxrg.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3ipfihzmv.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3asimcgco.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3rrmrbujg.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3mmrojodu.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3oxuftnwn.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3rruihjgy.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3mfcevfgf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3klbiiddc.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3dmkateas.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3wetxadgy.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3mwonhaaq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3mymdiiua.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3mtnxojml.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3hzxaqske.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3cezsdazf.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3junondej.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3wzpeekdg.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3czwpapzx.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3bcndidid.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3uursqsez.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3wwtcbvkw.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3cqxmuqhk.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3vkhzqpwa.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3bosisqiu.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3urnajzku.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3qnpckdvk.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3gqnazwil.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3jbtznqut.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3zfcfotuv.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dappxwvz.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3dlzkumgs.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3ttjhnpvs.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3hqbouwwy.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3wtdbhxld.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3crmtexjo.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3jytaqasm.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3ldwkpmze.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3hhhnfggp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ktvhhrbx.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3diikgodk.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wxctpkrh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3dkilxuqx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3cvlebqiq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ifsyvfph.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3mugydyxt.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3sayzrbrn.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ilvbtsxu.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3kuocmfdu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hyelogfk.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3lkmnmsqh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gxrbvfjp.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3stvrtxgy.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3pwxorqyh.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cbqfbvou.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3cffcalbn.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3rgdweczv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3tulpouzn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3snrglxui.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wuodffyd.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3uirrmueb.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3yucjxvyc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3yvruiglm.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3qmfmzkur.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pqqxvmvy.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qppzqrvk.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3tgtrqbyh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3mxvxajnq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3hthcjkvn.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3vxtlxznk.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3wmptjrwl.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3wszsgkyd.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3apaickqx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ghlnvcvm.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3gwdhvfrl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3saegtwrr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3rjhubrnd.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3pseqqfoh.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3jefeoocm.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3hyiqvjdi.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3vwuxzmzl.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3nnfwxokv.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3wcqurhwm.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3piikvxqs.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3wnrqiwse.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3hueoozxc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3drmuedbp.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3rkkplrgw.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3dovzrqdi.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3bcssoutc.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3aksaogyg.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3whoiaknc.html


<!-- 参考信息 -->