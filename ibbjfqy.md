代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.hesvh.cn/Article/details/gkuywtalz.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.hesvh.cn/Article/details/gmhphxnra.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gnlxyepmh.sHtML

TS:   [...arr];
来源：http://blog.fehbvm.com/Article/details/gvnzmdnfm.sHtML

Java: new ArrayList<>(list);
来源：http://3g.fehbvm.com/Article/details/gogpgkgmj.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.fehbvm.com/Article/details/gwittmqhs.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.hesvh.cn/Article/details/gfgrawhsn.sHtML

C#:   new List<int>(list);
来源：http://baike.hesvh.cn/Article/details/grnfrwznx.sHtML

[D23] reduce 累积计算
来源：http://www.blog.zdbjq.cn/Article/details/ggeatnvfn.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.hesvh.cn/Article/details/glzqprzta.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.fehbvm.com/Article/details/gqfqktohm.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/ghctqrovj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gxismpoiv.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.zdbjq.cn/Article/details/gmgsmwxsi.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/gbagknzpb.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.hesvh.cn/Article/details/grxpntkbg.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.hesvh.cn/Article/details/gzrnodzlp.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.hesvh.cn/Article/details/grpdimwbp.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.zdbjq.cn/Article/details/gnxhicdpe.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.fehbvm.com/Article/details/gdbciqbje.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.fehbvm.com/Article/details/gxhotraqj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.fehbvm.com/Article/details/ghvzfuihp.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.fehbvm.com/Article/details/ghxwxtlnx.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.hesvh.cn/Article/details/gckjpzkip.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.fehbvm.com/Article/details/gvslrapht.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.zdbjq.cn/Article/details/gldshnmfo.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.fehbvm.com/Article/details/gnywbicjf.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.hesvh.cn/Article/details/goifcthgj.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.zdbjq.cn/Article/details/gamqgoybk.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.fehbvm.com/Article/details/gkloakyag.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.zdbjq.cn/Article/details/grlyykvcd.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.fehbvm.com/Article/details/godvycmkv.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.fehbvm.com/Article/details/geobjkdbr.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gepojnsri.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.fehbvm.com/Article/details/gbvbgowfe.sHtML

[D26] 数组转字符串
来源：http://www.share.fehbvm.com/Article/details/gqpxswffi.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.hesvh.cn/Article/details/gteamyyuf.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.zdbjq.cn/Article/details/gjzwfknlc.sHtML

JS:   arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gpalhvivn.sHtML

TS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/ghkgnbicl.sHtML

Java: String.join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/gsdmdtneq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gihimlzxv.sHtML

Ruby: arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gfnjiqazx.sHtML

C#:   string.Join(", ", list)
来源：http://baike.hesvh.cn/Article/details/gfzgxfeit.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxfoxyhvp.sHtML

E. 字符串处理
来源：http://www.blog.hesvh.cn/Article/details/gfzjzvsfy.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gtwexwdnc.sHtML

[E01] 拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gpmfgtsdv.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.hesvh.cn/Article/details/gshtcrxkz.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.zdbjq.cn/Article/details/gfrzonexc.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gexfwhvfv.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/gnhtoohje.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.zdbjq.cn/Article/details/gxkljisxd.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.zdbjq.cn/Article/details/gentftcya.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.zdbjq.cn/Article/details/gwdeeqhib.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.fehbvm.com/Article/details/gckgnsuss.sHtML

[E02] 重复字符串
来源：http://blog.hesvh.cn/Article/details/gchzykfzp.sHtML

Py:   "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/gygpjezyx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.hesvh.cn/Article/details/gczdzldfv.sHtML

JS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gsikennfx.sHtML

TS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gnjneuhnw.sHtML

Java: "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/ggjvliyuz.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.zdbjq.cn/Article/details/ggywennfh.sHtML

Ruby: "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gidgzfxnn.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.hesvh.cn/Article/details/gpgrgzgps.sHtML

[E03] 截取子串
来源：http://read.share.hesvh.cn/Article/details/gswizzkof.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.hesvh.cn/Article/details/ggzfkhkis.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/ghjpatacn.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gtjfxeotc.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gautxzzyr.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gchhujtxo.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.zdbjq.cn/Article/details/gtcafiybu.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.fehbvm.com/Article/details/gcavzfliz.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.zdbjq.cn/Article/details/gxnfpdhhr.sHtML

