代发 wailian999

C#:   s.Replace("a", "b")
来源：http://hz.quarkkingdee.top/gttztvmgbi.html

[E07] 按分隔符拆分
来源：http://hz.pycfn.com/gtrweovcwi.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.sxryk.cn/gtfibxaplu.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.hnxiangtu.top/gtkjynteob.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.52xcode.cn/gtnqbpfjpy.html

TS:   s.split(",")
来源：http://hz.ydzc1.top/gtesvjpdmp.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.xziqi.cn/gtwlwdqmxb.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.yuxming.cn/gthgylkvka.html

Ruby: s.split(",");  s.split
来源：http://hz.cashguo.top/gtvxojblcp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.tianlin.xyz/gtfpcewgjg.html

[E08] 数组按分隔符合并
来源：http://hz.sxryk.cn/gtrnavtlll.html

Py:   ",".join(items)
来源：http://hz.jiagoushi.top/gthrtaxvdc.html

PHP:  implode(",", $items);
来源：http://hz.xziqi.cn/gtdiebnskl.html

JS:   items.join(",")
来源：http://hz.gogol.net.cn/gtihybblqr.html

TS:   items.join(",")
来源：http://hz.andypj.xyz/gtauawwmrq.html

Java: String.join(",", items)
来源：http://hz.sweek.top/gtojoalysx.html

Go:   strings.Join(items, ",")
来源：http://hz.yj20258.top/gtzvzkbznh.html

Ruby: items.join(",")
来源：http://hz.yangfankeji.com/gtdyzfgeww.html

C#:   string.Join(",", items)
来源：http://hz.cucudq.cn/gtwrjguiuv.html

[E09] 去除所有空白字符
来源：http://hz.yongpay.top/gtpgdfplhs.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.yongpay.top/gtlcepguqi.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.shuidangran.top/gtzsxbxgzq.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.kuanghao11.cn/gtrvfoghou.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.redwolf501.top/gteqqqxmgv.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.cheryme.top/gtnzqbruei.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.snrcjt.cn/gtcyrfjuue.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.yuxming.cn/gtebptcrzx.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.shzxlz.cn/gtaugkwgqn.html

[E10] 左侧补零 / 定长填充
来源：http://hz.gzhubu.top/gtzeusnskg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.52xcode.cn/gtqloexdmw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.xingfuxueyuan.xyz/gtsafwvmuz.html

JS:   "7".padStart(3, "0")
来源：http://hz.xuanzx.com/gtjoycvvqz.html

TS:   "7".padStart(3, "0")
来源：http://hz.iojbl.cn/gtpemjwcze.html

Java: String.format("%03d", 7)
来源：http://hz.yonumen.top/gtvzimqrit.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.chenjidiqi.icu/gthqvpmnim.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.pengpengdd.cyou/gtrneipzot.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.shanyushiyangtech.top/gtqqjbiuwy.html

[E11] 反转字符串
来源：http://hz.ppjwa.cn/gtbiujjrrd.html

Py:   s[::-1]
来源：http://hz.daxiang520.top/gtrgvcqixv.html

PHP:  strrev($s);
来源：http://hz.xinyue.icu/gteiohybgt.html

JS:   [...s].reverse().join("")
来源：http://hz.redwolf501.top/gtbfrshjdv.html

TS:   [...s].reverse().join("")
来源：http://hz.smart0.xyz/gtgovdrrvq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.chenjidiqi.icu/gtefdozytm.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.sweek.top/gtjsocmcto.html

Ruby: s.reverse
来源：http://hz.chenlongwang.top/gtefuujmet.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.jinyuanbaomall.cn/gtjpcfxptd.html

[E12] 统计某字符出现次数
来源：http://hz.zhaomingkeji.xyz/gtyobhtqjv.html

Py:   s.count("a")
来源：http://hz.jinghuilouyu.cn/gtptfoahkq.html

PHP:  substr_count($s, "a");
来源：http://hz.hammf.cn/gtobrmyrgb.html

JS:   s.split("a").length - 1
来源：http://hz.gotoacloud.top/gtsyrafmee.html

TS:   s.split("a").length - 1
来源：http://hz.jinqigfzy.top/gttgqiflxq.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.ydjk.org.cn/gttznmjoai.html

Go:   strings.Count(s, "a")
来源：http://hz.yj20258888.top/gtewdpsadr.html

Ruby: s.count("a")
来源：http://hz.ivvv.top/gtwcfcydmh.html

