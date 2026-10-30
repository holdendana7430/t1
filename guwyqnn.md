代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/goxdyxumb.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.fanxiaobao.xyz/Article/details/gcqkjytgz.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gudpgnqpb.sHtML

TS:   [...arr];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcsbjnwbq.sHtML

Java: new ArrayList<>(list);
来源：http://3g.fanxiaobao.xyz/Article/details/ghwqacvjx.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjguchpmn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.fanxiaobao.xyz/Article/details/gzslpevtr.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gocuvkslw.sHtML

[D23] reduce 累积计算
来源：http://3g.fanxiaobao.xyz/Article/details/gzkndgcsf.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fanxiaobao.xyz/Article/details/gzflyaegv.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.fanxiaobao.xyz/Article/details/gpvcgsaib.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjytjggy.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fanxiaobao.xyz/Article/details/gjzujliid.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.fanxiaobao.xyz/Article/details/gjkvdamtb.sHtML

Go:   // 手写循环
来源：http://baike.fanxiaobao.xyz/Article/details/grypwvlij.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.fanxiaobao.xyz/Article/details/gsmsykgfu.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.fanxiaobao.xyz/Article/details/ggkqgqlju.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geeumrfqi.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fanxiaobao.xyz/Article/details/genqhgskr.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghceuyqhg.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmkedfho.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqmamzmvd.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givophoig.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guovwbovi.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.fanxiaobao.xyz/Article/details/gtcfpnvix.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.fanxiaobao.xyz/Article/details/gfqplhwqa.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.fanxiaobao.xyz/Article/details/gowyikjuh.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvckvftz.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.fanxiaobao.xyz/Article/details/glbdganwh.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gztelrqpd.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqfeszsi.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gipevmwul.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.fanxiaobao.xyz/Article/details/gvqlghtpq.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.fanxiaobao.xyz/Article/details/goblieqzn.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbecwgpag.sHtML

[D26] 数组转字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gibzbpmxo.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqinynkge.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghoociyhu.sHtML

JS:   arr.join(", ")
来源：http://wap.fanxiaobao.xyz/Article/details/gtmkoqlms.sHtML

TS:   arr.join(", ")
来源：http://www.share.fanxiaobao.xyz/Article/details/gdcpkikdp.sHtML

Java: String.join(", ", list)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfjsaarb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.fanxiaobao.xyz/Article/details/glykbfcfq.sHtML

Ruby: arr.join(", ")
来源：http://blog.fanxiaobao.xyz/Article/details/gcfruadmo.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.fanxiaobao.xyz/Article/details/gopnszxsn.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gbnjpgsjy.sHtML

E. 字符串处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gmgczgtzm.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/grfofttjg.sHtML

[E01] 拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gevplkrma.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.fanxiaobao.xyz/Article/details/gpgwxksnj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.fanxiaobao.xyz/Article/details/gnztjqnsy.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fanxiaobao.xyz/Article/details/gdkkuuljq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fanxiaobao.xyz/Article/details/gylavdqzo.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gqjovxywv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.fanxiaobao.xyz/Article/details/ggbzevmsq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.fanxiaobao.xyz/Article/details/gzfzmmknx.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.fanxiaobao.xyz/Article/details/ghexgvqkz.sHtML

[E02] 重复字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gpyabznhc.sHtML

Py:   "ab" * 3
来源：http://mobile.fanxiaobao.xyz/Article/details/gjuoljsha.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gyptmhoqr.sHtML

JS:   "ab".repeat(3)
来源：http://wap.fanxiaobao.xyz/Article/details/gjinrirqo.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmxcwwev.sHtML

