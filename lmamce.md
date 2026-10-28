代发 wailian999

PHP:  implode(",", $items);
来源：http://hz.quarkkingdee.top/gtxibhhydd.html

JS:   items.join(",")
来源：http://hz.havefunace.top/gthnckgqzm.html

TS:   items.join(",")
来源：http://hz.hfpthk.cn/gtncumfuxk.html

Java: String.join(",", items)
来源：http://hz.ydzc1.top/gtejgiqsyn.html

Go:   strings.Join(items, ",")
来源：http://hz.zhongyouzk.top/gtpswcdnqs.html

Ruby: items.join(",")
来源：http://hz.yuxming.cn/gttjkkohnd.html

C#:   string.Join(",", items)
来源：http://hz.yvedp.cn/gtfjnfrzjj.html

[E09] 去除所有空白字符
来源：http://hz.zhijiandao.cn/gtsxkdtcmt.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.316326.xyz/gtnukeiilr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.mhx1999.top/gtfpcwuzti.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.zhijiandao.cn/gtzgwrxfwx.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.c1oappe.top/gtbkqqtcix.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.chenzaomai.com/gtfdvpdysg.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.dashuyun.cn/gtpszislve.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.jianghu66.top/gtkjywaekp.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.nanxuanxn.top/gtmegfzxhj.html

[E10] 左侧补零 / 定长填充
来源：http://hz.jqgfzy.top/gteanurlqd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.gotoacloud.top/gttwjmoltb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.ehwqpu.com/gtkeuwsrjk.html

JS:   "7".padStart(3, "0")
来源：http://hz.yuanzhike.top/gtjbhbmocm.html

TS:   "7".padStart(3, "0")
来源：http://hz.gotoacloud.top/gtrvpqomrp.html

Java: String.format("%03d", 7)
来源：http://hz.jyoumei.cn/gtmumskldw.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.wangdashe.top/gtguoloomi.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.jinqigfzy.top/gttugspkvu.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.daxiang520.top/gteffaruux.html

[E11] 反转字符串
来源：http://hz.shangyingyoupin.top/gtqwjryahr.html

Py:   s[::-1]
来源：http://hz.tian-w.cn/gtggfmlqpg.html

PHP:  strrev($s);
来源：http://hz.chenjidiqi.icu/gtobkfazft.html

JS:   [...s].reverse().join("")
来源：http://hz.jyoumei.cn/gtyaqmvexf.html

TS:   [...s].reverse().join("")
来源：http://hz.xuetiantiany.cn/gtkvgddeir.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.sxryk.cn/gtargfhevp.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.zycfv.cn/gtzrherqlx.html

Ruby: s.reverse
来源：http://hz.aizwys.cn/gtvmvahtlg.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.xylfe.cn/gttetnfzkq.html

[E12] 统计某字符出现次数
来源：http://hz.xylfe.cn/gtwpkywfbc.html

Py:   s.count("a")
来源：http://hz.zhixingplan.top/gtamlfenfh.html

PHP:  substr_count($s, "a");
来源：http://hz.redwolf501.top/gtfucuhlqa.html

JS:   s.split("a").length - 1
来源：http://hz.chenjidiqi.icu/gtmhqhwzhh.html

TS:   s.split("a").length - 1
来源：http://hz.zhijiandao.cn/gtcehqvmrt.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.chenzaomai.com/gtmmoyzahr.html

Go:   strings.Count(s, "a")
来源：http://hz.shanyushiyangtech.top/gtxdrjqlcp.html

Ruby: s.count("a")
来源：http://hz.cdnleiting.top/gtbloteblq.html

C#:   s.Count(c => c == 'a')
来源：http://hz.ydjk.org.cn/gtbpftvmqw.html

[E13] 逐字符遍历
来源：http://hz.ppjwa.cn/gtnemxyhqz.html

Py:   for ch in s: print(ch)
来源：http://hz.svipenyu.cn/gtbseepokc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.redwolf501.top/gtmciwdgze.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zhongyouzk.top/gtnosbckmf.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jinqigfzy.top/gtdeopvnrk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.shanyushiyangtech.top/gtxklmehmy.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.9152youxi.cn/gtxsdlqyrx.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.guowangkeji.top/gtvcxiwipa.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.52xcode.cn/gtpbxeqphb.html

