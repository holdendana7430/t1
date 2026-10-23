代发 wailian999

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3gsftmied.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3fparpkfw.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3fwuusurg.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3tdclddws.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3kmkssysf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xmxycwiy.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3ghysnair.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ehpyfdlc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fgmwlobm.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3pyzrkvli.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3dzggmbgs.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3mmipfemg.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3xgwnhbmo.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3iopqrfbk.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3notbdppv.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3mjwwiyej.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3evukaqgo.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3spnkcbzm.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ajcghxod.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3vogjannx.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3erbrmgwf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3sdjeqako.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3ofsprvbr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3twemehrz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3cfiuxddn.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3diuftghi.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3maskbrqi.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ziyprjcv.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3dwgkwidv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3crywdtqs.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vigozwan.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3pxcpvxbl.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3qeyvatcn.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3nqmqpdec.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3xfwdeddj.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3arqxlewy.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3txamvyfu.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3vzxschhm.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3fsunrygs.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3ndbqciyt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qfnqhntu.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3xjntcwhh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lumrylbn.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wixknblt.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3xtlrgyky.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3twcldrgf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ezdtpscz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3pjswtwgi.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3kfkaiwaz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3umiewmeb.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3vmyugulj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bqnzmxfx.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3luajynib.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3njlkqabs.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3aavzrhbd.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mqccgkit.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3xazmrgwp.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3cfwqlpqp.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qqmoundj.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3zqqgladf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3kjjkfwdd.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3vkhoqvpd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3mwsannme.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3goqvcofq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3sibfrwox.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3kennlmob.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3qjajsgeq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3prvqvwoh.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3dmbtftxr.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3qkyhvqhz.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3gzoamjwp.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3qhxjdvva.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3qtnaqvhv.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3xaggbvzd.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3qcahuenk.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3jdimakdi.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3njpnnkvq.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ftnilcdt.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3khkajefo.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3otuymsta.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3vmtdniwf.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3jxspolji.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3tqrvuwfw.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3dwgwuuzq.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3uyzqjuvg.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3vkwwmrkt.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3iqszxlqx.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3rgjsxilq.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3glcjgkjk.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qhqefean.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3tsknsnps.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3izaknidm.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xhbacoli.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jymmoydb.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3gxiaizrc.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3eqdxbbkd.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3roqbchhk.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3xyxfiqyb.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3yefmrtqk.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3uafsllsk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3dclfoghk.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3nisulkdl.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3xllbqpvx.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3tidwslll.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3hbnwekvw.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3uoiejlga.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3yefvzwml.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3mvjkngoo.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3nxbqqgcr.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3bmspambr.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ooqocuwv.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3tykvkkwr.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3nhnffcmy.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3vgrojusb.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3qaepgysi.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3pbxhzzpk.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3dbijceaf.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3srctrmyz.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3cqqpfkxp.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3pmokxssl.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3tfujwosd.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3endbeetm.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3jqkkykmi.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3xxeldskt.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3hnqkhixx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3szctcvqy.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3wuooywhb.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3puwnnzkm.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3wtyewyae.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3dwzrndpe.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3neatxdrw.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3xofnhsos.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3sjnuxqts.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ivtunpxw.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3mwftmakg.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3izunosfc.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rqkglexj.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3lyrskmxw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3btdjenow.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ivdbgkfn.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3sqspznro.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3eyburjzy.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3vyihqamq.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3nsqvxkrq.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3wmeenpbw.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3tfspmckq.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3awwwzbpw.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3ndhkccnn.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3sxqhgqmp.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3uvstvfke.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3vvnmbffe.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3aomoqtzo.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3aaionroa.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3rryjuacz.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3snowwjpe.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ftjxszdj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3zednferl.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3khsaprut.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3cyuhgfig.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3zplpdkpw.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3kqguuefn.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3xsuanktq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jjbounrj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3knjwftnq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3okflvftq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3swfygnst.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3eiixzise.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3oskfzune.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3zuelwlko.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3rmjgjskp.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3sjfkrgog.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3kgzjxhea.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sycyngox.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3hbeyniky.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3ociwaqyk.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3nggolwdp.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3jksfdexh.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zpfyljbq.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3wknoznft.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3rgznuxkz.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3fcaxhsfx.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3hsipzrno.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3xxvoynue.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3gwtyhhce.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3yquxkwjj.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3gjisixly.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3txgfgqxr.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3xdtaiqwq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3hbtlqlbi.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3gzoynarr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cqenjjgs.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3xkcvmkvm.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3llgqxsub.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3fjhvfbyq.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3wfqeizqg.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3ztdintcx.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3hjghofww.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3hcayvfwa.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3vzvqkexo.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3zegtvmvh.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3lwihqahs.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3tvldanve.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3wawypkmz.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3cvxfuans.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3zzzpnfes.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3bfqinyxz.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3yzuxmnyv.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3knxlnlfy.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3zzkhtqem.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3bnnzfhju.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3lptsvwco.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3xatmdlkr.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3dtgnvsls.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3fphdossy.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3nvgpwdek.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3sjnhhmne.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3uwufvkzd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3ncuwsnsr.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3xaufzlgf.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3snubobcs.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3fiyinnha.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3ysowsvgf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xewuvlry.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3xgcvtxxi.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3mzuurtam.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ippunzml.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3yigaklqv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qdpglirw.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3zydmqeti.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3lnxqosxv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3pdzriyky.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3slpxqjvj.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3nlcqkvlt.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zmsmdytg.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ayosjgem.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3pspovrvn.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3sgqavyqb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3bttjlabk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3efykwluo.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3khfneovu.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3vxpdvnoc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hrrxkkjj.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3xbkjbrrb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pfmhephh.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3axgbcyec.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3uzsbdhdf.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lccminjf.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3dtzpmzpo.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3qjowwsrp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3rlguhfwb.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3aitzvihk.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lxqmwawl.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zujfvjym.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3zedyxqin.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3fhqriknc.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ptbrwkgz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3lnilboza.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fsqfzzpx.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3oibdinwq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3udmqzohr.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3rcfhnulb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3xfskdsjo.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3kyiypqlp.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3yopseyiw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3vkayikil.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ikttriow.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3fzqfapli.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3rnzzxgik.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3ojmiptsf.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3igsbvtze.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3amvuvztm.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3aqddhdgt.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3uepieoch.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3mzhzzhim.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3debfubdk.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3kvyuoznd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3jgtmvexd.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3xsrzshag.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3tfeyauyt.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3acqciblt.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3lkqpkmek.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3wcvdcthz.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vrydntea.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3azwljxpi.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3krzblmmq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3vyhtnyig.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3ixborhqs.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zonufilf.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tggzgtgm.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3rnswctqw.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cmpbjkqv.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rcvbndjz.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fknanpgx.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sywfpchz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3jrvvkxya.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uhecmgts.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tcpcqymu.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tnisrgyw.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3ldddwzmy.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ityfbrry.html


<!-- 参考信息 -->