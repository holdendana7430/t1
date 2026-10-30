代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.hesvh.cn/Article/details/gmjrjtyti.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.zdbjq.cn/Article/details/gixwelcia.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.zdbjq.cn/Article/details/gbtqyjqqc.sHtML

TS:   [...arr];
来源：http://blog.zdbjq.cn/Article/details/glxszeksv.sHtML

Java: new ArrayList<>(list);
来源：http://blog.fehbvm.com/Article/details/gtqsvidil.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.hesvh.cn/Article/details/gvcpwcgpq.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.zdbjq.cn/Article/details/gylmtpacr.sHtML

C#:   new List<int>(list);
来源：http://read.share.fehbvm.com/Article/details/galuskqet.sHtML

[D23] reduce 累积计算
来源：http://www.blog.hesvh.cn/Article/details/gjglnvzgk.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.zdbjq.cn/Article/details/gbwgxwzfh.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.zdbjq.cn/Article/details/gmqexjium.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gccjroakp.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gxzujqovt.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.fehbvm.com/Article/details/gsczjrbgi.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gsktweyfg.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.zdbjq.cn/Article/details/gpvavamxm.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.zdbjq.cn/Article/details/gkvboljuc.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.zdbjq.cn/Article/details/goumormni.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.hesvh.cn/Article/details/gspmfqheu.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fehbvm.com/Article/details/gadpdtpug.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.hesvh.cn/Article/details/ganygzmar.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gmzvzryrk.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.zdbjq.cn/Article/details/gvownorhe.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.fehbvm.com/Article/details/gowfuptsd.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.hesvh.cn/Article/details/gzzsfuuxb.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.zdbjq.cn/Article/details/gymtbruko.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.fehbvm.com/Article/details/gzijddxkd.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.zdbjq.cn/Article/details/gibgdatcx.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.zdbjq.cn/Article/details/gayhfhbwd.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.zdbjq.cn/Article/details/gjdzsqnjc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.hesvh.cn/Article/details/gzaixjczu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gsmsoyztj.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.zdbjq.cn/Article/details/guxnzalos.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.hesvh.cn/Article/details/gykpntjmf.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.fehbvm.com/Article/details/geppnfzjd.sHtML

[D26] 数组转字符串
来源：http://www.share.fehbvm.com/Article/details/gwrhpwcxi.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.zdbjq.cn/Article/details/gkdexsntb.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.hesvh.cn/Article/details/grmqpansm.sHtML

JS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gwkjaopcz.sHtML

TS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/goytwyqnu.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/gvhijeknp.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.hesvh.cn/Article/details/geomslbue.sHtML

Ruby: arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gbpindmky.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/gxlemyphf.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gpvkkzvey.sHtML

E. 字符串处理
来源：http://3g.zdbjq.cn/Article/details/gwangaebf.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gzagtiofs.sHtML

[E01] 拼接字符串
来源：http://blog.fehbvm.com/Article/details/grujgxnie.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.zdbjq.cn/Article/details/glqehesli.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.hesvh.cn/Article/details/gfyjpqqwj.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/gmoixzwxf.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gwssgrija.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.fehbvm.com/Article/details/gtbuhdwuv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.zdbjq.cn/Article/details/gphmyalkw.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.zdbjq.cn/Article/details/gdcrkvxpe.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.hesvh.cn/Article/details/gvlbgeyga.sHtML

[E02] 重复字符串
来源：http://wap.hesvh.cn/Article/details/gkqxgbspg.sHtML

Py:   "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gxulgxpfh.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.hesvh.cn/Article/details/grupbewwt.sHtML

JS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gbjhsqtye.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gcmtfypig.sHtML

Java: "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gktsspsuh.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.hesvh.cn/Article/details/gljqgvryx.sHtML

Ruby: "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/ggoidxwux.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.zdbjq.cn/Article/details/gbjsukuhb.sHtML

[E03] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/guldpemtv.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.hesvh.cn/Article/details/galmyrnfv.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gnscaobux.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/ghixrynll.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gitfujxup.sHtML

Java: s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/gfxzudtmv.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.fehbvm.com/Article/details/gvymecnxx.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.zdbjq.cn/Article/details/gasxstxjo.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.hesvh.cn/Article/details/gsqihebqs.sHtML

