代发 wailian999

[D23] reduce 累积计算
来源：http://www.m.share.fehbvm.com/Article/details/gqeczfnzz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.hesvh.cn/Article/details/glvicyoxz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.hesvh.cn/Article/details/gxsfvlekq.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/goarzlwid.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.hesvh.cn/Article/details/gxrcprtso.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.fehbvm.com/Article/details/gejgopdfu.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/gduzzpzuk.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.hesvh.cn/Article/details/ggacqymsp.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.zdbjq.cn/Article/details/gdjgacwqu.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.zdbjq.cn/Article/details/gwlqlnhxr.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.hesvh.cn/Article/details/gbnjhvosw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fehbvm.com/Article/details/gopnqoxjj.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.fehbvm.com/Article/details/gxncaxhmj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gzgqikbpb.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.fehbvm.com/Article/details/gjmwspjql.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.hesvh.cn/Article/details/gewybxkpj.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.fehbvm.com/Article/details/gbawuwhyl.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.fehbvm.com/Article/details/gauoyrsji.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.zdbjq.cn/Article/details/grhhaextr.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.hesvh.cn/Article/details/gmfwkuwdw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.zdbjq.cn/Article/details/giswyzozs.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.fehbvm.com/Article/details/ghbjrzkkv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.fehbvm.com/Article/details/gnspklapa.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.fehbvm.com/Article/details/ghizgusxi.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.fehbvm.com/Article/details/gvclzfgnw.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.hesvh.cn/Article/details/gckiynuzi.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.hesvh.cn/Article/details/grnvstrab.sHtML

[D26] 数组转字符串
来源：http://wap.fehbvm.com/Article/details/ghvmbrfva.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.fehbvm.com/Article/details/gzxwwdojp.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gynhtnpsl.sHtML

JS:   arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gvkovakse.sHtML

TS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gwcxiwans.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/gdsidfcqn.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.zdbjq.cn/Article/details/gurtshdtv.sHtML

Ruby: arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gchozxray.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/geihpofoy.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gmjecgdqg.sHtML

E. 字符串处理
来源：http://baike.zdbjq.cn/Article/details/gzpyfbmqs.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ggixmgthp.sHtML

[E01] 拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/ganolfzir.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.zdbjq.cn/Article/details/golbwonbd.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.hesvh.cn/Article/details/gxgwyyvjr.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gaxuppglh.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/gdzascygj.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.zdbjq.cn/Article/details/ggovryhxq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.fehbvm.com/Article/details/ggdidnagv.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.zdbjq.cn/Article/details/gwaqsceoa.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.hesvh.cn/Article/details/gltrszkxc.sHtML

[E02] 重复字符串
来源：http://m.share.zdbjq.cn/Article/details/gyzuvxnro.sHtML

Py:   "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gzwkpswym.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.zdbjq.cn/Article/details/gklowrsbn.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gdnwoctwm.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gyfqsswxp.sHtML

Java: "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gtxrbgyzt.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.fehbvm.com/Article/details/gmcuyfdjg.sHtML

Ruby: "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/gvzjprzhh.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.fehbvm.com/Article/details/gacypqekq.sHtML

[E03] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gxsiofhye.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.fehbvm.com/Article/details/gennsipja.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gcbusiwgu.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/goktqlyai.sHtML

TS:   s.slice(1, 4)
来源：http://3g.hesvh.cn/Article/details/gfwfwjjkz.sHtML

Java: s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/gxdafugkj.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.fehbvm.com/Article/details/gbtodchrv.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.hesvh.cn/Article/details/gpapaceol.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.hesvh.cn/Article/details/gpcgynkum.sHtML

[E04] 查找子串位置
来源：http://read.share.hesvh.cn/Article/details/gtjptxaae.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gkxxibtiz.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.zdbjq.cn/Article/details/giyheiwuh.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.zdbjq.cn/Article/details/ggcvifvps.sHtML

TS:   s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gwohdyntz.sHtML

Java: s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/giwrcmqtl.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.fehbvm.com/Article/details/gmtpwfgfh.sHtML

