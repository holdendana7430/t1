代发 wailian999

[D23] reduce 累积计算
来源：http://baike.zdbjq.cn/Article/details/gyqmsefvz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.fehbvm.com/Article/details/gcaenvmgt.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.fehbvm.com/Article/details/gunqrysfh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/gdtpqagqq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gtlktuikn.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.zdbjq.cn/Article/details/gphrndawz.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/gjcphfxqn.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.hesvh.cn/Article/details/gzyfxjoxb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.fehbvm.com/Article/details/gheezjyli.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.zdbjq.cn/Article/details/ghhvpvurj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fehbvm.com/Article/details/gsqplnbar.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.zdbjq.cn/Article/details/gxhycgkqr.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gbqldyptj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gljynaklp.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.zdbjq.cn/Article/details/ghwnpxylr.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.zdbjq.cn/Article/details/gsdobmyhj.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.hesvh.cn/Article/details/gpkeffini.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.hesvh.cn/Article/details/gxyyevren.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.hesvh.cn/Article/details/gmrhbxbdk.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.hesvh.cn/Article/details/greqfllag.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.hesvh.cn/Article/details/gnexsgkde.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.fehbvm.com/Article/details/gdjtvtemt.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.fehbvm.com/Article/details/gaueoiiys.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.hesvh.cn/Article/details/gxnhjsyku.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.fehbvm.com/Article/details/gpffoohcz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.hesvh.cn/Article/details/gwuuwkzzg.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.zdbjq.cn/Article/details/gibvchxjk.sHtML

[D26] 数组转字符串
来源：http://m.share.hesvh.cn/Article/details/gknimgeza.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.hesvh.cn/Article/details/gtspbpfnp.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gnlpeehvv.sHtML

JS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gqomvfrtz.sHtML

TS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gcfzcifrs.sHtML

Java: String.join(", ", list)
来源：http://3g.fehbvm.com/Article/details/gkroaedhy.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.hesvh.cn/Article/details/gssddhdqn.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/ggkkdsbqz.sHtML

C#:   string.Join(", ", list)
来源：http://baike.fehbvm.com/Article/details/gicwoiczg.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gxkprtzis.sHtML

E. 字符串处理
来源：http://mobile.hesvh.cn/Article/details/ggajgscnr.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gqchbqhpe.sHtML

[E01] 拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gdaooglpz.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.zdbjq.cn/Article/details/grkgdsddn.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.fehbvm.com/Article/details/gwnxpeibw.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/gczqapxvm.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/gzevwzuov.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.hesvh.cn/Article/details/gskatxvuf.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.fehbvm.com/Article/details/gstylfbth.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.zdbjq.cn/Article/details/gneqjvhin.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gekurznrr.sHtML

[E02] 重复字符串
来源：http://mobile.hesvh.cn/Article/details/grydmgynu.sHtML

Py:   "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/ggwxuqnyh.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.zdbjq.cn/Article/details/gyjqcaoqp.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gvkucxvsz.sHtML

TS:   "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gcsrikjgo.sHtML

Java: "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gafwcghbc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.fehbvm.com/Article/details/gmnefrice.sHtML

Ruby: "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/ggyknqcjp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.zdbjq.cn/Article/details/gezjzzaiy.sHtML

[E03] 截取子串
来源：http://blog.zdbjq.cn/Article/details/gxbrnrkas.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.hesvh.cn/Article/details/gsqficxsv.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gnrnugaaw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/ghdhdihqy.sHtML

