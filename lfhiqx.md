代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.hfpthk.cn/gtfaravpst.html

TS:   s.split(",")
来源：http://hz.fzhhl.top/gtgtvzukqt.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.gotoacloud.top/gtjgvfvrwq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.chenlongwang.top/gtddhpoqkm.html

Ruby: s.split(",");  s.split
来源：http://hz.jyoumei.cn/gtsnnonvmf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.dashuyun.cn/gtusgsbggk.html

[E08] 数组按分隔符合并
来源：http://hz.yangfankeji.com/gtqmatjjwz.html

Py:   ",".join(items)
来源：http://hz.xylfe.cn/gtbokffdzk.html

PHP:  implode(",", $items);
来源：http://hz.jqgufenzy.top/gtuymoaqct.html

JS:   items.join(",")
来源：http://hz.hnxiangtu.top/gtfufqxrio.html

TS:   items.join(",")
来源：http://hz.zhijiandao.cn/gtizxrklei.html

Java: String.join(",", items)
来源：http://hz.jqgfzy.top/gtltricicy.html

Go:   strings.Join(items, ",")
来源：http://hz.quarkkingdee.top/gtucnsghpr.html

Ruby: items.join(",")
来源：http://hz.tanke756.top/gtpflbufuj.html

C#:   string.Join(",", items)
来源：http://hz.zhixingplan.top/gthdeudhvq.html

[E09] 去除所有空白字符
来源：http://hz.xinyue.icu/gtmujgfggu.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.aizwys.cn/gtkyxlhxfu.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.cucudq.cn/gtkwpwmafo.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.ppjwa.cn/gtienqkvqj.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.jqgfzy.top/gttflbrnzj.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.hfpthk.cn/gtxkgmcjna.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.yj20258.top/gtaldtyxxl.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.ywan-chungtsiang.top/gtfqrqdbcs.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.iojbl.cn/gtypykuulo.html

[E10] 左侧补零 / 定长填充
来源：http://hz.zhoulong.xyz/gtymspnjyg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.zycfv.cn/gtrrwqkwup.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.yuxming.cn/gtughbedng.html

JS:   "7".padStart(3, "0")
来源：http://hz.ydjk.org.cn/gtaeydodls.html

TS:   "7".padStart(3, "0")
来源：http://hz.jianghu66.top/gtdqztasqh.html

Java: String.format("%03d", 7)
来源：http://hz.shangyingyoupin.top/gtsavglrgq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.shuidangran.top/gtfugrxtfj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.shuidangran.top/gtzngdhcbv.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.zhijiandao.cn/gtxbfwqnsg.html

[E11] 反转字符串
来源：http://hz.9152youxi.cn/gtdinnmpls.html

Py:   s[::-1]
来源：http://hz.zhixingplan.top/gtylnaryoy.html

PHP:  strrev($s);
来源：http://hz.yuxming.cn/gtunnukpnq.html

JS:   [...s].reverse().join("")
来源：http://hz.ybcxt.top/gtswbrmyir.html

TS:   [...s].reverse().join("")
来源：http://hz.gotoacloud.top/gtpgolvcwn.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.jianghu66.top/gtkbszdkaw.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.tianlin.xyz/gtydpmuuvk.html

Ruby: s.reverse
来源：http://hz.shzxlz.cn/gtzhzurcmd.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.jyoumei.cn/gtmgmmcbkz.html

[E12] 统计某字符出现次数
来源：http://hz.nanxinkj.top/gtmnnhggcl.html

Py:   s.count("a")
来源：http://hz.zhijiandao.cn/gttkjpzzya.html

PHP:  substr_count($s, "a");
来源：http://hz.cqqwz.cn/gtrrryiqzx.html

JS:   s.split("a").length - 1
来源：http://hz.yuanzhike.top/gtznphferl.html

TS:   s.split("a").length - 1
来源：http://hz.shuidangran.top/gtumggyuiy.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.52xcode.cn/gtjiwlvoem.html

Go:   strings.Count(s, "a")
来源：http://hz.tian-w.cn/gtyqtgdcuw.html

Ruby: s.count("a")
来源：http://hz.yangfankeji.com/gtyxrpjmet.html

C#:   s.Count(c => c == 'a')
来源：http://hz.cdnleiting.top/gtqvzpfeww.html

[E13] 逐字符遍历
来源：http://hz.ppjwa.cn/gtkqtaeypl.html

