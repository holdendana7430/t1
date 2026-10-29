代发 wailian999

[D23] reduce 累积计算
来源：http://mobile.fehbvm.com/Article/details/gsvxbisns.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.hesvh.cn/Article/details/godfgwkud.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.hesvh.cn/Article/details/gehgqekpz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/grwmfwtvo.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gooelpdqm.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.zdbjq.cn/Article/details/gnhaxoxto.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gazbynlsv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.fehbvm.com/Article/details/gennfreei.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.zdbjq.cn/Article/details/gubqfjblu.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.zdbjq.cn/Article/details/gupwwwaqu.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gboqxzzfm.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.hesvh.cn/Article/details/gvstttscb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gtvfjndpd.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gejhtoazw.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.zdbjq.cn/Article/details/gqyjibbqf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.fehbvm.com/Article/details/gvvummmww.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.zdbjq.cn/Article/details/gzbdzxusa.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.zdbjq.cn/Article/details/gpntwsptm.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.hesvh.cn/Article/details/gcxcdscpu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.hesvh.cn/Article/details/gwvbstrwq.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.hesvh.cn/Article/details/gcqzhhjpa.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.fehbvm.com/Article/details/grgotkpid.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.fehbvm.com/Article/details/gtazdsyik.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gwntwpuva.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.fehbvm.com/Article/details/ggezsurii.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.hesvh.cn/Article/details/gpdacvpxs.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.fehbvm.com/Article/details/gkqnntthn.sHtML

[D26] 数组转字符串
来源：http://mobile.hesvh.cn/Article/details/gvlvmdjzp.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.zdbjq.cn/Article/details/gdhepimth.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.fehbvm.com/Article/details/gtwpfpszj.sHtML

JS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/ggkoeqbra.sHtML

TS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gpmfdbvpm.sHtML

Java: String.join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/gotwfvobg.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.fehbvm.com/Article/details/gltrhhynh.sHtML

Ruby: arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gjkymojwu.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gdaeolkmi.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwmscujad.sHtML

E. 字符串处理
来源：http://wap.fehbvm.com/Article/details/glldvkvpk.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/guadqfjqq.sHtML

[E01] 拼接字符串
来源：http://wap.fehbvm.com/Article/details/gttpzazoo.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.hesvh.cn/Article/details/gkoacnram.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.zdbjq.cn/Article/details/gwecbrzgd.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/gnifbivzf.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/gxjizgsqh.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.hesvh.cn/Article/details/ghqbmruaz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.fehbvm.com/Article/details/ggbboxxuj.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.zdbjq.cn/Article/details/grvgybymt.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.fehbvm.com/Article/details/gkfrecaev.sHtML

[E02] 重复字符串
来源：http://wap.zdbjq.cn/Article/details/gqdwwuxhw.sHtML

Py:   "ab" * 3
来源：http://baike.hesvh.cn/Article/details/gfojmkxkk.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.fehbvm.com/Article/details/gedvfseai.sHtML

JS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gfhvdgxoz.sHtML

TS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/ggyoeyadg.sHtML

Java: "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gelykyphc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.zdbjq.cn/Article/details/gzuyfwwzo.sHtML

Ruby: "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/gnjazbrfy.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.zdbjq.cn/Article/details/gxhrqmksw.sHtML

[E03] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/gslahkpvd.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.fehbvm.com/Article/details/gpcqmcgcm.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gbteanyas.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gykpukhkg.sHtML

TS:   s.slice(1, 4)
来源：http://blog.fehbvm.com/Article/details/gbnhlqrjd.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/galgzrocb.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/gorgxqidg.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.fehbvm.com/Article/details/ghinnowmw.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.zdbjq.cn/Article/details/gfxxgstiv.sHtML

[E04] 查找子串位置
来源：http://www.share.zdbjq.cn/Article/details/gofvxbkyi.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/govvbnbya.sHtML

PHP:  strpos($s, "x");
来源：http://wap.zdbjq.cn/Article/details/gqdpguyuz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.fehbvm.com/Article/details/gagraoaoh.sHtML

TS:   s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gxuvnkoht.sHtML

Java: s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gxuhmgtnm.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.fehbvm.com/Article/details/gcxefnbfm.sHtML

