代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.hesvh.cn/Article/details/gvtiyckic.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.fehbvm.com/Article/details/genfvwcte.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.hesvh.cn/Article/details/gkcpjnbhx.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.fehbvm.com/Article/details/gbqqgkxqa.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.fehbvm.com/Article/details/gqyguylxf.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/geuyxpdft.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.fehbvm.com/Article/details/gedlrwjlf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.hesvh.cn/Article/details/gwaektpvl.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.hesvh.cn/Article/details/ggowppsdq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.zdbjq.cn/Article/details/gemhpzijv.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.zdbjq.cn/Article/details/ghnaxzysj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.fehbvm.com/Article/details/gwidslnoj.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.fehbvm.com/Article/details/gxsulnwzy.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.hesvh.cn/Article/details/gjpwhmabd.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.zdbjq.cn/Article/details/gqmxpkvhw.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/guvltrtgq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.hesvh.cn/Article/details/gtmxvupkn.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.fehbvm.com/Article/details/gzqbvndeu.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.fehbvm.com/Article/details/grrzjllia.sHtML

[D26] 数组转字符串
来源：http://3g.fehbvm.com/Article/details/gesatpxce.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gbtobmetj.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.fehbvm.com/Article/details/gflyyehth.sHtML

JS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gntanvsdp.sHtML

TS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gfpaequbm.sHtML

Java: String.join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gpweozlro.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.fehbvm.com/Article/details/gfstxjubn.sHtML

Ruby: arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/glivntwyx.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fehbvm.com/Article/details/gzdwpbqfs.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvprbmxfc.sHtML

E. 字符串处理
来源：http://www.m.share.hesvh.cn/Article/details/gidtblqfg.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gahcdcenw.sHtML

[E01] 拼接字符串
来源：http://3g.hesvh.cn/Article/details/gtllevdez.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.fehbvm.com/Article/details/gpuossvgs.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.fehbvm.com/Article/details/gpxghlcty.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/gnozacxul.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/goyrqyqbp.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.fehbvm.com/Article/details/gkrmfgzmj.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.zdbjq.cn/Article/details/ghzalvsji.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.fehbvm.com/Article/details/gsqepcxhb.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.fehbvm.com/Article/details/gwgrarzkx.sHtML

[E02] 重复字符串
来源：http://m.share.fehbvm.com/Article/details/gzbqzgpsq.sHtML

Py:   "ab" * 3
来源：http://blog.fehbvm.com/Article/details/gpdjwupur.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.fehbvm.com/Article/details/gcomtftkm.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gunxizatn.sHtML

TS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gwunttzyj.sHtML

Java: "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gsffjazhh.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.hesvh.cn/Article/details/gtlibbnar.sHtML

Ruby: "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/ggwbdebcn.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.zdbjq.cn/Article/details/gnucilxag.sHtML

[E03] 截取子串
来源：http://3g.fehbvm.com/Article/details/gnlwwdoac.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.hesvh.cn/Article/details/gygyqlals.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gzaqyjndz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gsimtmijr.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gfunidvdq.sHtML

Java: s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/giedxlgdf.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.hesvh.cn/Article/details/gavvtmflb.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.hesvh.cn/Article/details/gsakmspbv.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.hesvh.cn/Article/details/gwlhglcfn.sHtML

[E04] 查找子串位置
来源：http://www.blog.fehbvm.com/Article/details/ggkbsgbdf.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.fehbvm.com/Article/details/grmnjlhrt.sHtML

PHP:  strpos($s, "x");
来源：http://wap.fehbvm.com/Article/details/gbohwwyil.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.hesvh.cn/Article/details/gvwowzakr.sHtML

TS:   s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gdjfxpiap.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gorortqzo.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.zdbjq.cn/Article/details/gxjvzeown.sHtML

Ruby: s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/graatoley.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gefufmsvo.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fehbvm.com/Article/details/gpnpcjzuz.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.fehbvm.com/Article/details/gyqcksfsf.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.fehbvm.com/Article/details/gzdbstcyv.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.hesvh.cn/Article/details/gqqomvnsr.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.zdbjq.cn/Article/details/giohubgwt.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gbiinjxbr.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.hesvh.cn/Article/details/glrpfgmck.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.hesvh.cn/Article/details/gtmilvuhz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gycdodahj.sHtML

