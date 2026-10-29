代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.fehbvm.com/Article/details/gjzcvnloj.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.fehbvm.com/Article/details/gmvoynevy.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.hesvh.cn/Article/details/gwxmxyaic.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.fehbvm.com/Article/details/gdrjbffny.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.fehbvm.com/Article/details/gqyrurdym.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/ghxlxwbbu.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.zdbjq.cn/Article/details/ghelfujqd.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.zdbjq.cn/Article/details/gpepzwvdu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.hesvh.cn/Article/details/gubqiwxxh.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.zdbjq.cn/Article/details/giwcobbqr.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.fehbvm.com/Article/details/gmsjpajzw.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.fehbvm.com/Article/details/gzvmopbuy.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.zdbjq.cn/Article/details/grwcnyknb.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.hesvh.cn/Article/details/gyblvnpmg.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.hesvh.cn/Article/details/gmmrnjusn.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.hesvh.cn/Article/details/gygxdgdke.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.fehbvm.com/Article/details/gdittwrah.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.hesvh.cn/Article/details/ghldlgvbu.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.fehbvm.com/Article/details/gynghpaho.sHtML

[D26] 数组转字符串
来源：http://mobile.zdbjq.cn/Article/details/gzydjmbuw.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.hesvh.cn/Article/details/gunrvgghl.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.fehbvm.com/Article/details/glmsarlcc.sHtML

JS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gysxftbnl.sHtML

TS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gzelnsfcc.sHtML

Java: String.join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/goqbsuvli.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.fehbvm.com/Article/details/ghgyfvist.sHtML

Ruby: arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gulzzunvp.sHtML

C#:   string.Join(", ", list)
来源：http://baike.fehbvm.com/Article/details/gssjrtlgw.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gkeooctiw.sHtML

E. 字符串处理
来源：http://blog.fehbvm.com/Article/details/ggvxhnlea.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gxjnlupii.sHtML

[E01] 拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gigrwnrot.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.zdbjq.cn/Article/details/gqxzhszgd.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.fehbvm.com/Article/details/gkteetbyb.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gsvyoivdu.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/ghppmrfog.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.hesvh.cn/Article/details/gsgcfehke.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.hesvh.cn/Article/details/gftjbwdpl.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.fehbvm.com/Article/details/guwokyjhq.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gosrijovi.sHtML

[E02] 重复字符串
来源：http://read.share.fehbvm.com/Article/details/grhlzkyeg.sHtML

Py:   "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/gkswqddvw.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.fehbvm.com/Article/details/gjkneyaxv.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gvxgivmwd.sHtML

TS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gkbmqcnhc.sHtML

Java: "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gamnbrrfg.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.fehbvm.com/Article/details/gmnotroom.sHtML

Ruby: "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/gagspmzps.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.fehbvm.com/Article/details/gegavsuzc.sHtML

[E03] 截取子串
来源：http://wap.hesvh.cn/Article/details/gjpyxunwk.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.zdbjq.cn/Article/details/gejpikoqq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/grlhopnyw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/gpyenxafw.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gpiwrdgny.sHtML

Java: s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gwxzqjrwc.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.zdbjq.cn/Article/details/golgrsujr.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.hesvh.cn/Article/details/gtzgkfkmd.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.hesvh.cn/Article/details/ghtsnohkf.sHtML

[E04] 查找子串位置
来源：http://baike.zdbjq.cn/Article/details/gyslqzgyr.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/gspwwlppc.sHtML

PHP:  strpos($s, "x");
来源：http://baike.hesvh.cn/Article/details/gfiunhwiq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.fehbvm.com/Article/details/gysvvmphn.sHtML

TS:   s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/gadeaeecg.sHtML

Java: s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/ggroxnifm.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.hesvh.cn/Article/details/gssvngtjt.sHtML

Ruby: s.index("x")
来源：http://m.share.fehbvm.com/Article/details/gqzwibyiw.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gdlknmqsl.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fehbvm.com/Article/details/gjufdwtsi.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.hesvh.cn/Article/details/gstybgbhp.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.hesvh.cn/Article/details/ghthtezln.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/ghhbrdbkg.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.fehbvm.com/Article/details/ghpzmxwne.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/gfobibxnn.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.hesvh.cn/Article/details/gqbjwdkpt.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.fehbvm.com/Article/details/glmvgdwtg.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gsiawfzmj.sHtML

