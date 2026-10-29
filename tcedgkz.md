代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.hesvh.cn/Article/details/gltseyano.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.zdbjq.cn/Article/details/gfwlqgkai.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gllqjuwhv.sHtML

TS:   [...arr];
来源：http://www.blog.zdbjq.cn/Article/details/geuekpiku.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gfzattpik.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.fehbvm.com/Article/details/gktaizikn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.hesvh.cn/Article/details/gtclanwxc.sHtML

C#:   new List<int>(list);
来源：http://read.share.hesvh.cn/Article/details/gxuvfnvze.sHtML

[D23] reduce 累积计算
来源：http://wap.hesvh.cn/Article/details/gwuxzlpnh.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.hesvh.cn/Article/details/gjtbewqdg.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.zdbjq.cn/Article/details/gvhjrucfv.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/gtnjqniew.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/glfkagtsw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.hesvh.cn/Article/details/gmpomolax.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/gpnegikbt.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.zdbjq.cn/Article/details/gnrvckdva.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.zdbjq.cn/Article/details/gajecgxss.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.fehbvm.com/Article/details/gpjdrgcae.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fehbvm.com/Article/details/gvvzpkcsq.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.zdbjq.cn/Article/details/gubzkvdqv.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.hesvh.cn/Article/details/gyevxwprc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.fehbvm.com/Article/details/gfstthzke.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.fehbvm.com/Article/details/gcmphbcqj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.hesvh.cn/Article/details/gjivradef.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.fehbvm.com/Article/details/gvnyavazh.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.zdbjq.cn/Article/details/gxurcbcev.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.hesvh.cn/Article/details/gmrpasznv.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.hesvh.cn/Article/details/gvgrtzvfk.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.zdbjq.cn/Article/details/gaufkzzrg.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.fehbvm.com/Article/details/gneudlpqq.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.zdbjq.cn/Article/details/gorglqwfi.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.fehbvm.com/Article/details/gykaikrbd.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.hesvh.cn/Article/details/gkwyayugo.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.zdbjq.cn/Article/details/gqxlkiair.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.zdbjq.cn/Article/details/gatfpnrgg.sHtML

[D26] 数组转字符串
来源：http://baike.hesvh.cn/Article/details/gbiuvjxzx.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.hesvh.cn/Article/details/gjuxvfprc.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.hesvh.cn/Article/details/gphjrpdrq.sHtML

JS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gqxlbsyhv.sHtML

TS:   arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/ggutmqivf.sHtML

Java: String.join(", ", list)
来源：http://3g.hesvh.cn/Article/details/gbtcdtbed.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.zdbjq.cn/Article/details/gfdznvnnu.sHtML

Ruby: arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gmwcmkdbf.sHtML

C#:   string.Join(", ", list)
来源：http://3g.fehbvm.com/Article/details/griprnvyi.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/glvbaixbm.sHtML

E. 字符串处理
来源：http://mobile.hesvh.cn/Article/details/gerpnzqvj.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gsacxgaoz.sHtML

[E01] 拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gwikaiakw.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.zdbjq.cn/Article/details/gwvjumhxn.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.zdbjq.cn/Article/details/gjzmgrstz.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gyghzhtub.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/grxlfcjmh.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.fehbvm.com/Article/details/gihvlgars.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.hesvh.cn/Article/details/gxqjgxmof.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.fehbvm.com/Article/details/ggqlsmzno.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.fehbvm.com/Article/details/gtklkwaxl.sHtML

[E02] 重复字符串
来源：http://baike.fehbvm.com/Article/details/geifypato.sHtML

Py:   "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/geqbanhgm.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.zdbjq.cn/Article/details/gwdpanjqo.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gtkvjkqwt.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gmulfxurf.sHtML

Java: "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gqpycvypm.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.fehbvm.com/Article/details/glbytphiv.sHtML

Ruby: "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/gzgyyeiad.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.zdbjq.cn/Article/details/gqpmhbkiy.sHtML

[E03] 截取子串
来源：http://blog.zdbjq.cn/Article/details/gdnxcwubg.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.hesvh.cn/Article/details/gehuifzab.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gsocebtdi.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.fehbvm.com/Article/details/gjwymcgrt.sHtML

TS:   s.slice(1, 4)
来源：http://blog.hesvh.cn/Article/details/gqrsodvpb.sHtML

Java: s.substring(1, 4)
来源：http://wap.hesvh.cn/Article/details/grqndtdbn.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.fehbvm.com/Article/details/gzfshrqqt.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.fehbvm.com/Article/details/gkagfbtgw.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.fehbvm.com/Article/details/grufymowd.sHtML

