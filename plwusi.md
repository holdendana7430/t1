代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.xuetiantiany.cn/gtypkvnyuu.html

[E03] 截取子串
来源：http://hz.shangyingyoupin.top/gtjxrsdwxi.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.cqqwz.cn/gtvawidcla.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.jqgfzy.top/gtxztpteqi.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.yj20258.top/gtktlfkdwn.html

TS:   s.slice(1, 4)
来源：http://hz.hywenlv.cn/gtkgmpyyac.html

Java: s.substring(1, 4)
来源：http://hz.svipenyu.cn/gtucufxznx.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.xylfe.cn/gtxuowxchz.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.sweek.top/gtbmmfsepc.html

C#:   s.Substring(1, 3)
来源：http://hz.yj20258.top/gtwzrnlxfb.html

[E04] 查找子串位置
来源：http://hz.yj20258888.top/gtkuqyqlrh.html

Py:   s.find("x");  s.index("x")
来源：http://hz.0kj1m.cn/gtxkzrmjyz.html

PHP:  strpos($s, "x");
来源：http://hz.jinqigufen.top/gtrhettkvl.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.gotoacloud.top/gtobdxzobd.html

TS:   s.indexOf("x")
来源：http://hz.yj20258.top/gtzbnxtdha.html

Java: s.indexOf("x")
来源：http://hz.fzhhl.top/gtfbqjvokc.html

Go:   strings.Index(s, "x")
来源：http://hz.smart0.xyz/gtraeqrvvl.html

Ruby: s.index("x")
来源：http://hz.tian-w.cn/gtkzmbyosy.html

C#:   s.IndexOf("x")
来源：http://hz.zhengqikj.top/gtnxagjrjk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.svipenyu.cn/gttpqgejoo.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.ywan-chungtsiang.top/gtjklvfbfb.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.yj20258.top/gtabzuqvie.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zhoulong.xyz/gtvkzjuaml.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.zycfv.cn/gtqexnilsc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.316326.xyz/gtsqxlbhkr.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.gaohongyu789.top/gtphddxpaw.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.ppjwa.cn/gtxqdsdxyh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.cucudq.cn/gtsffoomyo.html

[E06] 替换子串
来源：http://hz.bjfxy.top/gtboxnatap.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.c1oappe.top/gtyiaqzhmh.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.jlsjyb.cn/gtruvufwqb.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yuanzhike.top/gtkgswukbe.html

TS:   s.replaceAll("a", "b")
来源：http://hz.yj20258888.top/gtylcrclse.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.dianchejie.cn/gtomgkmihe.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.sufxvd.cn/gthcmvpcft.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.shanyushiyangtech.top/gtcjpecfvk.html

C#:   s.Replace("a", "b")
来源：http://hz.ydjk.org.cn/gtcksjzgxf.html

[E07] 按分隔符拆分
来源：http://hz.9152youxi.cn/gtavykrxqs.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.ppjwa.cn/gtsivctqzl.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.fengsongda.top/gtcdwrmqsv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.wangshuangyany.cn/gtvazobmeq.html

TS:   s.split(",")
来源：http://hz.tian-w.cn/gtkmjttydl.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.aizwys.cn/gtruvzbppu.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.ydjk.org.cn/gtolchyldp.html

Ruby: s.split(",");  s.split
来源：http://hz.cheryme.top/gtkvmsizjl.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.zhengqikj.top/gtuzjwpyfb.html

[E08] 数组按分隔符合并
来源：http://hz.jianghu66.top/gtfohisvps.html

Py:   ",".join(items)
来源：http://hz.yueranfly.top/gtsnnoncdp.html

PHP:  implode(",", $items);
来源：http://hz.cdnleiting.top/gtljozowtg.html

JS:   items.join(",")
来源：http://hz.c1oappe.top/gtwzzlbszs.html

TS:   items.join(",")
来源：http://hz.svipenyu.cn/gtmdwwneor.html

Java: String.join(",", items)
来源：http://hz.snrcjt.cn/gtwytzppdn.html

Go:   strings.Join(items, ",")
来源：http://hz.dianchejie.cn/gtrdcrbbxl.html

Ruby: items.join(",")
来源：http://hz.zycfv.cn/gtfpuccyqg.html

C#:   string.Join(",", items)
来源：http://hz.aibaodan.cn/gttpuczcrl.html