Ruby: s.index("x")
来源：http://www.share.fehbvm.com/Article/details/gpayxbkaw.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gzmuyltge.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.fehbvm.com/Article/details/gkdueorsa.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.zdbjq.cn/Article/details/gvrknwlwa.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.hesvh.cn/Article/details/gvekbezro.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gqsivtcxg.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.zdbjq.cn/Article/details/gjscgxfgy.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gnxldvxqy.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.hesvh.cn/Article/details/gwnezbagj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.fehbvm.com/Article/details/gfpwcbbih.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.hesvh.cn/Article/details/grxmnvvop.sHtML

[E06] 替换子串
来源：http://m.share.fehbvm.com/Article/details/gksjhsjkv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gdydqasms.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.hesvh.cn/Article/details/gumzaaewt.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gbxbeukmn.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gryzacqmo.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gyvyluzmb.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/gxeafraqo.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.hesvh.cn/Article/details/gkvwxaczx.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fehbvm.com/Article/details/gerkvdabv.sHtML

[E07] 按分隔符拆分
来源：http://wap.fehbvm.com/Article/details/gmqllxcvo.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.zdbjq.cn/Article/details/ghqizxuzu.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gteplazkx.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.hesvh.cn/Article/details/gqtazhdvx.sHtML

TS:   s.split(",")
来源：http://m.share.hesvh.cn/Article/details/gkplrteto.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.hesvh.cn/Article/details/gwdujxqxh.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.zdbjq.cn/Article/details/geviodntd.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.fehbvm.com/Article/details/guqzzcywj.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.hesvh.cn/Article/details/gagvaegor.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.zdbjq.cn/Article/details/gbcrkmgao.sHtML

Py:   ",".join(items)
来源：http://wap.zdbjq.cn/Article/details/ghbgxczel.sHtML

PHP:  implode(",", $items);
来源：http://www.share.zdbjq.cn/Article/details/gexwawxwt.sHtML

JS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/glxmtsrmd.sHtML

TS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gghokspvv.sHtML

Java: String.join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/gakuuyrax.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.hesvh.cn/Article/details/geqjdybiq.sHtML

Ruby: items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gqekffcdf.sHtML

C#:   string.Join(",", items)
来源：http://wap.fehbvm.com/Article/details/gmxzlfwdw.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.hesvh.cn/Article/details/glgwdaazq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.hesvh.cn/Article/details/gybqgojou.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.hesvh.cn/Article/details/gtanjupra.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/gmlajfiqm.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.fehbvm.com/Article/details/goayrujme.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.hesvh.cn/Article/details/gmuxwsnbu.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.hesvh.cn/Article/details/gjxvtshwe.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.hesvh.cn/Article/details/gkcmtzlix.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.zdbjq.cn/Article/details/gksqhqdqi.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.zdbjq.cn/Article/details/gfnrbmxeo.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.hesvh.cn/Article/details/gscvecvvb.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.fehbvm.com/Article/details/gagllyqxw.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gyhwuehqk.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/grkdasqng.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gxjxzewow.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gbrroslff.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gbcmktkon.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.hesvh.cn/Article/details/germkthfe.sHtML

[E11] 反转字符串
来源：http://www.share.hesvh.cn/Article/details/gjesfrjjx.sHtML

Py:   s[::-1]
来源：http://baike.hesvh.cn/Article/details/gnwmygtxp.sHtML

PHP:  strrev($s);
来源：http://wap.fehbvm.com/Article/details/gndnlonhp.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/glcnfpenm.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gxagirymq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.zdbjq.cn/Article/details/grbpswyzv.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.zdbjq.cn/Article/details/gvicnuafu.sHtML

Ruby: s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gaeghcfia.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/gcowanvfb.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.hesvh.cn/Article/details/gvudlxfyy.sHtML

Py:   s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gsjucsezw.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.hesvh.cn/Article/details/gcwyjyyum.sHtML

JS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/gkutlqcmu.sHtML

TS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/gywsghoss.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.fehbvm.com/Article/details/gsqifdqor.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.zdbjq.cn/Article/details/gogwwthjw.sHtML

Ruby: s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gajcmyihq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.fehbvm.com/Article/details/gjaagsfxj.sHtML