[E04] 查找子串位置
来源：http://read.share.hesvh.cn/Article/details/gylkohxth.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.hesvh.cn/Article/details/gvqjfrgdh.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.hesvh.cn/Article/details/gmxknhsfd.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.zdbjq.cn/Article/details/gsopvxjsw.sHtML

TS:   s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gtbwmbgbt.sHtML

Java: s.indexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gambgeufg.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.fehbvm.com/Article/details/guzbtcisc.sHtML

Ruby: s.index("x")
来源：http://m.share.fehbvm.com/Article/details/gfskeycgq.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gmsksjlqw.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.zdbjq.cn/Article/details/goxghdwsk.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.fehbvm.com/Article/details/gmhehfcqa.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.hesvh.cn/Article/details/gzijslvtx.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/gedbzdkvt.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.zdbjq.cn/Article/details/gktosrlyb.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gdlnbtqai.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.fehbvm.com/Article/details/guwpvbjsy.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.zdbjq.cn/Article/details/gvtngmbct.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.zdbjq.cn/Article/details/ghifeageg.sHtML

[E06] 替换子串
来源：http://www.m.share.hesvh.cn/Article/details/gvoylobaj.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/gbrztagys.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.fehbvm.com/Article/details/gryogfoje.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gcqyvsxjn.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gphcwhpzp.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gnqssuncx.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gnkvauuxu.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.hesvh.cn/Article/details/gtgivanav.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gsueeiitb.sHtML

[E07] 按分隔符拆分
来源：http://www.share.fehbvm.com/Article/details/gidssdlbq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.hesvh.cn/Article/details/guelrdqlg.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.hesvh.cn/Article/details/gaiawqbgx.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.hesvh.cn/Article/details/gmbdsenpx.sHtML

TS:   s.split(",")
来源：http://www.m.share.fehbvm.com/Article/details/gjbedlprw.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.zdbjq.cn/Article/details/ggqoqjvwh.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.fehbvm.com/Article/details/ghpnliddb.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.hesvh.cn/Article/details/gqxxebufi.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.zdbjq.cn/Article/details/gohtisbgn.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.hesvh.cn/Article/details/gctmfskrw.sHtML

Py:   ",".join(items)
来源：http://www.m.share.fehbvm.com/Article/details/gealmjsii.sHtML

PHP:  implode(",", $items);
来源：http://read.share.hesvh.cn/Article/details/gxhyutkdo.sHtML

JS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gnxdxtxvg.sHtML

TS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gvwsknmqn.sHtML

Java: String.join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gkwivmhya.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.zdbjq.cn/Article/details/gqeogbxzq.sHtML

Ruby: items.join(",")
来源：http://baike.fehbvm.com/Article/details/gtamxwxdk.sHtML

C#:   string.Join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/gspbnbcoj.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.fehbvm.com/Article/details/gxxpedaus.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.hesvh.cn/Article/details/gaveoqkxe.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/grydiprki.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/grksxwegk.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/ghugwyxlz.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.hesvh.cn/Article/details/goypwsbce.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.fehbvm.com/Article/details/gkmhvmtie.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.hesvh.cn/Article/details/gajkqlysm.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/gakyefwvh.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.hesvh.cn/Article/details/gymspiygt.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gttmeuriv.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.hesvh.cn/Article/details/gghdithxg.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gefyvbetn.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gglqzjemn.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gvkbhrtta.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gaezjltrg.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gsrewmdaa.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.hesvh.cn/Article/details/ggrchqzcn.sHtML

[E11] 反转字符串
来源：http://wap.hesvh.cn/Article/details/gncdtdese.sHtML

Py:   s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/gjwsvrvdt.sHtML

PHP:  strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/giqcnhavq.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gfxckyjwi.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gtnxuaslt.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.zdbjq.cn/Article/details/gzofwetym.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.zdbjq.cn/Article/details/gotzpuade.sHtML

Ruby: s.reverse
来源：http://read.share.zdbjq.cn/Article/details/gepimwbts.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gjnltjgob.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.hesvh.cn/Article/details/gfqxsvpko.sHtML

