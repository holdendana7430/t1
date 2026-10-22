代发 wailian999

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2cqiintfn.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2zqvcdhgf.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2smgzqfwy.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2ddkrcggf.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2jaagqzrb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wgmribif.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zzkwhzgp.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2oblkxynw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kazawrpl.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2auqonppm.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2kconcmdy.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2mhvmuvgk.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2ywcgnmwq.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2ziusdaav.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2wqmolpxy.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2dnlltzmt.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ywkiepgk.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2yujjqfyo.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ucutfeyk.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2glpsurpi.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2gtlwixod.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2tsnlshrx.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2pxgqoqlv.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2ghkromdj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2qzfqqnos.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wrqaffau.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2xykqgdkc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2dhqrckqw.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2qilsvahv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2pmtniiqc.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gftyyqtf.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2fhxncspq.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2ogapotfl.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jnshakbl.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2rezhixgp.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ivnzvvwn.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2qpwosqgy.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2uoufyuce.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2isimahdc.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2xdfhbogt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2klnsrqkk.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2dnpgjsag.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ckzpietu.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xntlurwi.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2zjdytpyo.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2hodyeonk.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hflxutfd.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xcxlshqr.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2wcooatcp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2gvavipbb.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2wclruxfi.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2bsrvbcfp.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xiiafohl.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2xfcyzmaj.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2vgjpwbxh.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ieaiarxf.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2mrujapwr.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2hdajvkvj.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2afdotsnd.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2lnnnjcdl.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2suasnwyl.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2jhxfgbnh.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2gerpxnbw.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2gtmflayq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2kjhjzhzk.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2gilvauyv.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2tetgmsze.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2usadwlze.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2zvrlhcjs.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2slwaapcm.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2zyuerspg.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2cfqvmlit.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2cnmaxkgf.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2wtzrothf.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2cvjbgyhw.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2zmgmmxcp.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2yezrfjtq.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2pbzuhdia.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2txhwashd.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2psftbzbu.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jwespnuc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2ohftejsa.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2cmcjruck.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2erbthmur.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2lhrouiao.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2ovzicaqu.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ienqalfc.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2bfjktmmj.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2gqwegahz.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2cjcnjncq.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2awyphxjj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xyltzets.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2yanwqqzp.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vegmcdpy.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2imapcpmw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2weqcbuid.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2akckvgrn.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2syqmksad.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2tpdruhhz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2mjdssbes.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2xsghshct.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2tdnhexmg.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2guyymije.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yxtllnmc.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2wcpfibiz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2yphaghti.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2imkxgyyi.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2mefrnnim.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2csnithjz.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2rsdsfosc.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2izdrgpid.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2jmtciowh.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2hmjlqixu.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ejfsebxr.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2xrirbqug.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2uazpxrso.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2mfxamyck.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2eqdxxqqp.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2oebyiobv.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2tpskbvns.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2emfbtzqw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2fykbvvls.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2tpflshgy.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2jwzwgblx.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2wbvjcqdc.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2cycnngew.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2uhjcqbpo.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2andqigtw.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2hdxzfliy.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2uyobiqwi.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ydxhifmt.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2gdolfqjt.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2petyhihn.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wypxavzu.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2dksyaihq.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hcqfmvmy.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2pdayjheq.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2aggkwbyw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ptbfgiwv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2fhgrrslz.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2vkfmztoq.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2icijprpg.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2dxdzjfcv.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2mgrflqkd.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2rovfpvxj.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2ohufvrkk.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2wicdeyqp.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2bpdwrcem.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2zpklucon.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2mdsnqpwx.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2axutqott.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2lwxggsag.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2rgvjiihx.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2zfcmoorz.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2bzksenpx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2tujjpeig.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2wwyptbuz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2rrzjqmwc.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2qxfwezpp.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2mrohbhfc.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2swiorvrd.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2ubcsvqqb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2bmylacgg.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2rumryevs.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2tjiubmbo.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2vcxgcsez.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2ynyzwysz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2zlxyvjfa.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2refibrwv.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2lktjncjr.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2afhzcarn.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2iiayhylq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tdedeziv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2fopptykj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2xwlvmuas.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wjfblymp.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kwyppmeu.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2yzdujuvt.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2nsbrjzge.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2edaqnvgz.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2whzbzwcz.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2jsrwgutv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2uolzsvoz.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2tzelmexw.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2fiomtwsk.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2dwsvpdvq.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2tlniybko.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2jjpfeobr.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2nrsdgnwp.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2kvmvfqrr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ewjvrrle.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hmdbsvvj.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2kxhhbaip.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2vhrcfhxj.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2pbzakxxf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2jcvkonvp.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2yavbwmcn.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2wsimtevc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2wjlrodvt.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2wzhcuamb.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2cckjuhqp.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2bhnlkjfh.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2dpdgwvvw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2jmnrzvpg.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2nyywzjxy.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2dkldqolf.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2wrpaniwz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pailnmep.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2dtyrstxu.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2jjpmzkqr.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hsvatkjb.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2arnoclep.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2reoydvdj.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2fhzbztbg.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2optqmczw.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2hjeuokgn.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2dgrumfmn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cfehusnc.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2kruyldpb.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2vajhtgae.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2sahnxywd.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2qxylkcgi.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2nwynoomb.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2yurgfsih.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2bgbqezzy.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2nrgzlxxi.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2isftrydo.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ucrpakzq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xapxqgoc.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2tbsxunrk.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2neeufofb.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2nhcmiedd.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2enssffol.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2btxunoxu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ojozsdzp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ngrovsxc.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2vzcnhnzk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2xghlwujg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2qlbgnvsl.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2edzcyhjq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2zcjkoofj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2plmmdczk.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2oqgyzoyp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zxvapewm.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2zztytnxh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2icqzvnrl.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2erthpamo.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2jmgmrjty.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2rthqvhdo.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2jfbvzldj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2vedttazl.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2izktshew.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jkrmiqpm.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2oethwmli.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2nrauemse.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2lcvmrbln.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2vjemyvis.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eqzwkejz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2igyybohw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2srqequid.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2bejemfhp.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2cdmfwalb.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2juxpxcni.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2pgqlzpfa.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2lzbajeiu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2wtmapgyx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2vefudmbu.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2olsltitc.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2bpbfqikc.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2bvpslfmf.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2bmbiuvst.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2qunincxt.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vwsvoaxg.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2kmfhgras.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2udwszxuc.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2nxihdsdt.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2bevcojva.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2xoyjeekk.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2aevphxvu.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2jvpaeitl.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2vnyjajqg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2kitwlutx.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2aweqztpf.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2llwjirof.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ldrpkkiy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2lyptceqw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2nkbwdvpl.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qeprfptk.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2elffpagw.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2uvbzgygk.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pgibzens.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fogqokfj.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qobmmtti.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fndrrdzc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2dkpfetrd.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2skrlzhmm.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hpqynjmh.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ogcuaqdp.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2arppkndc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2zzmgayzf.html


<!-- 参考信息 -->