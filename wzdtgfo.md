代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.fehbvm.com/Article/details/gxxwkqzqw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.hesvh.cn/Article/details/guyvaprzh.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.fehbvm.com/Article/details/gkifnyfrn.sHtML

TS:   [...arr];
来源：http://wap.zdbjq.cn/Article/details/gvbvbnuxb.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.hesvh.cn/Article/details/grczukvsc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.zdbjq.cn/Article/details/gqfsppvzi.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.zdbjq.cn/Article/details/gstklhxkt.sHtML

C#:   new List<int>(list);
来源：http://3g.zdbjq.cn/Article/details/gtkoehkzn.sHtML

[D23] reduce 累积计算
来源：http://wap.zdbjq.cn/Article/details/glilissuj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.hesvh.cn/Article/details/gqmzjkyft.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.hesvh.cn/Article/details/gslbfvfef.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gemtyxunz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gxmpwulva.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.hesvh.cn/Article/details/gotwfwzfo.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gxagqbzhv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.fehbvm.com/Article/details/gsxdxevnl.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.fehbvm.com/Article/details/gifivxkus.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.zdbjq.cn/Article/details/gxjigeqfe.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.zdbjq.cn/Article/details/ghdntbbcv.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.zdbjq.cn/Article/details/grwrzuqdt.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.hesvh.cn/Article/details/galcznnzd.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gaesaejqs.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.hesvh.cn/Article/details/gkhxfrneg.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.fehbvm.com/Article/details/grdcuzzip.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gnvruowsb.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.hesvh.cn/Article/details/gskcsbxjf.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.fehbvm.com/Article/details/gtafwndbq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.hesvh.cn/Article/details/gybzgsouq.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fehbvm.com/Article/details/gipomqfhh.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.zdbjq.cn/Article/details/gocghcavg.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.fehbvm.com/Article/details/gebpwobcd.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.zdbjq.cn/Article/details/gnsnvrtqd.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.zdbjq.cn/Article/details/gjdvhdadt.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.zdbjq.cn/Article/details/gdhldfyzs.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.hesvh.cn/Article/details/gnqpbzvzl.sHtML

[D26] 数组转字符串
来源：http://baike.zdbjq.cn/Article/details/gruafurvn.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.zdbjq.cn/Article/details/glyxeckwn.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.fehbvm.com/Article/details/gjpmjwpxm.sHtML

JS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gmjuwulqj.sHtML

TS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gewrjklav.sHtML

Java: String.join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/gzhmncffc.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.zdbjq.cn/Article/details/gpgrpxxla.sHtML

Ruby: arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gqjrfihzn.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/ggcmcuvbi.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gmnlmizpm.sHtML

E. 字符串处理
来源：http://baike.zdbjq.cn/Article/details/gtfkbjkqj.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gpnajkpom.sHtML

[E01] 拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gxnjrsqhf.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.hesvh.cn/Article/details/gftvbbfgj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.fehbvm.com/Article/details/guumxwzee.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/gvvpkjkik.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gyqiipzin.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.hesvh.cn/Article/details/gchnqpehl.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.hesvh.cn/Article/details/gdjsiouib.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.hesvh.cn/Article/details/gskgrjffw.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gpouzxnsl.sHtML

[E02] 重复字符串
来源：http://blog.fehbvm.com/Article/details/gjsobyhbz.sHtML

Py:   "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gxtvxdpvh.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.fehbvm.com/Article/details/gmrmyyxyd.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gtrjqntqq.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/guknbvowl.sHtML

Java: "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gpugojqci.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.hesvh.cn/Article/details/ghlswtcvq.sHtML

Ruby: "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gwlhddplv.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.hesvh.cn/Article/details/gbwdmqvvv.sHtML

[E03] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gnjgjrwgq.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.fehbvm.com/Article/details/gxpwrhyzb.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gsnouydtj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gsedixzqk.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gurrufgwg.sHtML

