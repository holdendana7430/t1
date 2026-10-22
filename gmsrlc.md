代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2eeexfoeg.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2wepqjnlj.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2jgnysrxp.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2hodzrtfe.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2xolydpos.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2cgqarekp.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2gzfrvpxc.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2cxudjcae.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2derqzgfp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vztffqec.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2otgjaxid.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kukfpdew.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2hwtugfoy.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2ujayrddf.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2syglsgjq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2uhphlnsa.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2mouoaxdu.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2yoplyhsq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2osegmnon.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jeqcuwmv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zcthupkk.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2eecvscti.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2nejopgij.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2jtxnjtmp.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2vaesvzde.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2kymzfvyh.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2xdmosurw.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2aadsuvji.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2zmcazeid.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2puhlhmmy.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2iunmbsts.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ozlrrxga.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2jsxhosne.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2twormncm.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2cfaconuu.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2ajgenxzy.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2mxksvhfa.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2fdrglmun.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2jlgozajw.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2crmceveh.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2vzzybmyw.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2oabwffmc.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2mnszwlsc.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2elzbsebb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dodwbffy.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2tzsvuzes.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nrbegxau.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ihveohkj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2ekzopcbk.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2yxfvlqbk.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vdteyrru.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ixdbzmia.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2lricihse.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2oeeijddp.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2crrjebte.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2oqitpmkn.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2walabpos.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2txhkwbaa.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xcoopyah.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2dkjahceq.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2mmlmzfbd.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2bcafcedx.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ixwrdwho.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2sijkjkpe.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2aiioxbvx.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2sxxzvqcn.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2yiasmpsk.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2urzstvdu.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2finswmwt.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2mebihvtm.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2taynzisk.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2cxcgpfvl.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2nyquxdpj.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2bgqbqrji.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2oprhgltu.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2fiwlmeva.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2dwgqobzu.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2ioqdxmxg.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2pwqmqwvx.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ntszgopy.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2hngmnijx.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2dbwdccwn.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2esqxlqmw.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2pctxnolw.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2bcvwduiu.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2afkfglyq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2rmccmqrd.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2nwebsrwh.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2kyeoesuw.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2pocfojxi.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2emslvcec.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2danijghb.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2wbnlimfa.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2hymgbqda.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2homzryof.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2myjiyhlz.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2rcvdodsn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rkdhyego.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2uvpzziaf.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2fqruxtlz.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ugbobawf.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2zrywnngw.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2ekzzeaot.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2posycwza.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2zlvvpgel.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2cpipeway.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2ztmaiykv.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2cjufrqmh.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2fnbvzfbe.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2ulbqbhfb.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2ehegpazi.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2qadfnlnn.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2dtlqojfs.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2oajqfnqb.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2oohxpfsn.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2pftscbaa.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2vymcinhi.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2xxdqxttn.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2oojjuvah.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2xgnzgtuk.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2xmkvrdob.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zeehqvqf.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2afwvqfwj.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2bnwmunig.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2xflkwiho.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2xynjfrrp.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2kvdfdqoe.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2yxvyjmov.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2lrkwqtxx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2atoeywjy.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2yccifyou.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2twyuurxi.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2leijhmqv.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2jbdyonoa.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ueneiukl.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2gakouqhz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2bwocqoqw.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2htzoapfi.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2jcsfzfvx.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2erpykgcc.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2nygeoyvy.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2drpvzbwo.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2xqybyobw.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2tvlaatmw.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2tpmzfkdb.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2rjovmtfx.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2fzelljbf.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2qqtwarop.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2nsswtekx.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2lkthyvbs.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2paclzlvb.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2sccaslds.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2qrpjrqnw.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2rddnjwqb.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2bcgujuix.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2ovpuwxpe.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2ofmizrsf.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2mfihbnty.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2wjazpkld.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2vlhsqgyn.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2sbfmmgxj.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zspgngcg.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2dgbknjdu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2xrkjimua.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2flyqubtf.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2nwxeunid.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2qiqsvjht.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2daapaxov.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2lennnjhh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2nxcrhiru.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2ypjdbjsm.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2aftrzlps.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2iceiasdb.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2vdqhodvw.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vqzcveuj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xnrjsock.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lfuicdxl.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2sgakvxim.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2dphlctsl.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2igdlctts.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2wzfgerxg.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2jlxxvkdq.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2etpeucva.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2zyvxwmcn.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2stxaioza.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2eyyfwxxx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2vypdclap.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2muvqjgjy.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2ixmbafjm.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2qqsnlraf.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2cpjlefhz.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2yrquqwtp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2norgksgi.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2vxpfaxli.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2prlfycob.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2wnkwsbln.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2xqjsdreo.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2kpfmjpvv.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2ygyxiagu.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2ynsaewur.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2iwrbvaxh.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2vxjhzing.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2kzwgozhg.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2wpcpvbfy.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2uvaiykvm.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2mvqfmhup.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2qnkozaty.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2mqxsqrzz.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2qppzsoxb.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2frhsvybr.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2bvopoamp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2pfpuzjmf.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2ykqgjkiq.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2efwpjkct.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2zaphrjyw.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2loyuoxxe.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2gkoddmvz.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2ofigsycq.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2slkutzbb.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2oqvwvyix.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2lydxbaem.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ktmamcdt.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2irdszpau.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2gaaivhlc.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2sbtujicv.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2fvgvvczw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2ynkwbqqw.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2zqwfyosk.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2dirxhoeu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ckmugwrs.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2wjtcitfn.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2sigrxabi.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vgvurfpc.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2mazsamdj.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2zukwgjxz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2detwmwgb.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2waemkvmt.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2jeparhow.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2vyvnznka.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2jrfugrvk.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2kpsjbjru.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2gfylhwfl.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2trshhyfe.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2shzrwmth.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2naqdbhyx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ivnyvgfn.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2qubjvqwd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vrppfpzy.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2vdyqhozp.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2orsifmiu.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2orbfsdfi.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2peamasxw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2tlyuxmld.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2iuxffike.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2mmkiswup.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aelgvnih.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jdssfcqj.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2hjlmoggq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2gqtnecsy.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2uvowzzme.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2igzmnyto.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2xfloxxma.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2fmyhblra.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2oenjcipc.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2dyhcuebj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2twbetyzu.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2omhgquua.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2zgdnpoge.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2qpgxlkov.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ilpkrfqa.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2tshgaqlv.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2pgtwaswg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2rierdolp.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2scthcaab.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2njuiunuo.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2nvdnnhao.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rpclvvbf.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2whhpgzom.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2fdqjbsyo.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2oqrxkpkd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2xnheoejp.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2mwotcudj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2lyktgpbh.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2qhtkigoi.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ccjvozmk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2nzdatvlw.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wmgxeklw.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lwgqozpg.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lshdhuey.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2mjyadmip.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2lnrgqbfn.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dqalnvzv.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lsdptdjr.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2okuhzvum.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gnuotfra.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xdgksaqz.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kivbxbsc.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qtqkreqz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2brxocgnn.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fahwqmbr.html


<!-- 参考信息 -->