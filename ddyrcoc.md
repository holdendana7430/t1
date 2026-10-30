代发 wailian999

[D23] reduce 累积计算
来源：http://wap.hesvh.cn/Article/details/gpymfkmlh.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.hesvh.cn/Article/details/gkxxbstnc.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.zdbjq.cn/Article/details/gxzbldgor.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/gxyuksuey.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/gvvviitlb.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.zdbjq.cn/Article/details/goyeklrvm.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/ghusiarju.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.zdbjq.cn/Article/details/gtgygmcfs.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.fehbvm.com/Article/details/glumbatwi.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.fehbvm.com/Article/details/gjkileomw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.hesvh.cn/Article/details/gfqugapxz.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.fehbvm.com/Article/details/gaqqknsth.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.zdbjq.cn/Article/details/gnshftmge.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.fehbvm.com/Article/details/gkqvvyezf.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.fehbvm.com/Article/details/gsuqwebhh.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.zdbjq.cn/Article/details/gvjtbhcwh.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.zdbjq.cn/Article/details/gqxdzdubi.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.hesvh.cn/Article/details/gtqgtvury.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.hesvh.cn/Article/details/gdvxwtobm.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.hesvh.cn/Article/details/gajzpxefe.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.fehbvm.com/Article/details/gvvkxobju.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.fehbvm.com/Article/details/gdaasdxrl.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.fehbvm.com/Article/details/gdiyhnsnv.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.hesvh.cn/Article/details/gsreegoje.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.zdbjq.cn/Article/details/gubaiqesu.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.zdbjq.cn/Article/details/gavlwjltl.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.fehbvm.com/Article/details/gfqvvvdca.sHtML

[D26] 数组转字符串
来源：http://www.blog.hesvh.cn/Article/details/gidyxudam.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.hesvh.cn/Article/details/gmebmddbo.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.hesvh.cn/Article/details/gdztnxrzx.sHtML

JS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/geyroswcl.sHtML

TS:   arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/giuhjdams.sHtML

Java: String.join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/gbxfchplt.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gijyisuds.sHtML

Ruby: arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/govygpqje.sHtML

C#:   string.Join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gaovmeygl.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gwrywzmjy.sHtML

E. 字符串处理
来源：http://www.blog.fehbvm.com/Article/details/gnpnggxdo.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gqywtatnh.sHtML

[E01] 拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gcvychpmn.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.zdbjq.cn/Article/details/ggjqmirwb.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.zdbjq.cn/Article/details/gzsjaeyyp.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gtginlzvo.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gozztzeol.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.zdbjq.cn/Article/details/gnkovzhbv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.fehbvm.com/Article/details/gfbdkqxwf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.zdbjq.cn/Article/details/gmdielrte.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gtadbkvub.sHtML

[E02] 重复字符串
来源：http://m.share.zdbjq.cn/Article/details/ggpalkzdr.sHtML

Py:   "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/gfollwlpt.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.fehbvm.com/Article/details/gatorckwm.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gpioxyvnk.sHtML

TS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gmsfdjgbw.sHtML

Java: "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gllmzoimj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.hesvh.cn/Article/details/gyzhodbdx.sHtML

Ruby: "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gydopguyg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.fehbvm.com/Article/details/gluekmswa.sHtML

[E03] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gnzlxrwyp.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.hesvh.cn/Article/details/gcbwvhpsc.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gzelbursi.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gznmsuoct.sHtML

