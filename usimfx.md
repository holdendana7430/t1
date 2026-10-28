代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.shanyushiyangkeji.top/gtvnqliram.html

[E03] 截取子串
来源：http://hz.yuanzhike.top/gtkhmcwhym.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.zhixingplan.top/gthirmbqzx.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.cucudq.cn/gtgkmtyuwn.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.shanyushiyangtech.top/gttlcbtcye.html

TS:   s.slice(1, 4)
来源：http://hz.cashguo.top/gtonniyyok.html

Java: s.substring(1, 4)
来源：http://hz.xuanzx.com/gtwqduohld.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.yuanzhike.top/gtmlujwbnk.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.zhiwuduotai.top/gttltrnikb.html

C#:   s.Substring(1, 3)
来源：http://hz.guannengcc.top/gtifvzgmeg.html

[E04] 查找子串位置
来源：http://hz.xuanzx.com/gtccvevkop.html

Py:   s.find("x");  s.index("x")
来源：http://hz.tian-w.cn/gtardrmcxe.html

PHP:  strpos($s, "x");
来源：http://hz.316326.xyz/gthkwsqhbu.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.zhijiandao.cn/gtcqkifasy.html

TS:   s.indexOf("x")
来源：http://hz.wangdashe.top/gttqthyvrz.html

Java: s.indexOf("x")
来源：http://hz.yj20258888.top/gtihjdkndc.html

Go:   strings.Index(s, "x")
来源：http://hz.yj20258888.top/gtznmdkcci.html

Ruby: s.index("x")
来源：http://hz.ydzc1.top/gtqeunpcbs.html

C#:   s.IndexOf("x")
来源：http://hz.cheryme.top/gtcqpvhasq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.316326.xyz/gtxmegbjrg.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.aizwys.cn/gtqggvslbr.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.jinqigfzy.top/gtdjhqdrdg.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zhixingplan.top/gtcghxrwpq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.zhengqikj.top/gtrlyvzqro.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.gzhubu.top/gtqlulfxeu.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.svipenyu.cn/gtnxvrmase.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.jianghu66.top/gtxmutuvor.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.haohaochexian.top/gtgvkxtmfu.html

[E06] 替换子串
来源：http://hz.nanxinkj.top/gtynfkmjbt.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.bjfxy.top/gtsntuckzv.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.yangfankeji.com/gtsssczgdn.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.cheryme.top/gtwfkiocvh.html

TS:   s.replaceAll("a", "b")
来源：http://hz.jianghu66.top/gtpmadebyj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jinqigufen.top/gtwddmfplg.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.aizwys.cn/gtxfkhtblm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.jyoumei.cn/gtiwchqgmv.html

C#:   s.Replace("a", "b")
来源：http://hz.kuanghao11.cn/gtclouxqzk.html

[E07] 按分隔符拆分
来源：http://hz.ydjk.org.cn/gtrdkxgpmf.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.jyoumei.cn/gtqcwyhbdo.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.nanxinkj.top/gttaccbuin.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.aibaodan.cn/gtrmgkqzjq.html

TS:   s.split(",")
来源：http://hz.sysykeji.top/gtwxsthzws.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.yongpay.top/gtiuyhhhgo.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.jinqigufen.top/gtvkwkpjxl.html

Ruby: s.split(",");  s.split
来源：http://hz.zhoulong.xyz/gtjsswejab.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.tanke756.top/gtpflrfcjl.html

[E08] 数组按分隔符合并
来源：http://hz.kuanghao11.cn/gtargxlhvn.html

Py:   ",".join(items)
来源：http://hz.iojbl.cn/gtropmvjaa.html

PHP:  implode(",", $items);
来源：http://hz.guowangkeji.top/gtynwykxco.html

JS:   items.join(",")
来源：http://hz.zhixingplan.top/gttanxzjes.html

TS:   items.join(",")
来源：http://hz.xuanzx.com/gtdohxozxs.html

Java: String.join(",", items)
来源：http://hz.jianghu66.top/gtajvlhivg.html

Go:   strings.Join(items, ",")
来源：http://hz.jinghuilouyu.cn/gteuytnmai.html

Ruby: items.join(",")
来源：http://hz.xylfe.cn/gtnsjxdpgd.html

C#:   string.Join(",", items)
来源：http://hz.daria6918.cn/gtwsymgzgf.html

