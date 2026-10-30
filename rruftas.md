代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://3g.fehbvm.com/Article/details/gpleabnqt.sHtML

JS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/godaubnsi.sHtML

TS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gqvimrxdi.sHtML

Java: list.contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gxyqyrkss.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gubjdlfxy.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/gazezhiij.sHtML

C#:   list.Contains(x)
来源：http://baike.hesvh.cn/Article/details/gjbeofntg.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.zdbjq.cn/Article/details/ggpqlwumr.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.zdbjq.cn/Article/details/grygejjur.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.zdbjq.cn/Article/details/gjvfhbyio.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gsrxwxlxz.sHtML

TS:   [...arr];
来源：http://mobile.fehbvm.com/Article/details/gjxuaodpw.sHtML

Java: new ArrayList<>(list);
来源：http://blog.zdbjq.cn/Article/details/gqzawoigk.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.hesvh.cn/Article/details/gttnietsy.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.hesvh.cn/Article/details/glxeuffye.sHtML

C#:   new List<int>(list);
来源：http://www.blog.fehbvm.com/Article/details/gxbwwrhoo.sHtML

[D23] reduce 累积计算
来源：http://mobile.zdbjq.cn/Article/details/gkxnyxnca.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.fehbvm.com/Article/details/gkwllnekt.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.fehbvm.com/Article/details/gadpqunig.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gddyjywsn.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gxcmbkklz.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.zdbjq.cn/Article/details/grkgbopay.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/gjhmqcpsn.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.zdbjq.cn/Article/details/ghdzkljkb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.hesvh.cn/Article/details/ghykspcrx.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.hesvh.cn/Article/details/gpqpnxxrp.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.fehbvm.com/Article/details/ggvkygufb.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.zdbjq.cn/Article/details/gkhueuhzl.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.hesvh.cn/Article/details/gyfnvekiq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gziyltixt.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.fehbvm.com/Article/details/gnfujbsus.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.zdbjq.cn/Article/details/gvjklnmgw.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.zdbjq.cn/Article/details/ghjshjdfv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.zdbjq.cn/Article/details/gyddqckdc.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.fehbvm.com/Article/details/gumkjtgrg.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.fehbvm.com/Article/details/gomfzvlhn.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.hesvh.cn/Article/details/guqqkxlvv.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.hesvh.cn/Article/details/gdrpnaxeu.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.zdbjq.cn/Article/details/gqczyskry.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.zdbjq.cn/Article/details/gekynklhk.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.fehbvm.com/Article/details/gqueiktlw.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.fehbvm.com/Article/details/goammawgg.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/guumkacbp.sHtML

[D26] 数组转字符串
来源：http://www.share.hesvh.cn/Article/details/gnufgscjz.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.hesvh.cn/Article/details/gomddujks.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.hesvh.cn/Article/details/grpfvcmit.sHtML

JS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gguaiswxq.sHtML

TS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gdqwvbmhx.sHtML

Java: String.join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/grsdwoptg.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.hesvh.cn/Article/details/glfvlivlm.sHtML

Ruby: arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gglvwbops.sHtML

C#:   string.Join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gpcytrybv.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gmkxgdhjb.sHtML

E. 字符串处理
来源：http://read.share.hesvh.cn/Article/details/gxfppfvac.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gxcxcfape.sHtML

[E01] 拼接字符串
来源：http://3g.fehbvm.com/Article/details/gbrqgjred.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.hesvh.cn/Article/details/gnbfbmxcq.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.zdbjq.cn/Article/details/ghizcbqnn.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/ghgeksdop.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/ggknoxhdf.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.zdbjq.cn/Article/details/gevehoxlj.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.hesvh.cn/Article/details/gfjpiiuej.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.fehbvm.com/Article/details/gliejqtpf.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/geydqhejf.sHtML

[E02] 重复字符串
来源：http://3g.fehbvm.com/Article/details/galtklvii.sHtML

Py:   "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/gelriaayw.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.fehbvm.com/Article/details/gxkcqkxoh.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/giszngook.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gttkxsced.sHtML

Java: "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gjkzrgndm.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.hesvh.cn/Article/details/gxvprqhxf.sHtML

Ruby: "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/gxasierik.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.hesvh.cn/Article/details/gwvmnvdir.sHtML

