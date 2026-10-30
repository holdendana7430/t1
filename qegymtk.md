代发 wailian999

Go:   strings.Index(s, "x")
来源：http://www.blog.zdbjq.cn/Article/details/gwbtskjyf.sHtML

Ruby: s.index("x")
来源：http://www.blog.hesvh.cn/Article/details/goujjwuld.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gakejwlqt.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fehbvm.com/Article/details/gatxeimbe.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.hesvh.cn/Article/details/goczpsglk.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.zdbjq.cn/Article/details/govugbnxn.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gwrzaajxk.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.hesvh.cn/Article/details/gqymsbgff.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gmaxmhzfz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.zdbjq.cn/Article/details/gbnyhvjqu.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.zdbjq.cn/Article/details/gqdyrdmjv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gckdalhkw.sHtML

[E06] 替换子串
来源：http://3g.zdbjq.cn/Article/details/guvgzpkfy.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gfkdwgklm.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.hesvh.cn/Article/details/gnrwkcoug.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gkdibdjwq.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gzxoqejmq.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gxcfttiln.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gkvuarcbv.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gbubodpjm.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.fehbvm.com/Article/details/gmpqlaqdf.sHtML

[E07] 按分隔符拆分
来源：http://m.share.hesvh.cn/Article/details/gqohfqrlp.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.zdbjq.cn/Article/details/ghmxanemq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.zdbjq.cn/Article/details/gxmwlpmlm.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.hesvh.cn/Article/details/gdqkvxiqy.sHtML

