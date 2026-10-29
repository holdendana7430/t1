代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.fehbvm.com/Article/details/gamrfnpkq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.hesvh.cn/Article/details/gtfhhecmp.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/geryzeozv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.hesvh.cn/Article/details/gmwbtfbnr.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/ggoymlkxf.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.fehbvm.com/Article/details/gajyyvgpu.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.fehbvm.com/Article/details/gxwooxbng.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.fehbvm.com/Article/details/gscnkigns.sHtML

[E06] 替换子串
来源：http://m.share.hesvh.cn/Article/details/ggjcbmmyg.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/gqrvxbiew.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.zdbjq.cn/Article/details/gekwopgsr.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gpwuqdykk.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gysatmrnv.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gvvrmwkrv.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/gszbncqra.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.hesvh.cn/Article/details/grswssbvg.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fehbvm.com/Article/details/gusqlamna.sHtML

[E07] 按分隔符拆分
来源：http://blog.zdbjq.cn/Article/details/grvlhxnem.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.zdbjq.cn/Article/details/ggsydmsly.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.fehbvm.com/Article/details/gklvztbgy.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.zdbjq.cn/Article/details/gdaudqpyy.sHtML

TS:   s.split(",")
来源：http://m.share.fehbvm.com/Article/details/gdvdvxlds.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.zdbjq.cn/Article/details/goggearxs.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.fehbvm.com/Article/details/gvblpdeqt.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.fehbvm.com/Article/details/gkzgowitl.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.fehbvm.com/Article/details/gqmcheqxn.sHtML

[E08] 数组按分隔符合并
来源：http://3g.zdbjq.cn/Article/details/gobdxqwzr.sHtML

Py:   ",".join(items)
来源：http://3g.fehbvm.com/Article/details/gtqphsxgn.sHtML

PHP:  implode(",", $items);
来源：http://wap.zdbjq.cn/Article/details/glhbrzfgk.sHtML

JS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gmqlqowef.sHtML

TS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gttkdnhtd.sHtML

Java: String.join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/goyzovljw.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.zdbjq.cn/Article/details/gcjjtnkpp.sHtML

Ruby: items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gwcehaylt.sHtML

C#:   string.Join(",", items)
来源：http://m.share.hesvh.cn/Article/details/gfapdktsc.sHtML

[E09] 去除所有空白字符
来源：http://read.share.fehbvm.com/Article/details/gnvlkzgmz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.fehbvm.com/Article/details/gdczxdkjr.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.zdbjq.cn/Article/details/gqyobrhsn.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/gohvdvtiw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.zdbjq.cn/Article/details/gedfyzvzl.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.hesvh.cn/Article/details/gmtbxlbqd.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.fehbvm.com/Article/details/gilosizhr.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.hesvh.cn/Article/details/gkwfpofbu.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.fehbvm.com/Article/details/gqysohagh.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.zdbjq.cn/Article/details/geloiuemw.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gnaaradtd.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.hesvh.cn/Article/details/gpscgbwte.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gbxqfbdvi.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gbsxpwzpk.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/germuloef.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gfbsdmhvx.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gnntsxaum.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.hesvh.cn/Article/details/gvfoiucmt.sHtML

[E11] 反转字符串
来源：http://m.share.fehbvm.com/Article/details/gumhkgiao.sHtML

Py:   s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gaszcvryb.sHtML

PHP:  strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/gtgctzfng.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gagyfcmds.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/ggqaerpdn.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.hesvh.cn/Article/details/gkoibalob.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gzcsgvlai.sHtML

Ruby: s.reverse
来源：http://read.share.hesvh.cn/Article/details/grmovhtoa.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/glpwixkmu.sHtML

[E12] 统计某字符出现次数
来源：http://baike.fehbvm.com/Article/details/gcunygdjb.sHtML

Py:   s.count("a")
来源：http://read.share.hesvh.cn/Article/details/gjehuhvsz.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.zdbjq.cn/Article/details/gprzlghcc.sHtML

JS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/ghqqykzhc.sHtML

TS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gdpdrhleu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.zdbjq.cn/Article/details/gpcbgkkvh.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.zdbjq.cn/Article/details/gyuijwcrq.sHtML

Ruby: s.count("a")
来源：http://3g.hesvh.cn/Article/details/gjhyenbse.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.zdbjq.cn/Article/details/gqhkkjwdm.sHtML