[E09] 去除所有空白字符
来源：http://hz.jinqigufen.top/gtikbcpvuk.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.tian-w.cn/gtxgtxoshq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.jlsjyb.cn/gtuwhjwvpc.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.yj20258.top/gtjjevkvzv.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.jinqigufen.top/gtgwivnaqn.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.jinghuilouyu.cn/gtvsxyeuqo.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.yj20258.top/gtzesermzm.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.ivvv.top/gtdgnybwek.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.gotoacloud.top/gtazchtmvp.html

[E10] 左侧补零 / 定长填充
来源：http://hz.nanxinkj.top/gtwbfljtiv.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.shangyingyoupin.top/gtwfkmefjs.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.cashguo.top/gtltwxogts.html

JS:   "7".padStart(3, "0")
来源：http://hz.hnqzz.top/gtkqcfaswf.html

TS:   "7".padStart(3, "0")
来源：http://hz.nanxuanxn.top/gtckmpnzcx.html

Java: String.format("%03d", 7)
来源：http://hz.hfpthk.cn/gtlybekomp.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.jinyuanbaomall.cn/gtjwrhbwdi.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.gaohongyu789.top/gtyexhosyo.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.gogol.net.cn/gtedmuetkb.html

[E11] 反转字符串
来源：http://hz.cucudq.cn/gtithkdmhw.html

Py:   s[::-1]
来源：http://hz.hnxiangtu.top/gtwnwlsqol.html

PHP:  strrev($s);
来源：http://hz.gogol.net.cn/gtyukauucv.html

JS:   [...s].reverse().join("")
来源：http://hz.jyoumei.cn/gtxcgptfco.html

TS:   [...s].reverse().join("")
来源：http://hz.nwbrower.top/gttykvpatl.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.chenjidiqi.icu/gtawrbnznb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.xingfuxueyuan.xyz/gtomnyzzwi.html

Ruby: s.reverse
来源：http://hz.0kj1m.cn/gtrcyjvfsd.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.yuxming.cn/gtkglbzxvh.html

[E12] 统计某字符出现次数
来源：http://hz.smart0.xyz/gtcrbhjrjl.html

Py:   s.count("a")
来源：http://hz.pycfn.com/gtoqgyzlwl.html

PHP:  substr_count($s, "a");
来源：http://hz.shzxlz.cn/gtfdpnehvg.html

JS:   s.split("a").length - 1
来源：http://hz.haohaochexian.top/gtzghpvege.html

TS:   s.split("a").length - 1
来源：http://hz.yangfankeji.com/gtqcypjmxx.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.9152youxi.cn/gtjqlwigmc.html

Go:   strings.Count(s, "a")
来源：http://hz.pengpengdd.cyou/gtqlqbdtbm.html

Ruby: s.count("a")
来源：http://hz.hongshengwenyu.top/gtjopvszyy.html

C#:   s.Count(c => c == 'a')
来源：http://hz.meibo888.top/gtbxqlspux.html

[E13] 逐字符遍历
来源：http://hz.gotoacloud.top/gtfwbjkgrq.html

Py:   for ch in s: print(ch)
来源：http://hz.dashuyun.cn/gtakdpgoxu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.9152youxi.cn/gtejdllago.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yonumen.top/gteinzbwxz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.svipenyu.cn/gtrqqsoxos.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.fzhhl.top/gthhecinnh.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.kuanghao11.cn/gttmffsneh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.daria6918.cn/gtervqiccb.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.smart0.xyz/gtpazjidwx.html

[E14] URL 编码与 Base64
来源：http://hz.hnqzz.top/gtjpumvjoq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.smart0.xyz/gtxjpgnlth.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.tian-w.cn/gtsqsfvshk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.shanyushiyangkeji.top/gtgrnngpqf.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.ydzc1.top/gtnrogrvie.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.cheryme.top/gtkwbddikp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.dianchejie.cn/gtmidgtnfq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.shanyushiyangtech.top/gtfgxrpomj.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.sxryk.cn/gtsaqqbedh.html

[E15] HTML 转义 / 反转义
来源：http://hz.pengpengdd.cyou/gtrhjrgkjd.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.redwolf501.top/gthbvomlhx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.sysykeji.top/gthowknigu.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.hnqzz.top/gtpubdysgc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.hammf.cn/gtinwubean.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.0kj1m.cn/gtbessjunw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.cucudq.cn/gtlnykcxcw.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.zhijiandao.cn/gtkqaxstcg.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.jinqigufen.top/gtwparraac.html