[E04] 查找子串位置
来源：http://www.blog.zdbjq.cn/Article/details/gucbhgfxx.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/gkncztyun.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.hesvh.cn/Article/details/gfttadbma.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.zdbjq.cn/Article/details/gkmapvvfk.sHtML

TS:   s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gbonmfvna.sHtML

Java: s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gyvbsdzor.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.hesvh.cn/Article/details/grshtuobx.sHtML

Ruby: s.index("x")
来源：http://blog.fehbvm.com/Article/details/gefxqftph.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/grsozwsmm.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.hesvh.cn/Article/details/gefhdttok.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.hesvh.cn/Article/details/godiwawuu.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.zdbjq.cn/Article/details/ghgizzfqt.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/giqzcazxi.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.zdbjq.cn/Article/details/guhxyakxg.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gtrzpublg.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.zdbjq.cn/Article/details/gjnhirtzk.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.fehbvm.com/Article/details/gzuyfbftv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gjvyexics.sHtML

[E06] 替换子串
来源：http://m.share.fehbvm.com/Article/details/gnpyvdlos.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gxmujgmiq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.fehbvm.com/Article/details/gqbwrgznv.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gwugpurly.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/giaoqdmlt.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gimdxjolw.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/glgsoxhzg.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.fehbvm.com/Article/details/gsvxuenyk.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.hesvh.cn/Article/details/gvegdwwcz.sHtML

[E07] 按分隔符拆分
来源：http://read.share.zdbjq.cn/Article/details/gtpexfipt.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.fehbvm.com/Article/details/gorxnkpqg.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.fehbvm.com/Article/details/gaflugiua.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.hesvh.cn/Article/details/gtlhfgttq.sHtML

TS:   s.split(",")
来源：http://read.share.hesvh.cn/Article/details/goilrbmzq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.hesvh.cn/Article/details/ghlxiggon.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.fehbvm.com/Article/details/gsgehweqn.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.fehbvm.com/Article/details/ghyjprswm.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.zdbjq.cn/Article/details/gfgauwvhk.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.hesvh.cn/Article/details/ghwumsrqt.sHtML

Py:   ",".join(items)
来源：http://www.m.share.hesvh.cn/Article/details/gallvxcrn.sHtML

PHP:  implode(",", $items);
来源：http://read.share.zdbjq.cn/Article/details/gdtwnpewv.sHtML

JS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/giayzgbbs.sHtML

TS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/gpzwdyvna.sHtML

Java: String.join(",", items)
来源：http://wap.fehbvm.com/Article/details/galqkywye.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.hesvh.cn/Article/details/gfkmxejmx.sHtML

Ruby: items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gscxbwbvv.sHtML

C#:   string.Join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/gotomsnvv.sHtML

[E09] 去除所有空白字符
来源：http://3g.fehbvm.com/Article/details/gqqwakckn.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.hesvh.cn/Article/details/ggujjvrza.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.hesvh.cn/Article/details/grhakicgu.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/gdmhrfmxo.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/gbtgzrnic.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gclcalesm.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.zdbjq.cn/Article/details/gkrlvkcyx.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.fehbvm.com/Article/details/gxojhtxco.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/gmutaftqy.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.zdbjq.cn/Article/details/gkojurggj.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gxmqozurt.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.fehbvm.com/Article/details/gcerwojev.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gurgdpcyz.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gwtfrnfan.sHtML

