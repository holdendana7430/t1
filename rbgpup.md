代发 wailian999

[E02] 重复字符串
来源：http://hz.nanxinkj.top/gtnqnijgwn.html

Py:   "ab" * 3
来源：http://hz.pycfn.com/gtegkfhtkm.html

PHP:  str_repeat("ab", 3);
来源：http://hz.zdqjudy.top/gtetplzuib.html

JS:   "ab".repeat(3)
来源：http://hz.nwbrower.top/gtmzgipkey.html

TS:   "ab".repeat(3)
来源：http://hz.daxiang520.top/gtznitbfss.html

Java: "ab".repeat(3)
来源：http://hz.jianghu66.top/gtaqezqcaz.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.xziqi.cn/gtlkrfhlmg.html

Ruby: "ab" * 3
来源：http://hz.dashuyun.cn/gtnpoerynu.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.hywenlv.cn/gtypdtfycn.html

[E03] 截取子串
来源：http://hz.zycfv.cn/gtvdgdfopu.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.fzhhl.top/gtlubdenzf.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.gogol.net.cn/gtxejaianc.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.cucudq.cn/gtwvakoqng.html

TS:   s.slice(1, 4)
来源：http://hz.dianchejie.cn/gtxcvxcufl.html

Java: s.substring(1, 4)
来源：http://hz.redwolf501.top/gtsgofefxi.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.zhiwuduotai.top/gtfwqythpv.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.havefunace.top/gtnfecagfc.html

C#:   s.Substring(1, 3)
来源：http://hz.birdmap.top/gttmwuvolo.html

[E04] 查找子串位置
来源：http://hz.jlsjyb.cn/gtdgcnetzf.html

Py:   s.find("x");  s.index("x")
来源：http://hz.sysykeji.top/gtvngkyvlg.html

PHP:  strpos($s, "x");
来源：http://hz.xingfuxueyuan.xyz/gtgnxklfqu.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.gogol.net.cn/gtdizjthmz.html

TS:   s.indexOf("x")
来源：http://hz.xingfuxueyuan.xyz/gtchudsqfb.html

Java: s.indexOf("x")
来源：http://hz.wangshuangyany.cn/gtbayzidzj.html

Go:   strings.Index(s, "x")
来源：http://hz.vqdsnc.cn/gtztfguugu.html

Ruby: s.index("x")
来源：http://hz.dianchejie.cn/gtfqrsbyrt.html

C#:   s.IndexOf("x")
来源：http://hz.jinqigufen.top/gtsxbuztvl.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.dashuyun.cn/gtqwszypwo.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.daria6918.cn/gttclmitng.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.xingfuxueyuan.xyz/gtiskkawla.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.sysykeji.top/gtivctfkwn.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.daxiang520.top/gtpcgxiepd.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hongshengwenyu.top/gtxesegvqp.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.zhixingplan.top/gtbxdjciot.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.zhiwuduotai.top/gtcwuvskhk.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.dianchejie.cn/gtupjntimb.html

[E06] 替换子串
来源：http://hz.jiagoushi.top/gtxpjpidsx.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.hnqzz.top/gtzmqnuxiy.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.haohaochexian.top/gtaidhjfpw.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.9152youxi.cn/gtlhvzixjq.html

TS:   s.replaceAll("a", "b")
来源：http://hz.kuanghao11.cn/gtprjttssl.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.sysykeji.top/gtwvpyldva.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.tian-w.cn/gtkfldjqul.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.tian-w.cn/gtrajsjopd.html

C#:   s.Replace("a", "b")
来源：http://hz.xinyue.icu/gtkpjryrhj.html

[E07] 按分隔符拆分
来源：http://hz.yueranfly.top/gtpdancrja.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.dianchejie.cn/gtxeypssrl.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.ivvv.top/gtecjzhxzf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.yongpay.top/gtsvjmgdik.html

TS:   s.split(",")
来源：http://hz.gzhubu.top/gtsrsjanmc.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.guowangkeji.top/gtmnnswetz.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.52xcode.cn/gtjccdppqk.html

Ruby: s.split(",");  s.split
来源：http://hz.ydzc1.top/gtbhiwwiqp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.hnqzz.top/gtwttkttgf.html

[E08] 数组按分隔符合并
来源：http://hz.zhijiandao.cn/gtgaqzhiwi.html

Py:   ",".join(items)
来源：http://hz.redwolf501.top/gtfznacgfs.html