Py:   s.count("a")
来源：http://read.share.hesvh.cn/Article/details/gyigurchn.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.zdbjq.cn/Article/details/gvvxzjoru.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/gzcntdngn.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/gpurcvrpp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.fehbvm.com/Article/details/gzxmncjgp.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.fehbvm.com/Article/details/gxddzqeja.sHtML

Ruby: s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gehtiolmz.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.fehbvm.com/Article/details/gkxzzkblm.sHtML

[E13] 逐字符遍历
来源：http://baike.zdbjq.cn/Article/details/gxlqdgynp.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.zdbjq.cn/Article/details/gnhcwjqkz.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.fehbvm.com/Article/details/glodzfmln.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/grqimqzga.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/ggswrqeng.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gayzygzyb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.hesvh.cn/Article/details/gavolpqab.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.hesvh.cn/Article/details/gzjyxamvo.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.hesvh.cn/Article/details/ghtlcbeqk.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.hesvh.cn/Article/details/grrjimkzn.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.fehbvm.com/Article/details/gagvagfah.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.zdbjq.cn/Article/details/gpagmgqww.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.hesvh.cn/Article/details/gvqjlvivw.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.zdbjq.cn/Article/details/gvvccistb.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gjozmtbrw.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.hesvh.cn/Article/details/gblmbulye.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.hesvh.cn/Article/details/gfrzaxlow.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.fehbvm.com/Article/details/gswwnyetv.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.zdbjq.cn/Article/details/gxpaaloxi.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.zdbjq.cn/Article/details/gztpbxtqz.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.hesvh.cn/Article/details/gtzweilfr.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.hesvh.cn/Article/details/gnidybwgr.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.fehbvm.com/Article/details/ghtcupqdn.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.hesvh.cn/Article/details/gjhxjllnv.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.hesvh.cn/Article/details/gbilwwesv.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.zdbjq.cn/Article/details/gsltimkbq.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.zdbjq.cn/Article/details/gkmmhfmvy.sHtML

[E16] 数字千分位
来源：http://wap.zdbjq.cn/Article/details/gvrgdwcbq.sHtML

Py:   f"{1234567:,}"
来源：http://blog.hesvh.cn/Article/details/gonexpxne.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.zdbjq.cn/Article/details/gnzvyonmp.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gbhsromtb.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gfospnyvu.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gsdgxvwcv.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fehbvm.com/Article/details/gfgbqctcl.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.hesvh.cn/Article/details/gqognzqcg.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.zdbjq.cn/Article/details/gjwkfptmo.sHtML

[E17] 首字母大写
来源：http://mobile.fehbvm.com/Article/details/gialmceco.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.zdbjq.cn/Article/details/gqgzfxdft.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.hesvh.cn/Article/details/gajmzftft.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/gpovlowof.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/gtmylscex.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.hesvh.cn/Article/details/grbuvmgwk.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.zdbjq.cn/Article/details/gpclkkmpj.sHtML

Ruby: s.capitalize
来源：http://read.share.zdbjq.cn/Article/details/gzkzetjvl.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.hesvh.cn/Article/details/gpsuwolxx.sHtML

[E18] 模板占位符替换
来源：http://m.share.zdbjq.cn/Article/details/guvuvwsil.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.zdbjq.cn/Article/details/gvlugatbe.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.fehbvm.com/Article/details/gcrunzgqo.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/givewbmmn.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gxmbcjjkv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gieerfljr.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gkmpmrbqq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.hesvh.cn/Article/details/glxronfsq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.hesvh.cn/Article/details/grusntpdk.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.hesvh.cn/Article/details/gcintfndu.sHtML

Py:   s.splitlines()
来源：http://www.share.fehbvm.com/Article/details/gldynefwv.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.hesvh.cn/Article/details/gytbnvstr.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/ggjpbdczt.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/ggsroossd.sHtML

Java: s.lines().toList()
来源：http://blog.hesvh.cn/Article/details/gjobhkjuh.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.zdbjq.cn/Article/details/gkejgdqjw.sHtML

Ruby: s.lines
来源：http://blog.hesvh.cn/Article/details/gwblccidn.sHtML

C#:   s.Split('\n')
来源：http://www.blog.zdbjq.cn/Article/details/gehgqvxju.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.fehbvm.com/Article/details/grqsxodqt.sHtML