Java: "ab".repeat(3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gllhqetjc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxnqvgfx.sHtML

Ruby: "ab" * 3
来源：http://read.share.fanxiaobao.xyz/Article/details/gmgxgemli.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.fanxiaobao.xyz/Article/details/gffjypbhn.sHtML

[E03] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/gxqikobuj.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.fanxiaobao.xyz/Article/details/gymaontdy.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gycgkmkhl.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.fanxiaobao.xyz/Article/details/gsucntxkm.sHtML

TS:   s.slice(1, 4)
来源：http://blog.fanxiaobao.xyz/Article/details/ghxyklnxo.sHtML

Java: s.substring(1, 4)
来源：http://baike.fanxiaobao.xyz/Article/details/garaahysb.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.fanxiaobao.xyz/Article/details/gbfgyyxyx.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdfutttg.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpnbmfhbu.sHtML

[E04] 查找子串位置
来源：http://blog.fanxiaobao.xyz/Article/details/gsnmulmpg.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.fanxiaobao.xyz/Article/details/gfsnllxpj.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggkqwkdtq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.fanxiaobao.xyz/Article/details/gqcoxjwwa.sHtML

TS:   s.indexOf("x")
来源：http://3g.fanxiaobao.xyz/Article/details/gtswrusty.sHtML

Java: s.indexOf("x")
来源：http://read.share.fanxiaobao.xyz/Article/details/gyrwnaonf.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.fanxiaobao.xyz/Article/details/gydtickbw.sHtML

Ruby: s.index("x")
来源：http://3g.fanxiaobao.xyz/Article/details/gnagwyxzn.sHtML

C#:   s.IndexOf("x")
来源：http://blog.fanxiaobao.xyz/Article/details/ggiyxcdir.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvppuauo.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdihyyzb.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.fanxiaobao.xyz/Article/details/gtjerqlwd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gycgpiuyb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.fanxiaobao.xyz/Article/details/gzstdfmxd.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fanxiaobao.xyz/Article/details/gdyzdqfnv.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.fanxiaobao.xyz/Article/details/gvysgrvum.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.fanxiaobao.xyz/Article/details/grvaprfef.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.fanxiaobao.xyz/Article/details/ggeriywsi.sHtML

[E06] 替换子串
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbexzobx.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnqnmdjz.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzmdrtwi.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpfvtssfi.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgeclzla.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzpnczoln.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmwpdtweh.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/gecpkdxca.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.fanxiaobao.xyz/Article/details/gtiykqjfe.sHtML

[E07] 按分隔符拆分
来源：http://read.share.fanxiaobao.xyz/Article/details/gvamwdiah.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.fanxiaobao.xyz/Article/details/gcxfcztbn.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.fanxiaobao.xyz/Article/details/gthbezafi.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyoahgtoq.sHtML

TS:   s.split(",")
来源：http://baike.fanxiaobao.xyz/Article/details/gpzviwlnw.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gnthmtasn.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjtkphsc.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.fanxiaobao.xyz/Article/details/gxugwmnbq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghcdvuqre.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxxnvkec.sHtML

Py:   ",".join(items)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbddfwjs.sHtML

PHP:  implode(",", $items);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgfyiuee.sHtML

JS:   items.join(",")
来源：http://wap.fanxiaobao.xyz/Article/details/gqoeqcyop.sHtML

TS:   items.join(",")
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxblrsml.sHtML

Java: String.join(",", items)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgayfzzr.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.fanxiaobao.xyz/Article/details/gyhuzgclh.sHtML

Ruby: items.join(",")
来源：http://3g.fanxiaobao.xyz/Article/details/gwnxcirzk.sHtML

C#:   string.Join(",", items)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbitxqvm.sHtML

[E09] 去除所有空白字符
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfhtdhst.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.fanxiaobao.xyz/Article/details/gdzmxshrf.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.fanxiaobao.xyz/Article/details/gfsuhioib.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.fanxiaobao.xyz/Article/details/gfnwttgvp.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.fanxiaobao.xyz/Article/details/gtacdhgge.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gastteomy.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.fanxiaobao.xyz/Article/details/gqcqobzri.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.fanxiaobao.xyz/Article/details/gwovqzqjb.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjdnomrh.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjesxbix.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.fanxiaobao.xyz/Article/details/gfiormblt.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzcbyynl.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.fanxiaobao.xyz/Article/details/gygguxavv.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkqbgbge.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgtwccxu.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.fanxiaobao.xyz/Article/details/gbnoapkzg.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmtitdzk.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.fanxiaobao.xyz/Article/details/glsrzboys.sHtML

[E11] 反转字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzsodugpj.sHtML

Py:   s[::-1]
来源：http://read.share.fanxiaobao.xyz/Article/details/glchanvph.sHtML

PHP:  strrev($s);
来源：http://baike.fanxiaobao.xyz/Article/details/giaukxaoz.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.fanxiaobao.xyz/Article/details/gkglyoalt.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.fanxiaobao.xyz/Article/details/gqlrqxlyj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.fanxiaobao.xyz/Article/details/gklkowsvh.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyypqvxbs.sHtML

Ruby: s.reverse
来源：http://3g.fanxiaobao.xyz/Article/details/grvobkzvs.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.fanxiaobao.xyz/Article/details/gjnmpewfq.sHtML

[E12] 统计某字符出现次数
来源：http://blog.fanxiaobao.xyz/Article/details/glwmwfnle.sHtML

Py:   s.count("a")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbyovrhf.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdgahvud.sHtML

JS:   s.split("a").length - 1
来源：http://3g.fanxiaobao.xyz/Article/details/gfhpqyjah.sHtML

TS:   s.split("a").length - 1
来源：http://wap.fanxiaobao.xyz/Article/details/gjsqurtzg.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.fanxiaobao.xyz/Article/details/glwyyqyxh.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmlaqlar.sHtML

Ruby: s.count("a")
来源：http://www.share.fanxiaobao.xyz/Article/details/gpwxaqgif.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glczoakww.sHtML

[E13] 逐字符遍历
来源：http://wap.fanxiaobao.xyz/Article/details/godmtojzs.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.fanxiaobao.xyz/Article/details/glxkdfbsq.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggelgeohr.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwtrjdzen.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkduwsjno.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.fanxiaobao.xyz/Article/details/gcrpmtptm.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gsgsofsrt.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.fanxiaobao.xyz/Article/details/ghesjclum.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjwdtnqo.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubeuuxli.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqnnbkwsx.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqncyyeu.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.fanxiaobao.xyz/Article/details/golzhyack.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpsyodost.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmszqnkz.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqmyjwap.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.fanxiaobao.xyz/Article/details/gvlqmgnky.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.fanxiaobao.xyz/Article/details/gamktibry.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.fanxiaobao.xyz/Article/details/ggrizbohq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.fanxiaobao.xyz/Article/details/giykbplty.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzpkklrzm.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gmlbtlpnx.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gwlafxhkg.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.fanxiaobao.xyz/Article/details/goyipivem.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlbfnbwq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/grflyrxzu.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gsjdbebja.sHtML

[E16] 数字千分位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwqmklua.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbocoebpx.sHtML

PHP:  number_format(1234567);
来源：http://m.share.fanxiaobao.xyz/Article/details/griryycyw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggibwoayy.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fanxiaobao.xyz/Article/details/gyeukuuki.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqdsgtwjm.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.fanxiaobao.xyz/Article/details/goevoqhxc.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekeqnvrt.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfylapls.sHtML

[E17] 首字母大写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnyurmgaf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbmxlzlu.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.fanxiaobao.xyz/Article/details/ggfzkewtb.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gppjvziji.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gawdjqylm.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzbyrdzqa.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjrhqlvow.sHtML

Ruby: s.capitalize
来源：http://3g.fanxiaobao.xyz/Article/details/guldzcxfn.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.fanxiaobao.xyz/Article/details/guyqfjvbx.sHtML

[E18] 模板占位符替换
来源：http://baike.fanxiaobao.xyz/Article/details/gindydtxr.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.fanxiaobao.xyz/Article/details/gfrocnnld.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.fanxiaobao.xyz/Article/details/glsnhaodu.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.fanxiaobao.xyz/Article/details/gysmpdjwc.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghlsvlmdt.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjapzont.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.fanxiaobao.xyz/Article/details/gedyltjjx.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.fanxiaobao.xyz/Article/details/gkefbolno.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.fanxiaobao.xyz/Article/details/gbwuobufr.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwcvgkgk.sHtML

Py:   s.splitlines()
来源：http://m.share.fanxiaobao.xyz/Article/details/gbiephjlg.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.fanxiaobao.xyz/Article/details/gepiztaqv.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.fanxiaobao.xyz/Article/details/gchzgmuac.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.fanxiaobao.xyz/Article/details/gaghfrzwm.sHtML

Java: s.lines().toList()
来源：http://wap.fanxiaobao.xyz/Article/details/gkvebmerf.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxwiperq.sHtML

Ruby: s.lines
来源：http://m.share.fanxiaobao.xyz/Article/details/gndncfqqn.sHtML

C#:   s.Split('\n')
来源：http://www.share.fanxiaobao.xyz/Article/details/gzgxzogbi.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.fanxiaobao.xyz/Article/details/goyvqueht.sHtML

Py:   if not s:
来源：http://wap.fanxiaobao.xyz/Article/details/gxwtwdztf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.fanxiaobao.xyz/Article/details/gvgwrvlbc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gueougxqj.sHtML

TS:   if (s === "") {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gvygfjcjy.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvpnlvcd.sHtML

Go:   if s == "" {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzfaxzhl.sHtML

Ruby: if s.empty?
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxgzfeyh.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gqbtfvjsy.sHtML

[E21] 超长截断加省略号
来源：http://3g.fanxiaobao.xyz/Article/details/gcuoqsizw.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.fanxiaobao.xyz/Article/details/goropspzd.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.fanxiaobao.xyz/Article/details/gayukrxal.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fanxiaobao.xyz/Article/details/gshanvqta.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fanxiaobao.xyz/Article/details/gehxxlkpa.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.fanxiaobao.xyz/Article/details/gprcwyotx.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvmsdiqj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxloldjn.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.fanxiaobao.xyz/Article/details/gxmndvlxw.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwfzntvcy.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.fanxiaobao.xyz/Article/details/ghxahyklw.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fanxiaobao.xyz/Article/details/gpzgceqda.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fanxiaobao.xyz/Article/details/ghmrbmpqk.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfshevfgj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.fanxiaobao.xyz/Article/details/gnvftzwap.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzqzlthi.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.fanxiaobao.xyz/Article/details/gkoxlziws.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.fanxiaobao.xyz/Article/details/gmomltrdm.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gfajlcgjb.sHtML

F. 文件与目录
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcljuzjjm.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwavfcns.sHtML

[F01] 读取整个文件
来源：http://blog.fanxiaobao.xyz/Article/details/ghyhigppd.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmlgqwwwm.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/gnoggeqgx.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvneotgjj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.fanxiaobao.xyz/Article/details/gyosokmpi.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.fanxiaobao.xyz/Article/details/gkmeikhai.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.fanxiaobao.xyz/Article/details/ggijqpzgh.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/grzvnjukd.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.fanxiaobao.xyz/Article/details/gvggwazed.sHtML

[F02] 逐行读取文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gikmlfryc.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.fanxiaobao.xyz/Article/details/gtsxxfgjd.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.fanxiaobao.xyz/Article/details/gsmepcoci.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gwdlgisap.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gvltydvvd.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.fanxiaobao.xyz/Article/details/glglkxmck.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.fanxiaobao.xyz/Article/details/grgvydnou.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.fanxiaobao.xyz/Article/details/gbxpipgdm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmfnskxs.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fanxiaobao.xyz/Article/details/gdseeblwk.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmqyttls.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/gwdewewia.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgcedayx.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fanxiaobao.xyz/Article/details/gzwsgfknu.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.fanxiaobao.xyz/Article/details/gwqbspuem.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvengbkr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.fanxiaobao.xyz/Article/details/gouqhjrgc.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmttcemi.sHtML

[F04] 追加写入文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwzlqfos.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.fanxiaobao.xyz/Article/details/gpzxjxpvb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgrhtnfi.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqnhjjsb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fanxiaobao.xyz/Article/details/ghgpxrikh.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.fanxiaobao.xyz/Article/details/gmzrkwluh.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzebwnvxn.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpnyrqqn.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.fanxiaobao.xyz/Article/details/gucaqppvo.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gsitvtcgh.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.fanxiaobao.xyz/Article/details/gjubixqen.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/gjdsedlnt.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gjiygkygf.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gqrajazrp.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.fanxiaobao.xyz/Article/details/gciitfryg.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfijivxwv.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gxabmqzjq.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gznrrmgot.sHtML

[F06] 删除文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbcmvnae.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gxuguivla.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaysardzz.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gvlekdmro.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwhqwuyh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.fanxiaobao.xyz/Article/details/gfvhndxsq.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/ggeszwskl.sHtML


<!-- 参考信息 -->