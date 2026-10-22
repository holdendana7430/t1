代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ovlkveyu.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2xdgxnbsc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2twvjtmhm.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2tvuegzgm.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2iohjcgvd.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2xxxldkzb.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2wapvxppg.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2uzwbasrh.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2ihxbixls.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jhnaflnd.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2adcrnspq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2dkiqmyvc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2afsqyrki.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2kirunkzs.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2qkjkkhup.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2frzunlop.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2uiozkzil.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2orhawmog.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2eamvoghs.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2bamhmzbz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2rucrcrgo.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2xszxfdhc.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2jewxldgu.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2ndprhrmc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2svahgrns.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2kedxbanw.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2nuqjivdo.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2kycjamaw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2zqvbmdje.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2viwriijb.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2ckesyadq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2chzbgtbh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2qjqjinlj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2djqyldmm.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jcxnxipv.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2egpchnfk.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2lotofhsx.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2xvsisqvb.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2teoamygg.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2qabytsyy.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2hfwncdve.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2cbogedmw.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2uitzxwby.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2wcrrmgec.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qkufgkxa.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2cqrqgfcc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2igolipmr.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zhxemcnk.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2ateevphv.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2sgxglgdv.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xnwtcknq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2hecbyhhj.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2yppcgmpv.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2xmclmwqp.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2fsonhimt.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gbxkxokp.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2myiswuug.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2rurfkblt.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nhvqrbnn.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2vtlehkph.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2lrphuuxx.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2mclfuefk.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2oyguvlox.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2qheezoyr.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2xcajeyek.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2ibblgmqn.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2ktmqapnd.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2hhkczrsr.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2xrgnuxtp.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2sbiboroo.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2vgtruanx.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2kjjtqzpa.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2levfvqmb.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2nlnpbpkc.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2rozffrbi.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2xjiwscpl.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2mgduaujn.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2uhcybqfi.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2cslccbmz.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2gzcmomqb.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2qynmkgmn.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2smpcwwal.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wklduopg.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2vjdyinud.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2foetwssp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2pcurrisu.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2gnawxxcw.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2pfdcchoo.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2rprcuqja.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2dicbujbm.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2wuehnudt.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2qxsnoqaz.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2tjctmfdj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2asblegkw.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2dsvqwidk.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hddrbust.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2yuircqso.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2pvfnvrcg.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2eapzyqjg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mevvbllk.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jnsnmifs.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2zkkqzjym.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2cmqwhoee.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2xthabdoc.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2jhsvuuko.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2xwbrovdh.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2rswjxjhw.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lrzalpik.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2vjozcgnr.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2jcblycno.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2qvhiisdv.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2anjbyosb.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2vlrjsspy.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2zaffssjm.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2emxsepyy.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2vxgqrxwk.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2yhwvbnxe.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2jkfyyqmq.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2jupgqebk.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2hdmbndnt.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2qjncggdh.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2epupctmc.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2rrsnlztn.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2tindjivt.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2skrawfmf.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2ntcubadj.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2fdvratpr.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2modgbbxt.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2glagxnyp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2khalfgei.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2wslrxpdn.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2pctfiqcb.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2bcaepkwb.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2petfthur.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ezvdhhoq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2oesqdcri.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2uxmvysmv.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2vpdrgxgf.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2crlcsifj.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ihvamnzb.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2spuvjhtv.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2hrwjlopz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2atyrabod.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2vnhxvqui.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2edhohtbr.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2rmostshu.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2ejpzcdvb.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2rzbnsusa.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2mshqlpit.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2bbygiumo.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2bknjdoxp.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2koytyybu.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2ykxadmpw.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2kpndddqh.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2tatkjmaf.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rbcldfqi.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2xlsjikoz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2ykbgfdtd.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ggiocwyi.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2blnforgb.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2xktoiyvr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2sxhmhqvy.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2jwlcqche.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2tzpytswf.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2llkfqddo.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2olnwvajs.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2kkkdcqtz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2niranxaa.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2irnjsrpw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2woqclejd.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2vwnutpow.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2uyqhajqr.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2hpxxwdmo.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2kgzvwchd.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2gwgoaaue.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2zmytaupt.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qxvyxwnq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2gzogqbdy.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2dwvqqbbj.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2vzzpqymi.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yarmzqtz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2ftitygzv.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2spckfeex.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2faibnfme.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2iuapmzfq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2hdyljntl.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2vxtqhbjp.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2ngcyiupk.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2jctujjks.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2qffustro.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2lumeoypn.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2uhikvsdq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2ztqedsaq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jhengnzn.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2hgdmfxvq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2lbdczeqk.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2lmgreejh.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2hkuybwkk.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2emitgsge.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2eiemogkn.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2pxmvpybh.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2vhlkbbci.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2dahiydqw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2fsupfzql.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2xhwbomzz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2qthzmeig.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2pszhcrhc.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2wdpmsqcf.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2xuczsrsz.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2myoabqve.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2srkyylpm.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2qudgwxfm.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2uqfxzkrt.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2ekhcydqo.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2dkmdoevv.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2oqluvdil.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2otvqkrtf.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2dvteokxx.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2vtixkeer.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2jtlgzqvt.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2yojzkeyl.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2lptjeoye.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2evxmfdiy.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zftmytwd.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2nswkjyod.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2sxqnpxyq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mumpumar.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2nzaxtusv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2taebsknz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ntxtgwqy.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2hqedxiwq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2hzxptxme.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2iserpzvy.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2qvmzdnva.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qdkhloxw.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vknewsue.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2hynpopnm.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rzeynfsh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2srnivjxc.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2clplukek.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2chlkmhdq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2fjhldjia.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2lxjvwqbh.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2spafttur.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2yajwhzkr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yiepeixt.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2uhhxakkr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2owtlsrgm.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2irfpwtri.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2hjravsbg.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lzwlhchw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2mspjjvah.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2cbsewwsn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2xuytzphz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2ltjnfisi.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pjuofxtf.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qwowogdb.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2nhayyphf.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2gurlkwfh.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2hwtzfnmc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2lmzqemiu.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dvfvxmbt.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2elqkdtfo.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2mqpalxhx.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2elqlnbxh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2kyixhytn.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2sgcxqohq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2thjrfjef.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2agopvqwc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2scvkrtqh.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2wzpqhtpf.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2itydzdjp.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2tgssjwqf.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2jyshwgkk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2fbeekvqd.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2mtztncdx.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jfcfvqva.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2anawflbv.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2iwwnbjci.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2gwzeovcm.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2hhtihbxp.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2cfzhowmy.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2yumxgbrw.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2rloqsjuz.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2karietsv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2gtrartdq.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tlukojwn.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2okganlue.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ijpddqdy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2jwtrudse.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2dknmjaqm.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2njcjpgfb.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eeihotmx.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2djxagwvj.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pavmaxxk.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tentipdf.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qelvqnwn.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nanxyiiz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2rgpirofg.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rrgduvte.html


<!-- 参考信息 -->