C#:   s.Count(c => c == 'a')
来源：http://hz.yvedp.cn/gtobjopcff.html

[E13] 逐字符遍历
来源：http://hz.snrcjt.cn/gtvymyqkob.html

Py:   for ch in s: print(ch)
来源：http://hz.xuetiantiany.cn/gtildinfro.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.sysykeji.top/gtfeozpnrt.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zhoulong.xyz/gtkmurzefi.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jinqigufen.top/gtklaffeje.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.fengsongda.top/gtggxtfahm.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.316326.xyz/gtticwuygs.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.shanyushiyangkeji.top/gtjknstuit.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.feifeiyinyue.top/gttsfjgojt.html

[E14] URL 编码与 Base64
来源：http://hz.yongpay.top/gtxqkwzblg.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.yj20258888.top/gtqdibtsqd.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.daria6918.cn/gtrkbvzidm.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.hnxiangtu.top/gtszlvjazz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.nanxinkj.top/gtmfjktkmc.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.zycfv.cn/gtkiotqvca.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.zhijiandao.cn/gtiqgmrapo.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.jinghuilouyu.cn/gtnmxhsnnx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.pycfn.com/gtjkdsnfch.html

[E15] HTML 转义 / 反转义
来源：http://hz.hammf.cn/gtafvtueer.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.yangfankeji.com/gtzindkayk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.jinqigfzy.top/gtzxwhydxr.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yj20258.top/gtxjezbwue.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.hfpthk.cn/gtzlklejif.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.hfpthk.cn/gtkqtcqdqo.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.52xcode.cn/gtcobiylwa.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.9152youxi.cn/gtlfjyabjd.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.aizwys.cn/gthyjyudye.html

[E16] 数字千分位
来源：http://hz.cqqwz.cn/gtrjubqlkb.html

Py:   f"{1234567:,}"
来源：http://hz.tanke756.top/gtfsbppvxl.html

PHP:  number_format(1234567);
来源：http://hz.yanxiufei.cn/gtxndyyhdw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.ppjwa.cn/gtshgpbigv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.jinyuanbaomall.cn/gtsgzslxqv.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.fengsongda.top/gtwexydkzz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.haohaochexian.top/gtvwwooeky.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.hongshengwenyu.top/gtkkeujjgy.html

C#:   1234567.ToString("N0")
来源：http://hz.xingfuxueyuan.xyz/gtxbmoyytg.html

[E17] 首字母大写
来源：http://hz.birdmap.top/gttjutniam.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.jqgufenzy.top/gtjyggilzu.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.hammf.cn/gtphddmioo.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zdqjudy.top/gtrysjhaox.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yanxiufei.cn/gtiinbanaj.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.ivvv.top/gtkhtlncxi.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.svipenyu.cn/gtdhioadbj.html

Ruby: s.capitalize
来源：http://hz.quarkkingdee.top/gtxiodgvkc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yj20258.top/gtssurnexr.html

[E18] 模板占位符替换
来源：http://hz.ehwqpu.com/gtjyqbtdpg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.dianchejie.cn/gtaigopica.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.xinyue.icu/gtllojdqgg.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.nanxuanxn.top/gtflfqctae.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.yueranfly.top/gtzplfqxum.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.xziqi.cn/gtglepsbjt.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.jqgufenzy.top/gtgmaucmmt.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.wangdashe.top/gtouvrkzyf.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.havefunace.top/gtgyduyxdh.html

[E19] 多行文本按行拆分
来源：http://hz.hywenlv.cn/gticlukfdr.html

Py:   s.splitlines()
来源：http://hz.gogol.net.cn/gtwyxbcnag.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.yvedp.cn/gtlmiycprd.html

JS:   s.split(/\r?\n/)
来源：http://hz.sxryk.cn/gtngtikbfz.html

TS:   s.split(/\r?\n/)
来源：http://hz.ydjk.org.cn/gtykxhhsms.html

Java: s.lines().toList()
来源：http://hz.xylfe.cn/gtbmzshxxj.html

Go:   strings.Split(s, "\n")
来源：http://hz.nanxinkj.top/gttceozcsr.html

Ruby: s.lines
来源：http://hz.ehwqpu.com/gtwouhnedx.html

C#:   s.Split('\n')
来源：http://hz.sufxvd.cn/gtqunikxcn.html

[E20] 判断字符串是否为空
来源：http://hz.shanyushiyangkeji.top/gthtjlulsu.html