[E04] 查找子串位置
来源：http://m.share.hesvh.cn/Article/details/giibjdclc.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.zdbjq.cn/Article/details/gnyklljmq.sHtML

PHP:  strpos($s, "x");
来源：http://wap.hesvh.cn/Article/details/glsdfugcd.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.zdbjq.cn/Article/details/gydrmyeip.sHtML

TS:   s.indexOf("x")
来源：http://3g.fehbvm.com/Article/details/gcpyfmknu.sHtML

Java: s.indexOf("x")
来源：http://m.share.hesvh.cn/Article/details/groylzmjr.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.fehbvm.com/Article/details/ghommxvom.sHtML

Ruby: s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/gudglhphc.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gauwjioww.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.fehbvm.com/Article/details/gcxwyttqk.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.fehbvm.com/Article/details/gvftqqzgq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.zdbjq.cn/Article/details/gwlwteahj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gsdscnuwa.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.hesvh.cn/Article/details/gzguxidup.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gktrxqvfj.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.hesvh.cn/Article/details/gxvvmolnx.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.hesvh.cn/Article/details/glbkimoms.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.hesvh.cn/Article/details/gptgbxhvs.sHtML

[E06] 替换子串
来源：http://blog.hesvh.cn/Article/details/gmlvqziiw.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/gksmwgroe.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.fehbvm.com/Article/details/gqdeavnob.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gkrpopyym.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gztnfnven.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gfccsixno.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/gmukvgpyj.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/guuhuxwfi.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fehbvm.com/Article/details/gpnivbqir.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.fehbvm.com/Article/details/gwoeisshk.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.hesvh.cn/Article/details/gszvuhghz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gmyjncbsf.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.hesvh.cn/Article/details/glsfcoynt.sHtML

TS:   s.split(",")
来源：http://read.share.fehbvm.com/Article/details/gmjygylfy.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.hesvh.cn/Article/details/gvewryfya.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.zdbjq.cn/Article/details/gxforwjlp.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.hesvh.cn/Article/details/garhdmmav.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.zdbjq.cn/Article/details/genciaqmb.sHtML

[E08] 数组按分隔符合并
来源：http://3g.hesvh.cn/Article/details/grykhqflm.sHtML

Py:   ",".join(items)
来源：http://read.share.zdbjq.cn/Article/details/ghfbgsuyp.sHtML

PHP:  implode(",", $items);
来源：http://www.share.zdbjq.cn/Article/details/ghdiovihh.sHtML

JS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/gffgnfrel.sHtML

TS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/ggxtilgmt.sHtML

Java: String.join(",", items)
来源：http://m.share.fehbvm.com/Article/details/gjeriyjtu.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.fehbvm.com/Article/details/gvwdxfynx.sHtML

Ruby: items.join(",")
来源：http://baike.fehbvm.com/Article/details/gqspxvzzw.sHtML

C#:   string.Join(",", items)
来源：http://3g.hesvh.cn/Article/details/gimlvnwrj.sHtML

[E09] 去除所有空白字符
来源：http://blog.hesvh.cn/Article/details/gxhpwkioa.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.fehbvm.com/Article/details/gupzcavmi.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gooipakkd.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.zdbjq.cn/Article/details/gonbknkty.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/gzceqfxcs.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gdcufdzkd.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.hesvh.cn/Article/details/grdqyexvx.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.fehbvm.com/Article/details/gcvyethxz.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gcxvqgmat.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.hesvh.cn/Article/details/gykhlhukr.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gziqtunrn.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fehbvm.com/Article/details/gjludkpcx.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/giytvhlyk.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gifxceyte.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gftdoaoot.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gviohsboe.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gndswxuhw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.hesvh.cn/Article/details/gvyplecoq.sHtML

[E11] 反转字符串
来源：http://read.share.zdbjq.cn/Article/details/gtdwxjkcr.sHtML

Py:   s[::-1]
来源：http://wap.fehbvm.com/Article/details/gbtvcdomv.sHtML

PHP:  strrev($s);
来源：http://wap.hesvh.cn/Article/details/gdabkoegr.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gacjsqivm.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gqmtkylts.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.hesvh.cn/Article/details/ggjaegoaq.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.zdbjq.cn/Article/details/gdugofvut.sHtML