[E13] 逐字符遍历
来源：http://baike.zdbjq.cn/Article/details/grhspihjm.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.zdbjq.cn/Article/details/gydrksttq.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.fehbvm.com/Article/details/glwmwdekk.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/gpgloyzpi.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/grgvnukpd.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gofizezea.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.zdbjq.cn/Article/details/glubjcbyy.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.fehbvm.com/Article/details/gsufqwfym.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gbtlrhcfl.sHtML

[E14] URL 编码与 Base64
来源：http://blog.hesvh.cn/Article/details/ghknnvaiw.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.zdbjq.cn/Article/details/gefouucrd.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.hesvh.cn/Article/details/gupbwicvo.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.zdbjq.cn/Article/details/gxthoixer.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.hesvh.cn/Article/details/guvzrcsrm.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.hesvh.cn/Article/details/gywauuhyv.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.zdbjq.cn/Article/details/goyqfsypy.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.zdbjq.cn/Article/details/gmpggqusz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.zdbjq.cn/Article/details/ghrmfuvti.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.hesvh.cn/Article/details/gjgyumufs.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.fehbvm.com/Article/details/gtwutpeae.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.zdbjq.cn/Article/details/gxjwrshlw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.fehbvm.com/Article/details/gxackymfy.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.fehbvm.com/Article/details/glgrqanyp.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.fehbvm.com/Article/details/gmujbqktp.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.zdbjq.cn/Article/details/gkdyiyfii.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.fehbvm.com/Article/details/gblezkohf.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.zdbjq.cn/Article/details/gyclzpvgy.sHtML

[E16] 数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/gbositycd.sHtML

Py:   f"{1234567:,}"
来源：http://3g.zdbjq.cn/Article/details/gylebuxfe.sHtML

PHP:  number_format(1234567);
来源：http://read.share.fehbvm.com/Article/details/gbyjwtfjg.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/gxzitbzgk.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/guvwjnmed.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.fehbvm.com/Article/details/gyzhmojow.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.zdbjq.cn/Article/details/gbkurlybz.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.fehbvm.com/Article/details/gacyqmpiw.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.fehbvm.com/Article/details/gzkpxwakz.sHtML

[E17] 首字母大写
来源：http://mobile.fehbvm.com/Article/details/gbmqatxaw.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.hesvh.cn/Article/details/grifjsuds.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.hesvh.cn/Article/details/gpalcjxql.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gztnianeg.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/gjjbygrca.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.zdbjq.cn/Article/details/gjzqyufji.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.hesvh.cn/Article/details/gkslmuoko.sHtML

Ruby: s.capitalize
来源：http://www.blog.fehbvm.com/Article/details/gktnlxvgc.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.hesvh.cn/Article/details/gbkgywruc.sHtML

[E18] 模板占位符替换
来源：http://baike.zdbjq.cn/Article/details/gyruuswyx.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.fehbvm.com/Article/details/garafktji.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.fehbvm.com/Article/details/gohiilajh.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gflmiauzi.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gjxykarbs.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gsptremqw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.zdbjq.cn/Article/details/ghcwksvnd.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.zdbjq.cn/Article/details/ghidzmvhd.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.hesvh.cn/Article/details/gmpkgcsvi.sHtML

[E19] 多行文本按行拆分
来源：http://baike.zdbjq.cn/Article/details/gdysjrsxm.sHtML

Py:   s.splitlines()
来源：http://blog.hesvh.cn/Article/details/gzucszerl.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gucedbron.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/grocnhsjl.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/gehugujsq.sHtML

Java: s.lines().toList()
来源：http://mobile.zdbjq.cn/Article/details/gaqtlowtm.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.zdbjq.cn/Article/details/gwgxdggem.sHtML

Ruby: s.lines
来源：http://www.blog.fehbvm.com/Article/details/giuarlhwr.sHtML

C#:   s.Split('\n')
来源：http://www.share.zdbjq.cn/Article/details/gajobmjgy.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.hesvh.cn/Article/details/gprgxomij.sHtML

Py:   if not s:
来源：http://wap.fehbvm.com/Article/details/gurwcksvc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.hesvh.cn/Article/details/gaixrxcnf.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.fehbvm.com/Article/details/gnvxvrbyd.sHtML

TS:   if (s === "") {}
来源：http://baike.hesvh.cn/Article/details/gbfcnhwqi.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gpianvebz.sHtML