[E09] 去除所有空白字符
来源：http://hz.hnxiangtu.top/gtasxallro.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.hnqzz.top/gtyllqwifx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.ydzc1.top/gtxsfgwsmf.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.chenzaomai.com/gtbtmlrdor.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.snrcjt.cn/gtwdvkljqq.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.hnqzz.top/gtjuoabniw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.hammf.cn/gtfsaepglj.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.zhoulong.xyz/gtzidauiok.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.daria6918.cn/gtzndteung.html

[E10] 左侧补零 / 定长填充
来源：http://hz.jinghuilouyu.cn/gtipfuarpt.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.hywenlv.cn/gtymamkyfk.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.jlsjyb.cn/gtrnkmilvj.html

JS:   "7".padStart(3, "0")
来源：http://hz.snrcjt.cn/gtievnavch.html

TS:   "7".padStart(3, "0")
来源：http://hz.ehwqpu.com/gtfjlxrmps.html

Java: String.format("%03d", 7)
来源：http://hz.jqgufenzy.top/gttrozqwbe.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.iojbl.cn/gttsbsabyk.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.xuetiantiany.cn/gtxpokeuzk.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.sysykeji.top/gtxgyiqzzf.html

[E11] 反转字符串
来源：http://hz.yanxiufei.cn/gtbtwwhmwy.html

Py:   s[::-1]
来源：http://hz.gogol.net.cn/gtkpgjvjio.html

PHP:  strrev($s);
来源：http://hz.aizwys.cn/gtabtxeuwv.html

JS:   [...s].reverse().join("")
来源：http://hz.chenlongwang.top/gteeggbwmj.html

TS:   [...s].reverse().join("")
来源：http://hz.shanyushiyangtech.top/gtemapgagi.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.shangyingyoupin.top/gtrlflrsqk.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.cashguo.top/gtpvcyjxns.html

Ruby: s.reverse
来源：http://hz.gaohongyu789.top/gtvzkvkuow.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.daxiang520.top/gtmhufwnpj.html

[E12] 统计某字符出现次数
来源：http://hz.yongpay.top/gtvuhwfxfv.html

Py:   s.count("a")
来源：http://hz.xylfe.cn/gtclaobbhm.html

PHP:  substr_count($s, "a");
来源：http://hz.yvedp.cn/gtcegzoziq.html

JS:   s.split("a").length - 1
来源：http://hz.chenlongwang.top/gtopzsasho.html

TS:   s.split("a").length - 1
来源：http://hz.aizwys.cn/gtifbdnmul.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.yj202588.top/gtqedpmwnx.html

Go:   strings.Count(s, "a")
来源：http://hz.zhijiandao.cn/gthubbqocw.html

Ruby: s.count("a")
来源：http://hz.zdqjudy.top/gtymbwrggi.html

C#:   s.Count(c => c == 'a')
来源：http://hz.chenjidiqi.icu/gtjixjkrwh.html

[E13] 逐字符遍历
来源：http://hz.yvedp.cn/gtbsfwosbx.html

Py:   for ch in s: print(ch)
来源：http://hz.jinghuilouyu.cn/gthvhpgcyk.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.nwbrower.top/gttvdvsgqg.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zhongyouzk.top/gtpdamvgjg.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.dianchejie.cn/gtyctfeinq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.sweek.top/gtajjhitww.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.nanxinkj.top/gtmokfqsko.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.chenzaomai.com/gtlcoafjxq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.gzhubu.top/gtsghkbdae.html

[E14] URL 编码与 Base64
来源：http://hz.hongshengwenyu.top/gtyymlgbyz.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.shzxlz.cn/gtookxkvdi.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.hnxiangtu.top/gtvjidekdq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.nanxinkj.top/gtmuighhqq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.shzxlz.cn/gtubogfchd.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.yj20258888.top/gtleqeijaa.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.jianghu66.top/gtbmortcbm.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.shzxlz.cn/gtgeahgttb.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.shanyushiyangtech.top/gtvphfmmtc.html

[E15] HTML 转义 / 反转义
来源：http://hz.zhongyouzk.top/gtgveadcrd.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.hnxiangtu.top/gtmizmxrla.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.daria6918.cn/gtpiqlreem.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yj20258.top/gtvabgjecc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.xziqi.cn/gtuyqzcrqa.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.ydzc1.top/gtshafyejb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.yj20258888.top/gtakbruqef.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.haohaochexian.top/gtrininbhz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.9152youxi.cn/gtqbowobhf.html