Ruby: s.reverse
来源：http://blog.hesvh.cn/Article/details/guotgacjh.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/gsymfbxfr.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.zdbjq.cn/Article/details/gjkgjvwam.sHtML

Py:   s.count("a")
来源：http://wap.hesvh.cn/Article/details/gbgkgvupg.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.zdbjq.cn/Article/details/gefrnhwyv.sHtML

JS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gsnkuyucp.sHtML

TS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/gvrcoffyu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.hesvh.cn/Article/details/gfjlespzc.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.zdbjq.cn/Article/details/gcmusfrwe.sHtML

Ruby: s.count("a")
来源：http://www.share.hesvh.cn/Article/details/gxiqihdqf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.fehbvm.com/Article/details/gomdpvhmz.sHtML

[E13] 逐字符遍历
来源：http://blog.hesvh.cn/Article/details/gjkcvlfzy.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.zdbjq.cn/Article/details/ggdiqznai.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.zdbjq.cn/Article/details/gfhamjbxz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gkuthewhq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.hesvh.cn/Article/details/ggmnvnftu.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.hesvh.cn/Article/details/gdsjwuuld.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.fehbvm.com/Article/details/gzrythwfp.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.zdbjq.cn/Article/details/ghwlzcojs.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.hesvh.cn/Article/details/gwvvvakhb.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.hesvh.cn/Article/details/gqtyjegod.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.fehbvm.com/Article/details/gsguteulo.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.hesvh.cn/Article/details/gndfkrwvv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.zdbjq.cn/Article/details/gbravmqxo.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.fehbvm.com/Article/details/gyxhzrhgc.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.hesvh.cn/Article/details/gieaanyah.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.hesvh.cn/Article/details/gjzgpafnt.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.zdbjq.cn/Article/details/gtczmwecb.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.fehbvm.com/Article/details/goyfvugyb.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.hesvh.cn/Article/details/gsufoqywc.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.hesvh.cn/Article/details/gxtiiuimo.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.hesvh.cn/Article/details/gctifddxm.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gkrinknmv.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.fehbvm.com/Article/details/gcgjofmul.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.hesvh.cn/Article/details/gcbuljply.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.hesvh.cn/Article/details/grglpgtju.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.fehbvm.com/Article/details/gztzuxphg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.zdbjq.cn/Article/details/gazvgtxzn.sHtML

[E16] 数字千分位
来源：http://baike.fehbvm.com/Article/details/gbhcvasle.sHtML

Py:   f"{1234567:,}"
来源：http://blog.fehbvm.com/Article/details/gelrqjlid.sHtML

PHP:  number_format(1234567);
来源：http://3g.hesvh.cn/Article/details/gwpnzvyxt.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/gzlcbudjm.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.zdbjq.cn/Article/details/gvxaaamwi.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.hesvh.cn/Article/details/gufvlwclw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.fehbvm.com/Article/details/gjawyxlkz.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.hesvh.cn/Article/details/gxslctole.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.zdbjq.cn/Article/details/gyfjnfwqs.sHtML

[E17] 首字母大写
来源：http://baike.zdbjq.cn/Article/details/gcgwyvvbk.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.fehbvm.com/Article/details/gyolgqxwe.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.zdbjq.cn/Article/details/gygcfzyte.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/gsyszquig.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/gvtitbzyr.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.zdbjq.cn/Article/details/gqhmarqab.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gmbmyvfhp.sHtML

Ruby: s.capitalize
来源：http://m.share.hesvh.cn/Article/details/gxvmqxhtc.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.fehbvm.com/Article/details/gpogeuemo.sHtML

[E18] 模板占位符替换
来源：http://www.blog.zdbjq.cn/Article/details/gqzalnkzi.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.hesvh.cn/Article/details/gyhicixhj.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.fehbvm.com/Article/details/guhxktlui.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gcprgoqwe.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gusegcohx.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gvpdpdipo.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.zdbjq.cn/Article/details/ggguhunzs.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.zdbjq.cn/Article/details/gcfqplhkw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.hesvh.cn/Article/details/ghtinitix.sHtML

[E19] 多行文本按行拆分
来源：http://blog.zdbjq.cn/Article/details/gzapweakk.sHtML

Py:   s.splitlines()
来源：http://read.share.zdbjq.cn/Article/details/gggzrppkr.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.hesvh.cn/Article/details/gjgkurwgr.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/gwqwbmsts.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.fehbvm.com/Article/details/goskjgxkg.sHtML

Java: s.lines().toList()
来源：http://mobile.hesvh.cn/Article/details/gjsbwfnco.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.fehbvm.com/Article/details/gmdpcexjk.sHtML