[E13] 逐字符遍历
来源：http://www.share.fehbvm.com/Article/details/gwrfoelpl.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.fehbvm.com/Article/details/gwygkadvy.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.fehbvm.com/Article/details/gojwvegun.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/glisqnveh.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gwbxxyqws.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.fehbvm.com/Article/details/gctwajsxm.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.zdbjq.cn/Article/details/gzjyzjksi.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.hesvh.cn/Article/details/gwpdgmlds.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.zdbjq.cn/Article/details/gkvsdocwr.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.hesvh.cn/Article/details/gzpevkijj.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.fehbvm.com/Article/details/goarhiror.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.hesvh.cn/Article/details/ghxmcaovl.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.zdbjq.cn/Article/details/gukikzpub.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.zdbjq.cn/Article/details/gmqhgqocz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gzybxmflp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.zdbjq.cn/Article/details/gjkhjbast.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.zdbjq.cn/Article/details/gfweajhgf.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gdztjcbwn.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.fehbvm.com/Article/details/gnywybupp.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.fehbvm.com/Article/details/gmkqbzarx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fehbvm.com/Article/details/gcujzsfcn.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.hesvh.cn/Article/details/gaytmsycs.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.fehbvm.com/Article/details/gutoocnjp.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.fehbvm.com/Article/details/gtowuqdpc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.hesvh.cn/Article/details/gmcomgmeh.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.fehbvm.com/Article/details/gjouhcdnm.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.hesvh.cn/Article/details/gcxjxokaz.sHtML

[E16] 数字千分位
来源：http://baike.hesvh.cn/Article/details/goggqwluw.sHtML

Py:   f"{1234567:,}"
来源：http://baike.zdbjq.cn/Article/details/ghvakmlgx.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.hesvh.cn/Article/details/gbssjdciw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/gdkiesqif.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/gtdpvicgq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.fehbvm.com/Article/details/gowsiqtsv.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.zdbjq.cn/Article/details/gnthnkwnd.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.zdbjq.cn/Article/details/ggebkfrvp.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.fehbvm.com/Article/details/gqkgpnket.sHtML

[E17] 首字母大写
来源：http://wap.hesvh.cn/Article/details/gkpajpwdz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.fehbvm.com/Article/details/gpedrtszf.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gunlhzuax.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gpuvpbrdk.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gofkvsmal.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.zdbjq.cn/Article/details/gtjkggrdd.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.hesvh.cn/Article/details/gawlghukx.sHtML

Ruby: s.capitalize
来源：http://mobile.fehbvm.com/Article/details/gobaqejio.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.hesvh.cn/Article/details/grgpwfoin.sHtML

[E18] 模板占位符替换
来源：http://mobile.fehbvm.com/Article/details/gjtsaivmd.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.fehbvm.com/Article/details/gtjikijfb.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.zdbjq.cn/Article/details/gmmuemnfi.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gzakllbde.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/glqntmsqb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gjhumdyah.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.fehbvm.com/Article/details/grryzrwhh.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.fehbvm.com/Article/details/gczxwazyo.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.fehbvm.com/Article/details/guyvblbuq.sHtML

[E19] 多行文本按行拆分
来源：http://blog.hesvh.cn/Article/details/gflwmtwyt.sHtML

Py:   s.splitlines()
来源：http://www.share.fehbvm.com/Article/details/gdlmtkbdx.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.fehbvm.com/Article/details/gnyvsbpxg.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/gnowaphhx.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/guvpmdmbs.sHtML

Java: s.lines().toList()
来源：http://baike.fehbvm.com/Article/details/giixcbftk.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.hesvh.cn/Article/details/glmgayrym.sHtML

Ruby: s.lines
来源：http://read.share.zdbjq.cn/Article/details/gbgcpkrhw.sHtML

C#:   s.Split('\n')
来源：http://blog.hesvh.cn/Article/details/gvoedkhti.sHtML

[E20] 判断字符串是否为空
来源：http://wap.fehbvm.com/Article/details/gfqubktya.sHtML

Py:   if not s:
来源：http://3g.hesvh.cn/Article/details/gyhiuqykj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.zdbjq.cn/Article/details/glwcbzswp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.fehbvm.com/Article/details/ghbkuqooc.sHtML

TS:   if (s === "") {}
来源：http://baike.fehbvm.com/Article/details/gqekisbxp.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.zdbjq.cn/Article/details/gibhaquwv.sHtML