[E16] 数字千分位
来源：http://hz.316326.xyz/gtldwhjciy.html

Py:   f"{1234567:,}"
来源：http://hz.jinqigfzy.top/gtpadzbrhn.html

PHP:  number_format(1234567);
来源：http://hz.xziqi.cn/gtnryvryyq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.shanyushiyangtech.top/gtglbbpyzq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.yangfankeji.com/gttjkxmplu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.316326.xyz/gtacrfbgio.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.mhx1999.top/gtvplkingq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.vqdsnc.cn/gtymvapjxc.html

C#:   1234567.ToString("N0")
来源：http://hz.dianchejie.cn/gtjxozvfgr.html

[E17] 首字母大写
来源：http://hz.zdqjudy.top/gtkyfxoofo.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.zdqjudy.top/gtgbiqjntm.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.zhengqikj.top/gteuiysark.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.c1oappe.top/gtvagobpex.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.svipenyu.cn/gtcygasmgt.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.chenlongwang.top/gtmgbwrilm.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.jlsjyb.cn/gtfleqjqcb.html

Ruby: s.capitalize
来源：http://hz.zhongyouzk.top/gttlirqhqk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.feifeiyinyue.top/gtiuymvoqv.html

[E18] 模板占位符替换
来源：http://hz.chenjidiqi.icu/gtnawmbuzh.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.tian-w.cn/gttveqbsmx.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.hywenlv.cn/gtdbbpxtzh.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.c1oappe.top/gtaqzxxptd.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.52xcode.cn/gtqhrdopav.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.jinqigfzy.top/gtnwxajzef.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.shangyingyoupin.top/gthbuothbp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.iojbl.cn/gtckdvapmn.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.cqqwz.cn/gtjckycnrz.html

[E19] 多行文本按行拆分
来源：http://hz.jianghu66.top/gtqigapzok.html

Py:   s.splitlines()
来源：http://hz.jinghuilouyu.cn/gtkdwuxewp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.yvedp.cn/gtxqwgmlqk.html

JS:   s.split(/\r?\n/)
来源：http://hz.chenzaomai.com/gtfzwbvgis.html

TS:   s.split(/\r?\n/)
来源：http://hz.yueranfly.top/gtnsmtlpyc.html

Java: s.lines().toList()
来源：http://hz.ppjwa.cn/gtehtpekvs.html

Go:   strings.Split(s, "\n")
来源：http://hz.yuanzhike.top/gtdvgyekhy.html

Ruby: s.lines
来源：http://hz.haohaochexian.top/gtyaongwed.html

C#:   s.Split('\n')
来源：http://hz.sxryk.cn/gtxlappzho.html

[E20] 判断字符串是否为空
来源：http://hz.jqgfzy.top/gtufhkmooa.html

Py:   if not s:
来源：http://hz.shangyingyoupin.top/gtmhzqoefo.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.hongshengwenyu.top/gtakhfujaz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.zhijiandao.cn/gtpgemrkvp.html

TS:   if (s === "") {}
来源：http://hz.shanyushiyangtech.top/gtmiyhoviy.html

Java: if (s.isEmpty()) {}
来源：http://hz.jyoumei.cn/gtqibkwhtj.html

Go:   if s == "" {}
来源：http://hz.ppjwa.cn/gtklncpawm.html

Ruby: if s.empty?
来源：http://hz.gzhubu.top/gtbmfaajiy.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.snrcjt.cn/gtdktsizdq.html

[E21] 超长截断加省略号
来源：http://hz.yj202588.top/gtuhuxavck.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.feifeiyinyue.top/gtdhntvlfw.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.jinqigufen.top/gtvofrwfwo.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ywan-chungtsiang.top/gtopdpgxpm.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ppjwa.cn/gtrvipepwt.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.guowangkeji.top/gtpzgnmoou.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.yuanzhike.top/gtczhccoxp.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.ydjk.org.cn/gtacwjhobt.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.zycfv.cn/gtvozzwehs.html