Py:   if not s:
来源：http://hz.zhijiandao.cn/gtvjnbrjee.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.guannengcc.top/gthcuqsrie.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.jlsjyb.cn/gtsgtqfzah.html

TS:   if (s === "") {}
来源：http://hz.hysaishi.cn/gtpnnrlsvn.html

Java: if (s.isEmpty()) {}
来源：http://hz.tanke756.top/gtzwvvkfie.html

Go:   if s == "" {}
来源：http://hz.pycfn.com/gtqgmomeuz.html

Ruby: if s.empty?
来源：http://hz.jinqigfzy.top/gtikmbdzhq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.hfpthk.cn/gtwqldnvlw.html

[E21] 超长截断加省略号
来源：http://hz.nanxuanxn.top/gtajuyqiue.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.zdqjudy.top/gtpdlyxnbi.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.xinyue.icu/gtkfnzlphz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.hywenlv.cn/gtrggxtysh.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.shuidangran.top/gtafvytlbf.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yonumen.top/gtqikuevwp.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.0kj1m.cn/gtaxpdhvqn.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.jinqigfzy.top/gtwaszhvsk.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.jinyuanbaomall.cn/gtmxbroyli.html

[E22] 字节长度与字符长度
来源：http://hz.havefunace.top/gtvjnntfzf.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.zhijiandao.cn/gtksipylau.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.chenjidiqi.icu/gtxoeodkws.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hywenlv.cn/gtbyqyzaup.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhengqikj.top/gttvlvpjjz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.9152youxi.cn/gtmtjrztms.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.vqdsnc.cn/gtpynagdor.html

Ruby: s.bytesize;  s.length
来源：http://hz.zycfv.cn/gtcanixrut.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.yvedp.cn/gtmfwdasxt.html

================================================================================
来源：http://hz.havefunace.top/gtnzwadwoq.html

F. 文件与目录
来源：http://hz.316326.xyz/gtpdodjccu.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtmchtppwy.html

[F01] 读取整个文件
来源：http://hz.shuidangran.top/gtasbjjswj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.dashuyun.cn/gtcbxsixpy.html

PHP:  file_get_contents("a.txt");
来源：http://hz.jiagoushi.top/gtjdouxfpj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.nanxuanxn.top/gtoicsosez.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.xuetiantiany.cn/gtopapjauy.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.jianghu66.top/gtglqnapeo.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.yangfankeji.com/gtymyfaywt.html

Ruby: File.read("a.txt")
来源：http://hz.cucudq.cn/gtijomtetb.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.c1oappe.top/gtwafybdfk.html

[F02] 逐行读取文件
来源：http://hz.yanxiufei.cn/gtrjsdasms.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.zycfv.cn/gtcusxpjpi.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.xylfe.cn/gtthfjewag.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zycfv.cn/gtegchkohm.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hnxiangtu.top/gtltavurdf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.yongpay.top/gtghvudsqv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.cqqwz.cn/gttjpuqhqg.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.fzhhl.top/gtxagvlhez.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.nwbrower.top/gthgsvvnqe.html

[F03] 写入文件（覆盖）
来源：http://hz.wangdashe.top/gtcwolznaz.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.havefunace.top/gtpcbckeau.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.xziqi.cn/gtipusabqs.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.fengsongda.top/gtjdigdzhf.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.chenlongwang.top/gtrmrusceo.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.jinqigfzy.top/gtfncnwppd.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.xingfuxueyuan.xyz/gtcbmavhho.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.cheryme.top/gtbobqmzzo.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.zhixingplan.top/gtqrgecaxt.html

[F04] 追加写入文件
来源：http://hz.quarkkingdee.top/gtvzavtkbm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.jinqigfzy.top/gtbkzzhssw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.sufxvd.cn/gtsakyccbj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.vqdsnc.cn/gtevkesfiz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.fengsongda.top/gtdwoqluvp.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.jlsjyb.cn/gttoqyyrnh.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.hywenlv.cn/gtazutazcv.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.gotoacloud.top/gtmmdpvznn.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.nanxuanxn.top/gtzxltfprk.html

[F05] 判断文件或目录是否存在
来源：http://hz.tianlin.xyz/gtnvvfclho.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.havefunace.top/gtllddshnn.html

PHP:  file_exists("a.txt");
来源：http://hz.sufxvd.cn/gtrkeoemex.html