[E06] 替换子串
来源：http://www.blog.fehbvm.com/Article/details/gtmeahtaf.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/gghatxwwh.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.zdbjq.cn/Article/details/gecolipgo.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gvmfehxik.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gmzkfppsj.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gpbfhnkts.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gqdhfdprj.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/grzmbsura.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.hesvh.cn/Article/details/gyqnzxmnz.sHtML

[E07] 按分隔符拆分
来源：http://m.share.zdbjq.cn/Article/details/giidvygof.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.hesvh.cn/Article/details/gdgzvuzob.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gwozajydf.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.zdbjq.cn/Article/details/gfusgcnxd.sHtML

TS:   s.split(",")
来源：http://blog.zdbjq.cn/Article/details/gaxhopluh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.zdbjq.cn/Article/details/gtidtcfbr.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.fehbvm.com/Article/details/glfarndnu.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.fehbvm.com/Article/details/goybnrvff.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.hesvh.cn/Article/details/guqmhscuw.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.fehbvm.com/Article/details/gljevupyk.sHtML

Py:   ",".join(items)
来源：http://www.share.fehbvm.com/Article/details/gaqsihcue.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.zdbjq.cn/Article/details/gvnykfbzk.sHtML

JS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gaphursns.sHtML

TS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gybfmbelt.sHtML

Java: String.join(",", items)
来源：http://www.share.fehbvm.com/Article/details/gezluokca.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.hesvh.cn/Article/details/guwrnkdqx.sHtML

Ruby: items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gkmqbvkym.sHtML

C#:   string.Join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/gurnjmfzv.sHtML

[E09] 去除所有空白字符
来源：http://wap.hesvh.cn/Article/details/gmkomrsjd.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.hesvh.cn/Article/details/grrzeqpdm.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.hesvh.cn/Article/details/gkujqvjzm.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/gkrfgogcn.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/gajsykcum.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gfpfjxazu.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.zdbjq.cn/Article/details/guslmezvi.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.zdbjq.cn/Article/details/gtookkiso.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.fehbvm.com/Article/details/gwziwibdb.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.hesvh.cn/Article/details/goebbrrju.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/genzrawyk.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.fehbvm.com/Article/details/gkymgonzx.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gywrjujzi.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gfpxefbau.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gxivtqxtv.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gvihemyka.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/guxwgdvsh.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.hesvh.cn/Article/details/geauxmtir.sHtML

[E11] 反转字符串
来源：http://wap.hesvh.cn/Article/details/gjasodacs.sHtML

Py:   s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/gsrfbhvog.sHtML

PHP:  strrev($s);
来源：http://mobile.hesvh.cn/Article/details/ggkxalawj.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/glgxmiuky.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gdpysjlno.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gsxyjfhfs.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.hesvh.cn/Article/details/gqjekqoio.sHtML

Ruby: s.reverse
来源：http://blog.fehbvm.com/Article/details/gtmidxmqa.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gvkwshnsn.sHtML

[E12] 统计某字符出现次数
来源：http://blog.fehbvm.com/Article/details/ggwtfmvlp.sHtML

Py:   s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/gcwheavqm.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.zdbjq.cn/Article/details/gztvwqvsj.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/gcmxnzkvt.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/grmdfcvsx.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.hesvh.cn/Article/details/gnfgpmbqg.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.zdbjq.cn/Article/details/gexvdezrg.sHtML

Ruby: s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/gfzwlsihy.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.hesvh.cn/Article/details/gsoebxkje.sHtML

[E13] 逐字符遍历
来源：http://mobile.zdbjq.cn/Article/details/gbztbgrqm.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.zdbjq.cn/Article/details/guzerpsiu.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.hesvh.cn/Article/details/gdywstwwc.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/gmzussjmv.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/gjlodapue.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.hesvh.cn/Article/details/gvdeskeav.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.fehbvm.com/Article/details/glumwvmts.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.fehbvm.com/Article/details/gfzbubzyi.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.fehbvm.com/Article/details/girvjgchz.sHtML