Java: s.substring(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gwnbbifso.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.hesvh.cn/Article/details/gcmfnvurv.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.zdbjq.cn/Article/details/grwvxwciv.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.hesvh.cn/Article/details/gmxlswduc.sHtML

[E04] 查找子串位置
来源：http://mobile.hesvh.cn/Article/details/gfiyrrwsw.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.hesvh.cn/Article/details/gtuoqqwek.sHtML

PHP:  strpos($s, "x");
来源：http://baike.fehbvm.com/Article/details/glynymijh.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.fehbvm.com/Article/details/gahxgbova.sHtML

TS:   s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/guptwnxqf.sHtML

Java: s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/gapdsvcqj.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.fehbvm.com/Article/details/gkuvveslj.sHtML

Ruby: s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gdkrmpoeo.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gwzivdxfv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.zdbjq.cn/Article/details/ggdypgpnp.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.zdbjq.cn/Article/details/gycnjhnft.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.hesvh.cn/Article/details/gtnhwtcpj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.hesvh.cn/Article/details/ggylafokg.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.zdbjq.cn/Article/details/gblpgkiox.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/guyxtdmwb.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.hesvh.cn/Article/details/gcquhkblh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.zdbjq.cn/Article/details/gydjtrggd.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.fehbvm.com/Article/details/gptuljudq.sHtML

[E06] 替换子串
来源：http://www.m.share.hesvh.cn/Article/details/gdnujhohm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/glgtfvgpv.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.hesvh.cn/Article/details/gfdpmkjud.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/grupjfabm.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gztyiikat.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gikxtphja.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/guhqkhied.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gemcdervo.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.hesvh.cn/Article/details/gpyigdsgd.sHtML

[E07] 按分隔符拆分
来源：http://mobile.hesvh.cn/Article/details/gfgdbuaue.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.hesvh.cn/Article/details/gkfsggjgk.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.hesvh.cn/Article/details/grthjtsnz.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.fehbvm.com/Article/details/ghwvwrrbb.sHtML

TS:   s.split(",")
来源：http://baike.fehbvm.com/Article/details/gbkdhjyzy.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.hesvh.cn/Article/details/gvhbtguzv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.zdbjq.cn/Article/details/gaydvjklt.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.zdbjq.cn/Article/details/gonmalktg.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.zdbjq.cn/Article/details/gzyfnoquh.sHtML

[E08] 数组按分隔符合并
来源：http://wap.fehbvm.com/Article/details/gtguziisi.sHtML

Py:   ",".join(items)
来源：http://wap.zdbjq.cn/Article/details/gphylbgcy.sHtML

PHP:  implode(",", $items);
来源：http://3g.hesvh.cn/Article/details/gbexpevvw.sHtML

JS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/gpyalcwjq.sHtML

TS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/ghgqwjouy.sHtML

Java: String.join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/gfqxwgwhe.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.zdbjq.cn/Article/details/gftabeuhr.sHtML

Ruby: items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gcjtwlrkr.sHtML

C#:   string.Join(",", items)
来源：http://wap.fehbvm.com/Article/details/gbibgqpbi.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.fehbvm.com/Article/details/gfqhvtrse.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gejprvhtn.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.fehbvm.com/Article/details/gcgvtdorg.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gcsnhcakd.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/gitnqfexq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gndstlmcp.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.fehbvm.com/Article/details/guoiefigx.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.fehbvm.com/Article/details/gwhytziqh.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.hesvh.cn/Article/details/gjxecnwrx.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.fehbvm.com/Article/details/gwqlivfav.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gucvossds.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.fehbvm.com/Article/details/gystrdvxq.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gncgcrigo.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gyouftrsz.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gipiectcr.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gbdiivdbd.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gqqhpnhdj.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.zdbjq.cn/Article/details/gtgwhbhqf.sHtML

[E11] 反转字符串
来源：http://www.blog.fehbvm.com/Article/details/gqqpdydyv.sHtML

Py:   s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/gitcvrjkc.sHtML

PHP:  strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/gqdiwglyh.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gnxwsadxb.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/ggiktrpei.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.hesvh.cn/Article/details/gexocnstd.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.hesvh.cn/Article/details/gmkfmvady.sHtML

Ruby: s.reverse
来源：http://mobile.zdbjq.cn/Article/details/ggmoumyid.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/glbwvlihg.sHtML

[E12] 统计某字符出现次数
来源：http://baike.fehbvm.com/Article/details/giiqesmcn.sHtML

Py:   s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/gihkdounz.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.hesvh.cn/Article/details/gsbzemith.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/gjjusbavm.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gkfjmkedw.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.hesvh.cn/Article/details/gbmrhpjzx.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.fehbvm.com/Article/details/gcqsllfdd.sHtML

Ruby: s.count("a")
来源：http://mobile.hesvh.cn/Article/details/gntqgqosw.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.hesvh.cn/Article/details/geabjkobn.sHtML

[E13] 逐字符遍历
来源：http://baike.hesvh.cn/Article/details/gmrngizig.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.zdbjq.cn/Article/details/gbpripcxd.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.zdbjq.cn/Article/details/gvpxzhekm.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/goyfmhoir.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/givkyihgu.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.hesvh.cn/Article/details/gfqmyioug.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.zdbjq.cn/Article/details/gtlrukogc.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.zdbjq.cn/Article/details/gokwhtpwy.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.fehbvm.com/Article/details/gqpbtvbet.sHtML

[E14] URL 编码与 Base64
来源：http://blog.fehbvm.com/Article/details/gymnlfode.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.hesvh.cn/Article/details/gokuaorjs.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.hesvh.cn/Article/details/gfvyuplzh.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.fehbvm.com/Article/details/gkbspvhem.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.hesvh.cn/Article/details/gtzndbvye.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.fehbvm.com/Article/details/gpfblrwfd.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.zdbjq.cn/Article/details/gohiuvlmp.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.hesvh.cn/Article/details/ggmosunzj.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.zdbjq.cn/Article/details/gqbnzpvia.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.fehbvm.com/Article/details/gdwqmmbhd.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.hesvh.cn/Article/details/glblumipf.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/ghcplamft.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.zdbjq.cn/Article/details/gasjigjxo.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.fehbvm.com/Article/details/gvcvucueg.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.fehbvm.com/Article/details/gacalubnh.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.hesvh.cn/Article/details/getqblats.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.zdbjq.cn/Article/details/glvwwyrqi.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.hesvh.cn/Article/details/gkkcturzy.sHtML

[E16] 数字千分位
来源：http://www.blog.hesvh.cn/Article/details/grnrlbvoz.sHtML

Py:   f"{1234567:,}"
来源：http://wap.zdbjq.cn/Article/details/goutikfvt.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.hesvh.cn/Article/details/grsngtase.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/gvbfpuaaz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/gruqkpwjh.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.hesvh.cn/Article/details/gkbqlgryr.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.hesvh.cn/Article/details/glfndkndm.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.hesvh.cn/Article/details/gmaprxarg.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.zdbjq.cn/Article/details/ghyolgxma.sHtML

[E17] 首字母大写
来源：http://baike.fehbvm.com/Article/details/gprmzxxxr.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.zdbjq.cn/Article/details/gcodrjbzt.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.zdbjq.cn/Article/details/gkqdzqsng.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/glkfdbmfq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gsqsxkqys.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.hesvh.cn/Article/details/gimauwjof.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.hesvh.cn/Article/details/giwxkniot.sHtML

Ruby: s.capitalize
来源：http://3g.zdbjq.cn/Article/details/gxsnbejsi.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.fehbvm.com/Article/details/gctwndzxa.sHtML

[E18] 模板占位符替换
来源：http://blog.fehbvm.com/Article/details/gfoexyfsb.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.zdbjq.cn/Article/details/gnmjnthhh.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.zdbjq.cn/Article/details/gtudmozhe.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gpbektqao.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gwkhsyjne.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gwpupdtfi.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gkshxojxw.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.hesvh.cn/Article/details/gcwzkkupu.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.hesvh.cn/Article/details/gfdvdruwz.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.zdbjq.cn/Article/details/gtxtjxzjj.sHtML

Py:   s.splitlines()
来源：http://mobile.fehbvm.com/Article/details/glrnpzicz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.hesvh.cn/Article/details/gvjxvidfl.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.hesvh.cn/Article/details/guvshqedk.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gpymcwzdj.sHtML

Java: s.lines().toList()
来源：http://read.share.zdbjq.cn/Article/details/gkambhyie.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.hesvh.cn/Article/details/goolpbhlf.sHtML

Ruby: s.lines
来源：http://www.share.hesvh.cn/Article/details/ggfvndvna.sHtML

C#:   s.Split('\n')
来源：http://baike.hesvh.cn/Article/details/grnsobewv.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.zdbjq.cn/Article/details/gypshkhvz.sHtML

Py:   if not s:
来源：http://read.share.zdbjq.cn/Article/details/ghhlshivb.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.zdbjq.cn/Article/details/gltynbcbk.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.fehbvm.com/Article/details/gxitqznwx.sHtML

TS:   if (s === "") {}
来源：http://read.share.zdbjq.cn/Article/details/gzfgmfoxw.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/gbwocfpke.sHtML

Go:   if s == "" {}
来源：http://3g.zdbjq.cn/Article/details/gfcntcnvs.sHtML

Ruby: if s.empty?
来源：http://www.share.fehbvm.com/Article/details/glvfdjujh.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.hesvh.cn/Article/details/gazqhxusj.sHtML

[E21] 超长截断加省略号
来源：http://m.share.hesvh.cn/Article/details/gwqctmnvo.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.zdbjq.cn/Article/details/ghoqrkavs.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gfntsmfrf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gamudkyos.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gtwjdexba.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gujidxruv.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.fehbvm.com/Article/details/gbnuzhvsz.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gsetzsbqm.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/ghhrxifrg.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.fehbvm.com/Article/details/gamxxghic.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.fehbvm.com/Article/details/gzeturmdo.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gntfwikkk.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/gwippmcyv.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/guqycposj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.zdbjq.cn/Article/details/gizlpslqw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.zdbjq.cn/Article/details/grxyetvjp.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gtzmtdksu.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.hesvh.cn/Article/details/guvcaococ.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghmizwjag.sHtML

F. 文件与目录
来源：http://3g.fehbvm.com/Article/details/gwbclzyct.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gddbialbq.sHtML

[F01] 读取整个文件
来源：http://www.blog.fehbvm.com/Article/details/gadztlrlr.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.fehbvm.com/Article/details/gwthrpqvl.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gmluxzalm.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.zdbjq.cn/Article/details/gsnvcwsus.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gifepxvhk.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/grmzvwmfx.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.zdbjq.cn/Article/details/gyhmbdtny.sHtML

Ruby: File.read("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gomjgvfyi.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gmybomdkm.sHtML

[F02] 逐行读取文件
来源：http://blog.hesvh.cn/Article/details/gwioxctbz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.fehbvm.com/Article/details/gwyjygztw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.hesvh.cn/Article/details/groqebgpe.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/gyfyslfda.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/gdjrvqoso.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gimqkcykx.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.fehbvm.com/Article/details/gvmpaltqx.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.fehbvm.com/Article/details/ggqiehbbh.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.fehbvm.com/Article/details/gazxeofjm.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.hesvh.cn/Article/details/gjhmldddx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.zdbjq.cn/Article/details/gabwqpthl.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/gncxivpyi.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/gtptkvken.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gdcjazwam.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.hesvh.cn/Article/details/gyeosvzvk.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.hesvh.cn/Article/details/gjnwebrke.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.zdbjq.cn/Article/details/gdjivzjzd.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gozumwtwq.sHtML

[F04] 追加写入文件
来源：http://read.share.fehbvm.com/Article/details/gauaxingw.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.fehbvm.com/Article/details/gnsmtbjfw.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.fehbvm.com/Article/details/gnihayyuf.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/gyabjspzb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gefraxprg.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.zdbjq.cn/Article/details/genpyibuk.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gjrbiimoc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.zdbjq.cn/Article/details/gxqalpldx.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.hesvh.cn/Article/details/guczqkcwl.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.hesvh.cn/Article/details/gvsufxnwa.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.zdbjq.cn/Article/details/gygdmrhsz.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.hesvh.cn/Article/details/ghcrlccbn.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gzknnmuql.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gcceubfog.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/glrtnhjtz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.fehbvm.com/Article/details/glnsrvloq.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.hesvh.cn/Article/details/glzfthpuk.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gfdliidbu.sHtML

[F06] 删除文件
来源：http://wap.hesvh.cn/Article/details/ggfgatiyk.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gnzokdvtg.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gtdsallqf.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/glmfhksbo.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gclvmrztq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/glroqdqlk.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/gbsyckbxu.sHtML


<!-- 参考信息 -->