JS:   fs.existsSync("a.txt")
来源：http://hz.chenjidiqi.icu/gtbjihvhxy.html

TS:   fs.existsSync("a.txt")
来源：http://hz.nwbrower.top/gtqhrkdplc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.jqgfzy.top/gtrsrhtubf.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.xinyue.icu/gtkzqqltnw.html

Ruby: File.exist?("a.txt")
来源：http://hz.c1oappe.top/gtsakksjrl.html

C#:   File.Exists("a.txt")
来源：http://hz.hongshengwenyu.top/gtgiryauyi.html

[F06] 删除文件
来源：http://hz.zhaomingkeji.xyz/gthffcwfqr.html

Py:   os.remove("a.txt")
来源：http://hz.ydzc1.top/gtfunbynsp.html

PHP:  unlink("a.txt");
来源：http://hz.cheryme.top/gtojftwwft.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.zhiwuduotai.top/gtfnismcsb.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.ppjwa.cn/gtgoemniux.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.zhongyouzk.top/gtjgobcvei.html

Go:   os.Remove("a.txt")
来源：http://hz.yonumen.top/gtgovaqryc.html

Ruby: File.delete("a.txt")
来源：http://hz.zhixingplan.top/gtkzaindyu.html

C#:   File.Delete("a.txt");
来源：http://hz.jinqigufen.top/gtgrdhqyye.html

[F07] 创建目录（含多级）
来源：http://hz.dashuyun.cn/gtpxsuinik.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yuxming.cn/gtuthbbnjf.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.pengpengdd.cyou/gtzgseoacz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.nanxuanxn.top/gtnvsbklzj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.tanke756.top/gtfxneaihq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.fengsongda.top/gtpyunjbpg.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.cdnleiting.top/gtqagtlyzn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.daxiang520.top/gtspkulead.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.hysaishi.cn/gtbapybbdl.html

[F08] 遍历目录
来源：http://hz.cheryme.top/gtavqtdemg.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.haohaochexian.top/gtlqspyajs.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.xingfuxueyuan.xyz/gtdejkveva.html

JS:   fs.readdirSync("dir")
来源：http://hz.jqgfzy.top/gtinjptcwn.html

TS:   fs.readdirSync("dir")
来源：http://hz.cqqwz.cn/gtugzoisjw.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.pycfn.com/gtpcglspyd.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.jinqigfzy.top/gtkzzyhihb.html

Ruby: Dir.children("dir")
来源：http://hz.gaohongyu789.top/gtfnabmnrg.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yueranfly.top/gtucdxgscd.html

[F09] 获取文件大小
来源：http://hz.wangshuangyany.cn/gtmhcdckzj.html

Py:   os.path.getsize("a.txt")
来源：http://hz.316326.xyz/gtlimmwsig.html

PHP:  filesize("a.txt");
来源：http://hz.redwolf501.top/gtktaonxnc.html

JS:   fs.statSync("a.txt").size
来源：http://hz.zhiwuduotai.top/gtxjixnxzr.html

TS:   fs.statSync("a.txt").size
来源：http://hz.nanxuanxn.top/gtsfhlhaek.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.chenlongwang.top/gtnlapjtwk.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.feifeiyinyue.top/gtrrfkzdod.html

Ruby: File.size("a.txt")
来源：http://hz.andypj.xyz/gtnwvlxvfa.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.jinghuilouyu.cn/gtwjrmrlmz.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.guowangkeji.top/gtupnwbqwr.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.aibaodan.cn/gtjfboavkc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.jinqigfzy.top/gtqcbrtnbs.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.yj202588.top/gtgyhnbipl.html

TS:   path.extname("a.txt")
来源：http://hz.316326.xyz/gthkfvnhcg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.xylfe.cn/gtmqkwrjkt.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.sxryk.cn/gtgwzcmkpo.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jinqigufen.top/gtfonsykgx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.fzhhl.top/gtstyupylm.html

[F11] 复制与移动文件
来源：http://hz.xylfe.cn/gtdtueeeiv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.sxryk.cn/gtoegxlygh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.zhixingplan.top/gtctnszhpk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.nanxuanxn.top/gtrhploqir.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ydjk.org.cn/gtvqjczkaz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.hnqzz.top/gtdeobpkhy.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yj20258.top/gtnsvsdegi.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.andypj.xyz/gtosoqpzod.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.ehwqpu.com/gthsxskdqe.html