Ruby: s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/gimleytau.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.hesvh.cn/Article/details/giqkwylyt.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.fehbvm.com/Article/details/gffflyhtv.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/giqefnsrf.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.fehbvm.com/Article/details/gfwsrjzmk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gyrxkdyiu.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.hesvh.cn/Article/details/gtbbzhocw.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gqfzxigpm.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.fehbvm.com/Article/details/gnhsmitnb.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.fehbvm.com/Article/details/gdtnzmnzn.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gyfhjyhfq.sHtML

[E06] 替换子串
来源：http://www.share.zdbjq.cn/Article/details/gfbmwiodu.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/gklcogdud.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.hesvh.cn/Article/details/gertwkhjg.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gjfykavyy.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gvovrmpif.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/ganqslnkm.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/gygngzwkt.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gvvrykupm.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.fehbvm.com/Article/details/geijkmnjq.sHtML

[E07] 按分隔符拆分
来源：http://baike.zdbjq.cn/Article/details/grwoahcqq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.hesvh.cn/Article/details/gbuzftmlk.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.hesvh.cn/Article/details/gccoanpmy.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.fehbvm.com/Article/details/gptmiupgt.sHtML

TS:   s.split(",")
来源：http://www.blog.hesvh.cn/Article/details/gxarvjume.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.hesvh.cn/Article/details/gyacgswml.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.fehbvm.com/Article/details/galhzfodr.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.fehbvm.com/Article/details/gcktsaftn.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.fehbvm.com/Article/details/gkizmsglw.sHtML

[E08] 数组按分隔符合并
来源：http://3g.fehbvm.com/Article/details/glvdcutiq.sHtML

Py:   ",".join(items)
来源：http://www.m.share.hesvh.cn/Article/details/gpjvusxjj.sHtML

PHP:  implode(",", $items);
来源：http://baike.zdbjq.cn/Article/details/gzoegaqgx.sHtML

JS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gaiodkmjv.sHtML

TS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/gtfigunta.sHtML

Java: String.join(",", items)
来源：http://wap.hesvh.cn/Article/details/gkwseyzes.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.hesvh.cn/Article/details/gnzhiertm.sHtML

Ruby: items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gxkxioinq.sHtML

C#:   string.Join(",", items)
来源：http://mobile.hesvh.cn/Article/details/gbarpbuty.sHtML

[E09] 去除所有空白字符
来源：http://baike.fehbvm.com/Article/details/gzpncebrm.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gyvjeqxsy.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.zdbjq.cn/Article/details/gxrgqkmml.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.fehbvm.com/Article/details/gwrbtmyvm.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/gpwbermry.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/gmcchlzay.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.fehbvm.com/Article/details/gcqontrvw.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.fehbvm.com/Article/details/gnpviihwb.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.fehbvm.com/Article/details/gdeazaobj.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.fehbvm.com/Article/details/gueveoqao.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gomvaodpe.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.zdbjq.cn/Article/details/gagrfoogx.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gvahhzile.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/grhtipuyz.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gksxdfotf.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/geylmunaq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gpxfszzec.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.hesvh.cn/Article/details/gdwuseubt.sHtML

[E11] 反转字符串
来源：http://baike.zdbjq.cn/Article/details/gpeysoqus.sHtML

Py:   s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/grxnshnyh.sHtML

PHP:  strrev($s);
来源：http://www.share.hesvh.cn/Article/details/gxmovgwij.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/giyrzdnok.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gkbumqlbz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.hesvh.cn/Article/details/gabnzvfxl.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.zdbjq.cn/Article/details/gdrxixtjl.sHtML

Ruby: s.reverse
来源：http://www.share.fehbvm.com/Article/details/gyzmirxta.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gfmoespsx.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.fehbvm.com/Article/details/gbvzrmsvt.sHtML

Py:   s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gsrftviir.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.zdbjq.cn/Article/details/gbgwizric.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/gsxsrxsle.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/gzefmsojb.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.hesvh.cn/Article/details/gqgweclfd.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.hesvh.cn/Article/details/gtgrovinf.sHtML

Ruby: s.count("a")
来源：http://www.share.hesvh.cn/Article/details/gcuoevuqf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.zdbjq.cn/Article/details/gaoqvkiun.sHtML