[E14] URL 编码与 Base64
来源：http://hz.nanxuanxn.top/gthzjefyjo.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.feifeiyinyue.top/gteqihnuff.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.zhoulong.xyz/gtyzqdesun.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.jqgufenzy.top/gtprbcdmlr.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.hnqzz.top/gtmjchqpdp.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.wangdashe.top/gtjnjkqbru.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.cashguo.top/gtjzxyslvo.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.jyoumei.cn/gtjsvletdc.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.svipenyu.cn/gtpmnfbeav.html

[E15] HTML 转义 / 反转义
来源：http://hz.0kj1m.cn/gtwaeizvwh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.tanke756.top/gtehmkkspr.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.ybcxt.top/gttvejkfzp.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.sxryk.cn/gtwdjpunvy.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.pycfn.com/gtwyzyuhpy.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.birdmap.top/gthyhhyppj.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.shangyingyoupin.top/gthjzefzwr.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.shangyingyoupin.top/gtwrspworg.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.hammf.cn/gtiffkwefx.html

[E16] 数字千分位
来源：http://hz.xuanzx.com/gtwuyltorn.html

Py:   f"{1234567:,}"
来源：http://hz.jinghuilouyu.cn/gtozfftihw.html

PHP:  number_format(1234567);
来源：http://hz.pycfn.com/gtygujjeuc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.sweek.top/gtvnorcbue.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhoulong.xyz/gtbfjevbxa.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.haohaochexian.top/gtueojzudy.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.jqgufenzy.top/gtvudszjyc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.wangshuangyany.cn/gtcefwnbud.html

C#:   1234567.ToString("N0")
来源：http://hz.bjfxy.top/gteqmdncjb.html

[E17] 首字母大写
来源：http://hz.pycfn.com/gtsevwhdvz.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.nanxinkj.top/gtichqxqqa.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.cashguo.top/gtxjzuakms.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jinghuilouyu.cn/gtmtjldfiz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yuanzhike.top/gtrowptaqi.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.chenlongwang.top/gtwpsdnmyb.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.xuetiantiany.cn/gtwwkrhivs.html

Ruby: s.capitalize
来源：http://hz.vqdsnc.cn/gtnfygjndd.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.pycfn.com/gtqwfgezwl.html

[E18] 模板占位符替换
来源：http://hz.yj20258888.top/gtsfmetvsg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.jinyuanbaomall.cn/gtplivqsns.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.yanxiufei.cn/gticxqhxis.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.nwbrower.top/gttsjlljnq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.yj20258888.top/gtiknpsnsq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.jinqigufen.top/gtdxqpahon.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.mhx1999.top/gtvvdxvscy.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.hongshengwenyu.top/gthzijlnvl.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.havefunace.top/gtfhexuavn.html

[E19] 多行文本按行拆分
来源：http://hz.svipenyu.cn/gtzfnmppug.html

Py:   s.splitlines()
来源：http://hz.sufxvd.cn/gtyrcihlpj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.tianlin.xyz/gtuzsmjsfp.html

JS:   s.split(/\r?\n/)
来源：http://hz.jinyuanbaomall.cn/gtmkfnxrun.html

TS:   s.split(/\r?\n/)
来源：http://hz.nwbrower.top/gtvzvvrfwb.html

Java: s.lines().toList()
来源：http://hz.xuetiantiany.cn/gtgfsldlre.html

Go:   strings.Split(s, "\n")
来源：http://hz.quarkkingdee.top/gtmkxjhdss.html

Ruby: s.lines
来源：http://hz.yuanzhike.top/gtncmhkbfz.html

C#:   s.Split('\n')
来源：http://hz.ehwqpu.com/gtvxdwosra.html

[E20] 判断字符串是否为空
来源：http://hz.zhixingplan.top/gtkelypmyr.html

Py:   if not s:
来源：http://hz.chenlongwang.top/gtpnawxgjn.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.52xcode.cn/gtrmrreowh.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.hammf.cn/gtblqcqkae.html

TS:   if (s === "") {}
来源：http://hz.jinqigufen.top/gtexshqlrt.html

Java: if (s.isEmpty()) {}
来源：http://hz.tianlin.xyz/gttfuclymb.html

Go:   if s == "" {}
来源：http://hz.meibo888.top/gtuwdkpiop.html

Ruby: if s.empty?
来源：http://hz.zhiwuduotai.top/gtcpmztsgd.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.zhiwuduotai.top/gtqjubzdwq.html