[F12] CSV 读写
来源：http://hz.xinyue.icu/gtgoqtvmif.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.sysykeji.top/gtdibaqhdx.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.zhoulong.xyz/gtfvlimvbc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.nanxuanxn.top/gtmbdxdcxo.html

TS:   // 同上
来源：http://hz.tanke756.top/gttkfvdvgj.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.hongshengwenyu.top/gtnuibelkq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.sysykeji.top/gtzcnjnyxg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.kuanghao11.cn/gtcroklflu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.meibo888.top/gtvtbdyuqw.html

================================================================================
来源：http://hz.c1oappe.top/gtwqrttowi.html

G. 面向对象
来源：http://hz.nanxinkj.top/gtmedoldxu.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtxlsosfua.html

[G01] 定义类
来源：http://hz.yj20258888.top/gtywqgcwwu.html

Py:   class User: pass
来源：http://hz.havefunace.top/gtkyddhtpd.html

PHP:  class User {}
来源：http://hz.hammf.cn/gtnxrpavcs.html

JS:   class User {}
来源：http://hz.gogol.net.cn/gttmwclmeq.html

TS:   class User { name: string = ""; }
来源：http://hz.kuanghao11.cn/gtrrdqtgza.html

Java: class User {}
来源：http://hz.meibo888.top/gtxkolvvox.html

Go:   type User struct { Name string }
来源：http://hz.ivvv.top/gtrqmwzmfp.html

Ruby: class User; end
来源：http://hz.zhijiandao.cn/gtmzmckxph.html

C#:   class User {}
来源：http://hz.jqgufenzy.top/gtxnbjfkgo.html

[G02] 构造函数
来源：http://hz.chenjidiqi.icu/gtpbsgsmdo.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.tanke756.top/gtqbywsrpy.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.jianghu66.top/gtdcqftggh.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.tanke756.top/gtccpzpzee.html

TS:   constructor(public name: string) {}
来源：http://hz.yanxiufei.cn/gthwswbsxv.html

Java: User(String name) { this.name = name; }
来源：http://hz.cdnleiting.top/gtgnxmulne.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.feifeiyinyue.top/gtdcsjklho.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.zhoulong.xyz/gtbdckhxod.html

C#:   public User(string name) { Name = name; }
来源：http://hz.cashguo.top/gththronlb.html

[G03] 实例属性
来源：http://hz.cqqwz.cn/gtbuusuidi.html

Py:   self.name = "x"
来源：http://hz.hfpthk.cn/gtizytxarf.html

PHP:  public string $name = "x";
来源：http://hz.gaohongyu789.top/gtepusbvwa.html

JS:   this.name = "x";
来源：http://hz.jlsjyb.cn/gthhrtfawu.html

TS:   name: string = "x";
来源：http://hz.guowangkeji.top/gtsopydsbc.html

Java: private String name;
来源：http://hz.yongpay.top/gtgccnyfjf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.tanke756.top/gtjrryxojy.html

Ruby: @name = "x"
来源：http://hz.xingfuxueyuan.xyz/gtqwfukcis.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.ydjk.org.cn/gtrjuwyyxg.html

[G04] 定义方法
来源：http://hz.gaohongyu789.top/gtgurlanft.html

Py:   def greet(self): return self.name
来源：http://hz.hnxiangtu.top/gtgqpmxltv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.aibaodan.cn/gtrmvubnlo.html

JS:   greet() { return this.name; }
来源：http://hz.gzhubu.top/gtpxxcobqi.html

TS:   greet(): string { return this.name; }
来源：http://hz.havefunace.top/gtedtirasn.html

Java: String greet() { return name; }
来源：http://hz.mhx1999.top/gtiqoxkjyl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.meibo888.top/gtsmoznakg.html

Ruby: def greet; @name; end
来源：http://hz.zhaomingkeji.xyz/gtqtpbskte.html

C#:   public string Greet() => Name;
来源：http://hz.jiagoushi.top/gtimkncswm.html

[G05] 继承
来源：http://hz.jianghu66.top/gtylqhgntb.html

Py:   class Admin(User): pass
来源：http://hz.guannengcc.top/gtiekbcyew.html

PHP:  class Admin extends User {}
来源：http://hz.jiagoushi.top/gtvnupseef.html

JS:   class Admin extends User {}
来源：http://hz.meibo888.top/gtzxhvtnxs.html

TS:   class Admin extends User {}
来源：http://hz.tianlin.xyz/gtfgscdhnl.html


<!-- 参考信息 -->