[E13] 逐字符遍历
来源：http://3g.fehbvm.com/Article/details/gimxglvmz.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.zdbjq.cn/Article/details/gedxehakx.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.hesvh.cn/Article/details/gmgubztwe.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/gctxrcdhi.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gjpbgurgl.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gonpvqhis.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.fehbvm.com/Article/details/gobvkifyg.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.fehbvm.com/Article/details/ghzmgyzsb.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.fehbvm.com/Article/details/gxxdvkdfo.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.hesvh.cn/Article/details/gkgdgkvov.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.fehbvm.com/Article/details/gepidkbat.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.zdbjq.cn/Article/details/ghacsetlh.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.hesvh.cn/Article/details/genufxzyj.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.fehbvm.com/Article/details/gjgljepfp.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gjtuikwyi.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.fehbvm.com/Article/details/grmoefdkj.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.fehbvm.com/Article/details/gczzeorhm.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/goesvvvki.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.hesvh.cn/Article/details/gejqzzobz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.zdbjq.cn/Article/details/gcgfavbio.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.hesvh.cn/Article/details/gfgbuurwy.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.zdbjq.cn/Article/details/gccoozjvi.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.fehbvm.com/Article/details/gaxxsxyqs.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.hesvh.cn/Article/details/gxhqrngeq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/ggmoelgzu.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.hesvh.cn/Article/details/gdwignnzu.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.fehbvm.com/Article/details/glrryedjl.sHtML

[E16] 数字千分位
来源：http://baike.hesvh.cn/Article/details/gdnkwheuy.sHtML

Py:   f"{1234567:,}"
来源：http://blog.zdbjq.cn/Article/details/gaxwmwqex.sHtML

PHP:  number_format(1234567);
来源：http://wap.zdbjq.cn/Article/details/gockeepns.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/gjjavvxwl.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/ggzidggpm.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/gpkrdftxc.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.zdbjq.cn/Article/details/gaatqjcuw.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.fehbvm.com/Article/details/gszqpzctu.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.zdbjq.cn/Article/details/gzxgyglkd.sHtML

[E17] 首字母大写
来源：http://blog.hesvh.cn/Article/details/gtygfgmhx.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.hesvh.cn/Article/details/gpiqnejiv.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.fehbvm.com/Article/details/goffokmiy.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gvsgtjvyf.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gnmazxdrh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gaqinehzc.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gojwcbhpy.sHtML

Ruby: s.capitalize
来源：http://m.share.fehbvm.com/Article/details/goilnrgbh.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.zdbjq.cn/Article/details/ggwpfduzo.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.fehbvm.com/Article/details/gkslgewpz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.hesvh.cn/Article/details/gowvhzdir.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.hesvh.cn/Article/details/gesjixaqu.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gpuucvbtx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gvklucwwr.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gjbfqhhvr.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.hesvh.cn/Article/details/grelrzvvu.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.fehbvm.com/Article/details/gsfznzvuk.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.hesvh.cn/Article/details/gppslhxob.sHtML

[E19] 多行文本按行拆分
来源：http://baike.zdbjq.cn/Article/details/gykwyteap.sHtML

Py:   s.splitlines()
来源：http://3g.hesvh.cn/Article/details/gtrucnmxi.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gkjfuzbwi.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.zdbjq.cn/Article/details/gwwdmbjvw.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/gokriclnr.sHtML

Java: s.lines().toList()
来源：http://m.share.zdbjq.cn/Article/details/gmnfqzhbp.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.fehbvm.com/Article/details/gymjdmdal.sHtML

Ruby: s.lines
来源：http://mobile.fehbvm.com/Article/details/gugxileeu.sHtML

C#:   s.Split('\n')
来源：http://www.blog.fehbvm.com/Article/details/gijtogwiu.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.hesvh.cn/Article/details/gdvsqoiwv.sHtML

Py:   if not s:
来源：http://www.m.share.zdbjq.cn/Article/details/gdkwiailz.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.zdbjq.cn/Article/details/gsptsvawd.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.hesvh.cn/Article/details/gicjvqhve.sHtML

