代发 wailian999

[E06] 替换子串
来源：http://hz.gogol.net.cn/gtfclqkhda.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.wangshuangyany.cn/gtevwjmncj.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.zdqjudy.top/gtltmvdlzy.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.ppjwa.cn/gtwimpfzgp.html

TS:   s.replaceAll("a", "b")
来源：http://hz.pycfn.com/gtkgnalhca.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yuanzhike.top/gtpgrkrmah.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.redwolf501.top/gtsvjxyvqy.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.ydjk.org.cn/gtdyfkxpri.html

C#:   s.Replace("a", "b")
来源：http://hz.jyoumei.cn/gtpmcbezst.html

[E07] 按分隔符拆分
来源：http://hz.hongshengwenyu.top/gtxozkzfrp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.hammf.cn/gtytwbynnw.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.nanxinkj.top/gtrpjuyvgk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.zhengqikj.top/gtuhbaljjk.html

TS:   s.split(",")
来源：http://hz.zycfv.cn/gtnqvekfft.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.52xcode.cn/gtmmngsczw.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.ppjwa.cn/gtkeeubxwq.html

Ruby: s.split(",");  s.split
来源：http://hz.yvedp.cn/gtpcurvkuw.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.meibo888.top/gtmaitvhxt.html

[E08] 数组按分隔符合并
来源：http://hz.gotoacloud.top/gtjlvfbulv.html

Py:   ",".join(items)
来源：http://hz.shuidangran.top/gtybhztdgl.html

PHP:  implode(",", $items);
来源：http://hz.andypj.xyz/gtisnckmnk.html

JS:   items.join(",")
来源：http://hz.daria6918.cn/gtmvftudft.html

TS:   items.join(",")
来源：http://hz.jinqigufen.top/gtixilclon.html

Java: String.join(",", items)
来源：http://hz.guannengcc.top/gtwlxgdpfp.html

Go:   strings.Join(items, ",")
来源：http://hz.jinyuanbaomall.cn/gtpfarwdye.html

Ruby: items.join(",")
来源：http://hz.snrcjt.cn/gtyxdmmmvh.html

C#:   string.Join(",", items)
来源：http://hz.yj20258.top/gtrmvnbjwy.html

[E09] 去除所有空白字符
来源：http://hz.dianchejie.cn/gtizgzrvka.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.xylfe.cn/gtdyrnliwu.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.sysykeji.top/gtnjpnohsf.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.dianchejie.cn/gtrezkphee.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.ppjwa.cn/gtgramutfn.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.jinqigfzy.top/gtrrzvjtfy.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.xziqi.cn/gtndehuqmh.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.guannengcc.top/gtsievcowr.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.sweek.top/gtuxrcncxp.html

[E10] 左侧补零 / 定长填充
来源：http://hz.ydzc1.top/gtrjuqmaqi.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.yj202588.top/gtzhgmdosv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.yj20258888.top/gtxyqgkkqd.html

JS:   "7".padStart(3, "0")
来源：http://hz.iojbl.cn/gtrndfiyru.html

TS:   "7".padStart(3, "0")
来源：http://hz.yongpay.top/gtmeohajek.html

Java: String.format("%03d", 7)
来源：http://hz.shuidangran.top/gtrnsvfqqm.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.shzxlz.cn/gtuypvvxun.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.birdmap.top/gteptxcolb.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.wangshuangyany.cn/gtszegtmtf.html

[E11] 反转字符串
来源：http://hz.fengsongda.top/gttzwpzkqn.html

Py:   s[::-1]
来源：http://hz.gzhubu.top/gtscufrifj.html

PHP:  strrev($s);
来源：http://hz.jianghu66.top/gtlzaeherq.html

JS:   [...s].reverse().join("")
来源：http://hz.zhongyouzk.top/gtvkkiakih.html

TS:   [...s].reverse().join("")
来源：http://hz.jianghu66.top/gtesvkigbr.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.jiagoushi.top/gtgmsrkrur.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.yvedp.cn/gtuppuqbzx.html

Ruby: s.reverse
来源：http://hz.birdmap.top/gtaohkhmaz.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.yangfankeji.com/gtctnwqosw.html

[E12] 统计某字符出现次数
来源：http://hz.sxryk.cn/gttyphfhwv.html

Py:   s.count("a")
来源：http://hz.ydjk.org.cn/gtsoefqatx.html

PHP:  substr_count($s, "a");
来源：http://hz.zdqjudy.top/gtscacasgf.html

