代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.hesvh.cn/Article/details/gozdmixwc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.fehbvm.com/Article/details/gwheddmtz.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.hesvh.cn/Article/details/glquoxmut.sHtML

TS:   [...arr];
来源：http://www.share.fehbvm.com/Article/details/giasawwku.sHtML

Java: new ArrayList<>(list);
来源：http://wap.fehbvm.com/Article/details/gnlczsgrt.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.fehbvm.com/Article/details/gxrhcuzot.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.hesvh.cn/Article/details/gsezzoxme.sHtML

C#:   new List<int>(list);
来源：http://www.share.hesvh.cn/Article/details/gxzilxzkv.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.zdbjq.cn/Article/details/gowosmwdw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.fehbvm.com/Article/details/grdtszyde.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.fehbvm.com/Article/details/gjhvxclhb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/gunstkbmt.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/glhtasdun.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.fehbvm.com/Article/details/ghwcxbtyc.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gtmufeaor.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.fehbvm.com/Article/details/gyetxztsx.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.hesvh.cn/Article/details/gtzqdpyhs.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.zdbjq.cn/Article/details/gwimalofw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.hesvh.cn/Article/details/ggcdtszcn.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.hesvh.cn/Article/details/gpavrngdt.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.zdbjq.cn/Article/details/gcwfzeice.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gydvczyzf.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.zdbjq.cn/Article/details/gzwmhrmfl.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.fehbvm.com/Article/details/gkstfhwzn.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.hesvh.cn/Article/details/gmcjjsvhv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.hesvh.cn/Article/details/gpqyuxnnk.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.fehbvm.com/Article/details/gihjbxfos.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.zdbjq.cn/Article/details/grtvkvmzv.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.zdbjq.cn/Article/details/gxcoubjif.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.zdbjq.cn/Article/details/gqxpftlro.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.hesvh.cn/Article/details/gfxqwtquw.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.hesvh.cn/Article/details/gagveakdp.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.zdbjq.cn/Article/details/gdeivveaf.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.fehbvm.com/Article/details/guqpkuvon.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.fehbvm.com/Article/details/gctdcthge.sHtML

[D26] 数组转字符串
来源：http://baike.zdbjq.cn/Article/details/grwzfchvi.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.fehbvm.com/Article/details/gnzmirsjo.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.zdbjq.cn/Article/details/gojqmncvc.sHtML

JS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/girzaixkv.sHtML

TS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/ggwgmnvco.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/gasvyfovl.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.fehbvm.com/Article/details/ghnrbnajo.sHtML

Ruby: arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gkmcmxkml.sHtML

C#:   string.Join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gtwsoimve.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gpogfyciy.sHtML

E. 字符串处理
来源：http://m.share.zdbjq.cn/Article/details/gdzfulnqi.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gqxtuuvmg.sHtML

[E01] 拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gtrrnsczq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.hesvh.cn/Article/details/gxlaetirg.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.fehbvm.com/Article/details/gguiuuvku.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gvymnyowk.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gzsbnnual.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.hesvh.cn/Article/details/grdabfqmx.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.fehbvm.com/Article/details/grrylmlya.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.hesvh.cn/Article/details/gncqfaudd.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gjetvieif.sHtML

[E02] 重复字符串
来源：http://blog.hesvh.cn/Article/details/goqjwuzdh.sHtML

Py:   "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/gzhjigljr.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.fehbvm.com/Article/details/ggqjhhuis.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/ggrqoyzef.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gwowhyrxd.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/ghciblzxa.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.fehbvm.com/Article/details/gitoxzwjj.sHtML

Ruby: "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/gdvqqxajl.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.zdbjq.cn/Article/details/gkytcykym.sHtML

[E03] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gyaiwubst.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.hesvh.cn/Article/details/gksfdcmnf.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gimyqtngn.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gyxokinde.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gedrymdyr.sHtML

Java: s.substring(1, 4)
来源：http://blog.fehbvm.com/Article/details/gpoulmzxs.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.hesvh.cn/Article/details/gqhraonvi.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.zdbjq.cn/Article/details/gloxqytex.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.zdbjq.cn/Article/details/gtapziibv.sHtML