[E16] 数字千分位
来源：http://hz.wangdashe.top/gtgracsjww.html

Py:   f"{1234567:,}"
来源：http://hz.wangdashe.top/gtcwaezdan.html

PHP:  number_format(1234567);
来源：http://hz.guannengcc.top/gtjhlrjcho.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.daria6918.cn/gtvebtmyuy.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.bjfxy.top/gtmpscqedk.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.xziqi.cn/gtziqswzrh.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.bjfxy.top/gtlclihjij.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.svipenyu.cn/gtxjooalln.html

C#:   1234567.ToString("N0")
来源：http://hz.nwbrower.top/gtquqhijqi.html

[E17] 首字母大写
来源：http://hz.tanke756.top/gtiiidursd.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.jinqigfzy.top/gthjbbkgaa.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.xziqi.cn/gtzrxqnazc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.bjfxy.top/gtzkxdrnfx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.aizwys.cn/gteumamekq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.zhoulong.xyz/gtfjduqryr.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.svipenyu.cn/gtkirhqbqu.html

Ruby: s.capitalize
来源：http://hz.redwolf501.top/gtehpuetqj.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.havefunace.top/gtuwvojbsi.html

[E18] 模板占位符替换
来源：http://hz.9152youxi.cn/gtbenvapwl.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.xinyue.icu/gtyqdymhys.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.yuxming.cn/gtzhdqqwvb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.yangfankeji.com/gthtxslogr.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.yj202588.top/gtcuazxnhj.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.svipenyu.cn/gtuyerrerc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.daria6918.cn/gtptizkcra.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.tianlin.xyz/gtsozhqbpe.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.zhongyouzk.top/gtcdxwbjqp.html

[E19] 多行文本按行拆分
来源：http://hz.havefunace.top/gthdbfweyg.html

Py:   s.splitlines()
来源：http://hz.dashuyun.cn/gtqjgoxxur.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.hysaishi.cn/gtuxumztfm.html

JS:   s.split(/\r?\n/)
来源：http://hz.ivvv.top/gtruqbqxza.html

TS:   s.split(/\r?\n/)
来源：http://hz.zdqjudy.top/gttxivzwby.html

Java: s.lines().toList()
来源：http://hz.ydzc1.top/gtgthgryvp.html

Go:   strings.Split(s, "\n")
来源：http://hz.hfpthk.cn/gtniyjzlds.html

Ruby: s.lines
来源：http://hz.yuxming.cn/gtvlnsjebv.html

C#:   s.Split('\n')
来源：http://hz.chenjidiqi.icu/gtpoqkmmnd.html

[E20] 判断字符串是否为空
来源：http://hz.jqgfzy.top/gtuxanzvxz.html

Py:   if not s:
来源：http://hz.shanyushiyangtech.top/gtjvugnrpz.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.jiagoushi.top/gtbqippnjj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.ehwqpu.com/gtgywlvzlt.html

TS:   if (s === "") {}
来源：http://hz.yvedp.cn/gtmxxvfodp.html

Java: if (s.isEmpty()) {}
来源：http://hz.cashguo.top/gtljxtzpzq.html

Go:   if s == "" {}
来源：http://hz.zycfv.cn/gtyebsaaok.html

Ruby: if s.empty?
来源：http://hz.yj20258.top/gtofhbjkhb.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.shzxlz.cn/gttglolfww.html

[E21] 超长截断加省略号
来源：http://hz.daria6918.cn/gtxmcyxpmo.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.nanxinkj.top/gtbunkxbwb.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.quarkkingdee.top/gtosnkyrzw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.9152youxi.cn/gtkrrwnddy.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.hysaishi.cn/gtuooyvkcz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.aibaodan.cn/gtdtqmtrgg.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.gzhubu.top/gtiyqgbuid.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.fengsongda.top/gtswgeplks.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.ivvv.top/gthlnteqvy.html

[E22] 字节长度与字符长度
来源：http://hz.xylfe.cn/gtqhljjpci.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.tanke756.top/gtqechkgef.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jqgfzy.top/gtwdpunmcp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zdqjudy.top/gtehyaxnkx.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.316326.xyz/gtdmwehtue.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.zhoulong.xyz/gtljikqsux.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.quarkkingdee.top/gtexvuafvp.html