PHP:  implode(",", $items);
来源：http://hz.pycfn.com/gtevrisiux.html

JS:   items.join(",")
来源：http://hz.aibaodan.cn/gtdlmzvqoi.html

TS:   items.join(",")
来源：http://hz.jqgfzy.top/gtxuivjhyj.html

Java: String.join(",", items)
来源：http://hz.hnxiangtu.top/gtamlihbgk.html

Go:   strings.Join(items, ",")
来源：http://hz.snrcjt.cn/gtgouzwnft.html

Ruby: items.join(",")
来源：http://hz.fzhhl.top/gtqlsllffc.html

C#:   string.Join(",", items)
来源：http://hz.xingfuxueyuan.xyz/gtvgekvkgu.html

[E09] 去除所有空白字符
来源：http://hz.mhx1999.top/gtnvdizqpj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.pycfn.com/gtzsybplfa.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.cqqwz.cn/gteksgjvmt.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.iojbl.cn/gtlzcueuil.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.yonumen.top/gtqxprikeo.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.tanke756.top/gthanhjfez.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.yj20258.top/gtjlbrudab.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.hnxiangtu.top/gtaheucejo.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.guowangkeji.top/gtxivyqgjf.html

[E10] 左侧补零 / 定长填充
来源：http://hz.ydzc1.top/gtfguanlyk.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.cqqwz.cn/gtmsyvfbsz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.shanyushiyangtech.top/gtwrusklyr.html

JS:   "7".padStart(3, "0")
来源：http://hz.jiagoushi.top/gtrlouhycf.html

TS:   "7".padStart(3, "0")
来源：http://hz.xylfe.cn/gtgivsrxnp.html

Java: String.format("%03d", 7)
来源：http://hz.gaohongyu789.top/gtiudshmup.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.shuidangran.top/gtgbopxkpz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.yj202588.top/gtjwidzoyg.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.cdnleiting.top/gthvivjuji.html

[E11] 反转字符串
来源：http://hz.yueranfly.top/gtcsnlytlj.html

Py:   s[::-1]
来源：http://hz.gzhubu.top/gtmwvssggv.html

PHP:  strrev($s);
来源：http://hz.zhixingplan.top/gtfavfeliz.html

JS:   [...s].reverse().join("")
来源：http://hz.jyoumei.cn/gtnysoqdwu.html

TS:   [...s].reverse().join("")
来源：http://hz.hnqzz.top/gtmgzwlkfg.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.wangdashe.top/gthwwzewfx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.yj202588.top/gtfptfbtsl.html

Ruby: s.reverse
来源：http://hz.tianlin.xyz/gtxsxknsbk.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.pengpengdd.cyou/gtilmhpczr.html

[E12] 统计某字符出现次数
来源：http://hz.hfpthk.cn/gtyffzqhbn.html

Py:   s.count("a")
来源：http://hz.yangfankeji.com/gtgquuyiaf.html

PHP:  substr_count($s, "a");
来源：http://hz.zhaomingkeji.xyz/gtuxasijaq.html

JS:   s.split("a").length - 1
来源：http://hz.yonumen.top/gtulmmoyrr.html

TS:   s.split("a").length - 1
来源：http://hz.hysaishi.cn/gtjvkxmzsv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.jqgufenzy.top/gtixpspqyj.html

Go:   strings.Count(s, "a")
来源：http://hz.yuanzhike.top/gteonjdxsb.html

Ruby: s.count("a")
来源：http://hz.snrcjt.cn/gtgegarzsv.html

C#:   s.Count(c => c == 'a')
来源：http://hz.nanxinkj.top/gtihqiegkn.html

[E13] 逐字符遍历
来源：http://hz.yj20258888.top/gtdizoudcl.html

Py:   for ch in s: print(ch)
来源：http://hz.52xcode.cn/gtfuyzbncg.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.shuidangran.top/gtucvmvybz.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.nanxuanxn.top/gtqjswxawo.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.iojbl.cn/gtxvbtrpme.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.kuanghao11.cn/gtzuyfshbz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.quarkkingdee.top/gtghvveprt.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.smart0.xyz/gtznezydpk.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.fengsongda.top/gtqvbmsymk.html

