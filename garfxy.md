代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2mocdhsjm.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2jnojfmte.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mgbmoeno.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qxzofdiy.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lyxxxwcs.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lhhraiub.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2qkjptcal.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2emjzojot.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xzvqtvax.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2xonfqmxe.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fqfnstcu.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2fimjqmye.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2zfxiowje.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2bwrebiim.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2mmvkphad.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2ttjvlsev.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2xqazzreu.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lvlzzhig.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ojokfrvu.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2cxganbcf.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qhlcgpqv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2oafavjfz.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2csxolxbz.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2goxrpkua.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2wjtdadpv.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2dduhqbxc.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2dqwmkuqn.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zjkkgcfb.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2tlcsxyds.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2wpwaxznn.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2yggbqsbp.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2jmzzdttq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2vkfkyshc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2hjlmnwop.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2mgwhgivg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2duiydykg.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2yibuxjgu.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fhixzuyx.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2ymyqkwzl.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zajrijtn.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2ohvfbuuv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2xjtxnlxv.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2hreanubk.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2unsvpohm.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2fribnxbm.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2kvwpnsgw.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2fosqrvob.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2wtnuimne.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2vdxwilmk.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2vvqtslgu.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2meggqzea.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2vgmefjyi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2njoihanx.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2qysrgsgo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ixfekmtb.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2yxrkjsgh.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2liokgejr.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xfxrttnd.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jmpygevx.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2nkusyzsg.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2zqgwshdj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2lxmelebo.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2cyjegfey.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2uotpnyff.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uhfvzzex.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2prhajowa.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jgizvkkj.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qdmgtsmv.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2odufxohc.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ciwnmopo.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2whcezhan.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2iwztlsdp.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2afiqgcoj.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2kngqxwrp.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2eqkieuqu.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2wvwwptbq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2mvnnmwvl.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2irtgnvro.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2lqurdwuz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2salfzrjs.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2bginqmkx.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2dpqrrxbn.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2wabcccjh.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2sjlvoczg.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2yfekrduf.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2golleqwj.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2cncyrqet.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2wklulpfn.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2nqhsabge.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2gxdzfhjj.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2vlsnjiil.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2phdnupfb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xcbomnyn.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2nvuqahdz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ymxoezel.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2sqjwekpm.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jrvejwjn.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2tmawstca.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2hmhrdwmq.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2txklfkfy.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2vnlmdime.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2sjjqkptv.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2tjpkxkyo.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ximoswss.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rbjfahdh.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zqfwkppg.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2ekcmbcnw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2roiokfxs.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lshpsqjg.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2cllndjfl.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2luvutcde.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2aselhjdn.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2dgmsrfqo.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2nlumlfpy.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2aglyfiai.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2vfgwkxsq.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2dipeevve.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2sdazpqfz.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2yclaalqq.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2qgqguedm.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2ivhvogin.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2unvlkapr.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2rfrirxqa.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2fbxzpfke.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2elveftef.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2vmkicxxp.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2xmudtucc.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2slkowrho.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2cimbbjmq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vmocarpe.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2xqlbvvww.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2iwfvokcb.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2njkzbocj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2wrfjplar.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2eiqpbyyq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2dexdqljs.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2uiabyqwo.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2vnryxmfd.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2aqmtlzsf.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2jrleomrd.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2wkbhebiq.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2hsakpmih.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2mfpucesj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2zcygjshz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2ivnpwmoq.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hwueirfh.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2rjfiuvow.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2fxzenehb.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dnpffsng.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2demtrhbu.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2joeemoud.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2zxdwrewc.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ftmrexud.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2sdjcnrqm.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2wtexmnez.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2uqmzepvf.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2zsrqedhf.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2syrcjncq.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2rtggyldw.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2rzdffwvb.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2mcnofwui.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2wqgnoeqn.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2fjracqqf.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tytgejze.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2qdwjlwmj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2ummcagxg.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2yabtpdwv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2mfeybeih.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ixceuaye.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ralnbmcp.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2ynolgdtw.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2wgmvktrn.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2ilddeixn.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2lstwekqe.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2prbubxbw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2aufhlfcy.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2vnlswjre.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2yxkmndkd.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2nfmskgat.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2ffjunorc.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2lckmxzfk.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2ghegllus.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2ujmvriyy.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hmyghqug.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2somksowg.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2tvgrnhpj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2hqrpwqwp.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xvmeqsom.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2mwmbkogn.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2avlubgpc.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2dmwztgqq.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2ofugehlz.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2xogxwqsj.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2znvxkkof.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2wlvaaywl.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2tzfmjmly.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2riidddnz.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2wqqgqpbd.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2wdgbjbyr.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2yjvkxttf.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2gixqfpqg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2znkpvxhn.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mgmofzoo.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dxwpspkb.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2exlprlqg.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2lprijmti.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2nehjbzsg.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2qzamrkaa.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2aapzyhan.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2abhmtzig.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2ijriwhuq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2imkjibwl.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2piqbpxwx.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2cjiaztyg.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2uyuwuurv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2bwsxjgyt.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2hrkmpzix.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2mxrkniyb.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2tdmxlbsu.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2xsnydose.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2urvzagkn.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2djwxluls.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2gqeybnpo.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hzyttqeo.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2jhgbojxl.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2jyfpwaff.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2njkfznlp.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2pzxbtyug.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2aenuegnn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2reyilgfw.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2eupkriqp.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2cstuuoza.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2ltrclzrw.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2ynsqpybu.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2ekxixmii.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2mhqmxmuj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2jvnhpzuo.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2gwchnljv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2pknsskqh.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qtjzzqwz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2tgxvuqgs.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2tfmejpku.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2djskanay.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2cxxohugc.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2oooqrkgn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rqargmpc.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2wustclut.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2xdmtrtpw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2yzrbmnwf.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2eamebppm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2kxjgtzgv.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2fmlzsgdw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2alpuuasg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dsjaicrt.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2dkbzzrcn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dntzhbnj.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2acjtpsts.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2uklqxlke.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qznquidk.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2midunhsw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2tidpitsv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ofkjlnin.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2feeftsmu.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2owkjengx.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2avqxaotr.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2lrowjxaa.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2tzkplifv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2xcdcovhg.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2mshrkuey.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2taorbsex.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2gwqxnnwt.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2wppjrxiw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2waedvove.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2zkbjxxib.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2mncbnlwi.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2pefhhkgx.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2rakadcds.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2hklozlxx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2kvcehejl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2xllsntwx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2jpfagzka.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2bwqingeg.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2sykfhugv.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2ijoyzqdj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2alxqxhnn.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2riuyqduz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2dwpcdjae.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rqtqllqh.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2wkdjykiq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2osfaxrkz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2mbydfldu.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2mdpdaxrq.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2bedotzhh.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2psvrsryo.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vgdwqsnb.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wzakhrgx.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dhleutiw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2fcfkzsst.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2rexqljdf.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aucmtdsv.html


<!-- 参考信息 -->