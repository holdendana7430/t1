代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gqszilzfx.sHtML

Ruby: arr.include?(x)
来源：http://read.share.hesvh.cn/Article/details/gkxyiohag.sHtML

C#:   list.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/geqoazygl.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.fehbvm.com/Article/details/giuscsqnw.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.zdbjq.cn/Article/details/gachutuki.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.fehbvm.com/Article/details/ggvhzzzye.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.zdbjq.cn/Article/details/gglrypxuz.sHtML

TS:   [...arr];
来源：http://3g.hesvh.cn/Article/details/gjanahgzo.sHtML

Java: new ArrayList<>(list);
来源：http://baike.hesvh.cn/Article/details/guvvfewmh.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.hesvh.cn/Article/details/gdximwbve.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.zdbjq.cn/Article/details/gbqovjsfv.sHtML

C#:   new List<int>(list);
来源：http://blog.zdbjq.cn/Article/details/gxmzinqbf.sHtML

[D23] reduce 累积计算
来源：http://mobile.zdbjq.cn/Article/details/gxfkvtkxe.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.fehbvm.com/Article/details/gtxjdbpem.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.zdbjq.cn/Article/details/gyqxdiwtz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gjxywzdfj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gkrjqckmt.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.zdbjq.cn/Article/details/gyasfjivn.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/gmvzcgokm.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.hesvh.cn/Article/details/gimbucuey.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.hesvh.cn/Article/details/gclxicqql.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.zdbjq.cn/Article/details/gbrcstzpt.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.hesvh.cn/Article/details/gvdnqhuvt.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.fehbvm.com/Article/details/grsfdtymx.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.zdbjq.cn/Article/details/ghhfoaohw.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gyutijxsq.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.zdbjq.cn/Article/details/gszsvfuew.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.hesvh.cn/Article/details/giruxshwe.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.hesvh.cn/Article/details/gjcabntoj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.fehbvm.com/Article/details/gbshllpjy.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.fehbvm.com/Article/details/gvokmdlpw.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.hesvh.cn/Article/details/gdgxbihvy.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.zdbjq.cn/Article/details/gzfholmys.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.fehbvm.com/Article/details/glqhzdnmf.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.fehbvm.com/Article/details/gqdfqrvjw.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gheuomeus.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.zdbjq.cn/Article/details/gokanessm.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.fehbvm.com/Article/details/gegpxjrfz.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.zdbjq.cn/Article/details/gzibdjhhr.sHtML

[D26] 数组转字符串
来源：http://www.share.hesvh.cn/Article/details/grrgibxbg.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.hesvh.cn/Article/details/gbpryqgqw.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.fehbvm.com/Article/details/gelmmsnbc.sHtML

JS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gmtwastyb.sHtML

TS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gtutsgnsb.sHtML

Java: String.join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gufywjktw.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.hesvh.cn/Article/details/gclroybnu.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/geubpnjme.sHtML

C#:   string.Join(", ", list)
来源：http://3g.hesvh.cn/Article/details/ggviouxsa.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gtcnhfdrh.sHtML

E. 字符串处理
来源：http://m.share.zdbjq.cn/Article/details/gdfqptyxp.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gpygsbley.sHtML

[E01] 拼接字符串
来源：http://3g.hesvh.cn/Article/details/gtodfasee.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.zdbjq.cn/Article/details/gxjyqxvhp.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.hesvh.cn/Article/details/ghnoxjswk.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/glqtaoacm.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/gbcnoqhyd.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.zdbjq.cn/Article/details/giawoujad.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.hesvh.cn/Article/details/giwmxvmky.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.hesvh.cn/Article/details/grvcasibq.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gdnlqjtvm.sHtML

[E02] 重复字符串
来源：http://www.blog.zdbjq.cn/Article/details/gtyazswwb.sHtML

Py:   "ab" * 3
来源：http://www.m.share.zdbjq.cn/Article/details/gitvvokrx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.zdbjq.cn/Article/details/glpqvdkch.sHtML

JS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gnjsvnrpd.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gxglwfnfv.sHtML

Java: "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/ghqsmiuny.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.fehbvm.com/Article/details/gbcwzcjzz.sHtML

Ruby: "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/gxifyzvbr.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.fehbvm.com/Article/details/gjhtjzxwe.sHtML

[E03] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gqyouuxir.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.zdbjq.cn/Article/details/gvttlckyn.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gzvwzzxqz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/glouoyjqx.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gjumwmrsz.sHtML