[E14] URL 编码与 Base64
来源：http://hz.fengsongda.top/gttaakzhbv.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.yanxiufei.cn/gtcbuipesa.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.316326.xyz/gtstrkneap.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.gaohongyu789.top/gtngnwlbwc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.shzxlz.cn/gtaeyhyjxf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.52xcode.cn/gttvgggrjr.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.ybcxt.top/gttlbzadmf.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.cheryme.top/gtpvqinbej.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.9152youxi.cn/gtxaazxzrj.html

[E15] HTML 转义 / 反转义
来源：http://hz.xylfe.cn/gtktseyyyt.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.sysykeji.top/gturgvqtcb.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.zhijiandao.cn/gtaqarigro.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.pycfn.com/gtbcatevvp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.mhx1999.top/gtalcbgsfc.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.zhengqikj.top/gteoefmpmq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.kuanghao11.cn/gtzolkgvlc.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.tian-w.cn/gtodtsztlv.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.daria6918.cn/gthwsfmxzu.html

[E16] 数字千分位
来源：http://hz.bjfxy.top/gtedwyyhad.html

Py:   f"{1234567:,}"
来源：http://hz.sxryk.cn/gtlaunbadp.html

PHP:  number_format(1234567);
来源：http://hz.zycfv.cn/gtqmrhmnsg.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.jqgufenzy.top/gtoehjoxuy.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.fzhhl.top/gtestmxski.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.nanxinkj.top/gtrjlqtxpr.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.yj202588.top/gtuokgbsbc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.tian-w.cn/gttmicfxwd.html

C#:   1234567.ToString("N0")
来源：http://hz.zhixingplan.top/gtsqsdagwb.html

[E17] 首字母大写
来源：http://hz.yuanzhike.top/gtamnabref.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.nanxuanxn.top/gtarxxbfgw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.dashuyun.cn/gtdwamjlnh.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.chenlongwang.top/gtgqzenucf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.sufxvd.cn/gtmcteuakr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.gogol.net.cn/gtjsjsgqqd.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.jinghuilouyu.cn/gtjptojvkk.html

Ruby: s.capitalize
来源：http://hz.shanyushiyangkeji.top/gtjjebhqcf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.sufxvd.cn/gtyqkhkdxw.html

[E18] 模板占位符替换
来源：http://hz.ppjwa.cn/gtgmmrmfce.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.chenjidiqi.icu/gttdejqydl.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.wangdashe.top/gtxrzacozx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.yanxiufei.cn/gtlnfvkyis.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.yvedp.cn/gtxrgatiuh.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.316326.xyz/gtnkxwvbsb.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.hammf.cn/gtlnsnfqpx.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.52xcode.cn/gtatudhdnv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.nwbrower.top/gtzdyvfkbd.html

[E19] 多行文本按行拆分
来源：http://hz.ydzc1.top/gtptyiuhme.html

Py:   s.splitlines()
来源：http://hz.pycfn.com/gtymzfefez.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.yueranfly.top/gtkmojyazt.html

JS:   s.split(/\r?\n/)
来源：http://hz.havefunace.top/gtuxtzmuzk.html

TS:   s.split(/\r?\n/)
来源：http://hz.aibaodan.cn/gtqkqdidba.html

Java: s.lines().toList()
来源：http://hz.shangyingyoupin.top/gtjqqiqiis.html

Go:   strings.Split(s, "\n")
来源：http://hz.316326.xyz/gtvieeyyef.html

Ruby: s.lines
来源：http://hz.ivvv.top/gtwiqtfqcp.html

C#:   s.Split('\n')
来源：http://hz.shanyushiyangkeji.top/gtgatoherf.html

[E20] 判断字符串是否为空
来源：http://hz.ybcxt.top/gtlqhnlxwr.html

Py:   if not s:
来源：http://hz.gotoacloud.top/gtgkbayyoj.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.hongshengwenyu.top/gthouylkjs.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.sweek.top/gtnvzkvdio.html

TS:   if (s === "") {}
来源：http://hz.sufxvd.cn/gtysbeoces.html

Java: if (s.isEmpty()) {}
来源：http://hz.redwolf501.top/gtkbrvuvga.html

Go:   if s == "" {}
来源：http://hz.jiagoushi.top/gtgxswluku.html

Ruby: if s.empty?
来源：http://hz.yuanzhike.top/gtdzomjqom.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.c1oappe.top/gtcvyjwhcu.html

