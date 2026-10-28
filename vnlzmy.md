代发 wailian999

C#:   s.Replace("a", "b")
来源：http://hz.hnqzz.top/gthivzhrzn.html

[E07] 按分隔符拆分
来源：http://hz.xingfuxueyuan.xyz/gtqubrvliv.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.316326.xyz/gtqwzlgmst.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.c1oappe.top/gtfumxtmwd.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.316326.xyz/gtbkrxhopq.html

TS:   s.split(",")
来源：http://hz.cashguo.top/gtdczsljoz.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.yj202588.top/gtaqddyaby.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.yongpay.top/gtlqjjbrah.html

Ruby: s.split(",");  s.split
来源：http://hz.zdqjudy.top/gtvaerakhq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.aizwys.cn/gtkucwnlpm.html

[E08] 数组按分隔符合并
来源：http://hz.snrcjt.cn/gtobdbdrgl.html

Py:   ",".join(items)
来源：http://hz.xylfe.cn/gtpqwejpuc.html

PHP:  implode(",", $items);
来源：http://hz.tian-w.cn/gtebfrtabh.html

JS:   items.join(",")
来源：http://hz.zhongyouzk.top/gtannvnmfn.html

TS:   items.join(",")
来源：http://hz.0kj1m.cn/gtueaqlovq.html

Java: String.join(",", items)
来源：http://hz.hongshengwenyu.top/gtysgpzfar.html

Go:   strings.Join(items, ",")
来源：http://hz.zhoulong.xyz/gtqvskunnj.html

Ruby: items.join(",")
来源：http://hz.sysykeji.top/gthaaptqnf.html

C#:   string.Join(",", items)
来源：http://hz.jyoumei.cn/gtdmlepuuw.html

[E09] 去除所有空白字符
来源：http://hz.jiagoushi.top/gtvaqemzrx.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.yuxming.cn/gtwnqgpiol.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.yj20258.top/gtcwgjyapy.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.bjfxy.top/gtarvrwguj.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.dashuyun.cn/gtmkvzruio.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.ppjwa.cn/gtpagovpiy.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.chenzaomai.com/gtpwekubuu.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.tanke756.top/gtxfqqyigl.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.chenlongwang.top/gtbzvtumge.html

[E10] 左侧补零 / 定长填充
来源：http://hz.fengsongda.top/gtqdpvlvlz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.haohaochexian.top/gthgibbcrq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.cdnleiting.top/gtbuootilm.html

JS:   "7".padStart(3, "0")
来源：http://hz.iojbl.cn/gtmassxhbl.html

TS:   "7".padStart(3, "0")
来源：http://hz.wangshuangyany.cn/gtirentojn.html

Java: String.format("%03d", 7)
来源：http://hz.mhx1999.top/gtakhwbymk.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.c1oappe.top/gtvluxxfzg.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.zhongyouzk.top/gtdxrrvrmq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.wangshuangyany.cn/gtberzjikk.html

[E11] 反转字符串
来源：http://hz.tian-w.cn/gthwbnudly.html

Py:   s[::-1]
来源：http://hz.hnxiangtu.top/gtsdpbgiae.html

PHP:  strrev($s);
来源：http://hz.sweek.top/gtmxehwbmc.html

JS:   [...s].reverse().join("")
来源：http://hz.aizwys.cn/gtpjoxniwc.html

TS:   [...s].reverse().join("")
来源：http://hz.chenlongwang.top/gtypdlmxnk.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.shangyingyoupin.top/gtcuhqibsh.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.dianchejie.cn/gtthxcikwe.html

Ruby: s.reverse
来源：http://hz.zhongyouzk.top/gtlrsjdjow.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.iojbl.cn/gtnkfzmqki.html

[E12] 统计某字符出现次数
来源：http://hz.cashguo.top/gtjsckpkay.html

Py:   s.count("a")
来源：http://hz.xinyue.icu/gtywltozjf.html

PHP:  substr_count($s, "a");
来源：http://hz.gzhubu.top/gtvmbetamn.html

JS:   s.split("a").length - 1
来源：http://hz.ydzc1.top/gtjxoijfzy.html

TS:   s.split("a").length - 1
来源：http://hz.guannengcc.top/gtumuxqxfz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.jqgfzy.top/gtxuiodzfg.html

Go:   strings.Count(s, "a")
来源：http://hz.jinghuilouyu.cn/gtsvcxzofh.html

Ruby: s.count("a")
来源：http://hz.guowangkeji.top/gtdvwpfvka.html