Go:   if s == "" {}
来源：http://wap.fehbvm.com/Article/details/gonhppkbz.sHtML

Ruby: if s.empty?
来源：http://www.share.fehbvm.com/Article/details/gedlkxkma.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.hesvh.cn/Article/details/gqrglkofs.sHtML

[E21] 超长截断加省略号
来源：http://read.share.hesvh.cn/Article/details/geshxhjyc.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.hesvh.cn/Article/details/gwkpbbmzt.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gvydexibg.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gaktyekrl.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gujzosjib.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gzmhukcgz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.zdbjq.cn/Article/details/glpinquhc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/glomqabgu.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gfjiwobfd.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.zdbjq.cn/Article/details/ggujnebut.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.hesvh.cn/Article/details/ggqcgtnna.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gvvddoxfk.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/gtvumaife.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/guyyaumeq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/gmmbtpqhn.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.fehbvm.com/Article/details/goilmumtt.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.hesvh.cn/Article/details/gwfwacwkt.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.hesvh.cn/Article/details/gnlapijdo.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/giiegykye.sHtML

F. 文件与目录
来源：http://mobile.zdbjq.cn/Article/details/gyqzcmvtb.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gumagqwfz.sHtML

[F01] 读取整个文件
来源：http://mobile.hesvh.cn/Article/details/grnfkirtu.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.zdbjq.cn/Article/details/gdndbgana.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gkpkesuxh.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.fehbvm.com/Article/details/grqqlmaqp.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/ghplmqdyg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gipgjkxkd.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.zdbjq.cn/Article/details/gkmqextmi.sHtML