[E21] 超长截断加省略号
来源：http://hz.bjfxy.top/gtittqilmu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.xuetiantiany.cn/gthqmmtizl.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.cashguo.top/gttspkwyvr.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.birdmap.top/gtrlfmqrtv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.fzhhl.top/gtifefkdod.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.feifeiyinyue.top/gttttsthvz.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.sweek.top/gtmcrnjpqz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.xuetiantiany.cn/gtwpzxzaoj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.xingfuxueyuan.xyz/gtvtjpagoa.html

[E22] 字节长度与字符长度
来源：http://hz.bjfxy.top/gtatgjenhk.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.zhijiandao.cn/gtycrmlbtj.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.shangyingyoupin.top/gtspxxnbtx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jianghu66.top/gtbeezedbd.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yanxiufei.cn/gtvpievpfk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.yj202588.top/gtlbsgzeye.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.vqdsnc.cn/gtvxfwfwlg.html

Ruby: s.bytesize;  s.length
来源：http://hz.yangfankeji.com/gtymulkpcy.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.haohaochexian.top/gtwmyybqdp.html

================================================================================
来源：http://hz.52xcode.cn/gtwnryzkrr.html

F. 文件与目录
来源：http://hz.jyoumei.cn/gtzlyyfzkd.html

================================================================================
来源：http://hz.hysaishi.cn/gtxphujbbi.html

[F01] 读取整个文件
来源：http://hz.havefunace.top/gtiedfvirl.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.xinyue.icu/gtxtnzuqsp.html

PHP:  file_get_contents("a.txt");
来源：http://hz.0kj1m.cn/gtazpdiywh.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.andypj.xyz/gtgokogzpn.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.hywenlv.cn/gthlovfywv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.aizwys.cn/gtrjchyuts.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.yueranfly.top/gtzjgwzaec.html

Ruby: File.read("a.txt")
来源：http://hz.shuidangran.top/gtsjzvmxcx.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.jyoumei.cn/gtdzbiydao.html

[F02] 逐行读取文件
来源：http://hz.ydzc1.top/gtorzkyiql.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.shuidangran.top/gtuiksmaaw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.jiagoushi.top/gtmaouyqhf.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yuanzhike.top/gtmmycqgzu.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.cucudq.cn/gtdtpjrwie.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.yuxming.cn/gtnzqvaodw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.meibo888.top/gtvbspfonf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.ppjwa.cn/gtdcokjvuh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.zhoulong.xyz/gtbpvnnpmd.html

[F03] 写入文件（覆盖）
来源：http://hz.316326.xyz/gtqqykfuzl.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.shanyushiyangtech.top/gtzijtqyoo.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.zhengqikj.top/gtnevrvvzr.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yongpay.top/gteayeemhk.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ivvv.top/gtdwpxttmd.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.jyoumei.cn/gtohmfvjub.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.sxryk.cn/gtkajsungo.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.gogol.net.cn/gtyrnzbmav.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.yuxming.cn/gtofqgvlyn.html

[F04] 追加写入文件
来源：http://hz.sweek.top/gteuixbezn.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.dashuyun.cn/gtrtlythne.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.hnqzz.top/gtlhqjspec.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.shangyingyoupin.top/gtmtjbjirj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhaomingkeji.xyz/gteycrjsfc.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.cdnleiting.top/gtsepmwpvh.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.chenjidiqi.icu/gtdwtmdsco.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.aibaodan.cn/gtakbhndfx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.xinyue.icu/gtopoawxxx.html

[F05] 判断文件或目录是否存在
来源：http://hz.wangdashe.top/gteuvlfews.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.shangyingyoupin.top/gtnnythtkq.html

PHP:  file_exists("a.txt");
来源：http://hz.yj20258.top/gtbfcdfqtm.html

JS:   fs.existsSync("a.txt")
来源：http://hz.316326.xyz/gtngahrixf.html

TS:   fs.existsSync("a.txt")
来源：http://hz.smart0.xyz/gtvunvvpmy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.tianlin.xyz/gtlsbxzdwb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.zhoulong.xyz/gtqhietnqs.html

Ruby: File.exist?("a.txt")
来源：http://hz.xuanzx.com/gtdgtgeltk.html

C#:   File.Exists("a.txt")
来源：http://hz.mhx1999.top/gtbkxfsbsv.html

[F06] 删除文件
来源：http://hz.hammf.cn/gtjyaeohmo.html

Py:   os.remove("a.txt")
来源：http://hz.0kj1m.cn/gtykpiklyq.html