[E21] 超长截断加省略号
来源：http://hz.cqqwz.cn/gtcskufsuw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.dashuyun.cn/gtvxtpmhga.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.52xcode.cn/gtsgawigcr.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ppjwa.cn/gthvivgsue.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zycfv.cn/gtnltucegq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.sxryk.cn/gtiivpjyru.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.ydzc1.top/gtawsjpehf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.shanyushiyangkeji.top/gtsfrrvmhu.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.wangdashe.top/gtegfelwgk.html

[E22] 字节长度与字符长度
来源：http://hz.daxiang520.top/gtjhzrkuat.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.gogol.net.cn/gtoczyhgem.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zdqjudy.top/gtsevwossb.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hysaishi.cn/gtdemjtovh.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.cqqwz.cn/gtwsfnycgs.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.yj20258.top/gtjachlywz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.iojbl.cn/gtgcahnjuq.html

Ruby: s.bytesize;  s.length
来源：http://hz.ydzc1.top/gtoflriqht.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.sxryk.cn/gtnayhqdec.html

================================================================================
来源：http://hz.yonumen.top/gtwxtcbzjh.html

F. 文件与目录
来源：http://hz.hnqzz.top/gtjlugmylz.html

================================================================================
来源：http://hz.316326.xyz/gtfmkmzbgk.html

[F01] 读取整个文件
来源：http://hz.jqgfzy.top/gtyehcfypu.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.pycfn.com/gtcqlxopgl.html

PHP:  file_get_contents("a.txt");
来源：http://hz.jiagoushi.top/gtjkrqsikf.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.gaohongyu789.top/gtnduxqgco.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.xuetiantiany.cn/gtlgiwbwyb.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.zhoulong.xyz/gthmkstrbr.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.sysykeji.top/gtbhvnwwwd.html

Ruby: File.read("a.txt")
来源：http://hz.smart0.xyz/gtbxrwcwnu.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.quarkkingdee.top/gtkoomcpxz.html

[F02] 逐行读取文件
来源：http://hz.sufxvd.cn/gtnqowdugx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.yonumen.top/gtwrobsbfj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.havefunace.top/gttwutthve.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.gzhubu.top/gtotlligqs.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yanxiufei.cn/gtnplzgmpa.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.guowangkeji.top/gttreosnxq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.havefunace.top/gtmyqyxbsv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.chenzaomai.com/gtbrlfduge.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.yangfankeji.com/gtogpdpmyg.html

[F03] 写入文件（覆盖）
来源：http://hz.tanke756.top/gtujdllvbn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.chenjidiqi.icu/gtnrsqoslm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.wangshuangyany.cn/gtyyqrwapt.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.fzhhl.top/gttrbvfvuc.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhaomingkeji.xyz/gtmnxvxekn.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.tanke756.top/gtdafprigy.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.dianchejie.cn/gtlanukejw.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.nwbrower.top/gtbnclkuko.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.yongpay.top/gtuuwyskjb.html

[F04] 追加写入文件
来源：http://hz.c1oappe.top/gtrvycvwxe.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yanxiufei.cn/gtcledztsm.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.quarkkingdee.top/gtqmvgdebw.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yonumen.top/gtudbhhldg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yuanzhike.top/gtoualjnfe.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.yueranfly.top/gtlaakvenh.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.ehwqpu.com/gtdeciosaa.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.redwolf501.top/gtpfoixoab.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.aibaodan.cn/gtikebwayx.html

[F05] 判断文件或目录是否存在
来源：http://hz.jyoumei.cn/gtkhlboskk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.pycfn.com/gtydwdryhl.html

PHP:  file_exists("a.txt");
来源：http://hz.sysykeji.top/gtcobyolro.html

JS:   fs.existsSync("a.txt")
来源：http://hz.gzhubu.top/gtudwieuwx.html

TS:   fs.existsSync("a.txt")
来源：http://hz.ehwqpu.com/gtiykpdzvd.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.zdqjudy.top/gtmughonps.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.shuidangran.top/gtfomudtgn.html

Ruby: File.exist?("a.txt")
来源：http://hz.dashuyun.cn/gtwlxhclyl.html

C#:   File.Exists("a.txt")
来源：http://hz.quarkkingdee.top/gtkmqqzugq.html

[F06] 删除文件
来源：http://hz.zdqjudy.top/gtkofrcqjf.html

Py:   os.remove("a.txt")
来源：http://hz.hnqzz.top/gtimqwdqzx.html

PHP:  unlink("a.txt");
来源：http://hz.zhixingplan.top/gttqgdyifc.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.svipenyu.cn/gtlzbbavfc.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.pengpengdd.cyou/gtcjardvmo.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.fzhhl.top/gticfiwxmw.html