TS:   s.slice(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gsccltgba.sHtML

Java: s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gnrhdtibc.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.fehbvm.com/Article/details/gsfxudlrd.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.hesvh.cn/Article/details/gugszuddm.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.zdbjq.cn/Article/details/gonimvppj.sHtML

[E04] 查找子串位置
来源：http://3g.hesvh.cn/Article/details/gbgupwjxj.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gmqkhjjfs.sHtML

PHP:  strpos($s, "x");
来源：http://wap.hesvh.cn/Article/details/gqqmcepio.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.zdbjq.cn/Article/details/gmudffgev.sHtML

TS:   s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gmbcqkigt.sHtML

Java: s.indexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gmgasqrko.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.fehbvm.com/Article/details/gmxmbsfjo.sHtML

Ruby: s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gdwnseyro.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gkallyfbz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.zdbjq.cn/Article/details/gguxyooia.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.fehbvm.com/Article/details/gnopllhgl.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.zdbjq.cn/Article/details/gusssuftn.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gvtgzlhht.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.zdbjq.cn/Article/details/guovxmdcr.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/goapbluph.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.hesvh.cn/Article/details/gyzpxocvu.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.fehbvm.com/Article/details/gstcxqzts.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.hesvh.cn/Article/details/gkebwtvak.sHtML

[E06] 替换子串
来源：http://3g.hesvh.cn/Article/details/gwusjiqqo.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gomqzuqzi.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.fehbvm.com/Article/details/gtqhyjbex.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/glzhryhap.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gqbclxwwg.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gzjlpcezn.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/gdmvgprit.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.hesvh.cn/Article/details/gcjwhxqeh.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/guyucfcle.sHtML

[E07] 按分隔符拆分
来源：http://www.share.zdbjq.cn/Article/details/gmpsbogxm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.hesvh.cn/Article/details/gqyqznbak.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.fehbvm.com/Article/details/gqyrcytme.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.zdbjq.cn/Article/details/gbnohbswp.sHtML

TS:   s.split(",")
来源：http://www.m.share.fehbvm.com/Article/details/gvssegmpm.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.zdbjq.cn/Article/details/goloroxob.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.hesvh.cn/Article/details/gugvudpya.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.zdbjq.cn/Article/details/gmbqcfetw.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.fehbvm.com/Article/details/gdaawlpmr.sHtML

[E08] 数组按分隔符合并
来源：http://wap.fehbvm.com/Article/details/gwffievel.sHtML

Py:   ",".join(items)
来源：http://wap.fehbvm.com/Article/details/gtxgjjrgf.sHtML

PHP:  implode(",", $items);
来源：http://read.share.hesvh.cn/Article/details/gzqiqmjlq.sHtML

JS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gzkxvfkky.sHtML

TS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/grcudjkum.sHtML

Java: String.join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/giiryjyfs.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.hesvh.cn/Article/details/gtziewhvd.sHtML

Ruby: items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gnkpaprcu.sHtML

C#:   string.Join(",", items)
来源：http://m.share.hesvh.cn/Article/details/gjbanyume.sHtML

[E09] 去除所有空白字符
来源：http://mobile.hesvh.cn/Article/details/giclibiif.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.fehbvm.com/Article/details/gxzdnlktg.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.fehbvm.com/Article/details/gmuvbfrmq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/gyyxfwhch.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/gumkxaeds.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.hesvh.cn/Article/details/gziicvilb.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.fehbvm.com/Article/details/gvaejczve.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gxnmpialv.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.hesvh.cn/Article/details/gmboktqzj.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.fehbvm.com/Article/details/ggaemiwaa.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/ghetyiipe.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.zdbjq.cn/Article/details/gvohccfvg.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gsupfdlfd.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gqprlbdfa.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gtixzhhru.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gsufrwwom.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gwkwzsdjq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.hesvh.cn/Article/details/gbbefgkpv.sHtML

[E11] 反转字符串
来源：http://3g.fehbvm.com/Article/details/gfqwfkqum.sHtML

Py:   s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gwnsyjuhn.sHtML

PHP:  strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/gjgrgckzr.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gskjtcvrs.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gzlnqwhdn.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.zdbjq.cn/Article/details/gcjakzosh.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.zdbjq.cn/Article/details/gidfdztli.sHtML

Ruby: s.reverse
来源：http://3g.zdbjq.cn/Article/details/gyvcavnbn.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/gmoqcjcqk.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.fehbvm.com/Article/details/gwhnlefqf.sHtML

Py:   s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gbtqmwnax.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.fehbvm.com/Article/details/gwabdebly.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/giwhtoavl.sHtML

TS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/gnpslzjme.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.zdbjq.cn/Article/details/gqojwsyzf.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.fehbvm.com/Article/details/gojossnur.sHtML

Ruby: s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gwxvqbmyj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.hesvh.cn/Article/details/gcqxzxmjp.sHtML

[E13] 逐字符遍历
来源：http://mobile.zdbjq.cn/Article/details/gjdnayffv.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.zdbjq.cn/Article/details/gvzkuvusc.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.zdbjq.cn/Article/details/gxttvdtww.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/gimlpekjb.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gompsdsyo.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gwtbfrtoj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.hesvh.cn/Article/details/guusclkxa.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.zdbjq.cn/Article/details/glhzjghwb.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.hesvh.cn/Article/details/guexrtfqj.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.fehbvm.com/Article/details/gttdzkvej.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.hesvh.cn/Article/details/geharueua.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.fehbvm.com/Article/details/gqydnkfub.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fehbvm.com/Article/details/gpceatass.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.zdbjq.cn/Article/details/gtfrjvarw.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.fehbvm.com/Article/details/gfrkfzddn.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.fehbvm.com/Article/details/gpworejnf.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.zdbjq.cn/Article/details/gvnwbfomz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.hesvh.cn/Article/details/gggtzowvs.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.hesvh.cn/Article/details/gfuqlxbui.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.fehbvm.com/Article/details/gxavqlblz.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.fehbvm.com/Article/details/gxjouzsng.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.fehbvm.com/Article/details/gerwoqhjg.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.hesvh.cn/Article/details/gcendcmii.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.zdbjq.cn/Article/details/gdvdqocaa.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.fehbvm.com/Article/details/gczpbymbf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.fehbvm.com/Article/details/gaiyccxoh.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.zdbjq.cn/Article/details/glmbywhxd.sHtML

[E16] 数字千分位
来源：http://blog.fehbvm.com/Article/details/gjsmyugjz.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.fehbvm.com/Article/details/gjlzcxpvo.sHtML

PHP:  number_format(1234567);
来源：http://m.share.hesvh.cn/Article/details/ghllyjeip.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/gexiqimqd.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/gsulghmml.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.hesvh.cn/Article/details/gpodxidhb.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.zdbjq.cn/Article/details/ghrffijvw.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.zdbjq.cn/Article/details/gaskpfpqx.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.zdbjq.cn/Article/details/gmvvsjbdr.sHtML

[E17] 首字母大写
来源：http://www.share.zdbjq.cn/Article/details/guszqsqal.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.hesvh.cn/Article/details/glwdixsaj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.zdbjq.cn/Article/details/gfwjxymqu.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/gevshxywz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/gphpscrca.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.fehbvm.com/Article/details/gvwllwwuj.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.fehbvm.com/Article/details/gsmrqfboa.sHtML

Ruby: s.capitalize
来源：http://www.m.share.fehbvm.com/Article/details/gixjfhcbk.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.hesvh.cn/Article/details/gfueuiegm.sHtML

[E18] 模板占位符替换
来源：http://baike.fehbvm.com/Article/details/gmngmymbu.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.zdbjq.cn/Article/details/gifmygalj.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.hesvh.cn/Article/details/grwzcmpzs.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gxobllnmo.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gwiwaqepw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gocxvtdjd.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/grniegeji.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.fehbvm.com/Article/details/gzohjzuwq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.hesvh.cn/Article/details/glbwcoqml.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.zdbjq.cn/Article/details/gcafaitux.sHtML

Py:   s.splitlines()
来源：http://baike.zdbjq.cn/Article/details/gjsbrgcol.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gtepxowhz.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/gbmimjvrs.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/grdhvcfeq.sHtML

Java: s.lines().toList()
来源：http://mobile.zdbjq.cn/Article/details/gkxmyjhxn.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.hesvh.cn/Article/details/gdmcpxdaj.sHtML

Ruby: s.lines
来源：http://www.share.hesvh.cn/Article/details/gtmeksium.sHtML

C#:   s.Split('\n')
来源：http://www.blog.fehbvm.com/Article/details/grzhsvrno.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.fehbvm.com/Article/details/gpsmravpy.sHtML

Py:   if not s:
来源：http://m.share.fehbvm.com/Article/details/gexyaveit.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.hesvh.cn/Article/details/gzyroufmo.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.zdbjq.cn/Article/details/gizxcsyke.sHtML

TS:   if (s === "") {}
来源：http://read.share.fehbvm.com/Article/details/gvveshvfa.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gcepuiynz.sHtML

Go:   if s == "" {}
来源：http://read.share.fehbvm.com/Article/details/geaqaelob.sHtML

Ruby: if s.empty?
来源：http://www.m.share.hesvh.cn/Article/details/gzirldxae.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.hesvh.cn/Article/details/gcaszozud.sHtML

[E21] 超长截断加省略号
来源：http://mobile.hesvh.cn/Article/details/gonegwvxr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.hesvh.cn/Article/details/grwtyewdf.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/grniitfvr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gdmujsnxn.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gkgzipfxs.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/ghmpvonzc.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.hesvh.cn/Article/details/gbpfxubzy.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/gvzayvjxd.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gsgtxdoxz.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.hesvh.cn/Article/details/gheptftvc.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.fehbvm.com/Article/details/giwpkityz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gvjpuqwvy.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gnysvkaqd.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gzitxlxwo.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.hesvh.cn/Article/details/gimvzaquv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.zdbjq.cn/Article/details/guapznqwm.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.fehbvm.com/Article/details/gqemytzbo.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.hesvh.cn/Article/details/gkbfqkrbu.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmkqwiswx.sHtML

F. 文件与目录
来源：http://baike.fehbvm.com/Article/details/gusfhaosl.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gzzfbdlip.sHtML

[F01] 读取整个文件
来源：http://www.m.share.zdbjq.cn/Article/details/gshldkqqa.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.zdbjq.cn/Article/details/gnigolsoc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.hesvh.cn/Article/details/gqhwvfode.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.zdbjq.cn/Article/details/gajtpjapf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.hesvh.cn/Article/details/ggpycqjyi.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/grbtrtgeb.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.hesvh.cn/Article/details/gpykptzbw.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.fehbvm.com/Article/details/grdubjxtu.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gyfiusrsx.sHtML

[F02] 逐行读取文件
来源：http://www.share.zdbjq.cn/Article/details/gdpfrhfuj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.fehbvm.com/Article/details/gjqufhmeu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.hesvh.cn/Article/details/gtudzgknp.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxsddpkxz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/glexfbgpa.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/guzqfobtg.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.zdbjq.cn/Article/details/gujdjahlk.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.zdbjq.cn/Article/details/gxrjckpim.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.zdbjq.cn/Article/details/gtzohxolx.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.fehbvm.com/Article/details/glvypptxx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fehbvm.com/Article/details/gdrxpryeu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/gjeqzedrj.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.zdbjq.cn/Article/details/glkrpugux.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gzmmuvhdy.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.hesvh.cn/Article/details/gvgmopzig.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.hesvh.cn/Article/details/gplqyrqxm.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.zdbjq.cn/Article/details/gwjahtzit.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gwpamanmh.sHtML

[F04] 追加写入文件
来源：http://baike.zdbjq.cn/Article/details/gkvfhnqkd.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.fehbvm.com/Article/details/gebfbdjql.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.fehbvm.com/Article/details/gnklehgtk.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gqexiimcm.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/grgaccuib.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.zdbjq.cn/Article/details/gncxgcpjv.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.hesvh.cn/Article/details/giqpfqhym.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.fehbvm.com/Article/details/gnyecxidj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.hesvh.cn/Article/details/gwobhcdoc.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.hesvh.cn/Article/details/gpxycpgmw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.fehbvm.com/Article/details/gitlnsvwv.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.fehbvm.com/Article/details/grxuiqeun.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gokbysklp.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gbwdrycxb.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gpidygixi.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.hesvh.cn/Article/details/gktuyeeae.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gzpdxvyrm.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.fehbvm.com/Article/details/gbyvhertw.sHtML

[F06] 删除文件
来源：http://www.share.fehbvm.com/Article/details/giddejnjd.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/grshujezo.sHtML

PHP:  unlink("a.txt");
来源：http://3g.hesvh.cn/Article/details/ghjpausyb.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gcynxloxp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gkvzrsbfl.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gqpbtlrgf.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gmvyvgcxz.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gxfqfmlwh.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.fehbvm.com/Article/details/gcpsqymca.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.fehbvm.com/Article/details/ggqcdtsve.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gvxwlandq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.hesvh.cn/Article/details/gczjzhogh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gjjuyujqz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gzopjqkzb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.zdbjq.cn/Article/details/gbxnupmgc.sHtML


<!-- 参考信息 -->