C#:   s.Count(c => c == 'a')
来源：http://hz.gotoacloud.top/gtmjqsoxfe.html

[E13] 逐字符遍历
来源：http://hz.daria6918.cn/gtcppynifv.html

Py:   for ch in s: print(ch)
来源：http://hz.yangfankeji.com/gthjmxtvpy.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.cqqwz.cn/gtvxnappbe.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.shuidangran.top/gtsbmkjcko.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.hfpthk.cn/gtluuyfkwn.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.gogol.net.cn/gtdmuacsfv.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.meibo888.top/gtzmyjgfvd.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.xinyue.icu/gtzdxuwqyc.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.kuanghao11.cn/gtutqxrtda.html

[E14] URL 编码与 Base64
来源：http://hz.quarkkingdee.top/gtjybflbje.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.jinqigufen.top/gtauqgjvfm.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.jinghuilouyu.cn/gtffalnsll.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.iojbl.cn/gtnkmmsnzn.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.cdnleiting.top/gtkjqdisei.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.52xcode.cn/gtzslkknzl.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.shzxlz.cn/gtepzaqzqc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.shanyushiyangkeji.top/gtctpeukpv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.cqqwz.cn/gtzlxromeh.html

[E15] HTML 转义 / 反转义
来源：http://hz.jinqigfzy.top/gttkncbgdq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.svipenyu.cn/gtqjbjujmf.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.tianlin.xyz/gtbjunjjsk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.shzxlz.cn/gtrdztpgji.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.smart0.xyz/gtpmctebsn.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.feifeiyinyue.top/gtkelzwuqh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.yonumen.top/gtbvelhkga.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.tianlin.xyz/gtocancgqo.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.ppjwa.cn/gtyndfytmi.html

[E16] 数字千分位
来源：http://hz.shuidangran.top/gtoytzhnbu.html

Py:   f"{1234567:,}"
来源：http://hz.ydzc1.top/gtkkqqhxsc.html

PHP:  number_format(1234567);
来源：http://hz.zhongyouzk.top/gtaqyeoeeg.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.yonumen.top/gttfyxgwag.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.tian-w.cn/gtqevavmrd.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.shanyushiyangtech.top/gtesylnoye.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.tanke756.top/gtdectdopm.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.zdqjudy.top/gtwymllzyi.html

C#:   1234567.ToString("N0")
来源：http://hz.hnxiangtu.top/gtmhzsdjpc.html

[E17] 首字母大写
来源：http://hz.quarkkingdee.top/gtgoayaeym.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.ppjwa.cn/gthopogkrr.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.mhx1999.top/gtoaxxhuqc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ppjwa.cn/gtrjjmkujw.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.dashuyun.cn/gtwwrjhjou.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.jinqigfzy.top/gtkijlqraa.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.sweek.top/gtiwtkkeew.html

Ruby: s.capitalize
来源：http://hz.yanxiufei.cn/gtztvcffto.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.316326.xyz/gtiupbnjxe.html

[E18] 模板占位符替换
来源：http://hz.aizwys.cn/gtyajqgtgo.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.fzhhl.top/gtetymkinz.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.bjfxy.top/gtohlutixp.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.hfpthk.cn/gtwuhjsyvh.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.xylfe.cn/gteiodrbkw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.jianghu66.top/gtbpxqftfm.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.ehwqpu.com/gtsgidrvaj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.andypj.xyz/gthrofbcoh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.jinqigufen.top/gttjgwsltm.html

[E19] 多行文本按行拆分
来源：http://hz.daria6918.cn/gtympnegnk.html

Py:   s.splitlines()
来源：http://hz.feifeiyinyue.top/gtbqcnqfbr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.fengsongda.top/gtrqmikhje.html

JS:   s.split(/\r?\n/)
来源：http://hz.hnqzz.top/gtzqvcsmlc.html

TS:   s.split(/\r?\n/)
来源：http://hz.tianlin.xyz/gtqzokoyhs.html

Java: s.lines().toList()
来源：http://hz.chenjidiqi.icu/gtnukhwtyq.html

Go:   strings.Split(s, "\n")
来源：http://hz.guannengcc.top/gtjfitwlpb.html

Ruby: s.lines
来源：http://hz.nanxuanxn.top/gtntrtvrmt.html

C#:   s.Split('\n')
来源：http://hz.yj20258.top/gtcbifikrf.html

[E20] 判断字符串是否为空
来源：http://hz.jiagoushi.top/gtdgvwhjow.html