Go:   os.Remove("a.txt")
来源：http://hz.ehwqpu.com/gtobsuplxg.html

Ruby: File.delete("a.txt")
来源：http://hz.mhx1999.top/gtgifisrln.html

C#:   File.Delete("a.txt");
来源：http://hz.tian-w.cn/gtmmsatxep.html

[F07] 创建目录（含多级）
来源：http://hz.sweek.top/gtffhsrqna.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.kuanghao11.cn/gtxdzdgjvj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.wangshuangyany.cn/gtsjuyrpmg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yj20258888.top/gtdkwzwoth.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.xinyue.icu/gtztgewkys.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.haohaochexian.top/gtphwwdviw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.tianlin.xyz/gtvpnkknts.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.jinghuilouyu.cn/gtamjyvwhm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.c1oappe.top/gtihkoagol.html

[F08] 遍历目录
来源：http://hz.aizwys.cn/gtpubgyxir.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yuanzhike.top/gtiplmbpmd.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.yonumen.top/gtyfwgruxv.html

JS:   fs.readdirSync("dir")
来源：http://hz.yuanzhike.top/gtgthgfkfl.html

TS:   fs.readdirSync("dir")
来源：http://hz.0kj1m.cn/gtuyixxhhu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.yvedp.cn/gtdtswxork.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.ivvv.top/gtdzzakgey.html

Ruby: Dir.children("dir")
来源：http://hz.cqqwz.cn/gtryqjsruv.html

C#:   Directory.GetFiles("dir")
来源：http://hz.aizwys.cn/gtbdxmzosh.html

[F09] 获取文件大小
来源：http://hz.yj202588.top/gttpeqspxm.html

Py:   os.path.getsize("a.txt")
来源：http://hz.cheryme.top/gtnfjnywcx.html

PHP:  filesize("a.txt");
来源：http://hz.gzhubu.top/gtxzmlpfth.html

JS:   fs.statSync("a.txt").size
来源：http://hz.316326.xyz/gtoobuzpgm.html

TS:   fs.statSync("a.txt").size
来源：http://hz.yuanzhike.top/gtayarqnil.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.yvedp.cn/gtbzvdxhos.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.xylfe.cn/gtiitiaqez.html

Ruby: File.size("a.txt")
来源：http://hz.jinyuanbaomall.cn/gtkgnhzbvr.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.cqqwz.cn/gtoibxvqkk.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yangfankeji.com/gtrazahkeo.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.redwolf501.top/gthpzwlzqa.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.guowangkeji.top/gtsubqtqca.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.hnqzz.top/gtlversfbp.html

TS:   path.extname("a.txt")
来源：http://hz.jlsjyb.cn/gtrrriphzz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.ywan-chungtsiang.top/gtwtzhbrdg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.sweek.top/gtogbhcydt.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.pengpengdd.cyou/gtwbhweifb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.nwbrower.top/gtdxohzqfz.html

[F11] 复制与移动文件
来源：http://hz.nwbrower.top/gtmqcmivec.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.gogol.net.cn/gtppfylohj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.nanxuanxn.top/gtfusejkjs.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hnxiangtu.top/gtizeicpfq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.c1oappe.top/gttklndari.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.zhijiandao.cn/gtwudsqrie.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yvedp.cn/gtigftpuzt.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.aibaodan.cn/gtexaztwqy.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.zhaomingkeji.xyz/gtverlfmcf.html

[F12] CSV 读写
来源：http://hz.jiagoushi.top/gtaymjonho.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.gogol.net.cn/gtnlpekskf.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.gotoacloud.top/gtqcnijmof.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.nwbrower.top/gtynugzkyy.html

TS:   // 同上
来源：http://hz.ybcxt.top/gtkaodybfq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.ywan-chungtsiang.top/gtlsucnnga.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.chenzaomai.com/gtrebjijkc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.hnqzz.top/gtpdvczdav.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.nanxuanxn.top/gtnjistmuz.html

================================================================================
来源：http://hz.jinqigufen.top/gtqamejmtg.html

G. 面向对象
来源：http://hz.cucudq.cn/gtlpanpthe.html

================================================================================
来源：http://hz.0kj1m.cn/gtdepmoars.html

[G01] 定义类
来源：http://hz.aizwys.cn/gthbapsyrk.html

Py:   class User: pass
来源：http://hz.zhijiandao.cn/gtcujdyuis.html

PHP:  class User {}
来源：http://hz.feifeiyinyue.top/gtsmodrjal.html

