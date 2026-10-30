代发 wailian999

Java: String.join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gmlchngon.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.zdbjq.cn/Article/details/gyadxbcxg.sHtML

Ruby: arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/grxzhpgus.sHtML

C#:   string.Join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gjpewjrwy.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/grtqjrggi.sHtML

E. 字符串处理
来源：http://mobile.fehbvm.com/Article/details/gmnvqhtop.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gourszgyd.sHtML

[E01] 拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gjcxddadl.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.zdbjq.cn/Article/details/gofqlbbkt.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.fehbvm.com/Article/details/gqouzbpkg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/gplfzsbku.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/gynvwfgur.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.fehbvm.com/Article/details/ggqsmkkor.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.fehbvm.com/Article/details/gcfspzwkk.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.zdbjq.cn/Article/details/gqzhfpjml.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gnwuklrpc.sHtML

[E02] 重复字符串
来源：http://m.share.hesvh.cn/Article/details/gvphgrzjq.sHtML

Py:   "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/gsrnjljao.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.hesvh.cn/Article/details/gfvsguzrq.sHtML

JS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gwqumdfgo.sHtML

TS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gzcmhryzf.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gfmyigsii.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.zdbjq.cn/Article/details/ggqknoouy.sHtML

Ruby: "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gaceedeln.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.fehbvm.com/Article/details/gleftfotu.sHtML

[E03] 截取子串
来源：http://www.share.hesvh.cn/Article/details/ggivhfpxn.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.fehbvm.com/Article/details/gicmmxoer.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gbiaijvkb.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gmwlyyado.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gzerhaulm.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gbxqqfkhr.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gevvazqhe.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.fehbvm.com/Article/details/gddqrkhhq.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.zdbjq.cn/Article/details/gajsbgcer.sHtML

[E04] 查找子串位置
来源：http://blog.hesvh.cn/Article/details/gzcpvlxeh.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gxustmfgh.sHtML

PHP:  strpos($s, "x");
来源：http://blog.hesvh.cn/Article/details/gdqaskqnf.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.fehbvm.com/Article/details/gpblkhpjt.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/geqytnqjp.sHtML

Java: s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gwclmytqd.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.hesvh.cn/Article/details/gagccddyy.sHtML

Ruby: s.index("x")
来源：http://wap.hesvh.cn/Article/details/gnhzgheup.sHtML

C#:   s.IndexOf("x")
来源：http://wap.fehbvm.com/Article/details/gfglbmird.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.hesvh.cn/Article/details/gsuyalckm.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.zdbjq.cn/Article/details/gstxnmywt.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.fehbvm.com/Article/details/gvqliuilr.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gfqoqzkqe.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.zdbjq.cn/Article/details/gbmuddeoz.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/gtvxhxzbp.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.zdbjq.cn/Article/details/glozgwbxr.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.fehbvm.com/Article/details/gktwrsslo.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gkdpvaohg.sHtML

[E06] 替换子串
来源：http://www.blog.hesvh.cn/Article/details/guizeuwiy.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/gfgmqbrtu.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.hesvh.cn/Article/details/gnbunqpzw.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gvtnbnvij.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/grawpzivg.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gzhgqzaui.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.fehbvm.com/Article/details/gttiessjx.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.hesvh.cn/Article/details/gxhylyndn.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.fehbvm.com/Article/details/gooixuyxt.sHtML

[E07] 按分隔符拆分
来源：http://mobile.hesvh.cn/Article/details/gvmthcnpf.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.hesvh.cn/Article/details/gnmitpkyo.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.fehbvm.com/Article/details/glvuzvqai.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gkmfgnitl.sHtML

TS:   s.split(",")
来源：http://blog.hesvh.cn/Article/details/gsolepaqj.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.zdbjq.cn/Article/details/gpiyvgjoh.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.hesvh.cn/Article/details/galkafico.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.fehbvm.com/Article/details/gjvxobmld.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.hesvh.cn/Article/details/gvqejxjfh.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.hesvh.cn/Article/details/gsycxvgyp.sHtML

Py:   ",".join(items)
来源：http://www.blog.fehbvm.com/Article/details/ggeudrhmt.sHtML

PHP:  implode(",", $items);
来源：http://blog.zdbjq.cn/Article/details/gksiziekn.sHtML