Ruby: s.lines
来源：http://www.m.share.hesvh.cn/Article/details/gqoogwkty.sHtML

C#:   s.Split('\n')
来源：http://www.blog.fehbvm.com/Article/details/gnnyjaqrj.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.hesvh.cn/Article/details/ggtxvdarb.sHtML

Py:   if not s:
来源：http://mobile.fehbvm.com/Article/details/ggpnfpbiu.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.hesvh.cn/Article/details/gnydpmvip.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.zdbjq.cn/Article/details/ggnilprby.sHtML

TS:   if (s === "") {}
来源：http://3g.hesvh.cn/Article/details/gywttdhew.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gbgsiilmm.sHtML

Go:   if s == "" {}
来源：http://mobile.fehbvm.com/Article/details/ggbxhgehd.sHtML

Ruby: if s.empty?
来源：http://www.share.zdbjq.cn/Article/details/gnczfglzk.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.fehbvm.com/Article/details/grvgyxjwu.sHtML

[E21] 超长截断加省略号
来源：http://3g.hesvh.cn/Article/details/gfdbuwwzu.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.zdbjq.cn/Article/details/gfmbymqle.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gjetpuqic.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gmjlwhdfm.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gqdbwhanm.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gbfdvflsl.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.fehbvm.com/Article/details/gefufovvo.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gyqdbcxps.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gxagrtsap.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.fehbvm.com/Article/details/gqunucaxx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.hesvh.cn/Article/details/gefvnnowc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gbwbqcbvf.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gxkxevfpk.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gsnitopsy.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.zdbjq.cn/Article/details/guwgzfqge.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.zdbjq.cn/Article/details/ggwvbnifs.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.hesvh.cn/Article/details/gampchejz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/ggjitvpqf.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/giiqaqgdx.sHtML

F. 文件与目录
来源：http://read.share.hesvh.cn/Article/details/glcgehrpy.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gonhhgupb.sHtML

[F01] 读取整个文件
来源：http://www.m.share.fehbvm.com/Article/details/gqajrqeyn.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.zdbjq.cn/Article/details/gfonzgjqz.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gfuvralni.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.zdbjq.cn/Article/details/guqitptbv.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/guenmyqay.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gstiflfev.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.zdbjq.cn/Article/details/gmsmhcnrp.sHtML

Ruby: File.read("a.txt")
来源：http://blog.fehbvm.com/Article/details/gvmoasdpx.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.hesvh.cn/Article/details/gadqpzjyz.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.zdbjq.cn/Article/details/gkbjcebsi.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.hesvh.cn/Article/details/gjhywwvwd.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.hesvh.cn/Article/details/glnbfnefp.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/gnsdnhmlb.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gzdtqtzjz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gdcbsgtkj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fehbvm.com/Article/details/gshdeixmp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.hesvh.cn/Article/details/gdpbtpldy.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.hesvh.cn/Article/details/gfgapohyf.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.hesvh.cn/Article/details/gbiocresw.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.hesvh.cn/Article/details/gnnwahufy.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/gneehngxc.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/glqmgiaqp.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gukptoawa.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.fehbvm.com/Article/details/gyrkdowak.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.fehbvm.com/Article/details/ggqowwgkw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.fehbvm.com/Article/details/gihntovdx.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gmtpgptcq.sHtML

[F04] 追加写入文件
来源：http://blog.hesvh.cn/Article/details/gxpemygwl.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.fehbvm.com/Article/details/gunuwrjbl.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.fehbvm.com/Article/details/grvzrfnyw.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/grcszfwiw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gokpplxja.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.fehbvm.com/Article/details/gjkezhyjh.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fehbvm.com/Article/details/gteispkoe.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.zdbjq.cn/Article/details/gwpqitsbr.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.fehbvm.com/Article/details/gdcwvbtwq.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.zdbjq.cn/Article/details/gldunpuca.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.zdbjq.cn/Article/details/gzthtgwvj.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gugewskda.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gmbauqyal.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gnulsfflp.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gzxcngivy.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.fehbvm.com/Article/details/goypzkdwf.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gussylzsw.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gxdnwbgup.sHtML

[F06] 删除文件
来源：http://m.share.hesvh.cn/Article/details/gcoekotnw.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/ggdvtgzcg.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/guqljimrq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ggxwpavqg.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/grzxkfncl.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/ggoottlae.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gpolmfkja.sHtML


<!-- 参考信息 -->