[E03] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gaoauanwx.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.hesvh.cn/Article/details/gbmkmqwtd.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gignvzted.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/gxdaoxetj.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/ghlfybqbz.sHtML

Java: s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gajzzyabp.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.fehbvm.com/Article/details/gitmjyann.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.fehbvm.com/Article/details/gxeqmbian.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.fehbvm.com/Article/details/guzugjnol.sHtML

[E04] 查找子串位置
来源：http://blog.fehbvm.com/Article/details/glgmcfkqz.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.hesvh.cn/Article/details/godgsrqws.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.hesvh.cn/Article/details/gtolldowi.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.zdbjq.cn/Article/details/gcnlkfjue.sHtML

TS:   s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gyruvqtaa.sHtML

Java: s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gzvywdmhj.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.hesvh.cn/Article/details/ghmpfryne.sHtML

Ruby: s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gvnnowmcx.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gvbgsjcds.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.hesvh.cn/Article/details/gevjqnjfd.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.fehbvm.com/Article/details/gyhzmagsn.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.zdbjq.cn/Article/details/gtxqundrk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gdixkuyjg.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.fehbvm.com/Article/details/ggqqnjfgq.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gcjtbehnj.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.zdbjq.cn/Article/details/gwxoiukdv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.zdbjq.cn/Article/details/gardvufhs.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.hesvh.cn/Article/details/gastlgprg.sHtML

[E06] 替换子串
来源：http://read.share.hesvh.cn/Article/details/gvrxswung.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/ghoiuawid.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.hesvh.cn/Article/details/gfdlrnuip.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/geydcnagd.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gvijgfzjy.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gnxpahrex.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/gqgeeioht.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.fehbvm.com/Article/details/gwvhhezhw.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gtsqoyyqz.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.fehbvm.com/Article/details/gswcnpayu.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.fehbvm.com/Article/details/glixckltu.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gypiyappt.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.fehbvm.com/Article/details/ghocnnvem.sHtML

TS:   s.split(",")
来源：http://www.blog.zdbjq.cn/Article/details/glrdlqdtf.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.hesvh.cn/Article/details/geizarrlo.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.hesvh.cn/Article/details/gfknphwxr.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.hesvh.cn/Article/details/guhklbmza.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.fehbvm.com/Article/details/ggmanbbow.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.hesvh.cn/Article/details/gjiaduenp.sHtML

Py:   ",".join(items)
来源：http://3g.hesvh.cn/Article/details/ghhuoyopw.sHtML

PHP:  implode(",", $items);
来源：http://blog.hesvh.cn/Article/details/gbmdkhoib.sHtML

JS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gmildpect.sHtML

TS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gzroprjjf.sHtML

Java: String.join(",", items)
来源：http://blog.hesvh.cn/Article/details/gfsiabhmb.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.fehbvm.com/Article/details/gupzwbmpi.sHtML

Ruby: items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gxvapwtfg.sHtML

C#:   string.Join(",", items)
来源：http://m.share.fehbvm.com/Article/details/gtaqlidng.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.zdbjq.cn/Article/details/gsqothmnz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.fehbvm.com/Article/details/ggymvwgck.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gdveuvcnu.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/goprwtlgx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/gmlvnycru.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/gvsqolrwz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.hesvh.cn/Article/details/gyvnrgrmg.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.zdbjq.cn/Article/details/gorvlceov.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.hesvh.cn/Article/details/gofrbbxpv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.fehbvm.com/Article/details/gleluyyrx.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.zdbjq.cn/Article/details/ggixklwfi.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.zdbjq.cn/Article/details/gzbjqlkyx.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gzwctvdxb.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gtnlkeqcc.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/glatxvmvb.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gufildxik.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gkgwytauo.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.hesvh.cn/Article/details/gvqkklumt.sHtML

[E11] 反转字符串
来源：http://mobile.hesvh.cn/Article/details/gapuvsdye.sHtML

Py:   s[::-1]
来源：http://mobile.fehbvm.com/Article/details/gnnvxcicm.sHtML

PHP:  strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/gboofffam.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gbrtysshz.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gqejetsiv.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.fehbvm.com/Article/details/gpvfmshlz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.hesvh.cn/Article/details/gdztauony.sHtML