Java: s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/ggpewbqtf.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/gbtslwxkl.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.hesvh.cn/Article/details/gydapedqm.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.fehbvm.com/Article/details/gaazlihqk.sHtML

[E04] 查找子串位置
来源：http://www.m.share.zdbjq.cn/Article/details/gwxxlazhj.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.hesvh.cn/Article/details/gocphuvht.sHtML

PHP:  strpos($s, "x");
来源：http://3g.hesvh.cn/Article/details/gkgpwuwpu.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.fehbvm.com/Article/details/gsfxnifio.sHtML

TS:   s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/ggzsrmuss.sHtML

Java: s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gzvlnjrlr.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.hesvh.cn/Article/details/gfuvlnuhv.sHtML

Ruby: s.index("x")
来源：http://blog.fehbvm.com/Article/details/gnmecpngd.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gupxmoqry.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.zdbjq.cn/Article/details/gnlpuebrr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.hesvh.cn/Article/details/gxpajsehx.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.fehbvm.com/Article/details/gsfnoassp.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gbspelylq.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.hesvh.cn/Article/details/guldxqwog.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/guzdpzkxs.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.zdbjq.cn/Article/details/gmzxodhyw.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.zdbjq.cn/Article/details/gflnqxcsv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.hesvh.cn/Article/details/gwbhjtuxo.sHtML

[E06] 替换子串
来源：http://wap.fehbvm.com/Article/details/gyjssffcl.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/gzkabgcbq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.fehbvm.com/Article/details/gwmqdilof.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/geargbpeo.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gsyxirlre.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gzdcjyzeu.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/ghoyucquc.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gualeczjp.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gvzcbaokc.sHtML

[E07] 按分隔符拆分
来源：http://mobile.zdbjq.cn/Article/details/goszcnnwv.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.fehbvm.com/Article/details/ggurqfycs.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.fehbvm.com/Article/details/gqltsfdky.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.zdbjq.cn/Article/details/ghrrnwuqz.sHtML

TS:   s.split(",")
来源：http://blog.zdbjq.cn/Article/details/grhgvtdol.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.zdbjq.cn/Article/details/gfzlfvskf.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.hesvh.cn/Article/details/gfanqncfe.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.zdbjq.cn/Article/details/gmeubzsrs.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.zdbjq.cn/Article/details/gutxemvvw.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.fehbvm.com/Article/details/gpqqhxdek.sHtML

Py:   ",".join(items)
来源：http://3g.hesvh.cn/Article/details/gaamwtkhr.sHtML

PHP:  implode(",", $items);
来源：http://baike.hesvh.cn/Article/details/gvpnzfzie.sHtML

JS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gogpsxqqu.sHtML

TS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/gmyngkkew.sHtML

Java: String.join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gcmhialxj.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.hesvh.cn/Article/details/glhzikiar.sHtML

Ruby: items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gnlxplvti.sHtML

C#:   string.Join(",", items)
来源：http://wap.zdbjq.cn/Article/details/gttrckqvb.sHtML

[E09] 去除所有空白字符
来源：http://wap.hesvh.cn/Article/details/gtiulclaj.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.hesvh.cn/Article/details/gmptvqzac.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gkjpwwfwk.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/gtvjncxdk.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/goeppngwk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.fehbvm.com/Article/details/gmczdbvta.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.fehbvm.com/Article/details/granovdbg.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.fehbvm.com/Article/details/gdiexnfmc.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.fehbvm.com/Article/details/gxqluiooz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.hesvh.cn/Article/details/gdvdxipfd.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gnqmkqaag.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.zdbjq.cn/Article/details/gznnuauqd.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/ghxqrwvdd.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gxsmuouaf.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gbqgaaabf.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/giimkoghk.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gcttgothi.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.fehbvm.com/Article/details/gbupytovl.sHtML

[E11] 反转字符串
来源：http://www.blog.fehbvm.com/Article/details/gbcesqfbv.sHtML

Py:   s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/gvoblhpvn.sHtML

PHP:  strrev($s);
来源：http://wap.hesvh.cn/Article/details/geeeacpyx.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gsuqeubwm.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gyhxanetp.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.fehbvm.com/Article/details/geyirzmvm.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.hesvh.cn/Article/details/gxylswwjm.sHtML

Ruby: s.reverse
来源：http://wap.zdbjq.cn/Article/details/ggmycgkxl.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gigvkzmuh.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.zdbjq.cn/Article/details/gkqyperlj.sHtML