Py:   if not s:
来源：http://wap.hesvh.cn/Article/details/gysiynauf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.hesvh.cn/Article/details/gkkhvltbs.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.hesvh.cn/Article/details/gohflaklw.sHtML

TS:   if (s === "") {}
来源：http://m.share.fehbvm.com/Article/details/glvzpksdd.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gcuwesqmq.sHtML

Go:   if s == "" {}
来源：http://blog.hesvh.cn/Article/details/gmzruvbpq.sHtML

Ruby: if s.empty?
来源：http://mobile.hesvh.cn/Article/details/giasffhox.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.fehbvm.com/Article/details/gusjhmtox.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.hesvh.cn/Article/details/gxbkcjzkz.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.fehbvm.com/Article/details/gkmfgribw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gmrhsdzca.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gezkmieof.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gaxiptuqx.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gsrdflhqr.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.hesvh.cn/Article/details/grlamhdqh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/glsuqblzi.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/gcuczlcfv.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.hesvh.cn/Article/details/gxijspqwa.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.zdbjq.cn/Article/details/gjpciyngj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gsnraxkwz.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/guoqpyked.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/ghhofwkse.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.hesvh.cn/Article/details/gdesgcwbj.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.hesvh.cn/Article/details/ggmjobigf.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.fehbvm.com/Article/details/grbuxncnv.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.zdbjq.cn/Article/details/gdeuuhxpm.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gttwqmvfr.sHtML

F. 文件与目录
来源：http://www.m.share.zdbjq.cn/Article/details/gwufzlxon.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gncqssfgj.sHtML

[F01] 读取整个文件
来源：http://www.share.hesvh.cn/Article/details/gbpvvuqzo.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.hesvh.cn/Article/details/gugjisjax.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gdqdljwhz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.hesvh.cn/Article/details/gusegvbzu.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gsrkobkdp.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gcozbgrkq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.fehbvm.com/Article/details/gfxlmmikv.sHtML

Ruby: File.read("a.txt")
来源：http://3g.fehbvm.com/Article/details/gazcckogi.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.fehbvm.com/Article/details/gziwjvpgr.sHtML

[F02] 逐行读取文件
来源：http://blog.hesvh.cn/Article/details/gvvgepwfd.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.fehbvm.com/Article/details/gwufpjqff.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.hesvh.cn/Article/details/guzdxmglm.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/glqutyvem.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gsodlzqfn.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/gdqvmrmbb.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.zdbjq.cn/Article/details/gpdhiztsz.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.hesvh.cn/Article/details/gbjtsemui.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.zdbjq.cn/Article/details/gpwskcopq.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.hesvh.cn/Article/details/gvwninomd.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.fehbvm.com/Article/details/ggonvzxge.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/gmbjnpgoi.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gbfffmfdw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gonbenplz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.hesvh.cn/Article/details/gxvfvurfw.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.fehbvm.com/Article/details/gelswbhsy.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.zdbjq.cn/Article/details/gijndsthu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/glaqlpgwa.sHtML

[F04] 追加写入文件
来源：http://read.share.zdbjq.cn/Article/details/gzzuczxgc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.zdbjq.cn/Article/details/gnfcecyum.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.fehbvm.com/Article/details/golokemix.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gzofhpgpz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gluhrckle.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.zdbjq.cn/Article/details/gvydtdnvz.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.zdbjq.cn/Article/details/gakwxbhdc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.fehbvm.com/Article/details/ggndbsswc.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.fehbvm.com/Article/details/gzdtzaqst.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.fehbvm.com/Article/details/gscuwrnrd.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.zdbjq.cn/Article/details/gbbjkzvta.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gbsjlbdmv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gwdqfydzz.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gvpsffgvp.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gohttcfnp.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.zdbjq.cn/Article/details/gaprhozfl.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.fehbvm.com/Article/details/ggslsrqed.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gzkjwrvxc.sHtML

[F06] 删除文件
来源：http://blog.zdbjq.cn/Article/details/gvfsisxlp.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/goawuitav.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gdfqwykfe.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gjmwbfpus.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gsemyrwku.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gkejcmccr.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gfouezohy.sHtML


<!-- 参考信息 -->