Py:   for ch in s: print(ch)
来源：http://hz.bjfxy.top/gtmtkoktmi.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.hammf.cn/gtmwzivwjc.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jqgufenzy.top/gtwdrwdmgz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zhiwuduotai.top/gtljrgqord.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.fengsongda.top/gtqqxmjyrb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.cqqwz.cn/gtiezhkifb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.chenjidiqi.icu/gtuyqfultu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.zhengqikj.top/gtpevvqlzs.html

[E14] URL 编码与 Base64
来源：http://hz.xuanzx.com/gtrgiquolv.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.daxiang520.top/gtjhgcqhhy.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.hywenlv.cn/gtpmobqcey.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.ehwqpu.com/gthysfhmpt.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.yueranfly.top/gtrkxjfyvh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.shzxlz.cn/gtypymykde.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.hywenlv.cn/gtcsaxwuue.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.dashuyun.cn/gtthbldlrz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.52xcode.cn/gtfpvppini.html

[E15] HTML 转义 / 反转义
来源：http://hz.ehwqpu.com/gtcbicidto.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.xingfuxueyuan.xyz/gtfqlszbrp.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.yvedp.cn/gtnssebzdw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.iojbl.cn/gtikarqxol.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.quarkkingdee.top/gtyzqcbmis.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.yj202588.top/gtgcnszpjp.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.jinqigfzy.top/gtirlbsplq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.wangdashe.top/gtqtslplsx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.guannengcc.top/gtmmiincln.html

[E16] 数字千分位
来源：http://hz.wangdashe.top/gtfyzxciey.html

Py:   f"{1234567:,}"
来源：http://hz.zhengqikj.top/gtbyaruzpj.html

PHP:  number_format(1234567);
来源：http://hz.sufxvd.cn/gtkgvewdny.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.vqdsnc.cn/gtbsneklyy.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.chenlongwang.top/gtzncfxgoo.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.haohaochexian.top/gtnvgrfzjc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.yj202588.top/gtrkrafhdv.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.pycfn.com/gtzwigbqnj.html

C#:   1234567.ToString("N0")
来源：http://hz.daria6918.cn/gtadiapplo.html

[E17] 首字母大写
来源：http://hz.bjfxy.top/gtjscjpcgm.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.nanxinkj.top/gtpwzwohbb.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.ppjwa.cn/gteapbjtpz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.cqqwz.cn/gtfutrrftj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ydzc1.top/gtellhodlr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.tanke756.top/gtejqjrwib.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.wangshuangyany.cn/gttinpbhzp.html

Ruby: s.capitalize
来源：http://hz.ydjk.org.cn/gtoeuhbqmv.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yuanzhike.top/gtuuqkgksd.html

[E18] 模板占位符替换
来源：http://hz.cashguo.top/gtzxruvvrb.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.shanyushiyangkeji.top/gtmozchsrf.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.jinyuanbaomall.cn/gtvqdrqrav.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.dashuyun.cn/gtjmpbxapx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.zhaomingkeji.xyz/gtscrbtooy.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.yonumen.top/gtclqwibhr.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.cashguo.top/gtoebkbett.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.birdmap.top/gteexiyucw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.c1oappe.top/gtaylnfvxz.html

[E19] 多行文本按行拆分
来源：http://hz.guowangkeji.top/gtgvojfipy.html

Py:   s.splitlines()
来源：http://hz.zhiwuduotai.top/gtupvxslvl.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.yuanzhike.top/gttcfpmfjd.html

JS:   s.split(/\r?\n/)
来源：http://hz.xziqi.cn/gtqnqnzgcw.html

TS:   s.split(/\r?\n/)
来源：http://hz.yj20258.top/gtopwhveic.html

Java: s.lines().toList()
来源：http://hz.dianchejie.cn/gthjxueheb.html

Go:   strings.Split(s, "\n")
来源：http://hz.yj20258888.top/gtiruqjgnv.html

Ruby: s.lines
来源：http://hz.316326.xyz/gttxmqlipn.html

C#:   s.Split('\n')
来源：http://hz.yueranfly.top/gtxaadwlmx.html

[E20] 判断字符串是否为空
来源：http://hz.chenlongwang.top/gtsoivzrgv.html

Py:   if not s:
来源：http://hz.gzhubu.top/gtrpsdnxyi.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.jqgufenzy.top/gtbbcamryu.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.chenzaomai.com/gtdutmeaom.html

TS:   if (s === "") {}
来源：http://hz.shangyingyoupin.top/gtycmbtfkt.html