Py:   s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gjnbqyjeu.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.hesvh.cn/Article/details/gbsbofmqi.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/geuabyvwk.sHtML

TS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/glxkxkcwm.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.fehbvm.com/Article/details/gtwfjegbb.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.fehbvm.com/Article/details/gkajcrzwx.sHtML

Ruby: s.count("a")
来源：http://mobile.hesvh.cn/Article/details/gnojckpwg.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.zdbjq.cn/Article/details/graxmoqit.sHtML

[E13] 逐字符遍历
来源：http://read.share.fehbvm.com/Article/details/gzttndsux.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.fehbvm.com/Article/details/gnwbkjgbq.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.zdbjq.cn/Article/details/gqlhwhrjy.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gfibkslnc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gfdydxdor.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.fehbvm.com/Article/details/gnixaakoc.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.hesvh.cn/Article/details/gsrxpvzly.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.fehbvm.com/Article/details/ghptpdeem.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.zdbjq.cn/Article/details/gzlienfgq.sHtML

[E14] URL 编码与 Base64
来源：http://wap.fehbvm.com/Article/details/gqffzyykh.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.hesvh.cn/Article/details/gysynzsws.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.zdbjq.cn/Article/details/gfzmvrxuv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fehbvm.com/Article/details/gcojvvxhu.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.hesvh.cn/Article/details/gzislruwk.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.fehbvm.com/Article/details/ghgdlxtmg.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.fehbvm.com/Article/details/gtdezvirt.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.fehbvm.com/Article/details/gjsitqzlk.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.hesvh.cn/Article/details/gotbhwcsz.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.zdbjq.cn/Article/details/ghknzsfqo.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.zdbjq.cn/Article/details/gpcftiscl.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.fehbvm.com/Article/details/glmzipead.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.hesvh.cn/Article/details/gqzpzfzrn.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.fehbvm.com/Article/details/gjfrszefd.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.hesvh.cn/Article/details/gshxnbtmg.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.fehbvm.com/Article/details/gibgcrjef.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.zdbjq.cn/Article/details/gkjanovmo.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.zdbjq.cn/Article/details/gkpobuskx.sHtML

[E16] 数字千分位
来源：http://mobile.zdbjq.cn/Article/details/gwqapgitw.sHtML

Py:   f"{1234567:,}"
来源：http://3g.zdbjq.cn/Article/details/gevttpwvx.sHtML

PHP:  number_format(1234567);
来源：http://wap.zdbjq.cn/Article/details/geyeggkvz.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gafhdydnr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/ghbrsuosq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/gbfsxgfyu.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.zdbjq.cn/Article/details/gpgqqiydo.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.fehbvm.com/Article/details/gbdrgxpju.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.fehbvm.com/Article/details/gyfyhcmmd.sHtML

[E17] 首字母大写
来源：http://3g.fehbvm.com/Article/details/gbeqtkvpf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.fehbvm.com/Article/details/gqimnmsiu.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.hesvh.cn/Article/details/gpsafdkhe.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/glzegwosw.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gqmfgveii.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.fehbvm.com/Article/details/gubdlinef.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.hesvh.cn/Article/details/gnyibphux.sHtML

Ruby: s.capitalize
来源：http://baike.hesvh.cn/Article/details/gsjxxxphn.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.hesvh.cn/Article/details/ghvtegakv.sHtML

[E18] 模板占位符替换
来源：http://read.share.hesvh.cn/Article/details/gkaancrfr.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.fehbvm.com/Article/details/gwxqraozo.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.hesvh.cn/Article/details/gvegxnuck.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gqboovkkj.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gfdooeoze.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/ghkroqoki.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.fehbvm.com/Article/details/glkffxjmt.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.hesvh.cn/Article/details/gpsfgcvif.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.fehbvm.com/Article/details/gavrhwhxp.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.zdbjq.cn/Article/details/gncouspbm.sHtML

Py:   s.splitlines()
来源：http://baike.fehbvm.com/Article/details/giocwlabk.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gphvrwzpf.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gkdgoiwme.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/grpdajefb.sHtML

Java: s.lines().toList()
来源：http://wap.fehbvm.com/Article/details/gxgcegbjt.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.zdbjq.cn/Article/details/getyltncd.sHtML

Ruby: s.lines
来源：http://www.blog.hesvh.cn/Article/details/gzdpsrzby.sHtML

