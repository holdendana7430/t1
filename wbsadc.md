代发 wailian999

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ztucuffq.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2urivaebi.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2fgziceem.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2jxdzwiyc.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2adzjremp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xnxqrdoa.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2knsjjtnn.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nfhboaqt.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2alwtdngw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2lqvtxpfs.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2rqhfukqc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2olfxftlr.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2tcyvnlbb.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2bietzywn.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2pkbrxbvq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2neyhalub.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2npfzpugk.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lwpejdsb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2khnzjofi.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2onyztrcf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2ltljnuuu.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2abedyewt.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2iokxdsox.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2ydvlricb.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2bfzmgyyj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2ecannkcf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2vchcqtyg.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2hfveyrmc.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2boqxsksr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2msetzvzf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2llemrbhk.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2osfayclk.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2caxbpbyz.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2oxpwfaho.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2wmvkblni.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ushshpoi.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2pwvprljy.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2cnwpsxcf.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2cddbriwk.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2govugdnt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wvlsxwqk.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2xamyojux.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zcrverwq.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2wrbwqocc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2eccygacj.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2vvedjdbz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2sgithabv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ducxuqmw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2bdtxilfh.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2hydkpnmv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2vsnvkahd.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dchanzod.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2rtiaulze.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2ocwdmyaw.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jobubilh.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ujzqehii.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2bwlmhzap.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ldcgspft.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2kvjipfqf.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2vkcawmou.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2txarmceu.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2xjphrezv.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2pdgvkbck.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2wlxrcrii.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2qrleucta.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2tyuhmpyh.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2nhvwklhl.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2fmyefkuk.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2fnpldtof.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2ufnjvayx.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2ddzisqpf.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2yibsewua.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2jhykvugp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2mqesvyot.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2mphkonpx.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2uxtomvqr.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2smgwhoky.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2nbvzmecd.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2tsxjgdmm.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2wriuvgnf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jprwzcvi.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2kebkalmq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2dczonihi.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2gdkrytdj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2dipftkgb.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2rgkgbbjo.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2qgjzidcm.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2yfnushcu.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2bfjnudvh.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jlyxrbmj.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2obxshbia.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zrafdoxl.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2offbasmu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qctpbibg.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2ytbaojkl.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hculungt.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vbvipaxe.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2ttrkjwre.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2xophyzzu.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2cdjerckc.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2xyqhjhoi.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2fwdfxxvt.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2ljxsbuxi.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lponpejw.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2pwhrkhmg.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2zbrksneo.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2xkyowygl.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2flixappa.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2tuacbtbi.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2bsduvikb.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2dcnecsco.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2lkzbapbi.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2yucztcle.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2mxsnuptm.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2yvbdtxvm.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2wvaqznjv.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2apwpmmxh.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jenwpazr.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2vscpydxk.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2nhzrjabu.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2gppegnvs.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2lbjmehkr.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2iadeetkd.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2govarbmu.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2mlzexasx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2vjupcvpl.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2lbypudsq.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2wampgcwd.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2xizadxke.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2gjqfkzil.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2lsfnslqk.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2yvtkdtfs.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2dbujqwnp.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2noinyrak.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2vaieautx.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ibsdrgbh.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bdomujpt.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2fdavcigc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2gwcugxjh.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2jatskmjj.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2krfhhofc.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2zxzaktnw.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2xegtiuxl.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2gopynmxt.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2qfxcwwox.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2lrzhnbgc.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ekjzcqib.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2hkotohlt.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2siljtvjs.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2dvoaxrts.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2iubvktjw.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2vyfwxqqg.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2vrdntzbv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2nsrmeime.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2mptnhajt.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2xhmvqwgi.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2wwjpketd.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2gwesfszv.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2aeftkekb.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2woblufve.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2xbasudxy.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2oikdqcsv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xplkzrmn.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2urfxaupg.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qeqtgzpt.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2sjojnmvi.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2lkhiodrq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2keizqnqj.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2qknkgpuz.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2vruqomat.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2smxjeylp.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2pjkvdadv.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2svropyvy.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ajedtbzm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2clohrarw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qypmtvnb.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dzdqxqym.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2avhkqtxf.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2pihfxbhy.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2hkqszqqa.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2adgmxxov.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2eqzctgty.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2frbnqjum.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ituuwibz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2brkktyup.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2lzwrsgwi.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2fknenwwd.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2qykefafu.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2klvvgkxo.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ywenxmhi.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ibsqrhuo.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2anqclxcb.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2lkkjpmog.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2rwlnpbjq.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2oudldwxf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2zwpwsqie.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2mbhhehyc.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2hmdiddlq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2xxsklacn.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2bkylvtub.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2egdktqwt.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2gpliwqbj.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ngdekcwx.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2yjzwvowx.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2eexkrbxu.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2purxcrwn.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2dhldnoqa.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vhozfceu.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2bgnfakaa.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2ntxxqyfv.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ifyvmiyd.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2evydxgcg.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2ysastnut.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2jlvjqmrn.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2rcbtqbnv.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2qnyijbpv.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2iqrqnmvc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2zoayhstl.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2jvpmlect.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2opmkyyia.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2nofkzkkl.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2hwzxetzt.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pzrjxgac.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2oudvamgk.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2bgzreyhn.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2owuypijd.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2hchydokt.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2leglgwks.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2aaxxrdpn.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2kxriytfq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2xcsgmbre.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2askpzgpb.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2ttjmtnnj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2jonycien.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ypovrpro.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2vegrdphg.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2vfwvcfdn.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2bzneruba.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2xivafxvd.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2nwcfjnhm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2quhbafkt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sarznppw.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2zwzttgen.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eiwkufzn.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2yswaincy.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2uwjtknsp.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wsorzguj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2zvzwjrpy.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2rygplrqu.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2agkjofnm.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2dduxfsuo.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zqxximbm.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2iywthcfj.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2wxpoeozg.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2lxiywimu.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2svxsbmaw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sgvigpge.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gtbvvflz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2irbfhexr.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2nrommiza.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2swsdwsrz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2genavfdl.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2cnlpuzev.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2iwcmricw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2pqmeeoux.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2oesefbez.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2vrgjwaco.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2hkkitfkc.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2xmpqulrs.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2rwupvjhb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2muszktpr.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2ilfuxxmr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zfrfahtx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2kcrhkkih.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2eblbenvg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2pkpxolum.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2ctqjagas.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2axllmivy.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2xmkpllws.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2rzcpiwjk.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2adcmetmg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2fudmvpft.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wmrimkaz.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pyvaaadu.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aqectmsg.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2gsbhzfpx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2chcbfxiq.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ekgbomyv.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lzoismpp.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2qgiagrdd.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ufnauzrl.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ryltjcyf.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hhynamda.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kjohcuyn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2qohkhxqo.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qwjcsxsz.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2izznckwd.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vltvrfhk.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2qfriarml.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2tbqvkjxt.html


<!-- 参考信息 -->