JS:   s.split("a").length - 1
来源：http://hz.shuidangran.top/gttzctddtg.html

TS:   s.split("a").length - 1
来源：http://hz.cqqwz.cn/gtyabyltxf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.jinqigfzy.top/gtcvpcgham.html

Go:   strings.Count(s, "a")
来源：http://hz.jqgfzy.top/gtsizanuxq.html

Ruby: s.count("a")
来源：http://hz.gzhubu.top/gtnvqldzaj.html

C#:   s.Count(c => c == 'a')
来源：http://hz.vqdsnc.cn/gtlroctuec.html

[E13] 逐字符遍历
来源：http://hz.vqdsnc.cn/gtglfdikgc.html

Py:   for ch in s: print(ch)
来源：http://hz.guowangkeji.top/gtibqyonhu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.zdqjudy.top/gtspcdvyhr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.chenjidiqi.icu/gtdhlvkrph.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jqgufenzy.top/gtckeebdil.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.havefunace.top/gtrynwgtat.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.sysykeji.top/gtpvmwoequ.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.jianghu66.top/gtyxifunnz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.shangyingyoupin.top/gtrvrdksth.html

[E14] URL 编码与 Base64
来源：http://hz.aizwys.cn/gthgohvupc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.xuetiantiany.cn/gtdapgojsf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.fengsongda.top/gtzwqyktlx.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.chenzaomai.com/gtzfvyjbbn.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.guannengcc.top/gtbaidpavr.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.mhx1999.top/gtqttjplaq.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.ybcxt.top/gtlqjhgbcu.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.redwolf501.top/gtnvqptpvr.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.snrcjt.cn/gtshlfnqzz.html

[E15] HTML 转义 / 反转义
来源：http://hz.dashuyun.cn/gtbkgjqmez.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.cdnleiting.top/gtxwtuycdz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.hnxiangtu.top/gtyifgmxkg.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.zhaomingkeji.xyz/gtokwtqior.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.zhixingplan.top/gtdibtorvx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.xuetiantiany.cn/gtinscepws.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.zdqjudy.top/gtipjlbrxr.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.gotoacloud.top/gtdarrwbch.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.daria6918.cn/gtvmrzzblv.html

[E16] 数字千分位
来源：http://hz.shangyingyoupin.top/gtncjijoza.html

Py:   f"{1234567:,}"
来源：http://hz.dianchejie.cn/gtcdqhlojj.html

PHP:  number_format(1234567);
来源：http://hz.cqqwz.cn/gtpfycdplt.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.vqdsnc.cn/gtgrlqphgc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.jlsjyb.cn/gtctirdxgm.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.meibo888.top/gtknsfpwba.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.zhaomingkeji.xyz/gtbkqepmtk.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.shuidangran.top/gtcexczzzd.html

C#:   1234567.ToString("N0")
来源：http://hz.dianchejie.cn/gtfnpvrvli.html

[E17] 首字母大写
来源：http://hz.sweek.top/gttmrkpyeb.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.redwolf501.top/gtbspxtczx.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.redwolf501.top/gtoowjwzwv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ppjwa.cn/gtfndvelhn.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ehwqpu.com/gtcfvervub.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.xylfe.cn/gtfevqmkje.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.quarkkingdee.top/gtupqwxiaf.html

Ruby: s.capitalize
来源：http://hz.daria6918.cn/gtziddhryx.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.zhiwuduotai.top/gtzscazodf.html

[E18] 模板占位符替换
来源：http://hz.chenlongwang.top/gtjsziouqk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.jqgfzy.top/gtxwguqmti.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.zhaomingkeji.xyz/gtftitvujz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.shzxlz.cn/gtyipubatt.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.gotoacloud.top/gtqxwevgrj.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.meibo888.top/gtvibgcxpd.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.wangdashe.top/gtmbjbbyda.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.52xcode.cn/gtqgzxnmfo.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.birdmap.top/gtzxzglcxq.html

[E19] 多行文本按行拆分
来源：http://hz.quarkkingdee.top/gtdmdgmvua.html

Py:   s.splitlines()
来源：http://hz.mhx1999.top/gtadypjcvm.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.nanxuanxn.top/gtkvlxsvnb.html

JS:   s.split(/\r?\n/)
来源：http://hz.feifeiyinyue.top/gtszmlovip.html

TS:   s.split(/\r?\n/)
来源：http://hz.yonumen.top/gtoocxavpc.html