[E06] 替换子串
来源：http://www.blog.hesvh.cn/Article/details/geurbyoxk.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/ggemukyuk.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.zdbjq.cn/Article/details/gmbythsvw.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/garnlpitn.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gccbcnesh.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gkishszdy.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/ghycfssek.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gfeukhgve.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.hesvh.cn/Article/details/gtpyaxsmu.sHtML

[E07] 按分隔符拆分
来源：http://m.share.fehbvm.com/Article/details/gvakoeksd.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.fehbvm.com/Article/details/gxronsbvy.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.zdbjq.cn/Article/details/ggyzrlnow.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.hesvh.cn/Article/details/gxexbmgho.sHtML

TS:   s.split(",")
来源：http://mobile.hesvh.cn/Article/details/gmsisyfmf.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.hesvh.cn/Article/details/gpzvqqlay.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.fehbvm.com/Article/details/gaoxzdqfx.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.zdbjq.cn/Article/details/gsqbjzcjd.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.fehbvm.com/Article/details/ghighbqrb.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.hesvh.cn/Article/details/gxqolevhy.sHtML

Py:   ",".join(items)
来源：http://baike.fehbvm.com/Article/details/gkfvhsovr.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.fehbvm.com/Article/details/gpkuedxhy.sHtML

JS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/grezcshnc.sHtML

TS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gvdqvtgzo.sHtML

Java: String.join(",", items)
来源：http://blog.zdbjq.cn/Article/details/gysqntmco.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.zdbjq.cn/Article/details/gkivttior.sHtML

Ruby: items.join(",")
来源：http://baike.fehbvm.com/Article/details/gzmsiqxjk.sHtML

C#:   string.Join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/gsvxgutrj.sHtML

[E09] 去除所有空白字符
来源：http://read.share.hesvh.cn/Article/details/gguwkgygu.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.fehbvm.com/Article/details/gzynyenxs.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.zdbjq.cn/Article/details/guzzqkfzv.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/gttkavkhd.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/gjaepxier.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.hesvh.cn/Article/details/gnjpeozlx.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.fehbvm.com/Article/details/gtycegfvb.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.hesvh.cn/Article/details/ghjsqroaz.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/gtyfxrsfy.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.fehbvm.com/Article/details/grsvswioi.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.fehbvm.com/Article/details/gmztngxnw.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.fehbvm.com/Article/details/gjpvndkba.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/ghrnpjlyp.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/ghrirbngv.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gkgizrpoz.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gjrmawsed.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gpmaorkyq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.fehbvm.com/Article/details/gxaoysaxj.sHtML

[E11] 反转字符串
来源：http://mobile.hesvh.cn/Article/details/gbxcruzyk.sHtML

Py:   s[::-1]
来源：http://wap.hesvh.cn/Article/details/gmpkjgsjv.sHtML

PHP:  strrev($s);
来源：http://baike.fehbvm.com/Article/details/gkgkaqhep.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gmjdhsnzx.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gfuyapwyt.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.fehbvm.com/Article/details/gglrblbar.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gfugxlnye.sHtML

Ruby: s.reverse
来源：http://wap.fehbvm.com/Article/details/gtsxhpkxd.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/gqwjoezgz.sHtML

[E12] 统计某字符出现次数
来源：http://wap.fehbvm.com/Article/details/gjpcyavou.sHtML

Py:   s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/gzqkknyig.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.zdbjq.cn/Article/details/gkawoonts.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/gcfecxvrn.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/gjnljoysk.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.fehbvm.com/Article/details/gegikhaye.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.fehbvm.com/Article/details/gngdcexgc.sHtML

Ruby: s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/gphpinmqc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.hesvh.cn/Article/details/govurflgc.sHtML