PHP:  unlink("a.txt");
来源：http://hz.cucudq.cn/gtuoadzhdb.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.smart0.xyz/gttmvfhcrl.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.hongshengwenyu.top/gtuznvmbpy.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.dianchejie.cn/gtyentqowp.html

Go:   os.Remove("a.txt")
来源：http://hz.aizwys.cn/gtuptjcrkc.html

Ruby: File.delete("a.txt")
来源：http://hz.pengpengdd.cyou/gtpzdvvvvf.html

C#:   File.Delete("a.txt");
来源：http://hz.birdmap.top/gtrmcsblql.html

[F07] 创建目录（含多级）
来源：http://hz.yongpay.top/gtpeqtlalw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.gzhubu.top/gtekdpksif.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.snrcjt.cn/gtzvfohjbm.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jinghuilouyu.cn/gtgshbezgw.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jinqigufen.top/gtsuotcswl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.guannengcc.top/gtsfxmhcny.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.nanxinkj.top/gtyhzqmyxg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.hfpthk.cn/gtjkidktds.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.tianlin.xyz/gtysoozptn.html

[F08] 遍历目录
来源：http://hz.cucudq.cn/gtzpllqdqd.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.shzxlz.cn/gtlehqcvce.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.xylfe.cn/gtigddyziw.html

JS:   fs.readdirSync("dir")
来源：http://hz.ppjwa.cn/gtibfgqktx.html

TS:   fs.readdirSync("dir")
来源：http://hz.zhijiandao.cn/gtjxkiutob.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.ydzc1.top/gtyfhzmgrh.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.tianlin.xyz/gtnsutvihk.html

Ruby: Dir.children("dir")
来源：http://hz.zhongyouzk.top/gtlyqiieyg.html

C#:   Directory.GetFiles("dir")
来源：http://hz.hfpthk.cn/gtdonhrtlz.html

[F09] 获取文件大小
来源：http://hz.shanyushiyangkeji.top/gtuwnnxmqt.html

Py:   os.path.getsize("a.txt")
来源：http://hz.cdnleiting.top/gtypvazyiz.html

PHP:  filesize("a.txt");
来源：http://hz.mhx1999.top/gtzxbmrwwn.html

JS:   fs.statSync("a.txt").size
来源：http://hz.tianlin.xyz/gtgvajxcdj.html

TS:   fs.statSync("a.txt").size
来源：http://hz.dianchejie.cn/gtcwgfncvk.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.xziqi.cn/gtaqomccpw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.zhoulong.xyz/gtuqgqacbo.html

Ruby: File.size("a.txt")
来源：http://hz.hnxiangtu.top/gtpbfdtnig.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.ydzc1.top/gtetyxvvfc.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.iojbl.cn/gtthnhvhkl.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.daxiang520.top/gtmqmquivx.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.hnxiangtu.top/gttllisbwh.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.zhengqikj.top/gtigyreasv.html

TS:   path.extname("a.txt")
来源：http://hz.jlsjyb.cn/gttzhsgycl.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.nanxinkj.top/gtqorrtpqd.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.feifeiyinyue.top/gtepeslsxj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.zycfv.cn/gtguuunshw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.jinyuanbaomall.cn/gtaklospmw.html

[F11] 复制与移动文件
来源：http://hz.hammf.cn/gtmvsqrrbm.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.jinghuilouyu.cn/gtggetpvfg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.cucudq.cn/gtevbofnko.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.wangshuangyany.cn/gtyybjjbcu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xuetiantiany.cn/gtbsxcocdj.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.zhoulong.xyz/gtlekoqwhc.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.xingfuxueyuan.xyz/gtqwwfoxgv.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.cheryme.top/gtmazauegk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.chenjidiqi.icu/gtwkugtwvu.html

[F12] CSV 读写
来源：http://hz.shzxlz.cn/gtioumiqsc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.yj20258.top/gtbruoljwo.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.cucudq.cn/gtixqdyrhr.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.ppjwa.cn/gtppszzmej.html

TS:   // 同上
来源：http://hz.nanxuanxn.top/gtnrxwsfmm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.hongshengwenyu.top/gtsvzdgfvm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yangfankeji.com/gtluuxkatw.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.yj20258888.top/gtwmyvaucl.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.ywan-chungtsiang.top/gtlcetrgba.html


<!-- 参考信息 -->