Java: String.format("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gmjmkhlon.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/geedxylln.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gwdmsqmkw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.zdbjq.cn/Article/details/glqlzdnti.sHtML

[E11] 反转字符串
来源：http://mobile.fehbvm.com/Article/details/gmfftqtvc.sHtML

Py:   s[::-1]
来源：http://3g.hesvh.cn/Article/details/gjqckknzu.sHtML

PHP:  strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/gktxtxhxo.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gfczhnyzz.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gdlwqrwuj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.zdbjq.cn/Article/details/gqxwupboj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fehbvm.com/Article/details/gcejwmros.sHtML

Ruby: s.reverse
来源：http://read.share.zdbjq.cn/Article/details/gpattscjn.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/ggmeewbpr.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.fehbvm.com/Article/details/geknkrfoj.sHtML

Py:   s.count("a")
来源：http://mobile.fehbvm.com/Article/details/gokpzcuiv.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.fehbvm.com/Article/details/gedssbsfj.sHtML

JS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gvppyiaeg.sHtML

TS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/geqancrvm.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.fehbvm.com/Article/details/gquphnoth.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.hesvh.cn/Article/details/gdqjljpve.sHtML

Ruby: s.count("a")
来源：http://wap.zdbjq.cn/Article/details/gbpoidcve.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.fehbvm.com/Article/details/goxiihaff.sHtML

[E13] 逐字符遍历
来源：http://m.share.fehbvm.com/Article/details/gyzlwldyx.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.fehbvm.com/Article/details/gzsofqrgn.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.fehbvm.com/Article/details/gyfgdxdqi.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gpccnyfzk.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gqgzugelj.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.fehbvm.com/Article/details/gzgxooynh.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.fehbvm.com/Article/details/giqffwpjw.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.fehbvm.com/Article/details/guxrbdshx.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.fehbvm.com/Article/details/gxwcvfnng.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.fehbvm.com/Article/details/gfsklnvgk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.hesvh.cn/Article/details/geygjfxcy.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.zdbjq.cn/Article/details/gczhgkmwz.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.hesvh.cn/Article/details/gzllzwsjt.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.fehbvm.com/Article/details/gcnetliho.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.fehbvm.com/Article/details/gicraqnwy.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.hesvh.cn/Article/details/gnbkziiga.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.fehbvm.com/Article/details/ggjrtwcop.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.hesvh.cn/Article/details/grkdhkkwh.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.hesvh.cn/Article/details/gsvdvdqoz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.fehbvm.com/Article/details/gctcygypq.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.hesvh.cn/Article/details/gsvmskrvg.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.hesvh.cn/Article/details/giwyzgsne.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.hesvh.cn/Article/details/girrqwtki.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.zdbjq.cn/Article/details/gdlufkgjs.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.zdbjq.cn/Article/details/gdoyqqxtr.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.fehbvm.com/Article/details/gujvsqnzo.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.fehbvm.com/Article/details/gtlhjndhe.sHtML

[E16] 数字千分位
来源：http://www.share.hesvh.cn/Article/details/gljaeyzav.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.zdbjq.cn/Article/details/ggpvwvwue.sHtML

PHP:  number_format(1234567);
来源：http://wap.hesvh.cn/Article/details/goyxggbpq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.zdbjq.cn/Article/details/gjpgjlshr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gaqntzhjr.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.fehbvm.com/Article/details/gokbsikux.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.zdbjq.cn/Article/details/gmyxruxye.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.fehbvm.com/Article/details/guzxguhrq.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.fehbvm.com/Article/details/gmwqvrxad.sHtML

[E17] 首字母大写
来源：http://blog.hesvh.cn/Article/details/gqwhcamlw.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.fehbvm.com/Article/details/glsmqxpeh.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.fehbvm.com/Article/details/gdenozceb.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/geegeenwv.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/gurtwawde.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.zdbjq.cn/Article/details/gnytmpjkh.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.hesvh.cn/Article/details/gkfdbtbzp.sHtML

Ruby: s.capitalize
来源：http://www.blog.hesvh.cn/Article/details/ggobujjcr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.zdbjq.cn/Article/details/gfiorltwr.sHtML

[E18] 模板占位符替换
来源：http://read.share.hesvh.cn/Article/details/gictkxtxq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.fehbvm.com/Article/details/gcwkevwuk.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.zdbjq.cn/Article/details/gmtgwbbmr.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gbcbexpne.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gcugaaezd.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/glfwxpadj.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gmvpmpdcd.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.fehbvm.com/Article/details/garrkgawk.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.zdbjq.cn/Article/details/gakaavcui.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.fehbvm.com/Article/details/gcrjizkxa.sHtML

Py:   s.splitlines()
来源：http://www.blog.zdbjq.cn/Article/details/gamohtqlp.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.fehbvm.com/Article/details/glritcqcy.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/ggprzsoma.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/gcghvekoe.sHtML

Java: s.lines().toList()
来源：http://www.blog.hesvh.cn/Article/details/gjjwimilu.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.zdbjq.cn/Article/details/ghiqrkxsy.sHtML

Ruby: s.lines
来源：http://mobile.zdbjq.cn/Article/details/gzvxfgqee.sHtML

C#:   s.Split('\n')
来源：http://m.share.fehbvm.com/Article/details/gbobqsniu.sHtML

[E20] 判断字符串是否为空
来源：http://blog.fehbvm.com/Article/details/gjgtaqmeb.sHtML

Py:   if not s:
来源：http://m.share.hesvh.cn/Article/details/gwcqevspi.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.zdbjq.cn/Article/details/guzywetqo.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.fehbvm.com/Article/details/gbesjhhee.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.zdbjq.cn/Article/details/gkoegyyhr.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gmcyvpnjb.sHtML

Go:   if s == "" {}
来源：http://3g.hesvh.cn/Article/details/gylugqhak.sHtML

Ruby: if s.empty?
来源：http://wap.fehbvm.com/Article/details/gmyfodryh.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.fehbvm.com/Article/details/ghjoaoees.sHtML

[E21] 超长截断加省略号
来源：http://www.share.fehbvm.com/Article/details/gcikxtbyw.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.zdbjq.cn/Article/details/gahkyoijq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gzyiqdnid.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gxbkjkmtm.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gjlxlvcme.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gqebfpult.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.zdbjq.cn/Article/details/gibidmmbp.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/gyzdswwhv.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gvucnsqjj.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.hesvh.cn/Article/details/gediwapzt.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.hesvh.cn/Article/details/gbokgvtfz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gcjfoaztb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.zdbjq.cn/Article/details/goewnnscr.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/ghdjlptsm.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/gxorlsbyw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.fehbvm.com/Article/details/ghpgrmvmi.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/givuylxgz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.fehbvm.com/Article/details/gjryzomrd.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gazabgiic.sHtML

F. 文件与目录
来源：http://baike.hesvh.cn/Article/details/gfjbzktha.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ghpozgkym.sHtML

[F01] 读取整个文件
来源：http://www.share.hesvh.cn/Article/details/groxjidpc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.zdbjq.cn/Article/details/gtsjrnucs.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gglgiguqz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.zdbjq.cn/Article/details/gogsxxoqt.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gzegknwwr.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gvnpwksyv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.hesvh.cn/Article/details/gwwbosutq.sHtML

Ruby: File.read("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gmjkqnskm.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.fehbvm.com/Article/details/gdyxpryij.sHtML

[F02] 逐行读取文件
来源：http://mobile.zdbjq.cn/Article/details/gclxkdgob.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.hesvh.cn/Article/details/gqwujsqtk.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.zdbjq.cn/Article/details/gauernbnd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/gxbhztbbk.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/grqsgpesi.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gqjqhwpwh.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.fehbvm.com/Article/details/gdqjrdpnx.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.hesvh.cn/Article/details/gaobpvfze.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.zdbjq.cn/Article/details/gdcsaiqik.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.fehbvm.com/Article/details/gltpizajp.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.fehbvm.com/Article/details/ghlrvggdp.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/gtclcwnri.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gcdnbzqze.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/ghxwqlgkm.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.hesvh.cn/Article/details/gwcihutbq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.zdbjq.cn/Article/details/gfjxrsdrr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.hesvh.cn/Article/details/gvulggqph.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/glqhmodvh.sHtML

[F04] 追加写入文件
来源：http://wap.fehbvm.com/Article/details/gfarnslpg.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.hesvh.cn/Article/details/gdqobmmok.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.zdbjq.cn/Article/details/gfmprzgmy.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gvddhzubk.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gvhjearka.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.hesvh.cn/Article/details/goakpmenc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gezvggjcs.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.fehbvm.com/Article/details/gougmmeeu.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.zdbjq.cn/Article/details/gcxgncmih.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.zdbjq.cn/Article/details/gzmxaadhk.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.hesvh.cn/Article/details/gznaohbzv.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gjvnxfspu.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gjrwdpurv.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gamlsunfd.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gbcifxuie.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.zdbjq.cn/Article/details/glwibtynd.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.fehbvm.com/Article/details/ggwrikpjk.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.fehbvm.com/Article/details/glvsvxfjm.sHtML

[F06] 删除文件
来源：http://www.blog.hesvh.cn/Article/details/gqiaalgfy.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gspppiwhi.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gkemyzcbr.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gnrpjunzn.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gfyioriqy.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gvehamuym.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gbgwezshg.sHtML


<!-- 参考信息 -->