TS:   s.slice(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gxipovecc.sHtML

Java: s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gynarczww.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.hesvh.cn/Article/details/gfkbqgeab.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.fehbvm.com/Article/details/gzvgclesj.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.hesvh.cn/Article/details/geyqnlafo.sHtML

[E04] 查找子串位置
来源：http://mobile.hesvh.cn/Article/details/ghqoiahey.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.hesvh.cn/Article/details/gzcvagltt.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.hesvh.cn/Article/details/gcboaacmv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.zdbjq.cn/Article/details/gpwjbgvji.sHtML

TS:   s.indexOf("x")
来源：http://read.share.fehbvm.com/Article/details/goiblgrtu.sHtML

Java: s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gdkfmsbfk.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.hesvh.cn/Article/details/gguudkgil.sHtML

Ruby: s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/gfkdcnvje.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gluefhsqn.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.fehbvm.com/Article/details/goqfxvmzt.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.hesvh.cn/Article/details/gttspuqqv.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.fehbvm.com/Article/details/gvyuvuqlg.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.hesvh.cn/Article/details/gmeyywoyj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.fehbvm.com/Article/details/gdtnutzeo.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gsmccuith.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.fehbvm.com/Article/details/gkmikbxpo.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.zdbjq.cn/Article/details/gbyjyfofk.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.fehbvm.com/Article/details/ggiobpanp.sHtML

[E06] 替换子串
来源：http://baike.hesvh.cn/Article/details/gncjerhyy.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/giuqgdchn.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.fehbvm.com/Article/details/goqqkfiha.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gccqjvoug.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gbqkyvmux.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gttoddipe.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/guhwdewbr.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gguorlwve.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gnzgkmvyx.sHtML

[E07] 按分隔符拆分
来源：http://wap.hesvh.cn/Article/details/gxobltyqt.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.zdbjq.cn/Article/details/gycgdpufm.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gyfzzrknx.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.hesvh.cn/Article/details/godsvlxjz.sHtML

TS:   s.split(",")
来源：http://www.m.share.hesvh.cn/Article/details/gohhzwymd.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.fehbvm.com/Article/details/gtejhztra.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.hesvh.cn/Article/details/gshetneqg.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.zdbjq.cn/Article/details/gsrfruicb.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.hesvh.cn/Article/details/gjsoquatr.sHtML

[E08] 数组按分隔符合并
来源：http://3g.zdbjq.cn/Article/details/gkazvdcam.sHtML

Py:   ",".join(items)
来源：http://www.m.share.zdbjq.cn/Article/details/gahlmfknk.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.hesvh.cn/Article/details/gfkifkcch.sHtML

JS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/gsgtnyyta.sHtML

TS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/gyddlcluc.sHtML

Java: String.join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gpoxzyefu.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.zdbjq.cn/Article/details/gddgvymde.sHtML

Ruby: items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gddbhrwbq.sHtML

C#:   string.Join(",", items)
来源：http://blog.zdbjq.cn/Article/details/guaumabhi.sHtML

[E09] 去除所有空白字符
来源：http://mobile.zdbjq.cn/Article/details/gzoiathzk.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.fehbvm.com/Article/details/gopivbqjn.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.zdbjq.cn/Article/details/ggnjfktsa.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/gxstidpsl.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.zdbjq.cn/Article/details/gsozubmsz.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.fehbvm.com/Article/details/gkqbugbgo.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.fehbvm.com/Article/details/gwqwhezkb.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.zdbjq.cn/Article/details/gxsxowlpn.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/gepxcwyie.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.zdbjq.cn/Article/details/gzmhexoeu.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gmoiutvme.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.zdbjq.cn/Article/details/gpcgmgukn.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gzzyqiqto.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/ggyaebacf.sHtML

Java: String.format("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gmrnywymm.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gaftfhwrc.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gunvhojrk.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.hesvh.cn/Article/details/gpujwjvnh.sHtML

[E11] 反转字符串
来源：http://www.blog.hesvh.cn/Article/details/gbklcsntp.sHtML

Py:   s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/gmdpqxnsf.sHtML

PHP:  strrev($s);
来源：http://wap.fehbvm.com/Article/details/gyqxnpsbj.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gnlmjkheg.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gsdogeida.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.hesvh.cn/Article/details/gogcqucpk.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.zdbjq.cn/Article/details/ginludnet.sHtML

Ruby: s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gtyhvotsq.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/gxukuvyhe.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.fehbvm.com/Article/details/gdksznecn.sHtML

Py:   s.count("a")
来源：http://read.share.hesvh.cn/Article/details/gttucxctv.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.hesvh.cn/Article/details/gtelanthv.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/gzvxxreze.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gdmeaakmf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.fehbvm.com/Article/details/gwiqdwyyj.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.hesvh.cn/Article/details/ghsrbitkl.sHtML

Ruby: s.count("a")
来源：http://read.share.fehbvm.com/Article/details/gmhaigxjn.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.hesvh.cn/Article/details/gxcbmmbcm.sHtML

[E13] 逐字符遍历
来源：http://blog.zdbjq.cn/Article/details/gsyaixpuv.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.zdbjq.cn/Article/details/ghejbvctu.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.zdbjq.cn/Article/details/gzmkqmjmo.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/glmtchcnc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gjzmmrlsi.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.hesvh.cn/Article/details/grrnjxgoi.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.fehbvm.com/Article/details/glstbmhfw.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.hesvh.cn/Article/details/gyeboitiq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.fehbvm.com/Article/details/gkasodvqg.sHtML

[E14] URL 编码与 Base64
来源：http://baike.zdbjq.cn/Article/details/gkhclcwpe.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.fehbvm.com/Article/details/gnvcqqndb.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.zdbjq.cn/Article/details/gofqttlsw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fehbvm.com/Article/details/gkrddewkb.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.fehbvm.com/Article/details/gyagsgbmn.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gldsbwsdq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.fehbvm.com/Article/details/gqbktilzy.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.fehbvm.com/Article/details/gfgkevegq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.hesvh.cn/Article/details/ggnfwunpu.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.hesvh.cn/Article/details/ghmtgrulu.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.zdbjq.cn/Article/details/gkxtxitnd.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.fehbvm.com/Article/details/gieajfdqo.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.hesvh.cn/Article/details/gzvacenvh.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.zdbjq.cn/Article/details/gpbfyqtdj.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.zdbjq.cn/Article/details/gdsvlpphw.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.fehbvm.com/Article/details/gndjexjdw.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.fehbvm.com/Article/details/gpsuyuend.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.zdbjq.cn/Article/details/gytayknfg.sHtML

[E16] 数字千分位
来源：http://www.blog.fehbvm.com/Article/details/gpzgiyxpp.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.zdbjq.cn/Article/details/gvnsqkxnd.sHtML

PHP:  number_format(1234567);
来源：http://read.share.zdbjq.cn/Article/details/gvtyqdcwj.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/gyxbsdwyk.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/gxigrahgu.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.hesvh.cn/Article/details/gsncyevmn.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.zdbjq.cn/Article/details/gqamlcjwc.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.fehbvm.com/Article/details/gpzfkbamp.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.hesvh.cn/Article/details/ghctdnjgn.sHtML

[E17] 首字母大写
来源：http://mobile.hesvh.cn/Article/details/guafikqiu.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.fehbvm.com/Article/details/gnkjgrdku.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.hesvh.cn/Article/details/gfmvryncp.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/gndiogjwx.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/gxrokyysm.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.zdbjq.cn/Article/details/ghpufycwz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.hesvh.cn/Article/details/gteauirip.sHtML

Ruby: s.capitalize
来源：http://blog.zdbjq.cn/Article/details/gnxqfhnrv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.hesvh.cn/Article/details/gdbyprcqa.sHtML

[E18] 模板占位符替换
来源：http://m.share.zdbjq.cn/Article/details/gzfgpbacb.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.zdbjq.cn/Article/details/gemiljdwo.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.hesvh.cn/Article/details/gdtzlimgt.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gzflqylmt.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gurvpafvn.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gemlimcod.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gulopkgvq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.hesvh.cn/Article/details/gqilsnxgh.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.hesvh.cn/Article/details/gfyygrjjr.sHtML

[E19] 多行文本按行拆分
来源：http://3g.hesvh.cn/Article/details/gosemcwgj.sHtML

Py:   s.splitlines()
来源：http://mobile.hesvh.cn/Article/details/gkkgizyua.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.fehbvm.com/Article/details/govuvbdks.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/ggowcdsmq.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gcniuqyuv.sHtML

Java: s.lines().toList()
来源：http://baike.zdbjq.cn/Article/details/gczciqmsb.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.hesvh.cn/Article/details/gvcnpowqx.sHtML

Ruby: s.lines
来源：http://wap.zdbjq.cn/Article/details/grcvjtzun.sHtML

C#:   s.Split('\n')
来源：http://m.share.zdbjq.cn/Article/details/gptpdajny.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.hesvh.cn/Article/details/gxhqlobfr.sHtML

Py:   if not s:
来源：http://baike.zdbjq.cn/Article/details/gmbnweqwd.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.zdbjq.cn/Article/details/gexuaqtop.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.fehbvm.com/Article/details/gkhirtmoh.sHtML

TS:   if (s === "") {}
来源：http://wap.fehbvm.com/Article/details/gshhbopra.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/geajmmezq.sHtML

Go:   if s == "" {}
来源：http://blog.fehbvm.com/Article/details/ghutsdvwe.sHtML

Ruby: if s.empty?
来源：http://read.share.fehbvm.com/Article/details/gyyjdfxpa.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.hesvh.cn/Article/details/gduvzrbpy.sHtML

[E21] 超长截断加省略号
来源：http://read.share.hesvh.cn/Article/details/gsbjsxfxo.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.hesvh.cn/Article/details/gwnbsvtic.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gatabgmlm.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gpjdoraod.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gzheoxony.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gvztlkhwo.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.hesvh.cn/Article/details/glaqlzrps.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gffjgpubo.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gghplhxfv.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.zdbjq.cn/Article/details/gismeowxi.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.fehbvm.com/Article/details/gaxsyhbat.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gvureikgg.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gasmctwop.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gsregbiqj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/gauqnnrix.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.hesvh.cn/Article/details/gdbadyvby.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.fehbvm.com/Article/details/gerfwojjn.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/gsysmjfja.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqziprglw.sHtML

F. 文件与目录
来源：http://www.blog.hesvh.cn/Article/details/gnzuwppll.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gapvpkmri.sHtML

[F01] 读取整个文件
来源：http://baike.fehbvm.com/Article/details/gepempgda.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.fehbvm.com/Article/details/gpgqgpwuo.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gxhpxngaf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.zdbjq.cn/Article/details/girwcjyql.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.fehbvm.com/Article/details/glmxyibsz.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gtxbearxv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.fehbvm.com/Article/details/gqalzghjj.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gflmlpxmv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gqdbmhrpn.sHtML

[F02] 逐行读取文件
来源：http://read.share.hesvh.cn/Article/details/gdmqqridy.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.hesvh.cn/Article/details/gqyqbyehb.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.zdbjq.cn/Article/details/gldudsfxw.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gyoheehjb.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gnvqpkrmw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/gdiffapsj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.hesvh.cn/Article/details/gpureonuv.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.zdbjq.cn/Article/details/gdbaibzfv.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.hesvh.cn/Article/details/gljmnurqo.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.hesvh.cn/Article/details/gthozpjna.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fehbvm.com/Article/details/gfcxpuunp.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/gqoxndgqh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gpslixvyb.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/ggjdujgzk.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.fehbvm.com/Article/details/gbohitvkr.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.hesvh.cn/Article/details/gsxkpnauo.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.hesvh.cn/Article/details/gtlqsmodf.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gxvgsnjcp.sHtML

[F04] 追加写入文件
来源：http://wap.hesvh.cn/Article/details/gwkpdcere.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gpssrvbyp.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.hesvh.cn/Article/details/gjhrcygyt.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/gequszdid.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/ghkrzxmdk.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.zdbjq.cn/Article/details/gjsbwnbvd.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.fehbvm.com/Article/details/gquchvedk.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.fehbvm.com/Article/details/gwdjqnbqz.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.hesvh.cn/Article/details/gsqgatfgw.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.zdbjq.cn/Article/details/gpqykpkqr.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.zdbjq.cn/Article/details/gjcuiwndk.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gclaynrrb.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/ggnzkwnpo.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/giagwwyxt.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gjllfgwmt.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.zdbjq.cn/Article/details/gijdpjhyn.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.hesvh.cn/Article/details/grxscegdc.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gricylrcs.sHtML

[F06] 删除文件
来源：http://wap.hesvh.cn/Article/details/griqkvqkv.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ghuqqaovk.sHtML

PHP:  unlink("a.txt");
来源：http://blog.fehbvm.com/Article/details/gbwvqalmm.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gwavhosil.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gllpzgnfs.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gusdbkswp.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gtipelqib.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gmaapcbdz.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.hesvh.cn/Article/details/gvmgytlyq.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.fehbvm.com/Article/details/gglofwfyh.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/gtvetuttv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.fehbvm.com/Article/details/gmrgahvcv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gepqqcugy.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/gdqpsjmsn.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.zdbjq.cn/Article/details/giokpliig.sHtML


<!-- 参考信息 -->