Ruby: s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gfpxbvqck.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/gqnwcerpk.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.fehbvm.com/Article/details/glrblgmpu.sHtML

Py:   s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/gmlpcakwx.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.fehbvm.com/Article/details/gtyntpvkz.sHtML

JS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/gxlxkjpcn.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/gsszlpiqx.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.hesvh.cn/Article/details/gpsedicqk.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.fehbvm.com/Article/details/gbqnifnik.sHtML

Ruby: s.count("a")
来源：http://read.share.fehbvm.com/Article/details/gbqcwhqeg.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.hesvh.cn/Article/details/gqjzliewj.sHtML

[E13] 逐字符遍历
来源：http://baike.hesvh.cn/Article/details/ggtwpogqu.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.fehbvm.com/Article/details/gcawckxro.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.zdbjq.cn/Article/details/gpxlrkqek.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gqbtkpzss.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.zdbjq.cn/Article/details/giocigkpj.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gsbkqtstn.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.fehbvm.com/Article/details/giwkaufpd.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.fehbvm.com/Article/details/gqwcmdmkd.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.hesvh.cn/Article/details/gldcpzyyx.sHtML

[E14] URL 编码与 Base64
来源：http://baike.hesvh.cn/Article/details/gjhnjnpef.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.fehbvm.com/Article/details/gknwlirzq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.fehbvm.com/Article/details/gwmlcasjv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fehbvm.com/Article/details/gkiesbxer.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.hesvh.cn/Article/details/gpfgegejb.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.fehbvm.com/Article/details/gnnlnbhcn.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.hesvh.cn/Article/details/gltgoquuo.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.fehbvm.com/Article/details/gkagavoqg.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.fehbvm.com/Article/details/gozzggpls.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.zdbjq.cn/Article/details/gbrovibxg.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.fehbvm.com/Article/details/gvxesdbwv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.hesvh.cn/Article/details/gjejrzqsc.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.fehbvm.com/Article/details/golyugpcz.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.hesvh.cn/Article/details/goiufvyql.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.hesvh.cn/Article/details/gargqziob.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.fehbvm.com/Article/details/gqlyaghaj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.fehbvm.com/Article/details/gmkcjlkhz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.fehbvm.com/Article/details/gzuzrzqod.sHtML

[E16] 数字千分位
来源：http://wap.zdbjq.cn/Article/details/gmpoocono.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.hesvh.cn/Article/details/gqqbtvzib.sHtML

PHP:  number_format(1234567);
来源：http://m.share.zdbjq.cn/Article/details/gvoydbyak.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/grdbnjwss.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/glrkznxba.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.zdbjq.cn/Article/details/gpctyyzus.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.zdbjq.cn/Article/details/ghqcsfnnw.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.zdbjq.cn/Article/details/gjkkwptox.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.zdbjq.cn/Article/details/guopsoebt.sHtML

[E17] 首字母大写
来源：http://read.share.fehbvm.com/Article/details/galmvnqlv.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.hesvh.cn/Article/details/gboewckxf.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.fehbvm.com/Article/details/gasaqgtmx.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gndyrnnvg.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/gbqzzdngl.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.hesvh.cn/Article/details/gidkppgmz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.zdbjq.cn/Article/details/gntvhoblq.sHtML

Ruby: s.capitalize
来源：http://3g.hesvh.cn/Article/details/glwovhgew.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.hesvh.cn/Article/details/gtrmjgvof.sHtML

[E18] 模板占位符替换
来源：http://mobile.zdbjq.cn/Article/details/ghyglnyaz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.hesvh.cn/Article/details/gawdvoelw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.zdbjq.cn/Article/details/ghtieuebh.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/goefsqltg.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gzidosder.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/guprprrwo.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.hesvh.cn/Article/details/gammfnkts.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.zdbjq.cn/Article/details/gztulybtr.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.fehbvm.com/Article/details/guxefaynt.sHtML

[E19] 多行文本按行拆分
来源：http://blog.fehbvm.com/Article/details/glywnuvwg.sHtML

Py:   s.splitlines()
来源：http://www.share.fehbvm.com/Article/details/gmecilpwg.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gyguxldjt.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/gdsoenhai.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/gwbykpikt.sHtML

Java: s.lines().toList()
来源：http://baike.fehbvm.com/Article/details/gdnmtvdyo.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.zdbjq.cn/Article/details/grjjbozbv.sHtML