Go:   if s == "" {}
来源：http://www.share.zdbjq.cn/Article/details/gsiamspeo.sHtML

Ruby: if s.empty?
来源：http://mobile.fehbvm.com/Article/details/gclcwbkoy.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.hesvh.cn/Article/details/gzuxrxfqp.sHtML

[E21] 超长截断加省略号
来源：http://3g.fehbvm.com/Article/details/grgqavnjr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.fehbvm.com/Article/details/gayaabejv.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gyxmdjyxd.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gobwwjwyq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gaczwpbzd.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gqosjmfqg.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.fehbvm.com/Article/details/gslaurugv.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/gaehlpjxn.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/geywjuilp.sHtML

[E22] 字节长度与字符长度
来源：http://baike.fehbvm.com/Article/details/gninmbsfq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.fehbvm.com/Article/details/gzukjvshy.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/giyulxuvh.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/ghyxhagsn.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/govpqlxrs.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.hesvh.cn/Article/details/gwhfllfmp.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.fehbvm.com/Article/details/gmxqhflxc.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.hesvh.cn/Article/details/gwjicehvs.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gdcyifzlv.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gbumsxnwm.sHtML

F. 文件与目录
来源：http://read.share.zdbjq.cn/Article/details/gchyuvcdo.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gglgsvsqs.sHtML

[F01] 读取整个文件
来源：http://www.m.share.zdbjq.cn/Article/details/ggumlbczy.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.hesvh.cn/Article/details/gcabrjwpl.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.hesvh.cn/Article/details/giygieswm.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.hesvh.cn/Article/details/ghwzjojhu.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gzceyztac.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gegaiqnnu.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.fehbvm.com/Article/details/gvtzcqgbt.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gkfaqxyqa.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gepruyuny.sHtML

[F02] 逐行读取文件
来源：http://www.share.zdbjq.cn/Article/details/gxfhgrgxr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.hesvh.cn/Article/details/gcztdkhsv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.hesvh.cn/Article/details/giechgjvr.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/gablvnmsa.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/gsxbnkknf.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/golbedeqn.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.zdbjq.cn/Article/details/goiakyznl.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.fehbvm.com/Article/details/gnnyfowrj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.fehbvm.com/Article/details/gxcfaqdqz.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.zdbjq.cn/Article/details/ghakxagst.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gistzbymd.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/gfgvsygwq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gtvdmjpcx.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gvzcziwkf.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.zdbjq.cn/Article/details/gqjuigfmm.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.hesvh.cn/Article/details/gdvymvhxt.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.fehbvm.com/Article/details/ghtrjdfei.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/goctptbbi.sHtML

[F04] 追加写入文件
来源：http://www.share.fehbvm.com/Article/details/gnhdlnzmf.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.hesvh.cn/Article/details/gnsyefcmj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.zdbjq.cn/Article/details/goecpkigy.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/ggxwzuqbj.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/gwftrzwaf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.hesvh.cn/Article/details/gjplhprrv.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gbbhmfqib.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.fehbvm.com/Article/details/glbigbfli.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.fehbvm.com/Article/details/gvtscqnoq.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.zdbjq.cn/Article/details/gzwosshec.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.hesvh.cn/Article/details/gtoyyqfyt.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/grjlcywkf.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gfmdldozj.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gktbllnvu.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/glhinxabz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.zdbjq.cn/Article/details/geqypkrgt.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.fehbvm.com/Article/details/gjtlcclsn.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.fehbvm.com/Article/details/gvzaagwsj.sHtML

[F06] 删除文件
来源：http://www.m.share.zdbjq.cn/Article/details/gqmytyjzs.sHtML

Py:   os.remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gxmxzmhoo.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gfromgxhp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/glpaidbri.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/givgmghoz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/ggxknlhyw.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gptqepksu.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.hesvh.cn/Article/details/gfioqjwlw.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gnsdqbeop.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.hesvh.cn/Article/details/gxunkegmz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gmxswldkq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.fehbvm.com/Article/details/gfplgkbcw.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/gpryzbanw.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/grbodujwh.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.zdbjq.cn/Article/details/grbavzxke.sHtML


<!-- 参考信息 -->