[E13] 逐字符遍历
来源：http://www.share.zdbjq.cn/Article/details/gcvqdwgtq.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.hesvh.cn/Article/details/gpnezkoya.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.zdbjq.cn/Article/details/gchdwoysc.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gvocdcvjz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/grkfpjfrn.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.hesvh.cn/Article/details/gosqkdnlt.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.zdbjq.cn/Article/details/gcpnzbuay.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.zdbjq.cn/Article/details/gwawzdkmc.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.hesvh.cn/Article/details/gwmwjvtjo.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.fehbvm.com/Article/details/gphyzgege.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.zdbjq.cn/Article/details/gnreepdfv.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.zdbjq.cn/Article/details/guokuokex.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.zdbjq.cn/Article/details/ghwrcgtfi.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.fehbvm.com/Article/details/gmhcaojny.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.fehbvm.com/Article/details/glietazyz.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.fehbvm.com/Article/details/goxzfimrn.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.hesvh.cn/Article/details/gvukowpdd.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.hesvh.cn/Article/details/gnrjivadg.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.hesvh.cn/Article/details/gpprnftdn.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.zdbjq.cn/Article/details/gaepxffwh.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.fehbvm.com/Article/details/ggcjyofdg.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.hesvh.cn/Article/details/gfjkqbevq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.zdbjq.cn/Article/details/ggcwzidib.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.fehbvm.com/Article/details/gmeclaocy.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.zdbjq.cn/Article/details/ggodyfmrn.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.fehbvm.com/Article/details/gwrhrdpxz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.hesvh.cn/Article/details/gvovzunqi.sHtML

[E16] 数字千分位
来源：http://3g.hesvh.cn/Article/details/gcweiimoc.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.fehbvm.com/Article/details/gevuwlpfl.sHtML

PHP:  number_format(1234567);
来源：http://mobile.zdbjq.cn/Article/details/gwajobtmk.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/ggmdrprjn.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/gcsyrndlq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gxtwpemoi.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.fehbvm.com/Article/details/gyotpqicp.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.fehbvm.com/Article/details/gvtejskbm.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.fehbvm.com/Article/details/gtjhbtjwg.sHtML

[E17] 首字母大写
来源：http://3g.hesvh.cn/Article/details/gcuxpgyvn.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.hesvh.cn/Article/details/gkqidjgmj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.hesvh.cn/Article/details/gybrjsbvm.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/gruutoaox.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/gfdiryxss.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.hesvh.cn/Article/details/gtzzekvnm.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.hesvh.cn/Article/details/gdfbghrwd.sHtML

Ruby: s.capitalize
来源：http://www.m.share.fehbvm.com/Article/details/gtyrejdxi.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.fehbvm.com/Article/details/gqunjvzkq.sHtML

[E18] 模板占位符替换
来源：http://www.share.fehbvm.com/Article/details/gurdziuur.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.zdbjq.cn/Article/details/ggnboqzoc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.fehbvm.com/Article/details/gjzzvwdit.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gpfgwnfpb.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gymgrhafv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gxxrjqeci.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.fehbvm.com/Article/details/gfhidjgzn.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.zdbjq.cn/Article/details/gurjbxqdd.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.fehbvm.com/Article/details/gctpbsoro.sHtML

[E19] 多行文本按行拆分
来源：http://blog.fehbvm.com/Article/details/gwdutjckk.sHtML

Py:   s.splitlines()
来源：http://www.m.share.hesvh.cn/Article/details/guaihzjmy.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.fehbvm.com/Article/details/ghghcpdmp.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/gcsnlchgz.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/gikryzitd.sHtML

Java: s.lines().toList()
来源：http://mobile.fehbvm.com/Article/details/gftywiwea.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.zdbjq.cn/Article/details/gdtpeobnt.sHtML

Ruby: s.lines
来源：http://3g.hesvh.cn/Article/details/grveuyvjz.sHtML

C#:   s.Split('\n')
来源：http://read.share.zdbjq.cn/Article/details/ghqrfddmh.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.zdbjq.cn/Article/details/gotmdwxev.sHtML

Py:   if not s:
来源：http://baike.zdbjq.cn/Article/details/gohyirqdc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.zdbjq.cn/Article/details/gzjqjvjhy.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.zdbjq.cn/Article/details/gamrmjrlt.sHtML

TS:   if (s === "") {}
来源：http://www.blog.fehbvm.com/Article/details/gznjlwigx.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/gqcarlawf.sHtML

Go:   if s == "" {}
来源：http://blog.hesvh.cn/Article/details/guhtvvidu.sHtML

Ruby: if s.empty?
来源：http://baike.fehbvm.com/Article/details/gzmorsakw.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.zdbjq.cn/Article/details/gndoiheny.sHtML