[E22] 字节长度与字符长度
来源：http://hz.hywenlv.cn/gtxkjaqine.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.jqgufenzy.top/gttpxfnahk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yonumen.top/gtfiztgjcs.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.sysykeji.top/gtgdxzhoax.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hywenlv.cn/gtonddnfun.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.nanxinkj.top/gteepnwccj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.sweek.top/gtwxkonplo.html

Ruby: s.bytesize;  s.length
来源：http://hz.daxiang520.top/gtdzdrzkpn.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.fengsongda.top/gthwvicdqx.html

================================================================================
来源：http://hz.pycfn.com/gtvgjngdxa.html

F. 文件与目录
来源：http://hz.gotoacloud.top/gtsmjllzsv.html

================================================================================
来源：http://hz.ehwqpu.com/gtsupyuaui.html

[F01] 读取整个文件
来源：http://hz.xingfuxueyuan.xyz/gtxctsuzhj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.aibaodan.cn/gtsxyaoxvl.html

PHP:  file_get_contents("a.txt");
来源：http://hz.xziqi.cn/gtjphlcyhx.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.ivvv.top/gttmytbfny.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.hywenlv.cn/gtjxjhfpmf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.guowangkeji.top/gtkrohnqlv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.pycfn.com/gtzlwapzwr.html

Ruby: File.read("a.txt")
来源：http://hz.yj202588.top/gtzscfbzor.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yvedp.cn/gtmzcttkga.html

[F02] 逐行读取文件
来源：http://hz.cheryme.top/gtrzkmolzw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.pycfn.com/gtgysfaqev.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.smart0.xyz/gtesspotud.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yueranfly.top/gtlxgkqikv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yongpay.top/gtqhbexglz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.chenlongwang.top/gttzflulzj.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.tian-w.cn/gteaiyvpuy.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.pycfn.com/gtvfwweoio.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.zhoulong.xyz/gtphignkko.html

[F03] 写入文件（覆盖）
来源：http://hz.jinghuilouyu.cn/gtdjjxqqwq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.xinyue.icu/gtohokzrcv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.shuidangran.top/gtqmkddpjh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhongyouzk.top/gtdadwcanu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.meibo888.top/gtmtdpgjxr.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.zycfv.cn/gtlliuimox.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.ehwqpu.com/gtbangidhu.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.jqgufenzy.top/gtrhqxnusf.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.kuanghao11.cn/gtymmnhnqw.html

[F04] 追加写入文件
来源：http://hz.xziqi.cn/gtatrzbpjr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.ppjwa.cn/gtgievnlpt.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.xinyue.icu/gtgjhjueqn.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.bjfxy.top/gtzortlplb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.nanxuanxn.top/gtmdccrvxz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.yj20258888.top/gtkjfqqgeg.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.sxryk.cn/gtnptsttii.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.cqqwz.cn/gtmtdgpcoy.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.havefunace.top/gtyjprbsqn.html

[F05] 判断文件或目录是否存在
来源：http://hz.ydzc1.top/gtvbooqtsr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.andypj.xyz/gtxtjwpmmg.html

PHP:  file_exists("a.txt");
来源：http://hz.yanxiufei.cn/gtwdeblggl.html

JS:   fs.existsSync("a.txt")
来源：http://hz.havefunace.top/gtbvydzetc.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zdqjudy.top/gtssrklonc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.316326.xyz/gtkjcbvuli.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.bjfxy.top/gtiojybuhu.html

Ruby: File.exist?("a.txt")
来源：http://hz.sysykeji.top/gtdahikxgf.html

C#:   File.Exists("a.txt")
来源：http://hz.guowangkeji.top/gtcjbwbily.html

[F06] 删除文件
来源：http://hz.dashuyun.cn/gtzjynixuo.html

Py:   os.remove("a.txt")
来源：http://hz.dianchejie.cn/gtttnopdjz.html

PHP:  unlink("a.txt");
来源：http://hz.haohaochexian.top/gtayxhslrc.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.ppjwa.cn/gteivrtotj.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.zhoulong.xyz/gtmzuowfmu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.yvedp.cn/gtvtbyqexz.html

Go:   os.Remove("a.txt")
来源：http://hz.ydzc1.top/gtkiggcrhf.html

Ruby: File.delete("a.txt")
来源：http://hz.aizwys.cn/gtwmckgudt.html

C#:   File.Delete("a.txt");
来源：http://hz.yj20258.top/gtvaeagvjq.html