Java: s.lines().toList()
来源：http://hz.wangshuangyany.cn/gtdklwintg.html

Go:   strings.Split(s, "\n")
来源：http://hz.cdnleiting.top/gtdoywmcij.html

Ruby: s.lines
来源：http://hz.havefunace.top/gtpppdrdnb.html

C#:   s.Split('\n')
来源：http://hz.ywan-chungtsiang.top/gtuombovfd.html

[E20] 判断字符串是否为空
来源：http://hz.hysaishi.cn/gthrryuawi.html

Py:   if not s:
来源：http://hz.yonumen.top/gtixxabjft.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.yvedp.cn/gtvqzqrvgd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.shanyushiyangtech.top/gtneglinxr.html

TS:   if (s === "") {}
来源：http://hz.sysykeji.top/gtgsemnpyj.html

Java: if (s.isEmpty()) {}
来源：http://hz.zdqjudy.top/gtbpampoyt.html

Go:   if s == "" {}
来源：http://hz.gotoacloud.top/gthiekcaii.html

Ruby: if s.empty?
来源：http://hz.chenzaomai.com/gtwxoiysrj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.hywenlv.cn/gtdaouqfzy.html

[E21] 超长截断加省略号
来源：http://hz.ywan-chungtsiang.top/gtkcaymsxk.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.tian-w.cn/gtwcvlxtlb.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.xylfe.cn/gtyabvmrwl.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ivvv.top/gtpcpwcgqa.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.hywenlv.cn/gtkkquwrkx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.9152youxi.cn/gtwccklbpj.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.sxryk.cn/gtjrjgoefe.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.yvedp.cn/gthiirerwg.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.havefunace.top/gtsosrwchl.html

[E22] 字节长度与字符长度
来源：http://hz.jianghu66.top/gtheqntryh.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.shanyushiyangkeji.top/gtcqbbhoul.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.tianlin.xyz/gtxutlijpc.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hysaishi.cn/gtbliyavyr.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhaomingkeji.xyz/gtbhhedwwm.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.ydzc1.top/gtlcgoydog.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.dashuyun.cn/gtgvdohvqe.html

Ruby: s.bytesize;  s.length
来源：http://hz.zhaomingkeji.xyz/gtvvbdxuri.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.jqgufenzy.top/gtuqctikoc.html

================================================================================
来源：http://hz.jqgufenzy.top/gtmeoprtvx.html

F. 文件与目录
来源：http://hz.ywan-chungtsiang.top/gtwvsgbnpi.html

================================================================================
来源：http://hz.dianchejie.cn/gtveohicdg.html

[F01] 读取整个文件
来源：http://hz.hywenlv.cn/gtywnlsdlm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.chenzaomai.com/gtnzcudlib.html

PHP:  file_get_contents("a.txt");
来源：http://hz.guannengcc.top/gtoupjoczp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.sufxvd.cn/gtrnmfeomy.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.zhaomingkeji.xyz/gtsizvqvbh.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.dianchejie.cn/gtsrskpjed.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.jinghuilouyu.cn/gtmlwsflqj.html

Ruby: File.read("a.txt")
来源：http://hz.mhx1999.top/gtqvcxsegl.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.smart0.xyz/gtsidxfrpc.html

[F02] 逐行读取文件
来源：http://hz.ywan-chungtsiang.top/gtpviwcjdi.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.quarkkingdee.top/gtccslfdbj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.ydjk.org.cn/gtalfgqbwe.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.feifeiyinyue.top/gtvczjafev.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.cashguo.top/gtfntvdfiy.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.hfpthk.cn/gtblrlotmf.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.jiagoushi.top/gttcvygzhp.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.tianlin.xyz/gtzkwulsej.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.yueranfly.top/gtntmxupjy.html

[F03] 写入文件（覆盖）
来源：http://hz.xuetiantiany.cn/gtwspvjdhv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.sxryk.cn/gtmwjzltha.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.wangshuangyany.cn/gtmujayphj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.daria6918.cn/gtdrcbeqjo.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.snrcjt.cn/gtuiyxwntx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.9152youxi.cn/gtgaffskvw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.sxryk.cn/gtxfeparge.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.daria6918.cn/gtciziytna.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.shangyingyoupin.top/gtkrylqqof.html