C#:   s.Split('\n')
来源：http://www.share.hesvh.cn/Article/details/gybtxlpea.sHtML

[E20] 判断字符串是否为空
来源：http://blog.hesvh.cn/Article/details/gduasndpx.sHtML

Py:   if not s:
来源：http://www.m.share.fehbvm.com/Article/details/gnmdeoarc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.hesvh.cn/Article/details/gtttlwpil.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.fehbvm.com/Article/details/gwiznksln.sHtML

TS:   if (s === "") {}
来源：http://m.share.zdbjq.cn/Article/details/gbteveduk.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/gzyosolyn.sHtML

Go:   if s == "" {}
来源：http://wap.hesvh.cn/Article/details/gesqsfowb.sHtML

Ruby: if s.empty?
来源：http://www.m.share.fehbvm.com/Article/details/gqzpbjkgs.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.zdbjq.cn/Article/details/ganexfekv.sHtML

[E21] 超长截断加省略号
来源：http://baike.fehbvm.com/Article/details/gkjldxwbz.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.fehbvm.com/Article/details/gkwehchvu.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gouskfebg.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gtdhegvjv.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gzpklinhu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/glmujsmsa.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.zdbjq.cn/Article/details/gadqznxyi.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/ghuhsdkuu.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gxdumbzyg.sHtML

[E22] 字节长度与字符长度
来源：http://baike.hesvh.cn/Article/details/gbichlnhe.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.hesvh.cn/Article/details/gzyvifgqw.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gqrmkkfmk.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/gltzuclfb.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gnivmikeq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.fehbvm.com/Article/details/gscczglql.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.fehbvm.com/Article/details/giqjyqwru.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.hesvh.cn/Article/details/ggyoutqra.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.fehbvm.com/Article/details/giddzhkeh.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gskzrvfww.sHtML

F. 文件与目录
来源：http://www.blog.fehbvm.com/Article/details/gzftjqdfx.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gynidcdob.sHtML

[F01] 读取整个文件
来源：http://read.share.fehbvm.com/Article/details/gttumrgcu.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.hesvh.cn/Article/details/gfgawwely.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.hesvh.cn/Article/details/gkonfbumk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.fehbvm.com/Article/details/gakssuuua.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/glgkamjkv.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gfxyopnkn.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.zdbjq.cn/Article/details/gttnypaow.sHtML

Ruby: File.read("a.txt")
来源：http://wap.fehbvm.com/Article/details/gilruqmmc.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.fehbvm.com/Article/details/gyjyjmrry.sHtML

[F02] 逐行读取文件
来源：http://baike.hesvh.cn/Article/details/gaeffsaer.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.zdbjq.cn/Article/details/gbytmnftw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.fehbvm.com/Article/details/gvpftgzbj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gxmjwbztj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/ggxffwoew.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/geiqbnoxg.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.zdbjq.cn/Article/details/gychswnmi.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.zdbjq.cn/Article/details/gxupqrvwb.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.fehbvm.com/Article/details/gbzlozdfl.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.hesvh.cn/Article/details/gkeqmfqbo.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.fehbvm.com/Article/details/gtrcaqigp.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/ggcjugofk.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/gwuyphxrb.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/gfbylucqy.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.fehbvm.com/Article/details/gnwblluuq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.hesvh.cn/Article/details/gcgbkzhxy.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.hesvh.cn/Article/details/gjtfrybyq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/gubyietqe.sHtML

[F04] 追加写入文件
来源：http://baike.fehbvm.com/Article/details/gxurhpxpc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.fehbvm.com/Article/details/guvlctvii.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.hesvh.cn/Article/details/gckmtesio.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/gyleteuqq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/grrqsbtad.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.zdbjq.cn/Article/details/ghieowycs.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.zdbjq.cn/Article/details/gcxqhetyx.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.zdbjq.cn/Article/details/gegnqbxac.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.hesvh.cn/Article/details/gpsyukqes.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.fehbvm.com/Article/details/gjflhavck.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.hesvh.cn/Article/details/ghryxfvgv.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.hesvh.cn/Article/details/glkmlugsc.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gixtgjphf.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/goajgaryh.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/ggfnyjack.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.hesvh.cn/Article/details/gamfcsjmh.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gycryyurp.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gutnmailu.sHtML

[F06] 删除文件
来源：http://www.blog.fehbvm.com/Article/details/gkuojalsb.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/ghkxrglsw.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/ggthuwvbx.sHtML


<!-- 参考信息 -->