Py:   if not s:
来源：http://hz.chenlongwang.top/gtvytecasq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.zhengqikj.top/gtcrpywrbn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.ywan-chungtsiang.top/gtbisoehqp.html

TS:   if (s === "") {}
来源：http://hz.feifeiyinyue.top/gtxtkkhahu.html

Java: if (s.isEmpty()) {}
来源：http://hz.birdmap.top/gttsvjleht.html

Go:   if s == "" {}
来源：http://hz.yanxiufei.cn/gtdkhqxsqy.html

Ruby: if s.empty?
来源：http://hz.cdnleiting.top/gtarkxzhdi.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.yvedp.cn/gtdyyaejly.html

[E21] 超长截断加省略号
来源：http://hz.zycfv.cn/gtyugxtddo.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.yj20258.top/gtdsltdrvd.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.bjfxy.top/gtkgojsamd.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.haohaochexian.top/gtierlprak.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.shzxlz.cn/gtfstxrual.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.xinyue.icu/gtehjvzczk.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.daria6918.cn/gtgweihwdc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.pengpengdd.cyou/gtlumjrdji.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.tianlin.xyz/gtveozjaug.html

[E22] 字节长度与字符长度
来源：http://hz.cdnleiting.top/gtjzjcbvby.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.xinyue.icu/gtstemwgcg.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.hnxiangtu.top/gtwcitvcjp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.shanyushiyangkeji.top/gtyhvygevm.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.quarkkingdee.top/gtxbjmxemh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.cashguo.top/gtuawbcljo.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.chenlongwang.top/gtwgwufbge.html

Ruby: s.bytesize;  s.length
来源：http://hz.zycfv.cn/gtgnggrggq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.gotoacloud.top/gtcgqwclqa.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtxbxdfzft.html

F. 文件与目录
来源：http://hz.yongpay.top/gtmfvvzlju.html

================================================================================
来源：http://hz.tian-w.cn/gtlwxyqgjp.html

[F01] 读取整个文件
来源：http://hz.xuetiantiany.cn/gtmmtqhodi.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yj20258.top/gtajltucdy.html

PHP:  file_get_contents("a.txt");
来源：http://hz.ywan-chungtsiang.top/gtskpodbao.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.jinqigufen.top/gttdtcvilh.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.yangfankeji.com/gtgkcugsby.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.aibaodan.cn/gttqmwrbjv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.iojbl.cn/gtdwdcuhfz.html

Ruby: File.read("a.txt")
来源：http://hz.cashguo.top/gtdlxilkfv.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.hywenlv.cn/gtpxjkohit.html

[F02] 逐行读取文件
来源：http://hz.jlsjyb.cn/gtfsxuvdkh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.xingfuxueyuan.xyz/gtaluxrker.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.iojbl.cn/gthvyofrta.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.daria6918.cn/gtfjiwgvwz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.sysykeji.top/gtpatqjbux.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.pycfn.com/gtcpxwfdnl.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.daxiang520.top/gtskbqycta.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.daria6918.cn/gtotutsiaz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.nanxinkj.top/gtvtscaubn.html

[F03] 写入文件（覆盖）
来源：http://hz.sweek.top/gttjscbydj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.jiagoushi.top/gtjzhqrvtf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.xuanzx.com/gtwogjayli.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zycfv.cn/gtyfusidlb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.c1oappe.top/gtbshozkds.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.yangfankeji.com/gthhtvxswy.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.meibo888.top/gtppsixoii.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.yuanzhike.top/gtqknnymmj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.cdnleiting.top/gtqyrzwzvz.html

[F04] 追加写入文件
来源：http://hz.xingfuxueyuan.xyz/gtdcymhhpv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.gogol.net.cn/gtctyhaukw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.316326.xyz/gtuuoedcie.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhiwuduotai.top/gtaocxrlcx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.c1oappe.top/gtscoimcei.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.wangshuangyany.cn/gtmbnlgsnh.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.jinqigufen.top/gtzoxhiped.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.hysaishi.cn/gtzetqzscv.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.ywan-chungtsiang.top/gtrfvbxvfq.html

[F05] 判断文件或目录是否存在
来源：http://hz.xinyue.icu/gtajdlghgi.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.zhongyouzk.top/gtjizpdjbl.html

PHP:  file_exists("a.txt");
来源：http://hz.nanxuanxn.top/gtzbimzjsw.html

