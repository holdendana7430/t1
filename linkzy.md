代发 wailian999

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2stcykodc.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2jkplqura.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2wtzjxydf.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2sqtpvmho.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2iaeyezna.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2fgznprnk.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2waquniyf.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2dnprkept.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2qilyiggv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2hptdvofv.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2tblsorzj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2kdxdfibh.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2zqghuksn.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2iclbbgja.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2ddgbiati.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2uiqudall.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xeeenrcg.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2uquywxbt.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2mpxpkxcs.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2hmqwmota.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2gwsplwod.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2xjdpvqro.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2dwynstke.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2mtlwutol.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2ulrbyeos.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2ihrpvaei.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2fxbdpsyd.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2cymhkhjj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2salvndqr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2fvojozct.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2nabqeyic.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dxabiwsx.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2leoplphj.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gxbpifdw.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2cxlcvphv.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2oolrruxe.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2ritmtpwl.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2bzjnjaky.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2gqdmxsyc.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2sonifzcg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uzndftkh.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2pqqblpbc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ygsvutxe.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2flgkoyao.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2nqxtbfjq.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2arsogrrp.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ishkfbtf.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2xzkyygcp.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2dvnymfrb.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2iptfybia.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2lbapzslz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ouezczbn.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2jnggouer.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2oegrzlxo.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dgkcyipb.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2lotrxzdv.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2usjhkmcl.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ufuvveyu.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2iiosziye.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2qmkcedfk.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ckvladmp.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2asrecjka.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2bsvwises.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2orcobhkw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2nijssbby.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2gkbdrbum.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2qvnoazcj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2qbvmwoff.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2iunmgzzg.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2hcbhjken.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2bvxiefxo.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qozycacz.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2sbfehvdm.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2swvfsdkf.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2fttftbnx.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2cssunean.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2eeapuskh.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2yuhkjtup.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2aoicwhrd.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2ukaybkmj.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2oyymgczf.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2mrimgegd.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ffufqawz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2lcgychfm.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2cebrqqru.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2rgwfcpgi.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2lcgnhdsm.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2cngqpolc.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2jtvrwqdd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2yzgphhpa.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2diizvliu.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hppunnbh.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2muxsweyb.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2knqnenga.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dvgrunym.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bnxudtvz.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2sgcwdbbl.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2ufpapmyq.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2ttqplkrc.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2yznnimhn.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2szmrigsj.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ylbvadlu.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2ucarpjro.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qivtaujh.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2ychxuthe.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2qjzpqssc.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2opfzxzjv.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2qynmhuoi.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2pzfrvwnt.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2kdwzlfcf.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2yjiurmzq.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2rlojpnat.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2dwuateln.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2vfqmhouo.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2lispaeek.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2wzzzuslk.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2oirwlznt.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2jjwxdngw.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2quptesfs.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2agcdxblv.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2caifxqmg.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2etzqjisf.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2rpedzrey.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2scwburim.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2lqqlbvom.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2knlxgydt.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2zftqnobh.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2lcxztoyh.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2cvgxsqgb.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2zcmqdcwb.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ncdblgby.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2mgrncdus.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2gmlsxfcf.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xdogpfft.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2mwsasogr.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jdanostc.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wbkghaqh.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lisdcyhb.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2bhdunkhf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2ywaiqzbk.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2npzjgbtz.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ytfaoadl.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2hdzasvqb.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2hzmdyuda.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2xowwqhlf.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2zfkfmdnt.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2srkbaolk.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2wywlnfwx.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2cgvwjcio.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2jruiruvs.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2eflgdoss.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2kguvgesk.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2rdblcvcc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2trctlvlb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2xodpxqpd.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2lhpggiqz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2donlxbdt.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2nnslokot.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2dovtymbu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ihlugnuj.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2uzqsvxio.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2igxrysqn.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2bkrtdiyp.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2whhcarrj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2omkmzgyz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2hdvdnjbf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2ujffyand.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2mevmlabl.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2xzanhtwb.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2xkjcbjpb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2nvoeqpzs.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2jngwnfnj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cxmvxzld.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2uifpytid.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2dlxdkqfy.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oapwfjci.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2udivklpa.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qrpzpchp.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ifjwdxhj.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2crmuiava.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2xzadordc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2ylvkowqh.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2tvtxxfxr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2saozpwae.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2cbuawfoh.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2swksedor.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2vwdjjerd.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2rzrpqmwu.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2pzddremz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hrwmkwwo.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zzduvqze.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ylcoiqwz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ykbuaqok.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2kkkzczkg.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2nxwhfxzm.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2pwdrperh.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2kmymfftd.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2omyhzhvu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2iaojtgnp.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2lopswqap.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2peybaqah.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2eayrsyvw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2seukjtxh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2bbapewag.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2gjfpetpu.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2kqjwhrfb.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2vgiybbih.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wpbkdsem.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2kgumzjcw.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2pyhyfrco.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qoprelhu.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2zzpmrinf.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2edcueulh.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2riscashf.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2dmfsfbjd.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2wmrpxitf.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2cicrrsgm.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gnplmqxr.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2hylnafmx.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2nttbdezr.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2ypduwwqy.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2mmrbrwul.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qjtleegn.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2ngktubhx.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2pcvjyuqq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2nvsxnhmp.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2zlqztlse.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2yclmwriu.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2phugwdfh.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2mhkwdepm.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2tfieoczy.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2lhzynucy.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2zzvougvi.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2uzsyeacs.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2wvpdylrl.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2eovqfjaf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2yplsrifd.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2vomygzwh.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2pesatrtr.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2xxrirlxl.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2heilgoup.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xiauzuta.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2iwkwygvk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jgzitzlh.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2xjfgfaar.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2wvbiiazi.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2twyftpzf.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2mhxtriok.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2orzfxyyn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2vbvdwuld.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2vtkclzvg.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tdnxfyhe.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ycbgabmt.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2zbyumbwy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2aglyorqh.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2rxbqjoce.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2pokfpknb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ujcooqkv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2jfdcngsb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2pylcjbro.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2rjdzcpxu.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2oribdhax.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2wgllgrxh.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2dafwyryx.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2ajjupmch.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2qpqmbqvv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ycojrqhq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ovclbsuh.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2haisjjrj.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2zqbqemcm.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2wvqemlix.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2kgkjfekj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2fxpeultq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2bztyxqjy.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2rdzuqewd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2kdstxsws.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2huftnhjw.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2oknwmfbs.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2yngdvjyp.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2pwxvrspl.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2woqyybsi.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2fihmbebb.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lmczdvqx.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tbutqvqn.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kyxpzvvg.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2nkioxtui.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2sphzjgzw.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sexsodnk.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qznpyklb.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2frwybenc.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ebopoewi.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wyalejfk.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kglbmeyi.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dhgcllzi.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2qrqyencj.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oblnadlr.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vsklazul.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ptfnwqgc.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2qpupbrcq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2xrxjxkyd.html


<!-- 参考信息 -->