[E14] URL 编码与 Base64
来源：http://blog.zdbjq.cn/Article/details/gnxhxxilj.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.zdbjq.cn/Article/details/gegggonww.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.zdbjq.cn/Article/details/gkgtghfxb.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.hesvh.cn/Article/details/gxesgxssg.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.fehbvm.com/Article/details/gupkycupk.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.fehbvm.com/Article/details/ggovvzxik.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.hesvh.cn/Article/details/gjxmnmhaz.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.zdbjq.cn/Article/details/gqnczfbpd.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gateygass.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.zdbjq.cn/Article/details/godgdulif.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.fehbvm.com/Article/details/gdjnkdfdx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fehbvm.com/Article/details/gtzxechbv.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.fehbvm.com/Article/details/gzwlbkdnp.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.zdbjq.cn/Article/details/ghmfcguue.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.hesvh.cn/Article/details/gcmkdigsy.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.fehbvm.com/Article/details/gzdcdsrnj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.fehbvm.com/Article/details/gdujemwju.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.hesvh.cn/Article/details/gcxfhcjtw.sHtML

[E16] 数字千分位
来源：http://3g.zdbjq.cn/Article/details/gscgihndc.sHtML

Py:   f"{1234567:,}"
来源：http://baike.zdbjq.cn/Article/details/gxakwfiwi.sHtML

PHP:  number_format(1234567);
来源：http://wap.fehbvm.com/Article/details/gopodjgzy.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/gluieqfvm.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/gmgveslky.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.fehbvm.com/Article/details/gpyxtfldp.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.hesvh.cn/Article/details/grenurnvm.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.fehbvm.com/Article/details/gyoykjlbg.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.zdbjq.cn/Article/details/gdzqqbqdb.sHtML

[E17] 首字母大写
来源：http://www.share.fehbvm.com/Article/details/gncewjglq.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.fehbvm.com/Article/details/guucwiwpc.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.zdbjq.cn/Article/details/gosshrxin.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/gazspckdh.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/gcjmzgxbg.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.fehbvm.com/Article/details/gkharmwfr.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.fehbvm.com/Article/details/gwvjbxcci.sHtML

Ruby: s.capitalize
来源：http://read.share.hesvh.cn/Article/details/gubzzxljm.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.fehbvm.com/Article/details/gnjtuobul.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fehbvm.com/Article/details/gmbbxthlr.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.hesvh.cn/Article/details/gzbuwfsjg.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.zdbjq.cn/Article/details/gtqobajlc.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gkkhobwcx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gldkelopy.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/ginqeukrx.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gexxwjplj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.hesvh.cn/Article/details/gnyzxoaqc.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.fehbvm.com/Article/details/gxjwrddlq.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.fehbvm.com/Article/details/gpoeelvcb.sHtML

Py:   s.splitlines()
来源：http://www.share.zdbjq.cn/Article/details/gzapsubiy.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gqbuvhvwr.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gfoxyzbfv.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/gsfcsbmsi.sHtML

Java: s.lines().toList()
来源：http://3g.fehbvm.com/Article/details/gqjxlsbuy.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.fehbvm.com/Article/details/gyhjsneqg.sHtML

Ruby: s.lines
来源：http://www.blog.hesvh.cn/Article/details/grkieejjt.sHtML

C#:   s.Split('\n')
来源：http://3g.hesvh.cn/Article/details/gtdwuqenb.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.fehbvm.com/Article/details/gengecwun.sHtML

Py:   if not s:
来源：http://www.share.zdbjq.cn/Article/details/gpwsnompf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.hesvh.cn/Article/details/gocidpiuy.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.hesvh.cn/Article/details/gwhfteihw.sHtML

TS:   if (s === "") {}
来源：http://read.share.zdbjq.cn/Article/details/gmpeelije.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/gfljrakvy.sHtML

Go:   if s == "" {}
来源：http://www.share.hesvh.cn/Article/details/gfckpgenj.sHtML

Ruby: if s.empty?
来源：http://m.share.zdbjq.cn/Article/details/gjeoahcke.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.zdbjq.cn/Article/details/gtkcpvoxn.sHtML

[E21] 超长截断加省略号
来源：http://wap.fehbvm.com/Article/details/gmilqovlx.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.hesvh.cn/Article/details/gzwkmvqrw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gzuqrddny.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gayeuklls.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/grvseuegm.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gtjzlokvh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.zdbjq.cn/Article/details/gllmypmtp.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gtjezgmjl.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gcicijknx.sHtML