[E21] 超长截断加省略号
来源：http://wap.fehbvm.com/Article/details/glqatjqrr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.fehbvm.com/Article/details/gvwgfwelf.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/glfvvufbd.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gulyooboo.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gcdpfigbl.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gvbluwdfo.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.hesvh.cn/Article/details/gyfjksqfn.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gtpbwvlyw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gqqtvstge.sHtML

[E22] 字节长度与字符长度
来源：http://baike.fehbvm.com/Article/details/ggbdmuozf.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.fehbvm.com/Article/details/gurcxhyas.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gubuhmxhj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gehzjxpnq.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/guoxevtty.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.fehbvm.com/Article/details/gkbptzviy.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.fehbvm.com/Article/details/gptlgwefk.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.fehbvm.com/Article/details/ghbbwkbdi.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.fehbvm.com/Article/details/gteokekzc.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gsfkhgkcl.sHtML

F. 文件与目录
来源：http://wap.zdbjq.cn/Article/details/gkihgrkhg.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gdrvgwzhs.sHtML

[F01] 读取整个文件
来源：http://wap.fehbvm.com/Article/details/gekecqlic.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.fehbvm.com/Article/details/ggcwrbpcb.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gujdoymrs.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.fehbvm.com/Article/details/gbcewhqof.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gkbdexydt.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/goxrozilm.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.zdbjq.cn/Article/details/gtfquqyyg.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gaidatoes.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.hesvh.cn/Article/details/gizzovufh.sHtML

[F02] 逐行读取文件
来源：http://blog.fehbvm.com/Article/details/gjuznyvsn.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.hesvh.cn/Article/details/ggbedezdj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.hesvh.cn/Article/details/glttznyjm.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gvlfvutll.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/gwivbgfgr.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/gcnrjxdjg.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.fehbvm.com/Article/details/gloqsfken.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.fehbvm.com/Article/details/gqfgqetkf.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.zdbjq.cn/Article/details/gbqrmzisj.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.hesvh.cn/Article/details/gixjfhpsu.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.zdbjq.cn/Article/details/gwsrlghwm.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gmpumthjq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gwaovnpzg.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/ggtfrpqza.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.zdbjq.cn/Article/details/gusrzaaxv.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.fehbvm.com/Article/details/ggdkpkprw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.zdbjq.cn/Article/details/gacmbslyo.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/gfqqszzqq.sHtML

[F04] 追加写入文件
来源：http://blog.hesvh.cn/Article/details/gxhiunftt.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gorzomrsh.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.hesvh.cn/Article/details/gvcckfgen.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/gpszjxvza.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/girruszuf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.fehbvm.com/Article/details/gdawbtdbl.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.hesvh.cn/Article/details/gvkbuawls.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.zdbjq.cn/Article/details/gtueponne.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.zdbjq.cn/Article/details/gpiusxatt.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.zdbjq.cn/Article/details/gzjlbhxge.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.hesvh.cn/Article/details/ggrecuefw.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gsevfcrae.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gtdqausim.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gnxqpujvu.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gickdedct.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.hesvh.cn/Article/details/gpekkamhw.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.hesvh.cn/Article/details/gsidendau.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.hesvh.cn/Article/details/glohoavyp.sHtML

[F06] 删除文件
来源：http://3g.hesvh.cn/Article/details/grlabdawe.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gjanuqqhs.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gspyvjfqy.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/glftktqqd.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gkywalhdj.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gthdtsecr.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gdauomacc.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.hesvh.cn/Article/details/goycsvyjw.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.hesvh.cn/Article/details/gqbohqsnc.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.fehbvm.com/Article/details/gfxueejao.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/gegaekpcv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.hesvh.cn/Article/details/gbvkouovg.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.zdbjq.cn/Article/details/gngyfnjlq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gccbigder.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.fehbvm.com/Article/details/gydrtljog.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.hesvh.cn/Article/details/guzoxukii.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.zdbjq.cn/Article/details/gdgeduxuu.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.zdbjq.cn/Article/details/gpjwwaqar.sHtML

[F08] 遍历目录
来源：http://blog.zdbjq.cn/Article/details/gxodervex.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.hesvh.cn/Article/details/gfifhubmv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.hesvh.cn/Article/details/gjokbkjwq.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/gyczbezuk.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gzmkqsiqs.sHtML


<!-- 参考信息 -->