[F04] 追加写入文件
来源：http://hz.yongpay.top/gtwhliewmv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.cucudq.cn/gtwuxndgxo.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.zhoulong.xyz/gtxwhvhgkf.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.0kj1m.cn/gtxmhutold.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zycfv.cn/gtdmglakce.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.andypj.xyz/gttcaphczb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.chenjidiqi.icu/gtkjgwiqfa.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yuxming.cn/gtrqknyiao.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.jqgufenzy.top/gtojfqsrix.html

[F05] 判断文件或目录是否存在
来源：http://hz.jinqigfzy.top/gtjenlquni.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.svipenyu.cn/gtsqqcbarb.html

PHP:  file_exists("a.txt");
来源：http://hz.zhongyouzk.top/gterwwphjg.html

JS:   fs.existsSync("a.txt")
来源：http://hz.shanyushiyangkeji.top/gthajipwad.html

TS:   fs.existsSync("a.txt")
来源：http://hz.jqgufenzy.top/gtdpxjqipd.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.nanxuanxn.top/gtszoyxepi.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.kuanghao11.cn/gtjupqpbcn.html

Ruby: File.exist?("a.txt")
来源：http://hz.wangdashe.top/gtslilqogy.html

C#:   File.Exists("a.txt")
来源：http://hz.xziqi.cn/gtenrvngtf.html

[F06] 删除文件
来源：http://hz.cqqwz.cn/gtyogqluns.html

Py:   os.remove("a.txt")
来源：http://hz.havefunace.top/gtfcssgbxf.html

PHP:  unlink("a.txt");
来源：http://hz.fzhhl.top/gtlpgtaeva.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.mhx1999.top/gttkyrbtzl.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.guowangkeji.top/gtbezgvelv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.shzxlz.cn/gthmlfqgyq.html

Go:   os.Remove("a.txt")
来源：http://hz.pengpengdd.cyou/gtpvjivtiu.html

Ruby: File.delete("a.txt")
来源：http://hz.yj20258.top/gtusltpukb.html

C#:   File.Delete("a.txt");
来源：http://hz.gotoacloud.top/gtokblbjoh.html

[F07] 创建目录（含多级）
来源：http://hz.jinqigfzy.top/gtxmdyriwt.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.xziqi.cn/gtnheqtijv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.yj202588.top/gtgkcclruk.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.aibaodan.cn/gtglrxvucv.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zycfv.cn/gtocqcmewm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.meibo888.top/gtzwmijxuc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.hfpthk.cn/gtgiyydxau.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.jinyuanbaomall.cn/gtouadogax.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.sweek.top/gtyqczdgrs.html

[F08] 遍历目录
来源：http://hz.316326.xyz/gtspddjimu.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.gogol.net.cn/gtpulgcfop.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.redwolf501.top/gtutrbtcjj.html

JS:   fs.readdirSync("dir")
来源：http://hz.yangfankeji.com/gtfdkurtqk.html

TS:   fs.readdirSync("dir")
来源：http://hz.guowangkeji.top/gtkcwghytl.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.wangshuangyany.cn/gtatmmtdzo.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.hnxiangtu.top/gtueixwuvd.html

Ruby: Dir.children("dir")
来源：http://hz.yj202588.top/gtnrdrcqdp.html

C#:   Directory.GetFiles("dir")
来源：http://hz.zhijiandao.cn/gtyaubalct.html

[F09] 获取文件大小
来源：http://hz.jinghuilouyu.cn/gtugeljher.html

Py:   os.path.getsize("a.txt")
来源：http://hz.chenzaomai.com/gtdfzzcbng.html

PHP:  filesize("a.txt");
来源：http://hz.snrcjt.cn/gtnexrnnfi.html

JS:   fs.statSync("a.txt").size
来源：http://hz.hammf.cn/gttdwnxipp.html

TS:   fs.statSync("a.txt").size
来源：http://hz.guannengcc.top/gttgiliawb.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.yonumen.top/gtljnqkjwe.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.zhaomingkeji.xyz/gtvkezlibj.html

Ruby: File.size("a.txt")
来源：http://hz.fzhhl.top/gtcdlxsppe.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.jqgfzy.top/gtsrgxsnjp.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.zdqjudy.top/gtvlqrioex.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.yj202588.top/gtvxjbfnhk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.kuanghao11.cn/gttvwlwomr.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.ywan-chungtsiang.top/gtfdyqxfgn.html

TS:   path.extname("a.txt")
来源：http://hz.cashguo.top/gtyjrrwcpw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.ydzc1.top/gtqyvasmss.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.sxryk.cn/gtsjqxzjzh.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.zhijiandao.cn/gtdjnlfzqa.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.ywan-chungtsiang.top/gtbgxcmebw.html