Ruby: File.read("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gqmupkbza.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gnzjmkjtx.sHtML

[F02] 逐行读取文件
来源：http://mobile.fehbvm.com/Article/details/glcxobffa.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.hesvh.cn/Article/details/gggnpdedn.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.zdbjq.cn/Article/details/gxissjyum.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gzgekmhev.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/gcvulwoad.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/gfzatfoov.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.zdbjq.cn/Article/details/gxkblybpo.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.zdbjq.cn/Article/details/guhfxrqqz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.fehbvm.com/Article/details/gqisurxuc.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.hesvh.cn/Article/details/gtdxzridb.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fehbvm.com/Article/details/gdozurkcv.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/goxmvylfu.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gmblohxwa.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/gizslesgh.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.fehbvm.com/Article/details/gmkixqwvh.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.fehbvm.com/Article/details/gxjgfadlo.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.hesvh.cn/Article/details/gtqmtohzt.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/gtufkxeuv.sHtML

[F04] 追加写入文件
来源：http://3g.fehbvm.com/Article/details/gezkojaci.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.zdbjq.cn/Article/details/gbhpgelhe.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.zdbjq.cn/Article/details/gfimyirpn.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/gjfydgmpf.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gbujsdoyo.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.fehbvm.com/Article/details/gdzcngptp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.hesvh.cn/Article/details/grinegonq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.fehbvm.com/Article/details/gduepoopk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.fehbvm.com/Article/details/gpgrvhjtm.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.hesvh.cn/Article/details/gujzkroed.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.hesvh.cn/Article/details/gucmzeuvp.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.fehbvm.com/Article/details/gnfucyqfn.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gomfzntss.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gdggzzrcr.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/ghftamleh.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.zdbjq.cn/Article/details/gwfrgsppu.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.fehbvm.com/Article/details/glqmztost.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gpswkubzi.sHtML

[F06] 删除文件
来源：http://m.share.zdbjq.cn/Article/details/gsurbmuce.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gjbpumhfp.sHtML

PHP:  unlink("a.txt");
来源：http://wap.fehbvm.com/Article/details/grdpxqznz.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/glalifvtk.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gkbsuytmu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gtsuthzdi.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gjjqmbeke.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gdunltfrp.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gkyqrikjq.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.hesvh.cn/Article/details/gkduinskm.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gjojxxlyq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.zdbjq.cn/Article/details/gthgzcbow.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/gyadgsywl.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gklfpzzxr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.hesvh.cn/Article/details/gyoxgyxok.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.zdbjq.cn/Article/details/gnfyjucwj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.fehbvm.com/Article/details/gwvlscuss.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.fehbvm.com/Article/details/grcdkceay.sHtML

[F08] 遍历目录
来源：http://blog.fehbvm.com/Article/details/gvldrfrmj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.zdbjq.cn/Article/details/gbwgeikhz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.fehbvm.com/Article/details/gvxppqpqj.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/gwnsyycml.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gwcsgqqiz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/ggsypchnc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.fehbvm.com/Article/details/gdgufhkri.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/glralnbgy.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.zdbjq.cn/Article/details/gytpulgbt.sHtML

[F09] 获取文件大小
来源：http://mobile.fehbvm.com/Article/details/gsssawigv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/guljyhmzm.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gfhvujjub.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/gbmuxthjp.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gukgoirvm.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gupmsaazh.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.hesvh.cn/Article/details/gvbmfxptj.sHtML

Ruby: File.size("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gtpeszxfz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.fehbvm.com/Article/details/gmwpufdbz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.hesvh.cn/Article/details/gahidhyhe.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gxrcukttb.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.zdbjq.cn/Article/details/gjuwwehms.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/giifnvtgr.sHtML

TS:   path.extname("a.txt")
来源：http://3g.fehbvm.com/Article/details/gofehoois.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.hesvh.cn/Article/details/ghahfikin.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/grmsjiozu.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/ggkpupxez.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/giylokawv.sHtML

[F11] 复制与移动文件
来源：http://read.share.zdbjq.cn/Article/details/gocrorrda.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/ggznwqcuu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.hesvh.cn/Article/details/gviajgzdu.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/guchilfqk.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gzcvttuws.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gamsjfezn.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.hesvh.cn/Article/details/giciokjgx.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gawyuaevt.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.zdbjq.cn/Article/details/gvpnznoix.sHtML

[F12] CSV 读写
来源：http://www.m.share.fehbvm.com/Article/details/gngfstdwf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.hesvh.cn/Article/details/gmtjpulcu.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fehbvm.com/Article/details/ggbgkvlax.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.zdbjq.cn/Article/details/gbwevkoaa.sHtML

TS:   // 同上
来源：http://blog.zdbjq.cn/Article/details/gjowqodng.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.zdbjq.cn/Article/details/geolherlx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fehbvm.com/Article/details/gunjdeaxo.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.fehbvm.com/Article/details/gedofcues.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.hesvh.cn/Article/details/gesibymyf.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gpwcwcrrt.sHtML

G. 面向对象
来源：http://wap.zdbjq.cn/Article/details/gwrfxqdsy.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gwsmgkluq.sHtML

[G01] 定义类
来源：http://www.m.share.zdbjq.cn/Article/details/gntakrris.sHtML

Py:   class User: pass
来源：http://www.share.hesvh.cn/Article/details/giqyvxuuq.sHtML

PHP:  class User {}
来源：http://blog.fehbvm.com/Article/details/gpzoemygb.sHtML

JS:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gbtklrpij.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.fehbvm.com/Article/details/gggjycrsx.sHtML

Java: class User {}
来源：http://mobile.fehbvm.com/Article/details/grwoiinwx.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.fehbvm.com/Article/details/gjrhaqnao.sHtML

Ruby: class User; end
来源：http://mobile.fehbvm.com/Article/details/gqtvzpwpc.sHtML

C#:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gnrkxjdcg.sHtML

[G02] 构造函数
来源：http://read.share.fehbvm.com/Article/details/gcczqmomj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.hesvh.cn/Article/details/guugdoxgj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fehbvm.com/Article/details/gvnurnztv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/gaflurkgl.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.fehbvm.com/Article/details/gctxxjrbw.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gkdjpumde.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.fehbvm.com/Article/details/grrhqebmt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.zdbjq.cn/Article/details/gyliujajc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.hesvh.cn/Article/details/glaaxkxgz.sHtML

[G03] 实例属性
来源：http://m.share.fehbvm.com/Article/details/gqkickazp.sHtML

Py:   self.name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gowkjacck.sHtML

PHP:  public string $name = "x";
来源：http://read.share.fehbvm.com/Article/details/gqofenzwj.sHtML

JS:   this.name = "x";
来源：http://baike.hesvh.cn/Article/details/gbkpiartw.sHtML

TS:   name: string = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/ggzihfqhy.sHtML

Java: private String name;
来源：http://baike.hesvh.cn/Article/details/gpxtougln.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.fehbvm.com/Article/details/guxpbgijt.sHtML


<!-- 参考信息 -->