[F07] 创建目录（含多级）
来源：http://hz.nanxinkj.top/gtfmbdiweh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yueranfly.top/gtribidlds.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.tanke756.top/gtngaijbjx.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.sysykeji.top/gtfbuyppjl.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.xuetiantiany.cn/gtmxweeobd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.kuanghao11.cn/gtaykzgzmy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.xylfe.cn/gtedxffwsz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.cqqwz.cn/gtjumwdlex.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.jiagoushi.top/gtvgnkqcbh.html

[F08] 遍历目录
来源：http://hz.meibo888.top/gtfgkuerke.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.chenzaomai.com/gthhhccqut.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.ehwqpu.com/gtiqhamiew.html

JS:   fs.readdirSync("dir")
来源：http://hz.iojbl.cn/gtrvhwtwla.html

TS:   fs.readdirSync("dir")
来源：http://hz.zhiwuduotai.top/gtrzotnkyu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.shanyushiyangkeji.top/gtuoinzszx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.0kj1m.cn/gtislktsnx.html

Ruby: Dir.children("dir")
来源：http://hz.tianlin.xyz/gtayzluoew.html

C#:   Directory.GetFiles("dir")
来源：http://hz.nanxuanxn.top/gtmgsfhwly.html

[F09] 获取文件大小
来源：http://hz.xuetiantiany.cn/gtbylntavn.html

Py:   os.path.getsize("a.txt")
来源：http://hz.yuanzhike.top/gtrxatcszz.html

PHP:  filesize("a.txt");
来源：http://hz.xuanzx.com/gtmcnpypym.html

JS:   fs.statSync("a.txt").size
来源：http://hz.yj20258.top/gtepcbhozy.html

TS:   fs.statSync("a.txt").size
来源：http://hz.chenzaomai.com/gtacvavwqy.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.ehwqpu.com/gtxngvjuqd.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.yanxiufei.cn/gtllknajaa.html

Ruby: File.size("a.txt")
来源：http://hz.birdmap.top/gtbpnwqrum.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.shangyingyoupin.top/gtnjgokdfr.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.316326.xyz/gteeinodei.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.gzhubu.top/gtnjxagdhg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.yj20258.top/gtfumxoope.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.zhoulong.xyz/gtukxicxgf.html

TS:   path.extname("a.txt")
来源：http://hz.tanke756.top/gtdidbnwce.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.yonumen.top/gtmdocjwle.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.shanyushiyangtech.top/gtjjisiilr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.yonumen.top/gtgnvcpjag.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.316326.xyz/gtxzgeemfq.html

[F11] 复制与移动文件
来源：http://hz.0kj1m.cn/gtuqakgads.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.shuidangran.top/gtrwnzsqgh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.cashguo.top/gtisgneahn.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.wangdashe.top/gtnjfprhkc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.9152youxi.cn/gtldhbpqdm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.yvedp.cn/gtecfruwkt.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.sufxvd.cn/gtkavkdtar.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.cucudq.cn/gtkdzpjebx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.fzhhl.top/gtmssaowvh.html

[F12] CSV 读写
来源：http://hz.meibo888.top/gtgbgplthn.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.yuxming.cn/gtdosbkxfn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.shanyushiyangkeji.top/gtxklerugh.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.shanyushiyangkeji.top/gtyxfcjsyb.html

TS:   // 同上
来源：http://hz.havefunace.top/gtnawlttgl.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.9152youxi.cn/gtpsxjnbdq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.daria6918.cn/gtjphldwtc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.yueranfly.top/gtzftqqrsl.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.zhoulong.xyz/gtqghnaezx.html

================================================================================
来源：http://hz.zhongyouzk.top/gtvutizqzd.html

G. 面向对象
来源：http://hz.hnxiangtu.top/gtklkfrryo.html

================================================================================
来源：http://hz.aizwys.cn/gtkhrvkfvz.html

[G01] 定义类
来源：http://hz.wangdashe.top/gtbbymszud.html

Py:   class User: pass
来源：http://hz.yangfankeji.com/gtonjivozk.html

PHP:  class User {}
来源：http://hz.cdnleiting.top/gtucujrwvz.html

JS:   class User {}
来源：http://hz.hnqzz.top/gtseergson.html

TS:   class User { name: string = ""; }
来源：http://hz.cdnleiting.top/gtclzgdktg.html


<!-- 参考信息 -->