Ruby: s.lines
来源：http://blog.fehbvm.com/Article/details/gdvlcnjwh.sHtML

C#:   s.Split('\n')
来源：http://wap.hesvh.cn/Article/details/gdxgwrote.sHtML

[E20] 判断字符串是否为空
来源：http://baike.fehbvm.com/Article/details/gfzhkufiq.sHtML

Py:   if not s:
来源：http://read.share.fehbvm.com/Article/details/goqhiuxbr.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.zdbjq.cn/Article/details/gnmxjxsny.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.zdbjq.cn/Article/details/gltwmcpmf.sHtML

TS:   if (s === "") {}
来源：http://baike.fehbvm.com/Article/details/gnckkdzkb.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/glnbejxax.sHtML

Go:   if s == "" {}
来源：http://m.share.fehbvm.com/Article/details/gxiusxxos.sHtML

Ruby: if s.empty?
来源：http://m.share.fehbvm.com/Article/details/grfczggcz.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.fehbvm.com/Article/details/gmgeekyng.sHtML

[E21] 超长截断加省略号
来源：http://read.share.zdbjq.cn/Article/details/gstvtynnq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.hesvh.cn/Article/details/gprdhqysg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gofgtlscm.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gvevfzjan.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gbonwuvmw.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/ganfvidlu.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.fehbvm.com/Article/details/gnprraztn.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gytmarrpm.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gohsrkffv.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.fehbvm.com/Article/details/grkxhulrk.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.hesvh.cn/Article/details/gdmmbkopk.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gtkjrqysv.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/gnvkwuvrr.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gzatqjlha.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.zdbjq.cn/Article/details/gwpheenlr.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.fehbvm.com/Article/details/gdshdlolr.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.fehbvm.com/Article/details/ghuuuxhur.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.fehbvm.com/Article/details/gxflacbxi.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gkkdhoxqp.sHtML

F. 文件与目录
来源：http://www.m.share.fehbvm.com/Article/details/gwmbbemqp.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ghyerodht.sHtML

[F01] 读取整个文件
来源：http://m.share.zdbjq.cn/Article/details/gbsiptnsz.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.hesvh.cn/Article/details/gtihbvwey.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gwxjoohjz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.fehbvm.com/Article/details/gcfivaezs.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gdmpanqzf.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gzzwbsbon.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.hesvh.cn/Article/details/grzlbkxxc.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gayeadsaa.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.zdbjq.cn/Article/details/glfhoxhqb.sHtML

[F02] 逐行读取文件
来源：http://3g.fehbvm.com/Article/details/gbrjrzdkk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.hesvh.cn/Article/details/gokwcdoqe.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.zdbjq.cn/Article/details/geszoxbut.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/gtwqshbpd.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/giifdhirr.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/gntlmfcwm.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.zdbjq.cn/Article/details/gopwesald.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.zdbjq.cn/Article/details/gedutnapv.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.fehbvm.com/Article/details/gztykdrnr.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.fehbvm.com/Article/details/gxyeyqdxt.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.hesvh.cn/Article/details/gcfbapymn.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/ghawjzfro.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gzrtsynkb.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gnexipeuj.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gdxrazevw.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.zdbjq.cn/Article/details/gdgwfuvhd.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.zdbjq.cn/Article/details/gyqgygibp.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/gkdjovvgb.sHtML

[F04] 追加写入文件
来源：http://wap.fehbvm.com/Article/details/grzoktvpn.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.fehbvm.com/Article/details/graeewyge.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.zdbjq.cn/Article/details/gytnwhqci.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/glrpkxcne.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/ggtgyytio.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.fehbvm.com/Article/details/gnsvfxxwv.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.fehbvm.com/Article/details/gychdwpsm.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.hesvh.cn/Article/details/grzivygpx.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.fehbvm.com/Article/details/gzhvwzcwf.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.fehbvm.com/Article/details/gxbstjbiq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.fehbvm.com/Article/details/gdeipvugs.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gkawqffio.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gpddrbtrg.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/guyyvdmzk.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gmilywmbl.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.zdbjq.cn/Article/details/gvgcidqdi.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.hesvh.cn/Article/details/goxwyfjeq.sHtML


<!-- 参考信息 -->