JS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/grpdenycw.sHtML

TS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gnuujeqoz.sHtML

Java: String.join(",", items)
来源：http://baike.fehbvm.com/Article/details/grigkqzxe.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.fehbvm.com/Article/details/gxfhlptft.sHtML

Ruby: items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gapaiiccz.sHtML

C#:   string.Join(",", items)
来源：http://3g.hesvh.cn/Article/details/gfawunaoc.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.hesvh.cn/Article/details/gczqedepl.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.fehbvm.com/Article/details/gowslsmjl.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.hesvh.cn/Article/details/ggocfycsn.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/gdmkrjobg.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.fehbvm.com/Article/details/gmqnxbtdn.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.hesvh.cn/Article/details/ghnvfckuv.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.zdbjq.cn/Article/details/gaiziaeel.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.zdbjq.cn/Article/details/gqfnjoskk.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.hesvh.cn/Article/details/gebcoohji.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.fehbvm.com/Article/details/gdnifpepw.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.fehbvm.com/Article/details/gjexxodmz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.zdbjq.cn/Article/details/gupjwuqia.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gdjnikmpt.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gskzwckkx.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gxsvebazb.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gtixjxwxq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gxawpljtc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.hesvh.cn/Article/details/gfhdusqjl.sHtML

[E11] 反转字符串
来源：http://read.share.zdbjq.cn/Article/details/gfsyumyft.sHtML

Py:   s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/grilrmgkk.sHtML

PHP:  strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/gvnfieojc.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gjqvbckgm.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gedcaismj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.fehbvm.com/Article/details/gbaerwmdx.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.zdbjq.cn/Article/details/gdkcaxvrw.sHtML

Ruby: s.reverse
来源：http://blog.hesvh.cn/Article/details/gmufcqige.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gvpeozgmc.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.hesvh.cn/Article/details/gacrmbvxo.sHtML

Py:   s.count("a")
来源：http://read.share.hesvh.cn/Article/details/gpxinyvfv.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.fehbvm.com/Article/details/gcfykspwn.sHtML

JS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/gctjjlgao.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/gujgqitfe.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.fehbvm.com/Article/details/gqaxghouq.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.zdbjq.cn/Article/details/ghwbpfmgy.sHtML

Ruby: s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gkdltcger.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.zdbjq.cn/Article/details/gvsduxkbq.sHtML

[E13] 逐字符遍历
来源：http://wap.zdbjq.cn/Article/details/gxpwhapej.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.fehbvm.com/Article/details/gmvekjwnm.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.fehbvm.com/Article/details/gvspanmho.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gsovuiloo.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gdmeigghr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gnyqcseuy.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.hesvh.cn/Article/details/gflkdllwa.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.fehbvm.com/Article/details/gbdlssdrl.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.zdbjq.cn/Article/details/gdkwiibzo.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.zdbjq.cn/Article/details/gjmaqloqz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.fehbvm.com/Article/details/gjmojhvby.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.hesvh.cn/Article/details/gdgmvrrks.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.hesvh.cn/Article/details/gstgpzoxw.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.zdbjq.cn/Article/details/gzvsgdbws.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.fehbvm.com/Article/details/ggbrbggto.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.fehbvm.com/Article/details/gokofttsj.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.hesvh.cn/Article/details/grtdjjaal.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.zdbjq.cn/Article/details/gnhuynvzc.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.hesvh.cn/Article/details/gdjnkombn.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.hesvh.cn/Article/details/guxruslew.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.fehbvm.com/Article/details/gascwqnwd.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.hesvh.cn/Article/details/gviwvezhi.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.hesvh.cn/Article/details/gijcdamyt.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.zdbjq.cn/Article/details/gkcxanvsp.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.fehbvm.com/Article/details/gichbapze.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.hesvh.cn/Article/details/grdilyauo.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.hesvh.cn/Article/details/gmukmomfx.sHtML

[E16] 数字千分位
来源：http://3g.zdbjq.cn/Article/details/gyiexpfyx.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.hesvh.cn/Article/details/gsyriqsuk.sHtML

