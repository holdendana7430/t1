代发 wailian999

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2sppuqttk.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2lgljlhwi.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2korkhaxl.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2rwmxajwz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2jrfdxmza.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2kltqmgrv.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2qdttsmmh.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2urplyheo.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2qlzictoj.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2lysxwqne.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2mximmzrt.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2pwdxhtiv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2njtwfoqb.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2gxjgdsgi.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2vtqbxahv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2pszihjub.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2fxzrvfci.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2vjearkio.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2yzzdlkpg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2facovzzy.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2cytqgiag.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2cyahgrma.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2iebzzdmi.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uojfytho.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2ntfyxfsl.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2tpnqglem.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2eramirgc.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2zvvzecby.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2vjivcfro.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2ehexajun.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2gxgczwqq.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2bghkwvnh.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2mvdqjidu.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2lofenmhz.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2wfvhproo.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2vrtdxhjp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qybmytpv.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2widwtzcc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2synfwrhh.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2jasrjnel.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2rgkgpqnc.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2bpknguxt.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2sjttfdhj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2cozlpymh.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2nrqzruqg.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2bcjizcac.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2owfwspsz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2onqsihhy.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2vqjqgteg.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2xzpasrwq.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2xzeusyhb.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ogkbbpkk.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2fonmetxl.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kfwswmew.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2oaypjayh.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2jiogfgvu.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2swlqlvxg.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2tzgnzfxf.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2zggszerb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2esmqhcmc.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2wckqtxer.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2adaynrgr.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ygqkkmer.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2yqycuvtx.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2fbwdlhbp.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2cxyzuxro.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2jisbbzks.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2yqtslgwm.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2rbcqerwi.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2ogxeonrz.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2zhefsmdb.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2fzdwopmv.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2tzkvgcwl.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ncavhhfo.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2kbamgbjo.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2fqggdfgz.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2vewpjtsg.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2jgoxlsvg.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2wrsghjad.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2frgddxiu.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2nrpynzep.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2ohnavcpf.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2qijjwfvl.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2deeprjze.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2brbniged.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xvznziii.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2iklxhhia.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2esqkbbmm.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2olpcldqd.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2cqspacqm.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2lfbelofr.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2mhrvqjxa.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2utkhjepo.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2cmpahkvd.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2qicglzxl.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fkhaulef.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2zzwsgpdt.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2quahmvrk.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2twgeljoq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xwxbitxe.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2rlrnvzjt.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2rwomlukb.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2fkvxqtxu.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2dqjljsak.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2dvklzuwy.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2wkkhaitn.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2dhedzvag.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2mqpsfmoo.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2qsqcdpma.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2rmyeuecy.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2bmrgqlwc.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2fejmorzg.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2vorektcu.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bovpzpfh.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2uqrtecyc.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2rdfiywgq.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2bpithpbm.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2qduzpbmn.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2jgvxnkpf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2vgxqcfeb.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2jnediecv.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2hgbiwtqu.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2kxicmazt.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2rfrixsgl.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2mcbcfmtk.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2tyyiznsd.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2zbdiggrb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2njobndll.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2ebbbvjrw.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2lifncvtj.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2xjxssdzj.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mqeugcbj.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jzynsflx.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2zlsutwyf.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2ykvrgkmr.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2jesoavim.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ukeyjgsj.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2pbotavxe.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2ssrlcfof.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2kmzrpckv.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2wdrxmvwx.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2rfjkbvtv.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2fuwzckvp.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2afluqtgj.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2lpwswwvw.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2lxvejngx.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2cfdafdeh.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bckluach.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2ojcrhfyu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2xpbutycx.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2dzjkhcpr.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2bkxesqiw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2fcgbsoil.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wmjnglys.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2sqhyrjrd.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2oanscuhj.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2tcqizrac.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2rtsbdrmh.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2tqfrjsrs.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2kulpbqiu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2powfugvu.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2oczutdpj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2tuauhdja.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2qncwijlj.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2liycvhrp.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2qtmfnnpg.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2lztrjgnd.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2urhysrit.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2rgorqkwp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2nduztdvv.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2iznlwbkv.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2edxjgmcg.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hfautysn.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2myitjood.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2awmdaajt.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2gnbdbveq.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2sosbtvbo.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2xobshhtg.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2rgbsnvhw.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2neveoktf.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2ultbnqzd.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2qjlhmqfx.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2fvohtiwk.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2imuqzsbj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2lafshzuy.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2qoysuqaj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2mgnmbkzk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ucsismsl.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2djwxldoh.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2tpjudnwv.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2qdfsuggr.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2jjhmuxsj.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2gmbmlldl.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2gmhyjljz.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2powihygy.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2xbfzedaz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2iexwagsw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2fvsgmzay.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ubwzrxzh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2mwyketsx.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2gwxlnjfi.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2wpjhyeeb.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2pocmigdn.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nplylqcf.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2kdkabqcp.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2sfbjjdjl.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2terorxbt.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2mqdtnacj.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2aphmaoek.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2vczacdnw.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2pdxhqpcm.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2eeeklydr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2igdmgzbq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2fnhcwqor.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2nhdyerui.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nymlxnou.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2tfpkelqo.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2pjgexpgr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ajtesudc.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2jburrzsa.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2zogylmhw.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2eyafmikg.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2dyfnusti.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2zcfejlkg.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2pmpyirnp.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2okcvqcjy.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xkeyvsmr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2dbafefpv.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2bezrzeuk.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2cfqmqbcy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2sjvowwdk.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2lwczymxi.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ptidenpb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2hnvsqdhd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2wkagvbzr.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ibfpnpht.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2fctfjacq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pvdfzgax.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2kdutpvln.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2puatllko.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ethlkgzl.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2kiwweych.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nwdnefbr.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2cwidazrs.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ohqlcysn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2xwqlyjuo.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2mokuvicj.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yvxrpyng.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2shdnsces.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2yxvnknpz.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2lljkqwek.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2erldlpxs.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tbhualsi.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dklmyiqm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2iifvpcfs.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2lasspirz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2hjoxlhzp.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2tojtwfti.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2lqjsjlil.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2dftkczri.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2dmhpkxhw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2grmongac.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2abemmydx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2yllspwyy.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2xzhmkrae.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2gwhphzws.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2axpgtywx.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2kehrpgpk.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2atirqdkb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2foivnzeb.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2afmchqgo.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2wcpdbcyv.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2guygngoq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2uhermydi.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2njkejlwq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2prryynox.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2pyilrxaf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2ofyfyzpc.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bglpnpvw.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rfuwpnnf.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vbwutrzk.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2gmmrtixg.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2swlnvtrt.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hmhqbgro.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hgezzrdq.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2mbzzpdte.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2idcrtgfa.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2snqdiwbn.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2marfxhuq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2adyczqxv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2rnyiauon.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gfanbpzo.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ipsmcamd.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vvzzdzhp.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2rujajypn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2mumvklrp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2dbualipy.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2xuytueom.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2mwwjfxda.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2bxjczmdz.html


<!-- 参考信息 -->