Ruby: s.bytesize;  s.length
来源：http://hz.pengpengdd.cyou/gtpgyxncho.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.sweek.top/gtbnrevvxd.html

================================================================================
来源：http://hz.sysykeji.top/gtjgzupsme.html

F. 文件与目录
来源：http://hz.chenjidiqi.icu/gtjocwmvtq.html

================================================================================
来源：http://hz.xylfe.cn/gtivkrrint.html

[F01] 读取整个文件
来源：http://hz.shanyushiyangtech.top/gtppyhffjn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.cdnleiting.top/gtzpfjzfot.html

PHP:  file_get_contents("a.txt");
来源：http://hz.hnxiangtu.top/gtosivablw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.cashguo.top/gtnnsrriac.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.ybcxt.top/gtssgjrbad.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.ydzc1.top/gthyawgjwg.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.pycfn.com/gtxgfenblr.html

Ruby: File.read("a.txt")
来源：http://hz.gogol.net.cn/gtlphbqvid.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yj20258888.top/gtnixkmcmv.html

[F02] 逐行读取文件
来源：http://hz.zhengqikj.top/gtwanbjtcl.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.gogol.net.cn/gtwmgxsrzz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.sweek.top/gtsldlyfxc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.nanxuanxn.top/gtpdiioafv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.cucudq.cn/gtycltunnm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.xuetiantiany.cn/gtzdmtqlhj.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.yongpay.top/gtpiblndrg.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yonumen.top/gteczwrzok.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.pengpengdd.cyou/gtbbrrmwpt.html

[F03] 写入文件（覆盖）
来源：http://hz.cqqwz.cn/gtuarpjaqm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.sysykeji.top/gtudmyllsd.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.jinyuanbaomall.cn/gtekbjbvsx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jinqigfzy.top/gterzlcbbn.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.svipenyu.cn/gtcwldiurq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.chenjidiqi.icu/gtjpjamosz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.yanxiufei.cn/gtswgyjcjm.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.hysaishi.cn/gtdzikaztp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.xingfuxueyuan.xyz/gtyfifcpbr.html

[F04] 追加写入文件
来源：http://hz.yj20258.top/gtcgawgkqn.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.vqdsnc.cn/gtlrvopoyu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.xinyue.icu/gtkzihonzz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.sweek.top/gtkvxloajb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.quarkkingdee.top/gtfpgdnnbu.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.tian-w.cn/gtjcdxlyun.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.0kj1m.cn/gtdqxmukak.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.sysykeji.top/gtiasmygxn.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.0kj1m.cn/gtxtjpfrrx.html

[F05] 判断文件或目录是否存在
来源：http://hz.wangdashe.top/gtugjglsof.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.jinqigfzy.top/gtbzgzejku.html

PHP:  file_exists("a.txt");
来源：http://hz.haohaochexian.top/gtextihacj.html

JS:   fs.existsSync("a.txt")
来源：http://hz.zhiwuduotai.top/gtuiehztkb.html

TS:   fs.existsSync("a.txt")
来源：http://hz.mhx1999.top/gtgbzxqdsn.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.wangshuangyany.cn/gtqvwollgg.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.aizwys.cn/gtujeabliq.html

Ruby: File.exist?("a.txt")
来源：http://hz.52xcode.cn/gtokspegvq.html

C#:   File.Exists("a.txt")
来源：http://hz.yuanzhike.top/gtrqcsaifv.html

[F06] 删除文件
来源：http://hz.nwbrower.top/gtviuflfyb.html

Py:   os.remove("a.txt")
来源：http://hz.feifeiyinyue.top/gtwlohlzas.html

PHP:  unlink("a.txt");
来源：http://hz.daria6918.cn/gtxwbmgaao.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.dianchejie.cn/gtscgywfyl.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.fzhhl.top/gtrzqylkho.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.chenjidiqi.icu/gtwfkvhwzp.html

Go:   os.Remove("a.txt")
来源：http://hz.shangyingyoupin.top/gtgssrqhei.html

Ruby: File.delete("a.txt")
来源：http://hz.yj202588.top/gtdcslkyci.html

C#:   File.Delete("a.txt");
来源：http://hz.guowangkeji.top/gtovgdpcbb.html