[E22] 字节长度与字符长度
来源：http://blog.zdbjq.cn/Article/details/gxfapqhtv.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.zdbjq.cn/Article/details/gkohmtxcn.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gzrwdpzor.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/ggfgpekar.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gjwwuhnde.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gjwxyxwyj.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.zdbjq.cn/Article/details/gotjekexg.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.hesvh.cn/Article/details/gdsfhyxhy.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/ggknzvpuj.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gbtjdifzx.sHtML

F. 文件与目录
来源：http://read.share.hesvh.cn/Article/details/ghfyasdhx.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gojktbyxo.sHtML

[F01] 读取整个文件
来源：http://mobile.hesvh.cn/Article/details/guhbsrbyv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.hesvh.cn/Article/details/gogiqeova.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.fehbvm.com/Article/details/gnlfxgpph.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.hesvh.cn/Article/details/gdujswtjs.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gtvdmmzvw.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gymboulgp.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.hesvh.cn/Article/details/gpyctfmjs.sHtML

Ruby: File.read("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gtygyszij.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gsfvjfsxk.sHtML

[F02] 逐行读取文件
来源：http://baike.fehbvm.com/Article/details/gdqqjqsji.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.hesvh.cn/Article/details/gjrlzlbvq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.fehbvm.com/Article/details/gokkgcyvl.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gduxbmaoj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/gzwxzktyl.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gplgwstcz.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.fehbvm.com/Article/details/gvvuaxwmo.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.hesvh.cn/Article/details/gxcwyewzv.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.zdbjq.cn/Article/details/gagmreyvm.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.hesvh.cn/Article/details/galpzmkgk.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.zdbjq.cn/Article/details/gogpopsng.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.fehbvm.com/Article/details/glgcehcoi.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gmjovtdor.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/goljdsznq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.zdbjq.cn/Article/details/gxuimdain.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.fehbvm.com/Article/details/gwlppltti.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.fehbvm.com/Article/details/gsghwwiuw.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.zdbjq.cn/Article/details/giotjeoyq.sHtML

[F04] 追加写入文件
来源：http://blog.hesvh.cn/Article/details/ghitqxoki.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.hesvh.cn/Article/details/gtxgrlkbr.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.hesvh.cn/Article/details/ghzdpgrly.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gbceopqtl.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gbtsqhkxq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.zdbjq.cn/Article/details/gtvvzgvzj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/ghrzgodhl.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.zdbjq.cn/Article/details/gfbfqfcfk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.hesvh.cn/Article/details/gxnwlcske.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.fehbvm.com/Article/details/ghodxxpeh.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.zdbjq.cn/Article/details/gfrtdldxd.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.fehbvm.com/Article/details/goeodgpyh.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gftvqinbi.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/ghcrrzrkf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gctojjqqs.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.hesvh.cn/Article/details/gigoagbik.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.fehbvm.com/Article/details/guulhekuk.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gxtlgnjmn.sHtML

[F06] 删除文件
来源：http://blog.fehbvm.com/Article/details/gsczhezbd.sHtML

Py:   os.remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/goovvjian.sHtML

PHP:  unlink("a.txt");
来源：http://3g.fehbvm.com/Article/details/gbfvsgtyw.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gdresjcjd.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gmhkrtknr.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gfytzgajn.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/geobnrmfu.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gzkampvfg.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.hesvh.cn/Article/details/gcaniuhcl.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.fehbvm.com/Article/details/gqlxrbvsp.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gmoznqtuo.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.zdbjq.cn/Article/details/gektumhzz.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gscvzktrb.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/guucatzqd.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.zdbjq.cn/Article/details/gyzughcry.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.hesvh.cn/Article/details/gruqseois.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.zdbjq.cn/Article/details/gohnjqwft.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.fehbvm.com/Article/details/gqvuqshnk.sHtML

[F08] 遍历目录
来源：http://blog.hesvh.cn/Article/details/gfbticlvy.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.hesvh.cn/Article/details/gyguigmfe.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fehbvm.com/Article/details/gycyrvqyf.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gzpenlhsi.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gfsytmzyo.sHtML


<!-- 参考信息 -->