JS:   fs.existsSync("a.txt")
来源：http://hz.zhaomingkeji.xyz/gtyxdneqni.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yj202588.top/gttypesvtb.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.jlsjyb.cn/gteebpdqyc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.shanyushiyangkeji.top/gtjbbivzyp.html

Ruby: File.exist?("a.txt")
来源：http://hz.jqgfzy.top/gtgwmsgegu.html

C#:   File.Exists("a.txt")
来源：http://hz.xuetiantiany.cn/gtmxfwdlzg.html

[F06] 删除文件
来源：http://hz.aibaodan.cn/gtrhhcbtfk.html

Py:   os.remove("a.txt")
来源：http://hz.guowangkeji.top/gtavbcayop.html

PHP:  unlink("a.txt");
来源：http://hz.ydjk.org.cn/gtrgjnronv.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.ywan-chungtsiang.top/gtwhiruajs.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.ywan-chungtsiang.top/gtntmklcut.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.pengpengdd.cyou/gtxgrsdjbu.html

Go:   os.Remove("a.txt")
来源：http://hz.hnxiangtu.top/gtupimvcks.html

Ruby: File.delete("a.txt")
来源：http://hz.ehwqpu.com/gtnslcxcxe.html

C#:   File.Delete("a.txt");
来源：http://hz.redwolf501.top/gtopvaulbu.html

[F07] 创建目录（含多级）
来源：http://hz.guannengcc.top/gtfxpnnfvt.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yvedp.cn/gthxesxdyn.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.aibaodan.cn/gtatnzhdgy.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.nanxuanxn.top/gtzonxioyf.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.bjfxy.top/gtodohdsyn.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.cdnleiting.top/gthnlohcpr.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.ppjwa.cn/gtzgajbapm.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.daxiang520.top/gtofsvrsqy.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.52xcode.cn/gtzugxjlog.html

[F08] 遍历目录
来源：http://hz.feifeiyinyue.top/gtywauemdh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yangfankeji.com/gtxnvihdrp.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.yonumen.top/gttbunhayx.html

JS:   fs.readdirSync("dir")
来源：http://hz.ehwqpu.com/gtckidsfil.html

TS:   fs.readdirSync("dir")
来源：http://hz.yvedp.cn/gthhunjxfn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.aibaodan.cn/gtgglhbamq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.cqqwz.cn/gtshpgmttm.html

Ruby: Dir.children("dir")
来源：http://hz.vqdsnc.cn/gtkiqmnzzp.html

C#:   Directory.GetFiles("dir")
来源：http://hz.shangyingyoupin.top/gtdrnkstjx.html

[F09] 获取文件大小
来源：http://hz.jiagoushi.top/gtnpfvehyo.html

Py:   os.path.getsize("a.txt")
来源：http://hz.hnxiangtu.top/gtsextwwci.html

PHP:  filesize("a.txt");
来源：http://hz.svipenyu.cn/gtutylkscn.html

JS:   fs.statSync("a.txt").size
来源：http://hz.yanxiufei.cn/gtqpngtunb.html

TS:   fs.statSync("a.txt").size
来源：http://hz.316326.xyz/gtdqwgmwta.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.smart0.xyz/gtmhyxbrns.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.shzxlz.cn/gtuvqbzogm.html

Ruby: File.size("a.txt")
来源：http://hz.daria6918.cn/gtkbatdroe.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.zhaomingkeji.xyz/gtokjhjdfr.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.ivvv.top/gtpxqfbeff.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.yonumen.top/gtintvstef.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.ybcxt.top/gtzeayrylu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.meibo888.top/gtcmkjzgai.html

TS:   path.extname("a.txt")
来源：http://hz.cqqwz.cn/gtiqijxvug.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.jinyuanbaomall.cn/gtcqmxpeny.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.tian-w.cn/gtmwqbrlgn.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.shanyushiyangtech.top/gtpotgwkyd.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.dashuyun.cn/gtfivhkegi.html

[F11] 复制与移动文件
来源：http://hz.haohaochexian.top/gtjmiywceb.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.yj20258.top/gtgcgigrmr.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.0kj1m.cn/gthbfvcpfr.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.c1oappe.top/gtnlpxvkcj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhongyouzk.top/gtzkeasjwy.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.aibaodan.cn/gtpgesivbt.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jqgufenzy.top/gtetzqtriu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.zhixingplan.top/gtnyaayuxx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.shangyingyoupin.top/gterwpakrz.html

[F12] CSV 读写
来源：http://hz.xinyue.icu/gtoqkiwmdi.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.hammf.cn/gtoczllddk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.xuetiantiany.cn/gtskxnytpe.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.ydzc1.top/gtdkuhkqln.html