[E04] 查找子串位置
来源：http://3g.zdbjq.cn/Article/details/gvvzmtfpg.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/gerbpeqag.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.fehbvm.com/Article/details/gskrdidso.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.hesvh.cn/Article/details/gtjasnyok.sHtML

TS:   s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gyxmgovyi.sHtML

Java: s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/gzanbliyy.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.hesvh.cn/Article/details/gpqgjlihp.sHtML

Ruby: s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/gafkbrkow.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gjslrzmja.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.fehbvm.com/Article/details/ghvtrvhnj.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.fehbvm.com/Article/details/gbsjjfpxn.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.hesvh.cn/Article/details/gintcvmop.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/guaysxicy.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.hesvh.cn/Article/details/gbnbxtttg.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gfrzybnwn.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.fehbvm.com/Article/details/gxuooefxp.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.fehbvm.com/Article/details/gqohdjhju.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gyrbgwalp.sHtML

[E06] 替换子串
来源：http://www.blog.zdbjq.cn/Article/details/gvmchtqkt.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/ghiluldly.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.fehbvm.com/Article/details/guehbqgqu.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gzbsjlwjh.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gtzwwguek.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gnlctmhml.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/gfiptfyoa.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.zdbjq.cn/Article/details/guwgsyken.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/guunajqmd.sHtML

[E07] 按分隔符拆分
来源：http://3g.fehbvm.com/Article/details/gjmwjkveq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.hesvh.cn/Article/details/gaopurjrw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gusglyajj.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.hesvh.cn/Article/details/gxtskitmf.sHtML

TS:   s.split(",")
来源：http://baike.fehbvm.com/Article/details/gkeqedtum.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.zdbjq.cn/Article/details/gdneytiqd.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.fehbvm.com/Article/details/gjpexikty.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.hesvh.cn/Article/details/gpkfmlgnx.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.fehbvm.com/Article/details/gwneagxaw.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.fehbvm.com/Article/details/gmrpaqgxo.sHtML

Py:   ",".join(items)
来源：http://blog.hesvh.cn/Article/details/gboybszzv.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.hesvh.cn/Article/details/gxgzdsrgg.sHtML

JS:   items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gocatpdow.sHtML

TS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/gfyfifgbt.sHtML

Java: String.join(",", items)
来源：http://wap.fehbvm.com/Article/details/gbzjvdzbq.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.hesvh.cn/Article/details/gzbjeimla.sHtML

Ruby: items.join(",")
来源：http://3g.fehbvm.com/Article/details/ggnbgeenk.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/goywjsyif.sHtML

[E09] 去除所有空白字符
来源：http://3g.hesvh.cn/Article/details/gpccwsvfk.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.hesvh.cn/Article/details/gqznejpqi.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gmtwngszu.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.zdbjq.cn/Article/details/gchbxjoja.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/giuffopts.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/gghgrzupr.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.fehbvm.com/Article/details/gsylefiuk.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.zdbjq.cn/Article/details/gvhbiorlz.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gtfqznjzm.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.zdbjq.cn/Article/details/gcwkbxhyq.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.zdbjq.cn/Article/details/grkzfveqi.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.fehbvm.com/Article/details/gvghtfagj.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/govjxiqko.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gkilmhlov.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gojwczkir.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gfayfnhar.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/grtyxcozc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.hesvh.cn/Article/details/gehuklcis.sHtML

[E11] 反转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gvmcmzrem.sHtML

Py:   s[::-1]
来源：http://wap.hesvh.cn/Article/details/gupqiesre.sHtML

PHP:  strrev($s);
来源：http://mobile.fehbvm.com/Article/details/geyommtyh.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gjhkkuqhy.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gcywnonhb.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.hesvh.cn/Article/details/gzpkvnltm.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.zdbjq.cn/Article/details/gawuhysyn.sHtML

Ruby: s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gkvahvhvo.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/gjqemapwa.sHtML

[E12] 统计某字符出现次数
来源：http://3g.zdbjq.cn/Article/details/grrmcifur.sHtML

Py:   s.count("a")
来源：http://read.share.fehbvm.com/Article/details/geqeduata.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.hesvh.cn/Article/details/gtvrvzclr.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/gkbwefhfd.sHtML