JS:   class User {}
来源：http://hz.yuanzhike.top/gtfflfemag.html

TS:   class User { name: string = ""; }
来源：http://hz.hywenlv.cn/gtouwkbodp.html

Java: class User {}
来源：http://hz.cdnleiting.top/gtoqpzftmw.html

Go:   type User struct { Name string }
来源：http://hz.yueranfly.top/gttcvkqxfn.html

Ruby: class User; end
来源：http://hz.jinqigufen.top/gtjnfkthvz.html

C#:   class User {}
来源：http://hz.zhengqikj.top/gtfeuwzzxo.html

[G02] 构造函数
来源：http://hz.xingfuxueyuan.xyz/gtopxeovqr.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.snrcjt.cn/gtltcosffc.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.ppjwa.cn/gtyetfkvof.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.c1oappe.top/gtkmbgyjsn.html

TS:   constructor(public name: string) {}
来源：http://hz.hammf.cn/gtoebbdfmn.html

Java: User(String name) { this.name = name; }
来源：http://hz.nanxuanxn.top/gtxwushecv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.vqdsnc.cn/gtvnlbhszk.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.ywan-chungtsiang.top/gtdajtoupy.html

C#:   public User(string name) { Name = name; }
来源：http://hz.jinqigfzy.top/gtovtwucdd.html

[G03] 实例属性
来源：http://hz.cheryme.top/gtiydkkbee.html

Py:   self.name = "x"
来源：http://hz.sweek.top/gtokxhxiow.html

PHP:  public string $name = "x";
来源：http://hz.xinyue.icu/gthnvdinuz.html

JS:   this.name = "x";
来源：http://hz.sxryk.cn/gtyhdfuvwn.html

TS:   name: string = "x";
来源：http://hz.iojbl.cn/gtrzskexiu.html

Java: private String name;
来源：http://hz.tian-w.cn/gtypkflmpk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.kuanghao11.cn/gtkqshkunm.html

Ruby: @name = "x"
来源：http://hz.zhiwuduotai.top/gtqsoypyxy.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.cqqwz.cn/gtqnhdreca.html

[G04] 定义方法
来源：http://hz.zhaomingkeji.xyz/gtpqyenvie.html

Py:   def greet(self): return self.name
来源：http://hz.kuanghao11.cn/gtqvnfbzqt.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yj20258.top/gtrivyqzyi.html

JS:   greet() { return this.name; }
来源：http://hz.shuidangran.top/gtwixoimwp.html

TS:   greet(): string { return this.name; }
来源：http://hz.yangfankeji.com/gtvokomivf.html

Java: String greet() { return name; }
来源：http://hz.tanke756.top/gtbwmureiw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.chenlongwang.top/gtqhrrjbxq.html

Ruby: def greet; @name; end
来源：http://hz.fzhhl.top/gtwfgtaddu.html

C#:   public string Greet() => Name;
来源：http://hz.gzhubu.top/gttuanvdve.html

[G05] 继承
来源：http://hz.yongpay.top/gtnivwufwg.html

Py:   class Admin(User): pass
来源：http://hz.c1oappe.top/gteqcgiire.html

PHP:  class Admin extends User {}
来源：http://hz.yuanzhike.top/gtbngiffbm.html

JS:   class Admin extends User {}
来源：http://hz.9152youxi.cn/gtthbumpuo.html

TS:   class Admin extends User {}
来源：http://hz.cqqwz.cn/gtldomcjco.html

Java: class Admin extends User {}
来源：http://hz.yanxiufei.cn/gtcbtimfrk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.guannengcc.top/gthjdthquf.html

Ruby: class Admin < User; end
来源：http://hz.andypj.xyz/gtcqouyxiu.html

C#:   class Admin : User {}
来源：http://hz.havefunace.top/gtsdbtfpyj.html

[G06] 重写方法
来源：http://hz.hnqzz.top/gtjknzrghl.html

Py:   def greet(self): return "admin"
来源：http://hz.tanke756.top/gtaukpoytz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.iojbl.cn/gtllmzknqk.html

JS:   greet() { return "admin"; }
来源：http://hz.vqdsnc.cn/gtbhpqskrl.html

TS:   greet(): string { return "admin"; }
来源：http://hz.tanke756.top/gtdhvlwmci.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.meibo888.top/gtksumqqcu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.cheryme.top/gtioafznqy.html

Ruby: def greet; "admin"; end
来源：http://hz.52xcode.cn/gtjudfiqfw.html


<!-- 参考信息 -->