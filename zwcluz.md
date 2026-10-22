代发 wailian999

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2rbpxrilo.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2fgmspthb.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2cgotfufa.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2xreyxydp.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2cuiinfkr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2vnnanrxf.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ovejpsmq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2lyzpbsuf.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fmdtblsr.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2rzraquot.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2mjktluwo.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2wynhggez.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2jprcsvln.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2vhaoulxs.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2dmwjydrd.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2zarkohhu.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2cxttqmpq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2lhbfoywg.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2tnrurkry.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2stlodqmi.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2cmgvomac.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2plczxray.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2hfmzsdyr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2humtgnbo.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2xeradvso.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vsueewgd.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2zlsqggde.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2vhxpicnc.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2whkxdvnf.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xkwfjumv.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vsvslawc.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2tahbqkvp.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2wlvzzjnz.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2zbjwneex.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2vktazmau.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2icschhnh.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2itseqcwm.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2lqjdyogo.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2aiptqukz.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2rckmmfby.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2liorelos.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2qsetebmk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tvyerngk.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ymsduhpu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2xgscqken.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mwjjojya.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2yqquvlzs.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2xpvcdtnk.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2acpfakoh.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qapssair.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2balbznnx.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vdetaejb.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uerzsplo.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2fotfxono.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2lsheoaee.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2wpjwpill.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2akiphbpc.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2elxtlpdx.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2zobamzsc.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2drmqwmfv.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2hpmlnusl.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2nqvyenfk.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2ybbeqrid.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2imnarfae.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2uhgrnkfm.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ddzwyhkm.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2srrdejej.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2shyyxyxb.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2jwxlnbxs.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2xjjfcpoe.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2mkypjvwr.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2udktfsed.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2wqrmmuwc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2auafetwo.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2qvthsqcw.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2puptdfeq.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2echoofgw.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ettxsndy.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ouikmmid.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2fbbpglde.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2dxumpzqx.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2nlwyvmjt.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2mzxjprcw.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ijzyryqy.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2vtclukiu.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2mwpronyd.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2kjfumrmy.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2iuwmvzon.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2ykhxhymv.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2ehsryrbu.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2pmhhdgva.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hxwaokjc.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2cxcclawq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2avjmeeyf.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2tgvffwsp.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2chkbzmzk.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2tzqgoqaz.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2bjlivewq.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2pvxcorsu.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zlqulejl.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2ashklrpb.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2wreaoqfm.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2ssjcvyof.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2hslbfuvz.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2rvnlcwjy.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2wukjzstu.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2ootodwxo.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2rjqsndse.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2bpnwispb.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2tjexskjf.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2cdzvvyxt.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2zcdyeybg.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2sbzsqrsw.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2iirjydol.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2jungogph.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2fovanjtd.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2rgawooec.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2wskequbx.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ajdvlniu.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2fecukzoy.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2myfxgndj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2ckbcdwap.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2vkwiyhmj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2dgjolalt.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2nmbwfrwd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2xuwqglhx.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2szyfrxwn.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2einethdk.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2uerarycl.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2hvqcyxbq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2mwnacpbp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2mgauzadw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2nfgpjdgw.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2chupgnho.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2wchhlxjv.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2gcuncdav.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ywfiuahg.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2hvccijro.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2yhpzduwx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2xtjzmymd.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2jvgqkptq.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2gmoqnckt.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2htdilfqm.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2pnrohenl.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2xcswfsxl.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2xydipuba.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2xidfxbrd.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2agodpmcu.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2bsakdhgy.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2dbvyjikd.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2mijjxerd.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2bzeohwvj.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2dljzrsxl.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2bjjoupfl.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2yxwxdpir.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ekepuxws.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2pmysgbtl.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2vnoeiktx.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2upfubbkj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2zlyueube.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2wbcaxhwk.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2nrqmdfqy.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2wojdywrc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2spvommgi.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2gdsfysxc.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ctgalhtb.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2ktqbiwwx.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2wrmqpjgm.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2kwzcubbt.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2ngnbrugh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2feptfaiw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2vrkudnvq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2lvbdedxn.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2lescnvcg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2zzzsndbu.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lnhjvdsw.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2xqktxdwz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iqriyzcn.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2edstbnen.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ptzctiif.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2lbeshyhw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2hdumqtuz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2npwjpdai.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2xhixbiun.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2qqejnoju.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2fciohogq.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2zqnfpzas.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2jnqegklk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2prgtpmrj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2lzjhhpdq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ejlbhrcx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gyybeeux.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2zlacxnll.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2isksvhgi.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2dngvytcl.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2fkepojdt.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2ukfdbpnk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2kvaqpphq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2lvdmjzag.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2fleehmyg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ecjuzqxs.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ufkapszj.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2frumsywq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2qwkcfnwf.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2lpfyxedt.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2xpdhzebi.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2matfgjom.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bobuhukn.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2abvcffzu.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2rpovjosd.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ptnchwyc.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qmvjgqbb.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2zuhaonjv.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2mxzjxbzu.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2ribdmsrm.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2mdvwxrre.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2vyuxonuc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2nbhswsiq.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2nihhnrkn.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ejliwcro.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2mprgtthc.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2zxcchqcl.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eborbxpv.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2nrwkywek.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2suftyeub.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ekcpveiw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2sfmptkml.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2byxpaynm.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2xdhhyvgd.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2hhyeatbk.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gtfsunvx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2siiztryv.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2rtyzunol.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xulzigud.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2wdpbnrhq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2kfthxzrl.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2egwndtsw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2yrgrqvla.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2xxnkdwxw.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2sblqljoz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2grhxnmne.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2flrbefpq.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2ffpzfugn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bebugrem.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2avulhpcm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2kvxpgzts.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hlqgagul.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2kpzllfmf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2vatgelcs.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2yewjbcxf.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2vplhcqko.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fxtfbqma.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rwzdyjqa.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2qnpncvrn.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2azyhpdns.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2gnhiwmce.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2srsylbpd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2jztlknnv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2kvqrjorw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2zwoyxkfw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2kcomzkmu.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2ibhlgkvp.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2sbmpjcgo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ibtpsdiv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2gpwozwom.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2oqsoucnx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2dulnrabz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ehebwkby.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2uyfszews.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2gemdmoku.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2wgncpdkt.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2ujefokpt.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2etdnsjlp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2cxlwjnru.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2caxcrull.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ukbzordf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2ujwazptg.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hmomhbay.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2zpurgsyz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2eujpjozb.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2skrdduaa.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2htmnhapb.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kslxhwez.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ubsnvypi.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2woireccq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2gfnscndc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2irvivfpm.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wmmponbb.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uiseusyr.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2ugkcaylf.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pkyxepwx.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jmwtwqae.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mohyqryb.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rvdeyqlk.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2pfcdtxvy.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mpdyfvls.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kirgkruv.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ejwzfdtd.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2ycybrlao.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2wsxgxmly.html


<!-- 参考信息 -->