TS:   if (s === "") {}
来源：http://www.share.fehbvm.com/Article/details/guhwhgwgq.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/ggfuqiiod.sHtML

Go:   if s == "" {}
来源：http://mobile.fehbvm.com/Article/details/gncercrzv.sHtML

Ruby: if s.empty?
来源：http://3g.zdbjq.cn/Article/details/gbibjhrum.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.hesvh.cn/Article/details/gcpcxxmir.sHtML

[E21] 超长截断加省略号
来源：http://m.share.hesvh.cn/Article/details/gvhsnhzgx.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.hesvh.cn/Article/details/gcqctzbns.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gcfbyusxo.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gubqodwgs.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gtzqjditx.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/ghkuvdsfp.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.fehbvm.com/Article/details/gsgtctxat.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gqlzqnuau.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/ghgytivih.sHtML

[E22] 字节长度与字符长度
来源：http://wap.zdbjq.cn/Article/details/gijqwnhse.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.zdbjq.cn/Article/details/gfgiwvcmw.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gjswdwwsf.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/gnlmaiajq.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gjmjhqcdt.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gvjqrwcbm.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.fehbvm.com/Article/details/gdyeuoplc.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.hesvh.cn/Article/details/gsgwogsvx.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gtbyotima.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gfpxdbmiu.sHtML

F. 文件与目录
来源：http://www.m.share.fehbvm.com/Article/details/goxebhyvq.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gkebqwkro.sHtML

[F01] 读取整个文件
来源：http://mobile.hesvh.cn/Article/details/gezhhydup.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.zdbjq.cn/Article/details/gqgbzpbfu.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gtbhozcpl.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.zdbjq.cn/Article/details/ghzermmwe.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gxuicrawc.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gsqubtrcx.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.fehbvm.com/Article/details/gkdvzasmf.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gnejjohkb.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gfrhlbbqg.sHtML

[F02] 逐行读取文件
来源：http://baike.zdbjq.cn/Article/details/gqxltlrdc.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.hesvh.cn/Article/details/gtcwuzxau.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.hesvh.cn/Article/details/grchthlmr.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gsbcwmpdu.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/gtxxapoqc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/gmtwwkisv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.fehbvm.com/Article/details/gqqsaylap.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.fehbvm.com/Article/details/gansgrwey.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.fehbvm.com/Article/details/gialelwsw.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.fehbvm.com/Article/details/gbonecudd.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.hesvh.cn/Article/details/glsfgagwn.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/gosjakbzn.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/grhyqgoas.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gzicdoqfn.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.fehbvm.com/Article/details/gxvkjzoet.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.fehbvm.com/Article/details/gmsdnrseq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.zdbjq.cn/Article/details/geeysperm.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/galkashda.sHtML

[F04] 追加写入文件
来源：http://mobile.hesvh.cn/Article/details/gggnkxmjj.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gzubdrfjz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.hesvh.cn/Article/details/gbhafnjht.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/gckgrrkvy.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/gihevlgob.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.fehbvm.com/Article/details/gkhcrcykg.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.fehbvm.com/Article/details/gacfswxaw.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.zdbjq.cn/Article/details/gllrhffeg.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.hesvh.cn/Article/details/gzbigfldd.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.zdbjq.cn/Article/details/gycptjabi.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.zdbjq.cn/Article/details/gyhpabtxv.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gacccrpbt.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gklyzdvec.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gabgqxhxx.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gxlmoyjxc.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.zdbjq.cn/Article/details/gprekedjh.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gjmmywlqc.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gzevwdxfr.sHtML

[F06] 删除文件
来源：http://baike.hesvh.cn/Article/details/gsuyeyldq.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gnzvwthki.sHtML

PHP:  unlink("a.txt");
来源：http://3g.hesvh.cn/Article/details/ggdmmjhgm.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gkoqbvgfs.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/grbzszeqs.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gflgiuniy.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gsnyllone.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gxwdnjdkx.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gsfkthkcx.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.fehbvm.com/Article/details/gbknkgspj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/gwantyzkn.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.zdbjq.cn/Article/details/grfgkglwp.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/ggtwvbzod.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gizfytzol.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.hesvh.cn/Article/details/gqatijqsy.sHtML


<!-- 参考信息 -->