TS:   // 同上
来源：http://hz.jinyuanbaomall.cn/gteqggecyr.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.yueranfly.top/gtpbfhnqpc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.hnqzz.top/gtpprkmrhq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.gogol.net.cn/gtmvvuqeru.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.shanyushiyangtech.top/gtbimyrcke.html

================================================================================
来源：http://hz.yangfankeji.com/gtairrqnyr.html

G. 面向对象
来源：http://hz.xinyue.icu/gtynamsyoc.html

================================================================================
来源：http://hz.zhoulong.xyz/gtmigfttmn.html

[G01] 定义类
来源：http://hz.redwolf501.top/gturiulqwr.html

Py:   class User: pass
来源：http://hz.guowangkeji.top/gtsdvpxplj.html

PHP:  class User {}
来源：http://hz.sufxvd.cn/gtahxzdpdl.html

JS:   class User {}
来源：http://hz.hnxiangtu.top/gtmdnzmttb.html

TS:   class User { name: string = ""; }
来源：http://hz.zhixingplan.top/gtkpqftgth.html

Java: class User {}
来源：http://hz.gotoacloud.top/gtbplpeptz.html

Go:   type User struct { Name string }
来源：http://hz.0kj1m.cn/gtsnemireg.html

Ruby: class User; end
来源：http://hz.dashuyun.cn/gtmpccdcnv.html

C#:   class User {}
来源：http://hz.cdnleiting.top/gtboxonthc.html

[G02] 构造函数
来源：http://hz.vqdsnc.cn/gtqwgdfjrd.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.jinyuanbaomall.cn/gtbjtnajjy.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.zhoulong.xyz/gtumtnqzem.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.pengpengdd.cyou/gtjftgytss.html

TS:   constructor(public name: string) {}
来源：http://hz.zycfv.cn/gtvlqxqojq.html

Java: User(String name) { this.name = name; }
来源：http://hz.fzhhl.top/gtcrtpzyjt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.chenzaomai.com/gtacdwavto.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.zhaomingkeji.xyz/gttarpkhvr.html

C#:   public User(string name) { Name = name; }
来源：http://hz.zhiwuduotai.top/gtvwcouaxy.html

[G03] 实例属性
来源：http://hz.chenjidiqi.icu/gtlovccdxl.html

Py:   self.name = "x"
来源：http://hz.tanke756.top/gtlzuprvie.html

PHP:  public string $name = "x";
来源：http://hz.aibaodan.cn/gtmywjnicr.html

JS:   this.name = "x";
来源：http://hz.jqgfzy.top/gtklljtyhe.html

TS:   name: string = "x";
来源：http://hz.ivvv.top/gtzfpbonua.html

Java: private String name;
来源：http://hz.jinyuanbaomall.cn/gttqedespl.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.jinyuanbaomall.cn/gtyxehkqgm.html

Ruby: @name = "x"
来源：http://hz.kuanghao11.cn/gtwqxeoxhk.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.nanxinkj.top/gtmnstyrzy.html

[G04] 定义方法
来源：http://hz.sufxvd.cn/gtlprlmsyx.html

Py:   def greet(self): return self.name
来源：http://hz.ybcxt.top/gtbyhxqrpl.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.hammf.cn/gtxxygrhue.html

JS:   greet() { return this.name; }
来源：http://hz.dianchejie.cn/gtqxawcrjt.html

TS:   greet(): string { return this.name; }
来源：http://hz.guowangkeji.top/gtknnbfehx.html

Java: String greet() { return name; }
来源：http://hz.jqgfzy.top/gtyatfucoj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.tianlin.xyz/gtaszlztor.html

Ruby: def greet; @name; end
来源：http://hz.xinyue.icu/gtonlxsnsv.html

C#:   public string Greet() => Name;
来源：http://hz.tian-w.cn/gtxtmflpyy.html

[G05] 继承
来源：http://hz.tianlin.xyz/gtivnddgvm.html

Py:   class Admin(User): pass
来源：http://hz.jqgufenzy.top/gtboosflvo.html

PHP:  class Admin extends User {}
来源：http://hz.zdqjudy.top/gtvsgzbczf.html

JS:   class Admin extends User {}
来源：http://hz.zdqjudy.top/gtqlcpkafr.html

TS:   class Admin extends User {}
来源：http://hz.yanxiufei.cn/gtuavtvydy.html


<!-- 参考信息 -->