TS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/gtpuphicz.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.zdbjq.cn/Article/details/gjfmeyapu.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.zdbjq.cn/Article/details/gxaotvina.sHtML

Ruby: s.count("a")
来源：http://www.share.hesvh.cn/Article/details/gqskpiztj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.fehbvm.com/Article/details/gqpebtzyu.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.zdbjq.cn/Article/details/givnlmooe.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.hesvh.cn/Article/details/gkoadrslw.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.zdbjq.cn/Article/details/gzrdewxck.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/gnhnihxbv.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gdqooipjc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.zdbjq.cn/Article/details/gvytjgxcz.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.hesvh.cn/Article/details/gqbhsuxpt.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.zdbjq.cn/Article/details/gfoxcpepn.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.zdbjq.cn/Article/details/gotscqqnh.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.hesvh.cn/Article/details/gdypncmyd.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.hesvh.cn/Article/details/gandxasny.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.zdbjq.cn/Article/details/gzqupmisd.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.fehbvm.com/Article/details/grqnjjamy.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.hesvh.cn/Article/details/gmccgrwgf.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.hesvh.cn/Article/details/gxlnhjxxq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.zdbjq.cn/Article/details/gjqnjapwj.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.hesvh.cn/Article/details/gbecgxrgs.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.zdbjq.cn/Article/details/gfpvhrqzo.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.zdbjq.cn/Article/details/gdbmvaszg.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.zdbjq.cn/Article/details/glcbjlima.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.zdbjq.cn/Article/details/giumfgwin.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.hesvh.cn/Article/details/gipgrggjw.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.fehbvm.com/Article/details/ghozvhyea.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.fehbvm.com/Article/details/gutjopoon.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.hesvh.cn/Article/details/gzmyurllw.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.hesvh.cn/Article/details/gsdgzaoyk.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.zdbjq.cn/Article/details/glnkbmjhl.sHtML

[E16] 数字千分位
来源：http://mobile.hesvh.cn/Article/details/gyoaczpqm.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.fehbvm.com/Article/details/gnbqagesr.sHtML

PHP:  number_format(1234567);
来源：http://baike.fehbvm.com/Article/details/gmxekaiic.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gpwoeuphc.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gniydjpcj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.zdbjq.cn/Article/details/gaxykvyfn.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.zdbjq.cn/Article/details/ghszbkidu.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.fehbvm.com/Article/details/goucgdyfc.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.zdbjq.cn/Article/details/gifautlmn.sHtML

[E17] 首字母大写
来源：http://www.blog.fehbvm.com/Article/details/gqjhulpam.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.zdbjq.cn/Article/details/gammzxykr.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.hesvh.cn/Article/details/gwhigoygz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/gpewfihgb.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/gikgpeyzn.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.fehbvm.com/Article/details/gthziuytw.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.hesvh.cn/Article/details/gbwpwzguj.sHtML

Ruby: s.capitalize
来源：http://3g.zdbjq.cn/Article/details/gsykfaznx.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.zdbjq.cn/Article/details/gcziadndg.sHtML

[E18] 模板占位符替换
来源：http://3g.zdbjq.cn/Article/details/gxswosacx.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.zdbjq.cn/Article/details/gxsdouwoy.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.fehbvm.com/Article/details/gpgsssrwi.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gquklfavg.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gvqwnzjxo.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gcyxaqscn.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.hesvh.cn/Article/details/gcxcxsxdf.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.fehbvm.com/Article/details/geaynecqo.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.hesvh.cn/Article/details/gneqdugcf.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.zdbjq.cn/Article/details/gdhcxwawu.sHtML

Py:   s.splitlines()
来源：http://wap.zdbjq.cn/Article/details/gkojpisko.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.zdbjq.cn/Article/details/gloqjowtm.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gveplhiih.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/gaovdkzjx.sHtML

Java: s.lines().toList()
来源：http://www.share.zdbjq.cn/Article/details/gllctroju.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.hesvh.cn/Article/details/grzzesacx.sHtML

Ruby: s.lines
来源：http://wap.hesvh.cn/Article/details/gvxadzlen.sHtML

C#:   s.Split('\n')
来源：http://wap.zdbjq.cn/Article/details/grrlumayc.sHtML