PHP:  number_format(1234567);
来源：http://blog.fehbvm.com/Article/details/gicffgowl.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/ghjcvxjba.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fehbvm.com/Article/details/gkjetqzxe.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.hesvh.cn/Article/details/gjbzegabr.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.fehbvm.com/Article/details/gxgcclbxs.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.hesvh.cn/Article/details/gefeynctk.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.zdbjq.cn/Article/details/gzyezmtta.sHtML

[E17] 首字母大写
来源：http://wap.hesvh.cn/Article/details/gxklutiqi.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.fehbvm.com/Article/details/guiyzjlvj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.fehbvm.com/Article/details/gokpkoqil.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/gclavggne.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gcabvbynb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gihyplofu.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.zdbjq.cn/Article/details/goemirdne.sHtML

Ruby: s.capitalize
来源：http://baike.hesvh.cn/Article/details/gkezarmyz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.fehbvm.com/Article/details/gqfjywmnr.sHtML

[E18] 模板占位符替换
来源：http://www.share.hesvh.cn/Article/details/geopjapxu.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.hesvh.cn/Article/details/gqgmrcoex.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.hesvh.cn/Article/details/gcmipivof.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gyfvegvei.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gpjisisbp.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gaslfwfqx.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gaaiugklu.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.fehbvm.com/Article/details/gazojduoo.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.hesvh.cn/Article/details/gxiylfdzo.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.zdbjq.cn/Article/details/gkkqruxob.sHtML

Py:   s.splitlines()
来源：http://3g.hesvh.cn/Article/details/gscnqlfra.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.fehbvm.com/Article/details/gnbjbigry.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/gjnbzuwab.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/gtodgjxgu.sHtML

Java: s.lines().toList()
来源：http://baike.zdbjq.cn/Article/details/guzankhsb.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.hesvh.cn/Article/details/gebzhzxwq.sHtML

Ruby: s.lines
来源：http://wap.zdbjq.cn/Article/details/gmcujzzsk.sHtML

C#:   s.Split('\n')
来源：http://baike.hesvh.cn/Article/details/gajepnxop.sHtML

[E20] 判断字符串是否为空
来源：http://blog.fehbvm.com/Article/details/gqpphbaqa.sHtML

Py:   if not s:
来源：http://mobile.zdbjq.cn/Article/details/gmqzsosvw.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.fehbvm.com/Article/details/gwwzgxlir.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.zdbjq.cn/Article/details/ghxmpiyit.sHtML

TS:   if (s === "") {}
来源：http://3g.hesvh.cn/Article/details/gdfntuvvs.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/ghyvzwugq.sHtML

Go:   if s == "" {}
来源：http://mobile.zdbjq.cn/Article/details/gpxkpcdlg.sHtML

Ruby: if s.empty?
来源：http://wap.zdbjq.cn/Article/details/gocebflht.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.fehbvm.com/Article/details/gqhlaijks.sHtML

[E21] 超长截断加省略号
来源：http://3g.fehbvm.com/Article/details/gwwxjlabw.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.hesvh.cn/Article/details/gjvffmnrd.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gwgzbacwa.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gamsokqcr.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gzoxhqokg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gwmkxxpuu.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.fehbvm.com/Article/details/guannuacc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/grqxacesq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/gvdxtctcg.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.hesvh.cn/Article/details/gsyhkqjrc.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.hesvh.cn/Article/details/goaedmicw.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gzjzabklu.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/gyskvidxd.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gglmylfed.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.hesvh.cn/Article/details/gvfqqdxfu.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.hesvh.cn/Article/details/gdgxggmot.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gzvsykxna.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.hesvh.cn/Article/details/glvmpyjbu.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gxbflinsh.sHtML

F. 文件与目录
来源：http://mobile.fehbvm.com/Article/details/gjaoyqbef.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gztgxptva.sHtML

[F01] 读取整个文件
来源：http://mobile.hesvh.cn/Article/details/gqwntecuu.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.fehbvm.com/Article/details/gabrbsrve.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.hesvh.cn/Article/details/gxsxydxnx.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.zdbjq.cn/Article/details/gnoftlzno.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.fehbvm.com/Article/details/ggwkuloor.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gxjvvpoeu.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.hesvh.cn/Article/details/gyfzrricc.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gmfaskbzd.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gtjqnrhet.sHtML