Java: if (s.isEmpty()) {}
来源：http://hz.sysykeji.top/gtqackcmwh.html

Go:   if s == "" {}
来源：http://hz.jianghu66.top/gtyyjvjtzd.html

Ruby: if s.empty?
来源：http://hz.chenjidiqi.icu/gtasjbfhue.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.ywan-chungtsiang.top/gttplzdxcp.html

[E21] 超长截断加省略号
来源：http://hz.guannengcc.top/gtfqoegfty.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.cashguo.top/gtjoioxlzs.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.yj202588.top/gtjsarjmcs.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yongpay.top/gtbpwlagbn.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ivvv.top/gtqeuduncw.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.dashuyun.cn/gtvetzuots.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.yuxming.cn/gtrdxghwrf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.xylfe.cn/gtkhoexpge.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.zhijiandao.cn/gtzwlpilqr.html

[E22] 字节长度与字符长度
来源：http://hz.cucudq.cn/gtvhroghsg.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.jinqigufen.top/gtvwwyxrot.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.iojbl.cn/gtnignenjo.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhengqikj.top/gtmmlegune.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jianghu66.top/gtmvjktkpr.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.zdqjudy.top/gtsmxxfrvy.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.ppjwa.cn/gtmjdzrefr.html

Ruby: s.bytesize;  s.length
来源：http://hz.yj20258888.top/gtlbrfvapm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.yanxiufei.cn/gtvotqknjc.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtgwlehwpv.html

F. 文件与目录
来源：http://hz.jinqigfzy.top/gtpjysexvw.html

================================================================================
来源：http://hz.fzhhl.top/gtbrljfjwi.html

[F01] 读取整个文件
来源：http://hz.birdmap.top/gtkmrgkrtl.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.jiagoushi.top/gtuipgnvam.html

PHP:  file_get_contents("a.txt");
来源：http://hz.wangdashe.top/gtwsmcwewk.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.xziqi.cn/gtlbmihrwd.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.guannengcc.top/gtrlxkfyny.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.yuxming.cn/gtttxygalr.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.mhx1999.top/gtpjbihvnk.html

Ruby: File.read("a.txt")
来源：http://hz.fzhhl.top/gtclnvbsnk.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.gogol.net.cn/gtgztygzvu.html

[F02] 逐行读取文件
来源：http://hz.sxryk.cn/gtylrtloom.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.xuanzx.com/gtsvlmgbcv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.xuetiantiany.cn/gtmcbpfcgq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yongpay.top/gtaeuuvjvi.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zdqjudy.top/gtpkjswvrh.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.snrcjt.cn/gtwzyhijcq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.0kj1m.cn/gtpznyrmlb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.xingfuxueyuan.xyz/gttzrcmjia.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.zhongyouzk.top/gttjptudvd.html

[F03] 写入文件（覆盖）
来源：http://hz.ppjwa.cn/gtrmkkwnzd.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.shanyushiyangtech.top/gttdmytgoe.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.sysykeji.top/gtkfpscbcq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.dianchejie.cn/gthpsoglyh.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jinghuilouyu.cn/gthygbaiai.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.zhongyouzk.top/gtxbfoooxu.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.wangdashe.top/gtoragrjjl.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.xuetiantiany.cn/gtrtaakdge.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.sufxvd.cn/gtgertcxxo.html

[F04] 追加写入文件
来源：http://hz.svipenyu.cn/gtxtpogkzs.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.wangshuangyany.cn/gtbgivoiww.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.9152youxi.cn/gtdodtbfeh.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.cqqwz.cn/gtxgfvadvu.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.fengsongda.top/gtwhftpdjr.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.zhoulong.xyz/gtfdrpimqr.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.mhx1999.top/gtihagljgz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.wangdashe.top/gtbyndvwdt.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.cheryme.top/gtqcpvtuft.html

[F05] 判断文件或目录是否存在
来源：http://hz.guannengcc.top/gtrwmvauou.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.yangfankeji.com/gtesbfgmuk.html

PHP:  file_exists("a.txt");
来源：http://hz.jinqigfzy.top/gtanfvlvit.html

JS:   fs.existsSync("a.txt")
来源：http://hz.52xcode.cn/gtcrmsmjyi.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yj20258888.top/gtbprueume.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.meibo888.top/gtiqlbirxb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.xuetiantiany.cn/gtwngdvhcn.html

Ruby: File.exist?("a.txt")
来源：http://hz.yj20258888.top/gtsdzlyehs.html