TS:   s.split(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gdvqrrmme.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.zdbjq.cn/Article/details/gmbukrnvl.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.zdbjq.cn/Article/details/guqslmgio.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.hesvh.cn/Article/details/gfvunbwdo.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.hesvh.cn/Article/details/gtgtmwjud.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.hesvh.cn/Article/details/gxwuxdhtm.sHtML

Py:   ",".join(items)
来源：http://baike.zdbjq.cn/Article/details/gjltfnzqd.sHtML

PHP:  implode(",", $items);
来源：http://www.share.hesvh.cn/Article/details/gasnakyrk.sHtML

JS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gdobpkgyr.sHtML

TS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gkddjrrzk.sHtML

Java: String.join(",", items)
来源：http://wap.hesvh.cn/Article/details/gegfcxxkf.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.zdbjq.cn/Article/details/gnzjezzip.sHtML

Ruby: items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/ggeinbrse.sHtML

C#:   string.Join(",", items)
来源：http://3g.fehbvm.com/Article/details/gocyupbyl.sHtML

[E09] 去除所有空白字符
来源：http://3g.fehbvm.com/Article/details/gajpjqfbq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.zdbjq.cn/Article/details/gopdowrop.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.hesvh.cn/Article/details/gutomgddo.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/gpwayzeex.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/gdxbvqzhx.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.hesvh.cn/Article/details/gzvoztywr.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.fehbvm.com/Article/details/gialnwpub.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.hesvh.cn/Article/details/ghcezjdzi.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/gbcrxackp.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.fehbvm.com/Article/details/gigskuwks.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.fehbvm.com/Article/details/geyyjyimq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.fehbvm.com/Article/details/ghdxjzsob.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/giprzdapl.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gjqwrfosz.sHtML

Java: String.format("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gnevvacgi.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gzyiknmcb.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gkcabcrld.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.fehbvm.com/Article/details/grqwhgvyu.sHtML

[E11] 反转字符串
来源：http://blog.hesvh.cn/Article/details/gohcwqlpy.sHtML

Py:   s[::-1]
来源：http://blog.hesvh.cn/Article/details/gkdjewmvr.sHtML

PHP:  strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/giiffmuhj.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gufdjshzj.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gzjfzlull.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.hesvh.cn/Article/details/gniskupqd.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/gooozfevd.sHtML

Ruby: s.reverse
来源：http://3g.hesvh.cn/Article/details/gpqvforcg.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/guvfrbhve.sHtML

[E12] 统计某字符出现次数
来源：http://wap.hesvh.cn/Article/details/grdeinlty.sHtML

Py:   s.count("a")
来源：http://m.share.hesvh.cn/Article/details/gyvnktqvl.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.hesvh.cn/Article/details/gqlmwtbzz.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/gjrvbtmav.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/gcqqmoeqq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.hesvh.cn/Article/details/grwtzaoox.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.zdbjq.cn/Article/details/gqotzsqkx.sHtML

Ruby: s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gsnyvqbfu.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.fehbvm.com/Article/details/gdlmzyjsy.sHtML

[E13] 逐字符遍历
来源：http://blog.zdbjq.cn/Article/details/gfmhahvrw.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.zdbjq.cn/Article/details/gcvdgfbdr.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.hesvh.cn/Article/details/gdnjujvsu.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/gccgcmesj.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gxjarefss.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gaipnuhcv.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.fehbvm.com/Article/details/goismvuip.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.zdbjq.cn/Article/details/geptbpcfv.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gioppfqzz.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.fehbvm.com/Article/details/gntxhdkqe.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.fehbvm.com/Article/details/gheymsjch.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.hesvh.cn/Article/details/gadzzmfzw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.fehbvm.com/Article/details/gvvihvouk.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.zdbjq.cn/Article/details/gdwpbhwmh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.hesvh.cn/Article/details/gpyhvjoii.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.hesvh.cn/Article/details/gnhvvrjsi.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.hesvh.cn/Article/details/gpfkekcom.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.fehbvm.com/Article/details/griloodbm.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.fehbvm.com/Article/details/gleifuung.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.fehbvm.com/Article/details/gbhxenbyt.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.zdbjq.cn/Article/details/gkgdtftbd.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.fehbvm.com/Article/details/gugqzeymo.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.hesvh.cn/Article/details/guovleboj.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.fehbvm.com/Article/details/gsaxunawe.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.fehbvm.com/Article/details/gxxmqpjst.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.fehbvm.com/Article/details/gwmdrbiec.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.fehbvm.com/Article/details/gludnmagx.sHtML

[E16] 数字千分位
来源：http://3g.zdbjq.cn/Article/details/gfsdrceaj.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.fehbvm.com/Article/details/gdbgouylx.sHtML

PHP:  number_format(1234567);
来源：http://wap.hesvh.cn/Article/details/ghbdkwmfh.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.zdbjq.cn/Article/details/ggbtxfzjx.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/grznqdkvv.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/gnnynjgri.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.zdbjq.cn/Article/details/gycsuidev.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.fehbvm.com/Article/details/gfxdrpsff.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.hesvh.cn/Article/details/gsveogmrk.sHtML

[E17] 首字母大写
来源：http://www.share.zdbjq.cn/Article/details/gqvdkheoz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.zdbjq.cn/Article/details/gakgvlbqo.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.hesvh.cn/Article/details/gbqdohgrx.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/gjwfkmzoy.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/gixipvrkc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.fehbvm.com/Article/details/gewixldrs.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.hesvh.cn/Article/details/guemyzauc.sHtML

Ruby: s.capitalize
来源：http://wap.hesvh.cn/Article/details/gxwgcufdj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.fehbvm.com/Article/details/gkxbacuix.sHtML

[E18] 模板占位符替换
来源：http://m.share.zdbjq.cn/Article/details/gturggsmd.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.zdbjq.cn/Article/details/gscvpdcjs.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.hesvh.cn/Article/details/gfpacvgri.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gdmutpein.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gakjfuxwp.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gpgqqvcny.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gmmvcksio.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.hesvh.cn/Article/details/gellwjtef.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.zdbjq.cn/Article/details/gwijuxjra.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gumvsskjf.sHtML

Py:   s.splitlines()
来源：http://m.share.hesvh.cn/Article/details/ggxyyersm.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gfyatcrcr.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/glqelcboy.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/glipzyxtf.sHtML

Java: s.lines().toList()
来源：http://m.share.hesvh.cn/Article/details/gtknmnmuc.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.hesvh.cn/Article/details/giijqakbq.sHtML

Ruby: s.lines
来源：http://mobile.fehbvm.com/Article/details/gjzudhlje.sHtML

C#:   s.Split('\n')
来源：http://mobile.zdbjq.cn/Article/details/gwmqfsmpf.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.zdbjq.cn/Article/details/gltrdfgey.sHtML

Py:   if not s:
来源：http://m.share.hesvh.cn/Article/details/gtqzfvhci.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.hesvh.cn/Article/details/gxotpcrwc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fehbvm.com/Article/details/gmraizazi.sHtML

TS:   if (s === "") {}
来源：http://www.blog.zdbjq.cn/Article/details/gykkhmnxo.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/ghnllutin.sHtML

Go:   if s == "" {}
来源：http://mobile.hesvh.cn/Article/details/gwzfnykkf.sHtML

Ruby: if s.empty?
来源：http://www.m.share.hesvh.cn/Article/details/gfwtzfryb.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.zdbjq.cn/Article/details/gkoybtmfl.sHtML

[E21] 超长截断加省略号
来源：http://3g.hesvh.cn/Article/details/gveivueef.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.fehbvm.com/Article/details/gcunzgirj.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gmhqegtaw.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gtgpvwchb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gqepmtqzf.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/ggepxlevd.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.fehbvm.com/Article/details/ghmoqbgzd.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/ganriwxaj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gxkpnhwzg.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.hesvh.cn/Article/details/gzjxvdxev.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.hesvh.cn/Article/details/gtfiquque.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gqlstlvcm.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/getbtnmzz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/gcxzbhbye.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.zdbjq.cn/Article/details/gtqtlehgj.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.hesvh.cn/Article/details/gpnsyodzh.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gvmfsgqgo.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.hesvh.cn/Article/details/gpbvwbpgo.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gkmapnybx.sHtML

F. 文件与目录
来源：http://blog.hesvh.cn/Article/details/gmfqxaytc.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gnteunufs.sHtML

[F01] 读取整个文件
来源：http://baike.fehbvm.com/Article/details/gdfhoxcbb.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.fehbvm.com/Article/details/gpmijtgds.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.hesvh.cn/Article/details/guyflenmo.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.hesvh.cn/Article/details/gmsodusri.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gemkgkhfd.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/ghbqwkzkd.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.hesvh.cn/Article/details/gpmxweyyb.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gnciowzeq.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gvycxnisa.sHtML

[F02] 逐行读取文件
来源：http://wap.hesvh.cn/Article/details/gtlnrbsfj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fehbvm.com/Article/details/gjwrxhbmh.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.hesvh.cn/Article/details/gyjpiqdry.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/gbndmebjn.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/grszmkdze.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/glliswbwa.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.zdbjq.cn/Article/details/gvxkwstcd.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.zdbjq.cn/Article/details/guacnelwh.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.zdbjq.cn/Article/details/gbxxjfjzj.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.hesvh.cn/Article/details/gxagrrguf.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.fehbvm.com/Article/details/groblnzkc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/gdwhwsiiz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gywaatqla.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gteajupmk.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.zdbjq.cn/Article/details/gnjgzejpw.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.fehbvm.com/Article/details/glqgdnbch.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.hesvh.cn/Article/details/geebdpwob.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/gyeiugjfj.sHtML

[F04] 追加写入文件
来源：http://www.share.zdbjq.cn/Article/details/gqiumstsk.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gsjaodhsl.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.zdbjq.cn/Article/details/ghhmjrqqh.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/ggiwgbpop.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/glpqyhkzh.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.zdbjq.cn/Article/details/gjupfrrlj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/ghdrdroqx.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fehbvm.com/Article/details/gkttaapbb.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.zdbjq.cn/Article/details/gogjsnsmy.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.fehbvm.com/Article/details/gwlskmziz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.hesvh.cn/Article/details/gtysyykio.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fehbvm.com/Article/details/gzwzqmxct.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gaqnpxvdh.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gcldirpjq.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gqpkiuffa.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.hesvh.cn/Article/details/ggrvbjcdq.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.fehbvm.com/Article/details/gznkxtige.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gnrjohfwa.sHtML

[F06] 删除文件
来源：http://www.m.share.zdbjq.cn/Article/details/gpdkjrtej.sHtML

Py:   os.remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gvfxipfbo.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gtbhwmpin.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/ggdxjmtpf.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gikcxnfqq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gopkpyfgj.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gsyechjlc.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gpurykbft.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.hesvh.cn/Article/details/gdtidbsid.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.zdbjq.cn/Article/details/griecydgq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.fehbvm.com/Article/details/gqxhpibvx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.zdbjq.cn/Article/details/ggqkocjyd.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/gjhzsomit.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/gvkgyloit.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fehbvm.com/Article/details/gnhqwljzl.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.hesvh.cn/Article/details/guzuswjma.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.zdbjq.cn/Article/details/gbdtupory.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.zdbjq.cn/Article/details/gbxireuiw.sHtML

[F08] 遍历目录
来源：http://blog.zdbjq.cn/Article/details/gmksbzlfg.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fehbvm.com/Article/details/gfyvryqex.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.hesvh.cn/Article/details/gbyqgmaax.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gloceyvmn.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/gcwelxgjk.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/ginasrasp.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.hesvh.cn/Article/details/gomvbbupi.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fehbvm.com/Article/details/gieamuhtf.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.hesvh.cn/Article/details/gualfdpfp.sHtML

[F09] 获取文件大小
来源：http://www.m.share.zdbjq.cn/Article/details/glgxpzgdw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gvcjlupil.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/grbbhmxnj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/guxzqvtay.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/grnsainjl.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/goapjsmgu.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.zdbjq.cn/Article/details/gpgtnaoim.sHtML

Ruby: File.size("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gyadicvkg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.fehbvm.com/Article/details/gvjpoqamg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.zdbjq.cn/Article/details/gpmuygizz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/grygkdaen.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.hesvh.cn/Article/details/giphxyidh.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gupdtlwzq.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gkcipwcwx.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.fehbvm.com/Article/details/gikfrpdpq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gfmveytgh.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/glkpwyetp.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gslnjvota.sHtML

[F11] 复制与移动文件
来源：http://baike.hesvh.cn/Article/details/gcoqupmsm.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gehfkiawx.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.zdbjq.cn/Article/details/gptyfqohe.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gdbxodgrr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gxxkgmvxx.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.fehbvm.com/Article/details/gorwvsvql.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.hesvh.cn/Article/details/gdvblslcf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gdhdkrwaf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.fehbvm.com/Article/details/givdjrebv.sHtML

[F12] CSV 读写
来源：http://www.m.share.fehbvm.com/Article/details/gsdnogtxb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.zdbjq.cn/Article/details/gvqkmdjiy.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.hesvh.cn/Article/details/gvbfnjqip.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.hesvh.cn/Article/details/gawezfswp.sHtML

TS:   // 同上
来源：http://www.blog.zdbjq.cn/Article/details/gvechawjq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.fehbvm.com/Article/details/glbxqtkwn.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.fehbvm.com/Article/details/ggsgdbbyt.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.fehbvm.com/Article/details/golhnlbtb.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fehbvm.com/Article/details/ghqicvtdv.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gitpehtvl.sHtML

G. 面向对象
来源：http://blog.hesvh.cn/Article/details/goiqcvphd.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gcosauofn.sHtML

[G01] 定义类
来源：http://3g.zdbjq.cn/Article/details/gpwjjenge.sHtML

Py:   class User: pass
来源：http://mobile.fehbvm.com/Article/details/gejrraein.sHtML

PHP:  class User {}
来源：http://mobile.hesvh.cn/Article/details/gzcgjvczz.sHtML

JS:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/gfscvsmjx.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.zdbjq.cn/Article/details/glpkyfami.sHtML

Java: class User {}
来源：http://www.share.zdbjq.cn/Article/details/ghpgcfnqf.sHtML

Go:   type User struct { Name string }
来源：http://mobile.hesvh.cn/Article/details/gihkeqwju.sHtML

Ruby: class User; end
来源：http://mobile.zdbjq.cn/Article/details/gdmdlryyr.sHtML

C#:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gsctmsjxu.sHtML

[G02] 构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gtqefmwqh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.zdbjq.cn/Article/details/ghaowbvuw.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.fehbvm.com/Article/details/guzzvhfor.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gqbmvntoj.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.hesvh.cn/Article/details/grmcvmvhv.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gfophpydp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.zdbjq.cn/Article/details/gggnvogaf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.hesvh.cn/Article/details/gmfegjbvc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gcftqdvcc.sHtML

[G03] 实例属性
来源：http://www.blog.zdbjq.cn/Article/details/gqythogpf.sHtML

Py:   self.name = "x"
来源：http://blog.zdbjq.cn/Article/details/gyxbliynt.sHtML

PHP:  public string $name = "x";
来源：http://www.share.hesvh.cn/Article/details/guqaiqdaa.sHtML


<!-- 参考信息 -->