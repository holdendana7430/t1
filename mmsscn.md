代发 wailian999

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3gtvueiue.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3ullqezjf.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3urhqjurz.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3aqrnxlns.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3muimkmwn.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tbtpwimk.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3gbrshaeg.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3obetfbsc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vgvfuvhr.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3mxzeskmr.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ocvmbvue.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3gfmnltsg.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3gihdtjwx.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3vqsjzrbu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3aetlgame.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3airastlr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bumlzsxo.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qzevfxvq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3ahattujp.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3janqixce.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3wbhahsfj.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3eqpqrbve.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3eecbjoya.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3vruffrge.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3vtszmref.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3okiszysp.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3mexxpfas.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3pvfpojhx.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3icjuwfyo.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3olzultqo.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3kftdxsrb.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3agutjbze.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3yedwywuu.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pbtcfucp.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3gjfjnesw.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ohzusmru.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3ogwbfeeb.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3wcjvilwb.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ouixwjnm.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3ntootgxl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jwzxzfrq.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3fsamhddv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wjffhxqf.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3szjvpvba.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3twzltpcd.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3bkaskfjf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3lglltojt.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ftjzcuhi.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3smfnejjp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3ixixjqzt.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3zfjtavjx.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fhwsoopk.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3auqfxhgb.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3tuykbacn.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vpntyexp.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3yrxoxawx.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3zinfldhu.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zwlytpyd.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3cgkunung.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3wbnawfbc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3cokxyvul.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3leybmwlt.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3ywzmgclw.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3lryxfdrw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3wtegeztz.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3uzmumsvi.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3wjvfhcob.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3zeubpvhk.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3udrxxigy.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3usyfakqp.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3ghvmauti.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3nyebumkl.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3fsneweza.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3dxvyctye.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3iqpxwvvp.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3qkwzxyme.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3glvnqkgr.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3trhrybob.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3nzghpgpq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3cgzhlffi.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3vqpmcjvr.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3bhkxljyd.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3nkmjjrwn.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3nfqlloav.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3yaifelgw.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3uoyhiyqm.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3hnqzqrxv.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3qgybadta.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3isixbdna.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3oitqycqj.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3gbeuqznb.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ecosaxfa.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hvvguvnt.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3znwblbos.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3tkfsdmzg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3oicrsiyp.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hedxrdul.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3kempjsai.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3wylmhjaz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3rjpzmsvj.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3prnxsgfr.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3ougzqfpb.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3chnkfqes.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nqpyjzzn.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3uouvbooo.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3vciuumzi.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3nzekbpak.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3vbvspytk.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3nabeimlq.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3saufekdz.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3xaqadlzc.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3zmcugnzy.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3tseqpttp.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3apwlqlyq.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3euxlpbbf.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3qhazmwsn.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ynuiczsg.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zuacvixv.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3wzscfrdg.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3tdocjzai.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3sakfqnjo.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3ydueinfg.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3xyaqthdn.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3ecterovb.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3macnxkok.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3vhylfthy.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3ehepgeik.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ijwgtnej.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3rmdwjrhe.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3gwipuiym.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3fakvhdvq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3lliwpsok.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3jbhruwtz.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3blghdetq.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3gyzblmns.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3bkjkvrvq.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kmslgjnf.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3wnvfdzbh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3blrmboxw.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3rsotnqxf.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3gwchsvgd.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ojbiijhr.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3occmapln.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3pxadcxuo.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3lzpkutml.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3ayszfqts.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3jgphdbfq.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3czkrlpbm.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3zmcovjlf.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3koaijolp.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3gmfnjjoo.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3avmrbvkw.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3hvubwjpb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3yqowksob.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3uqgkaujp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3nkdfntdv.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3jbsybnsr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vxfhbqof.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3birkglad.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ucpprlon.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3vaytwamq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3htsumwmv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3pavyiiop.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3bybxpffp.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3wknpxxty.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3hwyzyamf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3cgxixrgi.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3lgzaxocs.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3sbbkvngv.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3jjpsudpj.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ijcdsiyk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3psfwqmdo.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3mlaersso.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3iguysyru.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3hylqgpwt.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3ugrppykm.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uobicphl.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ogbbouso.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3qjjpoolc.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3fwzysank.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3rxnmpmwq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3ifulxvsw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3woucdkhr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3hvjlpijn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3sukdmfwe.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3tqzwytww.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3axkfttha.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3kigwqjvb.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3ethnomqp.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3ziqzenor.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hvcijmsu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3btfclsph.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3oibkrqbp.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3uhxnqhec.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3vizseday.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3xyoemtgu.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3vwgbtuif.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3mglmyshs.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3xypmyzoc.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3nxnzsyux.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3qhdbcfls.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3noqkpfck.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3drogrhsw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3uruyvcyf.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3ndpasbax.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3ialiyqan.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3ydtuflbl.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3btgzetgm.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3iuwjcyua.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3qyuetyrl.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3bdjyzvio.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3bkxbnkjk.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3kcqepzcy.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3bgbdcykx.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3pfdujcyu.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3irjufpjl.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3ofwiazyd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nxmlubyp.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3vilouiae.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fwuarsdo.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3lhhmfztj.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3casfdjhv.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3stppwlii.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3cmplglrs.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3qswlljap.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3zlwueeqc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3yvszwyyv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3inrubaon.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3kgkwyeji.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3peapqfbh.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ywzsiaqi.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3lnkdzbqf.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3oqrzhrug.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3akidcitk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3dhftynbg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3egkmbrzj.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3wlsgjuag.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3siwfwkbj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3zffhiwjd.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3acutyizi.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3vjsruzwt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nashffny.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3vosklqrl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qljycysy.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3mknukrec.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3wnyknyal.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yxqkeice.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3pewnxzri.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3fqadqbuw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3rzhgdhfx.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3mdacavth.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ldctjohh.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tppikjpa.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3jwsjypbi.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3iyrroxhb.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3fnltnpqb.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gucookah.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3cbjtcfyq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3hjegkubf.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3hutdqxbl.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3ycftbfxs.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3cjvfidno.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3dqkeqvyh.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3pgqbqpoa.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3npxttnrl.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ydfkhknp.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3hfwnmzqi.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3rgymeanf.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3tfsurygi.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3ekczoucs.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3utctelmq.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3hrwxqgqx.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3kccxzyhl.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3xnixuzar.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3tcycunfb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3lgzfhkpr.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3aovzddsn.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3qijwqgfq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3mpfziirp.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3bpkgrwlx.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3tjmburfr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3cuotqzny.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3aansepzh.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xsoazbjy.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bdfyqgpv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3xmimnpso.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3spdnlviu.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xxlbpaln.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eegstllu.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3ffuskvar.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cjptrkyj.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3llmgbrro.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jzpvxgcv.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sylhxzhl.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3tiiwkdlk.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bclwwwri.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wstnfxpv.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ubbafypd.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3jxpxslfz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3ttpbcekk.html


<!-- 参考信息 -->