C#:   File.Exists("a.txt")
来源：http://hz.zhixingplan.top/gtqhtdzibf.html

[F06] 删除文件
来源：http://hz.jinqigufen.top/gtsakeisnl.html

Py:   os.remove("a.txt")
来源：http://hz.quarkkingdee.top/gtiymzhihv.html

PHP:  unlink("a.txt");
来源：http://hz.fzhhl.top/gtnewkprka.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.jlsjyb.cn/gtcsznwugq.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.zhongyouzk.top/gtydapyujg.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.feifeiyinyue.top/gtjqihvxbh.html

Go:   os.Remove("a.txt")
来源：http://hz.pycfn.com/gtycjuvnes.html

Ruby: File.delete("a.txt")
来源：http://hz.andypj.xyz/gtssejeuuu.html

C#:   File.Delete("a.txt");
来源：http://hz.iojbl.cn/gtwnkybrsw.html

[F07] 创建目录（含多级）
来源：http://hz.hammf.cn/gtnnaethtt.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yuanzhike.top/gthpfyiuuf.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.redwolf501.top/gtvwfkmjwo.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zdqjudy.top/gthrwcayni.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.gotoacloud.top/gtwcovnqdf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.jinqigufen.top/gttvtzdxeg.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.ydzc1.top/gtxhfahmga.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.gaohongyu789.top/gtjxxwqdal.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.daria6918.cn/gttzbqcequ.html

[F08] 遍历目录
来源：http://hz.wangdashe.top/gtovahmjea.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yuanzhike.top/gtagzuorai.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.jyoumei.cn/gtqpaokcvb.html

JS:   fs.readdirSync("dir")
来源：http://hz.vqdsnc.cn/gtazsqjjsk.html

TS:   fs.readdirSync("dir")
来源：http://hz.yongpay.top/gtvoonxhpn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.jlsjyb.cn/gtamrlijae.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.gzhubu.top/gtglvjjtnt.html

Ruby: Dir.children("dir")
来源：http://hz.shangyingyoupin.top/gtxnzawxpd.html

C#:   Directory.GetFiles("dir")
来源：http://hz.cqqwz.cn/gtzkroexka.html

[F09] 获取文件大小
来源：http://hz.sxryk.cn/gtgqoodidh.html

Py:   os.path.getsize("a.txt")
来源：http://hz.gotoacloud.top/gttohltaqk.html

PHP:  filesize("a.txt");
来源：http://hz.smart0.xyz/gtlcrrhqsg.html

JS:   fs.statSync("a.txt").size
来源：http://hz.9152youxi.cn/gtrlvmfhtw.html

TS:   fs.statSync("a.txt").size
来源：http://hz.jinqigfzy.top/gtlevrqjdw.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.tian-w.cn/gtobvziliz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.ppjwa.cn/gtvjercqwh.html

Ruby: File.size("a.txt")
来源：http://hz.c1oappe.top/gtxstuekrc.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.daria6918.cn/gtixbmaqpr.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.fengsongda.top/gtqrrdtxej.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.cheryme.top/gtaxbmkifu.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.yuanzhike.top/gtpbjafocm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.birdmap.top/gtmvssxecv.html

TS:   path.extname("a.txt")
来源：http://hz.hongshengwenyu.top/gtnnuufivb.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.jqgufenzy.top/gtkositdoc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.wangdashe.top/gtcdsqtexz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.yvedp.cn/gtdcvorelh.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.shangyingyoupin.top/gtrfocfzqr.html

[F11] 复制与移动文件
来源：http://hz.yongpay.top/gtpthigemu.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.yj202588.top/gtwvcoscwh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.pycfn.com/gtbssjdtth.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yanxiufei.cn/gtdhqpfyyp.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhongyouzk.top/gtprtsvzjc.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.hysaishi.cn/gtmohedlvn.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.hnxiangtu.top/gtyuvtytys.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.yj202588.top/gtknuebmlt.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.zhiwuduotai.top/gtpabqxdmk.html

[F12] CSV 读写
来源：http://hz.andypj.xyz/gtlwsvpbsc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.ehwqpu.com/gtdqatmnfm.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.xuetiantiany.cn/gteaescplz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.guannengcc.top/gtaxehszwp.html

TS:   // 同上
来源：http://hz.jinyuanbaomall.cn/gtwldwauax.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.guowangkeji.top/gttzezjizz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.c1oappe.top/gtymqspvkn.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.zhoulong.xyz/gtfdixvhau.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.chenzaomai.com/gtmiqvciob.html