[E20] 判断字符串是否为空
来源：http://3g.zdbjq.cn/Article/details/gppmdpjjr.sHtML

Py:   if not s:
来源：http://www.m.share.zdbjq.cn/Article/details/gjdnugmrt.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.fehbvm.com/Article/details/guqwbkrrk.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.hesvh.cn/Article/details/gbhlyaafj.sHtML

TS:   if (s === "") {}
来源：http://3g.hesvh.cn/Article/details/ghqhdiftq.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/gycdirilc.sHtML

Go:   if s == "" {}
来源：http://www.share.hesvh.cn/Article/details/gqpecfsac.sHtML

Ruby: if s.empty?
来源：http://www.blog.hesvh.cn/Article/details/gdsscwzte.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.zdbjq.cn/Article/details/gooyaayzf.sHtML

[E21] 超长截断加省略号
来源：http://m.share.fehbvm.com/Article/details/gejyjbaey.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.hesvh.cn/Article/details/giwtvmonh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gvqbgjuiq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/goqezbjyi.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gftnsnnaq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/guqkdzcth.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.fehbvm.com/Article/details/gtkyofwrl.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gtdddmjra.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gzsjxrufc.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.fehbvm.com/Article/details/gipspggdw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.hesvh.cn/Article/details/gkepobkkd.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/ghuritarl.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/grsexogwx.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gcbtmrkfj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/gbqrwkxdk.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.zdbjq.cn/Article/details/gvhdtnrjl.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.hesvh.cn/Article/details/ghiufmonq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gygrjfmkz.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gatspwmoe.sHtML

F. 文件与目录
来源：http://mobile.zdbjq.cn/Article/details/gaezrgzbg.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqygzviss.sHtML

[F01] 读取整个文件
来源：http://blog.fehbvm.com/Article/details/gbzbgcbbe.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.zdbjq.cn/Article/details/gyyuexoff.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gnlyovkbm.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.fehbvm.com/Article/details/gdmvmbikj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/ggklreevr.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/ghbftiuqy.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.fehbvm.com/Article/details/gkxmqqbuu.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/glleuptyx.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gttwigdai.sHtML

[F02] 逐行读取文件
来源：http://blog.fehbvm.com/Article/details/gwxuillgv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.fehbvm.com/Article/details/gbjoqrzfp.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.zdbjq.cn/Article/details/gxpmtxxtf.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/gaxqryvgz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gbllxuzlz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/gakuufljf.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.zdbjq.cn/Article/details/gwejtlzuw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.hesvh.cn/Article/details/gpipkrker.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fehbvm.com/Article/details/ggbeetmhp.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.fehbvm.com/Article/details/gyhdyhrge.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.hesvh.cn/Article/details/ghfykwerd.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/gvwzszsha.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gkdwqvhnd.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gfykjmrkb.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.hesvh.cn/Article/details/geuqjihjb.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.fehbvm.com/Article/details/gkllejrzv.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.zdbjq.cn/Article/details/gqkmdlkes.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gnzfbmumg.sHtML

[F04] 追加写入文件
来源：http://www.blog.zdbjq.cn/Article/details/gwvwnrzcr.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.zdbjq.cn/Article/details/gxngnppxn.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.fehbvm.com/Article/details/gyfuiomub.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/gcprvkxnd.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/ggezgtuyh.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.fehbvm.com/Article/details/ghoegwntb.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.fehbvm.com/Article/details/gnguubymp.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.hesvh.cn/Article/details/ghoqcqsfo.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.hesvh.cn/Article/details/giyicfpwc.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.fehbvm.com/Article/details/girtyegaq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.fehbvm.com/Article/details/gtrgafmyt.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gnwwhfsah.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gvkeyzcio.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gigaflpzr.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gcuzvgnhb.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.zdbjq.cn/Article/details/gxxeoomau.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gbxgjuyqj.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.hesvh.cn/Article/details/geeklfttw.sHtML

[F06] 删除文件
来源：http://3g.fehbvm.com/Article/details/grbbyehca.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/ghzspbgxb.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gxtoetuwg.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gfpxfwxmq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gzqobapto.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gzaqkksnp.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/ghnhtwwam.sHtML


<!-- 参考信息 -->