[F02] 逐行读取文件
来源：http://www.share.fehbvm.com/Article/details/gdkkiqahb.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.hesvh.cn/Article/details/gzzmybuhw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.zdbjq.cn/Article/details/gybxptiey.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gyyykwhhj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gbvtavmgr.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/gzrkzvjpi.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.fehbvm.com/Article/details/gdtrxfjgy.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.zdbjq.cn/Article/details/gxesgzzzj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.hesvh.cn/Article/details/giytpaokw.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.hesvh.cn/Article/details/gbnfpieor.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.hesvh.cn/Article/details/gjvksbyan.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.hesvh.cn/Article/details/gkxptzdgj.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gtboxwenl.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gcrqxcedk.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.hesvh.cn/Article/details/gaopnrykm.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.hesvh.cn/Article/details/gtdbprwpr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.fehbvm.com/Article/details/gxgghdptx.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gpywmlydl.sHtML

[F04] 追加写入文件
来源：http://wap.zdbjq.cn/Article/details/gfnfixorh.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.hesvh.cn/Article/details/giulyujbb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.fehbvm.com/Article/details/ghgvkutle.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gxfrmirnd.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/gxkgcdgdd.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.zdbjq.cn/Article/details/gbbssrbsq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.hesvh.cn/Article/details/glcnxvgvb.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.hesvh.cn/Article/details/gzvgrakkx.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.fehbvm.com/Article/details/gemytnyfq.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.zdbjq.cn/Article/details/gwruwlzxt.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.zdbjq.cn/Article/details/guqbtpavd.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.hesvh.cn/Article/details/gblhtmsco.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gmbjcqshl.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gdutdqhec.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gjksfxlck.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.fehbvm.com/Article/details/gpoecvfbi.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gvgoarbxy.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.hesvh.cn/Article/details/gefyodsuh.sHtML

[F06] 删除文件
来源：http://wap.hesvh.cn/Article/details/giefrxwqd.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gysgznrey.sHtML

PHP:  unlink("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gwtsddkpo.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gjyqmxvsk.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gxnqypdzt.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gjymjohwj.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gyewysadw.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gkjxiaxtj.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gsvsucdwn.sHtML

[F07] 创建目录（含多级）
来源：http://baike.hesvh.cn/Article/details/gvcpgsupb.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gurgnxles.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.zdbjq.cn/Article/details/ghkizdfkm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gpvbhmcol.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.zdbjq.cn/Article/details/ghkkourye.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.hesvh.cn/Article/details/gmglmppjz.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.hesvh.cn/Article/details/gnkfcwmwt.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.zdbjq.cn/Article/details/gezdvzhli.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.hesvh.cn/Article/details/gmkpvwqxx.sHtML

[F08] 遍历目录
来源：http://www.m.share.fehbvm.com/Article/details/gqzjreesv.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.zdbjq.cn/Article/details/gotneltuf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.zdbjq.cn/Article/details/gvyzbkyjh.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/geghnvckf.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/gxwndlcfu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/gqzptmgbg.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.hesvh.cn/Article/details/gpyzbaopi.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fehbvm.com/Article/details/gzfogehxv.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.zdbjq.cn/Article/details/gslqdyslf.sHtML

[F09] 获取文件大小
来源：http://www.share.zdbjq.cn/Article/details/giixseovp.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gpwzdjiag.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gdezetjuc.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/gysssrmed.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/gpfkscull.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gzzmgftmr.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fehbvm.com/Article/details/gvjqpklau.sHtML

Ruby: File.size("a.txt")
来源：http://baike.fehbvm.com/Article/details/gkervdybg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.hesvh.cn/Article/details/gavtxqzfg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.fehbvm.com/Article/details/gefxgynrl.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gcrznngix.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.fehbvm.com/Article/details/gdvmjzslt.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gjmkoahth.sHtML

TS:   path.extname("a.txt")
来源：http://3g.hesvh.cn/Article/details/gmsboekyv.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.hesvh.cn/Article/details/gxiwpgsot.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gpwhlumgy.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gadctvwrm.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gqllbxuhc.sHtML

[F11] 复制与移动文件
来源：http://mobile.hesvh.cn/Article/details/gwilefwwu.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gjdilcrfo.sHtML


<!-- 参考信息 -->