================================================================================
来源：http://hz.guannengcc.top/gtndggbsvc.html

G. 面向对象
来源：http://hz.wangdashe.top/gtqwvelaup.html

================================================================================
来源：http://hz.zhoulong.xyz/gtsjptslos.html

[G01] 定义类
来源：http://hz.guannengcc.top/gtpzjnczig.html

Py:   class User: pass
来源：http://hz.gotoacloud.top/gtghglromk.html

PHP:  class User {}
来源：http://hz.hammf.cn/gtuhdwlyfm.html

JS:   class User {}
来源：http://hz.gotoacloud.top/gtzekauidr.html

TS:   class User { name: string = ""; }
来源：http://hz.zhaomingkeji.xyz/gtdawkeiyo.html

Java: class User {}
来源：http://hz.gotoacloud.top/gtgdxvqetd.html

Go:   type User struct { Name string }
来源：http://hz.wangshuangyany.cn/gtbmijsrwr.html

Ruby: class User; end
来源：http://hz.hywenlv.cn/gtlpovsioa.html

C#:   class User {}
来源：http://hz.hywenlv.cn/gtcbbnafop.html

[G02] 构造函数
来源：http://hz.52xcode.cn/gtazlrmfdt.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yj20258.top/gtnqthfowe.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.feifeiyinyue.top/gtygjappxw.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.daxiang520.top/gtttmxunon.html

TS:   constructor(public name: string) {}
来源：http://hz.ehwqpu.com/gtsztaajbj.html

Java: User(String name) { this.name = name; }
来源：http://hz.yueranfly.top/gtyqqvmutz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.shuidangran.top/gtoxydusud.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yanxiufei.cn/gttzqfrjhr.html

C#:   public User(string name) { Name = name; }
来源：http://hz.cheryme.top/gtjmeujirx.html

[G03] 实例属性
来源：http://hz.guowangkeji.top/gtrvgxhcim.html

Py:   self.name = "x"
来源：http://hz.zhiwuduotai.top/gtertytapi.html

PHP:  public string $name = "x";
来源：http://hz.hnqzz.top/gtegiyryue.html

JS:   this.name = "x";
来源：http://hz.cheryme.top/gtsrxkjswc.html

TS:   name: string = "x";
来源：http://hz.hnxiangtu.top/gtkwrlgtoq.html

Java: private String name;
来源：http://hz.jinqigufen.top/gtpkxdantv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.xylfe.cn/gtrndzzrqz.html

Ruby: @name = "x"
来源：http://hz.zhoulong.xyz/gtjpyfbqss.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yanxiufei.cn/gtssabarsl.html

[G04] 定义方法
来源：http://hz.gzhubu.top/gtennmbaqn.html

Py:   def greet(self): return self.name
来源：http://hz.tianlin.xyz/gtssiacjrj.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.quarkkingdee.top/gtawogmfge.html

JS:   greet() { return this.name; }
来源：http://hz.jyoumei.cn/gtmwmscqdp.html

TS:   greet(): string { return this.name; }
来源：http://hz.yanxiufei.cn/gtqbjqdkcx.html

Java: String greet() { return name; }
来源：http://hz.jqgfzy.top/gtsxrewxnp.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jiagoushi.top/gtqgokypwi.html

Ruby: def greet; @name; end
来源：http://hz.ppjwa.cn/gtxfubtxut.html

C#:   public string Greet() => Name;
来源：http://hz.yonumen.top/gtcjbeqsqj.html

[G05] 继承
来源：http://hz.ehwqpu.com/gtjpplhkbv.html

Py:   class Admin(User): pass
来源：http://hz.pengpengdd.cyou/gtulsehmhi.html

PHP:  class Admin extends User {}
来源：http://hz.daria6918.cn/gtahgtyqxt.html

JS:   class Admin extends User {}
来源：http://hz.cucudq.cn/gtmepuwfts.html

TS:   class Admin extends User {}
来源：http://hz.xuetiantiany.cn/gtbznolury.html

Java: class Admin extends User {}
来源：http://hz.kuanghao11.cn/gtvafayhif.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.jyoumei.cn/gtstvfinzw.html

Ruby: class Admin < User; end
来源：http://hz.gzhubu.top/gtgockiyrb.html

C#:   class Admin : User {}
来源：http://hz.tian-w.cn/gtqqxpmuub.html


<!-- 参考信息 -->