[F07] 创建目录（含多级）
来源：http://hz.zhengqikj.top/gtycucgnie.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.ybcxt.top/gtxmqkklwk.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.snrcjt.cn/gtxpvfxyii.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.bjfxy.top/gtjsabzjjg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yj202588.top/gtwylnvrxh.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.aizwys.cn/gtkrmxtyds.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jlsjyb.cn/gtnhbpqwdj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.cheryme.top/gtbrwwavpk.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.jqgfzy.top/gtpapiflms.html

[F08] 遍历目录
来源：http://hz.9152youxi.cn/gtrxezhmsl.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.nwbrower.top/gtsjnjuutn.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.pengpengdd.cyou/gtahuawixj.html

JS:   fs.readdirSync("dir")
来源：http://hz.tianlin.xyz/gtawrnbmwv.html

TS:   fs.readdirSync("dir")
来源：http://hz.aizwys.cn/gtodekszih.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.jqgfzy.top/gtlqstjshs.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.jqgufenzy.top/gtncqxzjvj.html

Ruby: Dir.children("dir")
来源：http://hz.yueranfly.top/gtybfvwrws.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yonumen.top/gtmsbhbice.html

[F09] 获取文件大小
来源：http://hz.hfpthk.cn/gtbehybnfe.html

Py:   os.path.getsize("a.txt")
来源：http://hz.yvedp.cn/gtwfsuefms.html

PHP:  filesize("a.txt");
来源：http://hz.tanke756.top/gtrbotqikk.html

JS:   fs.statSync("a.txt").size
来源：http://hz.ehwqpu.com/gtzcelvlua.html

TS:   fs.statSync("a.txt").size
来源：http://hz.zhijiandao.cn/gtjykzsjoj.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.xylfe.cn/gtixjwiwdr.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.kuanghao11.cn/gtdgrahuom.html

Ruby: File.size("a.txt")
来源：http://hz.hammf.cn/gtjtqthpss.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.zhengqikj.top/gtaotexpsz.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.gzhubu.top/gtkecfatyl.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.ydjk.org.cn/gtaxgwzvma.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.gaohongyu789.top/gtrmsuhxmk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.jinghuilouyu.cn/gtmbxlhwbs.html

TS:   path.extname("a.txt")
来源：http://hz.svipenyu.cn/gttbylfcro.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.yj202588.top/gtecfmfzwz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.0kj1m.cn/gtsknegjsv.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.snrcjt.cn/gtexmcytzz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.jianghu66.top/gtbjsndzfr.html

[F11] 复制与移动文件
来源：http://hz.yj202588.top/gtzlmsonui.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.xingfuxueyuan.xyz/gtlvuxlits.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.xingfuxueyuan.xyz/gtnkbxkqeb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.gaohongyu789.top/gthhhbbhel.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yj20258888.top/gtglcpkrfb.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.chenjidiqi.icu/gtxlwumxqp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.snrcjt.cn/gtfzkzmbyv.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.zdqjudy.top/gtcmhbfqgo.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.svipenyu.cn/gtavwdnikr.html

[F12] CSV 读写
来源：http://hz.c1oappe.top/gtvjbgnacp.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.zhixingplan.top/gtjmhmxpif.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.tianlin.xyz/gtmyikhwhc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.jqgfzy.top/gtsdqpznjr.html

TS:   // 同上
来源：http://hz.9152youxi.cn/gtcmrcbitm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.0kj1m.cn/gtswumoifx.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.daxiang520.top/gtllihoiic.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.pycfn.com/gtobfpwuem.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.316326.xyz/gtmzhuxatr.html

================================================================================
来源：http://hz.aizwys.cn/gtkkmvfhzv.html

G. 面向对象
来源：http://hz.aibaodan.cn/gtvrxeihpa.html

================================================================================
来源：http://hz.jlsjyb.cn/gtyehnpdwh.html

[G01] 定义类
来源：http://hz.jyoumei.cn/gtsrywltnw.html

Py:   class User: pass
来源：http://hz.xziqi.cn/gtguwiynnb.html

PHP:  class User {}
来源：http://hz.0kj1m.cn/gtrjchrtpv.html

JS:   class User {}
来源：http://hz.andypj.xyz/gtytvjxzan.html

TS:   class User { name: string = ""; }
来源：http://hz.hnxiangtu.top/gtwimhevkw.html


<!-- 参考信息 -->