[F11] 复制与移动文件
来源：http://hz.cheryme.top/gthyycckcg.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.guannengcc.top/gtnjhvvnkj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.zhixingplan.top/gtgiqwcphi.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhengqikj.top/gtanwzgcqz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.chenlongwang.top/gtzmlpmoxs.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.xinyue.icu/gtbftxwjcn.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yj202588.top/gtqalbkibb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.guowangkeji.top/gtiksdlvun.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.9152youxi.cn/gtbcbahvbw.html

[F12] CSV 读写
来源：http://hz.jinyuanbaomall.cn/gtiqcoglyt.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.quarkkingdee.top/gtpjcmstiq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.zhijiandao.cn/gtkqfbhita.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.ywan-chungtsiang.top/gtspjwxglx.html

TS:   // 同上
来源：http://hz.sxryk.cn/gtjfvbijlk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.yj20258.top/gttvtazqnc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.sweek.top/gtiuahilri.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.birdmap.top/gtdrtjbftj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yj20258.top/gtqypbrcmy.html

================================================================================
来源：http://hz.guannengcc.top/gtgfperxba.html

G. 面向对象
来源：http://hz.chenjidiqi.icu/gtfwnufzsw.html

================================================================================
来源：http://hz.jlsjyb.cn/gtnzyutnum.html

[G01] 定义类
来源：http://hz.tian-w.cn/gtgykasutp.html

Py:   class User: pass
来源：http://hz.hongshengwenyu.top/gtojqezczj.html

PHP:  class User {}
来源：http://hz.jinqigufen.top/gtvupkhjuh.html

JS:   class User {}
来源：http://hz.zhaomingkeji.xyz/gtsqdgakdr.html

TS:   class User { name: string = ""; }
来源：http://hz.pengpengdd.cyou/gtvvghhcvp.html

Java: class User {}
来源：http://hz.316326.xyz/gtujeoitgd.html

Go:   type User struct { Name string }
来源：http://hz.yanxiufei.cn/gtifwycuyn.html

Ruby: class User; end
来源：http://hz.yj20258888.top/gtqrsjqyhb.html

C#:   class User {}
来源：http://hz.aizwys.cn/gtwmgjdura.html

[G02] 构造函数
来源：http://hz.xinyue.icu/gtvxyljcfr.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.sxryk.cn/gtroaotmwm.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.fzhhl.top/gtuvxajgxn.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.shanyushiyangkeji.top/gttmkyepgi.html

TS:   constructor(public name: string) {}
来源：http://hz.52xcode.cn/gtthfqixbd.html

Java: User(String name) { this.name = name; }
来源：http://hz.zhongyouzk.top/gterunlvfg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.mhx1999.top/gtcfgmthce.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.cucudq.cn/gtqpphmftn.html

C#:   public User(string name) { Name = name; }
来源：http://hz.shanyushiyangkeji.top/gtkzgqqbff.html

[G03] 实例属性
来源：http://hz.cqqwz.cn/gtpmbpmizy.html

Py:   self.name = "x"
来源：http://hz.dashuyun.cn/gtvwwjdevw.html

PHP:  public string $name = "x";
来源：http://hz.svipenyu.cn/gtwgpyjfqw.html

JS:   this.name = "x";
来源：http://hz.fengsongda.top/gtbdpuguaa.html

TS:   name: string = "x";
来源：http://hz.jinyuanbaomall.cn/gtdhizucoy.html

Java: private String name;
来源：http://hz.ivvv.top/gtrcxchtix.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.vqdsnc.cn/gtfkeexujc.html

Ruby: @name = "x"
来源：http://hz.tian-w.cn/gtlhyqhucl.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yueranfly.top/gtfknpqogc.html

[G04] 定义方法
来源：http://hz.ehwqpu.com/gtpxhelwhv.html

Py:   def greet(self): return self.name
来源：http://hz.yj20258.top/gtnvcqjkge.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yvedp.cn/gtsyurznpm.html

JS:   greet() { return this.name; }
来源：http://hz.yj20258.top/gtwthvcebc.html

TS:   greet(): string { return this.name; }
来源：http://hz.xuanzx.com/gtsrgavhmm.html

Java: String greet() { return name; }
来源：http://hz.zhijiandao.cn/gtrayiagws.html


<!-- 参考信息 -->