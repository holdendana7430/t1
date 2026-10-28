代发 wailian999

PHP:  implode(",", $items);
来源：http://hz.tian-w.cn/gtxtylfvpc.html

JS:   items.join(",")
来源：http://hz.chenlongwang.top/gtgexwucsm.html

TS:   items.join(",")
来源：http://hz.zycfv.cn/gtkgjtxasn.html

Java: String.join(",", items)
来源：http://hz.fzhhl.top/gtvfppxfpm.html

Go:   strings.Join(items, ",")
来源：http://hz.jinqigfzy.top/gtvarcusth.html

Ruby: items.join(",")
来源：http://hz.yangfankeji.com/gtomzbpnop.html

C#:   string.Join(",", items)
来源：http://hz.yuanzhike.top/gtlyfkkskv.html

[E09] 去除所有空白字符
来源：http://hz.yangfankeji.com/gtetxwgxrb.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.9152youxi.cn/gthjqgocre.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.sysykeji.top/gtromqeigb.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.c1oappe.top/gtustbcfen.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.shuidangran.top/gtzumawfcq.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.chenzaomai.com/gtcjipqdlq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.yangfankeji.com/gtlmxaqqel.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.fzhhl.top/gtygakkjwt.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.9152youxi.cn/gtzbzaxafz.html

[E10] 左侧补零 / 定长填充
来源：http://hz.zycfv.cn/gtjzmgreef.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.wangshuangyany.cn/gtrsmksufz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.ivvv.top/gtrhfddxkt.html

JS:   "7".padStart(3, "0")
来源：http://hz.hammf.cn/gtnbwdjtcd.html

TS:   "7".padStart(3, "0")
来源：http://hz.zhaomingkeji.xyz/gtgbjquatl.html

Java: String.format("%03d", 7)
来源：http://hz.sufxvd.cn/gtbyqoiwcd.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.yj20258.top/gtxbykgcvt.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.shzxlz.cn/gtoumcgnzc.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.tanke756.top/gtnvfdiwii.html

[E11] 反转字符串
来源：http://hz.cheryme.top/gtftnschpm.html

Py:   s[::-1]
来源：http://hz.gotoacloud.top/gtuzgjtmrd.html

PHP:  strrev($s);
来源：http://hz.mhx1999.top/gthkwtksvz.html

JS:   [...s].reverse().join("")
来源：http://hz.smart0.xyz/gtmhsnlvfe.html

TS:   [...s].reverse().join("")
来源：http://hz.0kj1m.cn/gtdalepgqv.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.shuidangran.top/gtdxfjvxgi.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.zhaomingkeji.xyz/gtjknjtqxx.html

Ruby: s.reverse
来源：http://hz.shuidangran.top/gtwmnokuoi.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.pycfn.com/gtrozlficq.html

[E12] 统计某字符出现次数
来源：http://hz.0kj1m.cn/gtewvzprjx.html

Py:   s.count("a")
来源：http://hz.yangfankeji.com/gthpavvgle.html

PHP:  substr_count($s, "a");
来源：http://hz.gogol.net.cn/gtkkejngms.html

JS:   s.split("a").length - 1
来源：http://hz.ehwqpu.com/gtwsovcpqd.html

TS:   s.split("a").length - 1
来源：http://hz.yanxiufei.cn/gtwhnallnl.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.daria6918.cn/gtyohhabza.html

Go:   strings.Count(s, "a")
来源：http://hz.jlsjyb.cn/gtdpjdcqtl.html

Ruby: s.count("a")
来源：http://hz.aizwys.cn/gtmyanoasz.html

C#:   s.Count(c => c == 'a')
来源：http://hz.andypj.xyz/gttttcdxuu.html

[E13] 逐字符遍历
来源：http://hz.chenzaomai.com/gtbcnwluce.html

Py:   for ch in s: print(ch)
来源：http://hz.svipenyu.cn/gtcycwxcjf.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.gzhubu.top/gtdpnuyeam.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ppjwa.cn/gtqemjaezr.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.hywenlv.cn/gtyetidmak.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.xuanzx.com/gtlvgxutcw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.chenjidiqi.icu/gtjkjepatt.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.tianlin.xyz/gtfbocfwit.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.sweek.top/gtkaekgpgi.html

[E14] URL 编码与 Base64
来源：http://hz.yanxiufei.cn/gtycpaemxg.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.shangyingyoupin.top/gthgczfiyj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.shanyushiyangtech.top/gtkoefttay.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.kuanghao11.cn/gtjefdukid.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.yj20258888.top/gtkbbvaxlq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.haohaochexian.top/gthxevkvum.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.jinghuilouyu.cn/gtqcrlsbzr.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.guowangkeji.top/gtegmnynjj.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.hfpthk.cn/gtjyswhfjy.html

[E15] HTML 转义 / 反转义
来源：http://hz.wangdashe.top/gtoltmpbrl.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.tanke756.top/gtjzuqbryr.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.xziqi.cn/gtqnonlplx.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yvedp.cn/gtqldullkr.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.kuanghao11.cn/gtxinisgxk.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.mhx1999.top/gtubtqcbpz.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.tian-w.cn/gtzkxqitap.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.pycfn.com/gtwnvndazq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.52xcode.cn/gtxrzzsdlf.html

[E16] 数字千分位
来源：http://hz.sxryk.cn/gtykhehxas.html

Py:   f"{1234567:,}"
来源：http://hz.ivvv.top/gtrmeftwvc.html

PHP:  number_format(1234567);
来源：http://hz.xuanzx.com/gtocfmhgbf.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.fzhhl.top/gtvxxwigbk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.bjfxy.top/gtziufeydt.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.jqgfzy.top/gtdytwzpdq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.tian-w.cn/gtahqxqxbd.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.kuanghao11.cn/gtkiivcxrd.html

C#:   1234567.ToString("N0")
来源：http://hz.jqgufenzy.top/gtusbivrjo.html

[E17] 首字母大写
来源：http://hz.yangfankeji.com/gtaqzchung.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.cqqwz.cn/gtcswtdnwx.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.fengsongda.top/gtjqkrbrdu.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.shanyushiyangkeji.top/gttqhapuie.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.shanyushiyangkeji.top/gtikmbhnyx.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.c1oappe.top/gtzgbcfxqn.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.zhixingplan.top/gtsckdcvbn.html

Ruby: s.capitalize
来源：http://hz.fzhhl.top/gtgoluoixw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.quarkkingdee.top/gtrrqsxdaa.html

[E18] 模板占位符替换
来源：http://hz.vqdsnc.cn/gtrwsdssrw.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.ywan-chungtsiang.top/gthrudmmhh.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.smart0.xyz/gtjjbyvwoo.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.hnqzz.top/gtvylcyfdo.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.iojbl.cn/gtiitdlyow.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.cucudq.cn/gtfergpswn.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.yj20258888.top/gtbxcprumu.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.ybcxt.top/gtwxnlzrjt.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.daxiang520.top/gtpqydbefb.html

[E19] 多行文本按行拆分
来源：http://hz.zhoulong.xyz/gtxixitwsm.html

Py:   s.splitlines()
来源：http://hz.hywenlv.cn/gtwovopvfh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.gotoacloud.top/gtoyvcqhaj.html

JS:   s.split(/\r?\n/)
来源：http://hz.pycfn.com/gtzcnfqutp.html

TS:   s.split(/\r?\n/)
来源：http://hz.zhengqikj.top/gtxinrwkuf.html

Java: s.lines().toList()
来源：http://hz.xingfuxueyuan.xyz/gtazlincrz.html

Go:   strings.Split(s, "\n")
来源：http://hz.shanyushiyangkeji.top/gtzahiocib.html

Ruby: s.lines
来源：http://hz.smart0.xyz/gtepvdujrm.html

C#:   s.Split('\n')
来源：http://hz.yvedp.cn/gtkaafngcs.html

[E20] 判断字符串是否为空
来源：http://hz.nanxuanxn.top/gttrtgoywd.html

Py:   if not s:
来源：http://hz.sxryk.cn/gtzgvhvgse.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.gzhubu.top/gtnovxeeee.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.9152youxi.cn/gtjminiiqc.html

TS:   if (s === "") {}
来源：http://hz.svipenyu.cn/gtiatifvdb.html

Java: if (s.isEmpty()) {}
来源：http://hz.yangfankeji.com/gtfwpgabvc.html

Go:   if s == "" {}
来源：http://hz.ehwqpu.com/gteqriwext.html

Ruby: if s.empty?
来源：http://hz.kuanghao11.cn/gtdcgwnxnf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.dianchejie.cn/gtuycxoauq.html

[E21] 超长截断加省略号
来源：http://hz.aizwys.cn/gtxqrxzuxm.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.yueranfly.top/gtgdyigxrr.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.hammf.cn/gtmwvklbzr.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jinqigfzy.top/gtrnpytrti.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.cdnleiting.top/gtzklfvnio.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.zhongyouzk.top/gtgbthupux.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.tanke756.top/gtsisuttkq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.jiagoushi.top/gtavxfgtxy.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.hywenlv.cn/gtimxwbary.html

[E22] 字节长度与字符长度
来源：http://hz.cheryme.top/gtqemwirqo.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.0kj1m.cn/gtgxuemtcw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jqgufenzy.top/gtqetnfhuc.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.meibo888.top/gtsdzwntdk.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.xuetiantiany.cn/gtdtuqdgjz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.ybcxt.top/gtuvrbofne.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.hfpthk.cn/gtscpgiksx.html

Ruby: s.bytesize;  s.length
来源：http://hz.hywenlv.cn/gtzrdnshwi.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.shanyushiyangkeji.top/gtoijhsano.html

================================================================================
来源：http://hz.hywenlv.cn/gtyukwcezx.html

F. 文件与目录
来源：http://hz.yj20258888.top/gtuyjlrdqm.html

================================================================================
来源：http://hz.aibaodan.cn/gtkqlaypsq.html

[F01] 读取整个文件
来源：http://hz.snrcjt.cn/gtqrvpuovn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.jinqigufen.top/gtlwuvxspx.html

PHP:  file_get_contents("a.txt");
来源：http://hz.hysaishi.cn/gtvaertmsb.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.52xcode.cn/gtgoowirrl.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.ydjk.org.cn/gtswpnwwuq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.snrcjt.cn/gtiffvogfq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.yongpay.top/gtmvjgmbjg.html

Ruby: File.read("a.txt")
来源：http://hz.yueranfly.top/gtemuvtymv.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.iojbl.cn/gtbpufnugx.html

[F02] 逐行读取文件
来源：http://hz.smart0.xyz/gtqsjlcdgu.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.yongpay.top/gtcffvzioi.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.shanyushiyangtech.top/gtlfgmcysw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xinyue.icu/gtvkzafztl.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.dashuyun.cn/gtcwagbjlt.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.sysykeji.top/gtykbilijb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.cucudq.cn/gtsnwjzfaz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.tian-w.cn/gtvcrclgum.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.feifeiyinyue.top/gtkmfrfbpm.html

[F03] 写入文件（覆盖）
来源：http://hz.pengpengdd.cyou/gtshrwjkfj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.zhaomingkeji.xyz/gtlbwtjuis.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.gotoacloud.top/gtkdvonzjj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.iojbl.cn/gtvevruumd.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jinghuilouyu.cn/gtrzlddgxb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.cashguo.top/gtqjlsliao.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.tian-w.cn/gtaskimyfy.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.gzhubu.top/gtzzsazfky.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.xingfuxueyuan.xyz/gtvqslynmp.html

[F04] 追加写入文件
来源：http://hz.zhongyouzk.top/gtqcxjnutf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.jqgufenzy.top/gtwzhdkrpp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.tanke756.top/gtvtmqpnes.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.gotoacloud.top/gtcghkeunx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.nanxinkj.top/gtuwsvonnf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.xinyue.icu/gtkbenjsyb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.tanke756.top/gthuucqtag.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yj202588.top/gtqcjyqofs.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.chenjidiqi.icu/gtxtcsjonk.html

[F05] 判断文件或目录是否存在
来源：http://hz.shanyushiyangtech.top/gtijkghexs.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.hnxiangtu.top/gtsoyrzupq.html

PHP:  file_exists("a.txt");
来源：http://hz.hongshengwenyu.top/gtkepzgvls.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yj20258.top/gthhhwncss.html

TS:   fs.existsSync("a.txt")
来源：http://hz.iojbl.cn/gtsjefgjka.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.aizwys.cn/gtmcmwevws.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.jinghuilouyu.cn/gtxdwgmrvy.html

Ruby: File.exist?("a.txt")
来源：http://hz.sysykeji.top/gtuwtgitnj.html

C#:   File.Exists("a.txt")
来源：http://hz.xuetiantiany.cn/gtdbdcqirb.html

[F06] 删除文件
来源：http://hz.jlsjyb.cn/gtkyiaovtx.html

Py:   os.remove("a.txt")
来源：http://hz.guannengcc.top/gtymepbqha.html

PHP:  unlink("a.txt");
来源：http://hz.redwolf501.top/gtkdzcvgpm.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.gaohongyu789.top/gtdopgambs.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.daria6918.cn/gtadlgdmjp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.smart0.xyz/gthukwocxd.html

Go:   os.Remove("a.txt")
来源：http://hz.jqgfzy.top/gtpzuvgqmo.html

Ruby: File.delete("a.txt")
来源：http://hz.cdnleiting.top/gtsdaddxgb.html

C#:   File.Delete("a.txt");
来源：http://hz.sxryk.cn/gttlxopogs.html

[F07] 创建目录（含多级）
来源：http://hz.jiagoushi.top/gtrvijtpvi.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.tianlin.xyz/gtcknigkig.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.sxryk.cn/gtqlilkixv.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.xingfuxueyuan.xyz/gtzwkhbxfl.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.meibo888.top/gtqfmejlvw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.cdnleiting.top/gteylypqpe.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.quarkkingdee.top/gtdrrnyoay.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.nanxinkj.top/gtbupqiuek.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.birdmap.top/gtevabzqcd.html

[F08] 遍历目录
来源：http://hz.fzhhl.top/gtyzikmdxf.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.bjfxy.top/gtziuabknb.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.xziqi.cn/gtjvaincwt.html

JS:   fs.readdirSync("dir")
来源：http://hz.redwolf501.top/gtcohqyria.html

TS:   fs.readdirSync("dir")
来源：http://hz.tianlin.xyz/gtiflpfyts.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.nanxinkj.top/gtepworrnt.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.ybcxt.top/gtidwrzvlz.html

Ruby: Dir.children("dir")
来源：http://hz.cheryme.top/gtgfmcqpkt.html

C#:   Directory.GetFiles("dir")
来源：http://hz.jlsjyb.cn/gtaivhitqo.html

[F09] 获取文件大小
来源：http://hz.ydzc1.top/gtfqsibblr.html

Py:   os.path.getsize("a.txt")
来源：http://hz.cdnleiting.top/gtsktrdbrz.html

PHP:  filesize("a.txt");
来源：http://hz.zhongyouzk.top/gtrjgnvsqa.html

JS:   fs.statSync("a.txt").size
来源：http://hz.havefunace.top/gtabiafnnk.html

TS:   fs.statSync("a.txt").size
来源：http://hz.xuanzx.com/gtvlwfhqrv.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jianghu66.top/gtzebwffou.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.jqgfzy.top/gtmltdjxoh.html

Ruby: File.size("a.txt")
来源：http://hz.shuidangran.top/gtexbkzbqy.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.aibaodan.cn/gthbsiflol.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.ywan-chungtsiang.top/gtbgumpxmy.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jiagoushi.top/gtgmhvnwyl.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.kuanghao11.cn/gtmlhlxkhq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.vqdsnc.cn/gtmjdxajrc.html

TS:   path.extname("a.txt")
来源：http://hz.gogol.net.cn/gtswvlyodc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.haohaochexian.top/gtxtvkntcx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.cucudq.cn/gtvuctwiwv.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jyoumei.cn/gtfbtyqova.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.cheryme.top/gtzdaenuye.html

[F11] 复制与移动文件
来源：http://hz.ppjwa.cn/gtppkdepjo.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.yanxiufei.cn/gtmolknkte.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.chenzaomai.com/gtyisbvexb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.daria6918.cn/gtdpqodjdq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.9152youxi.cn/gttgmbrimp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.smart0.xyz/gtjdlbrhpl.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.ehwqpu.com/gtogcwftou.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.hongshengwenyu.top/gttrlrwjja.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.tanke756.top/gtnrbzwdko.html

[F12] CSV 读写
来源：http://hz.nanxuanxn.top/gtktzvcber.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.yueranfly.top/gtxcpdmodh.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.shanyushiyangtech.top/gtjwswvgtw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.nwbrower.top/gtmapexbji.html

TS:   // 同上
来源：http://hz.tianlin.xyz/gtnizofldl.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.yvedp.cn/gtwuvjswpe.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.sxryk.cn/gtqmwbgqka.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.yongpay.top/gtfiqtvpzs.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.shangyingyoupin.top/gtskopzeby.html

================================================================================
来源：http://hz.hfpthk.cn/gtbdgwskkv.html

G. 面向对象
来源：http://hz.havefunace.top/gtuxhlgduf.html

================================================================================
来源：http://hz.hnqzz.top/gtlemiftrl.html

[G01] 定义类
来源：http://hz.andypj.xyz/gtmsquutwo.html

Py:   class User: pass
来源：http://hz.ydjk.org.cn/gttvsfypny.html

PHP:  class User {}
来源：http://hz.pengpengdd.cyou/gtimmzxakp.html

JS:   class User {}
来源：http://hz.sweek.top/gtgnxtuhhy.html

TS:   class User { name: string = ""; }
来源：http://hz.ydzc1.top/gtjhzpoqky.html

Java: class User {}
来源：http://hz.cheryme.top/gtohlmpgon.html

Go:   type User struct { Name string }
来源：http://hz.iojbl.cn/gtcpkbziqu.html

Ruby: class User; end
来源：http://hz.zdqjudy.top/gtcsmqlmjo.html

C#:   class User {}
来源：http://hz.xinyue.icu/gtdapiqlnt.html

[G02] 构造函数
来源：http://hz.ywan-chungtsiang.top/gtnhtgnbsz.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.chenlongwang.top/gtvfiwdplp.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.jinqigufen.top/gtxfwptuln.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.jqgfzy.top/gtnzimilrf.html

TS:   constructor(public name: string) {}
来源：http://hz.yvedp.cn/gtijsagxbp.html

Java: User(String name) { this.name = name; }
来源：http://hz.feifeiyinyue.top/gtntqckclg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.hnxiangtu.top/gthwuctlgw.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.hysaishi.cn/gtyfwoipeq.html

C#:   public User(string name) { Name = name; }
来源：http://hz.ywan-chungtsiang.top/gtphkjiuxk.html

[G03] 实例属性
来源：http://hz.ydzc1.top/gtsjzuiwnr.html

Py:   self.name = "x"
来源：http://hz.redwolf501.top/gtzvixklcs.html

PHP:  public string $name = "x";
来源：http://hz.nanxuanxn.top/gtagulohjr.html

JS:   this.name = "x";
来源：http://hz.cashguo.top/gtlqbgxryw.html

TS:   name: string = "x";
来源：http://hz.cashguo.top/gtnsztfwyv.html

Java: private String name;
来源：http://hz.yonumen.top/gtfikjkecz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.smart0.xyz/gtneejizvy.html

Ruby: @name = "x"
来源：http://hz.xuanzx.com/gtwxbqzrgm.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jinghuilouyu.cn/gtvjraheog.html

[G04] 定义方法
来源：http://hz.cashguo.top/gtqrzphcze.html

Py:   def greet(self): return self.name
来源：http://hz.xingfuxueyuan.xyz/gtayfqisdt.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.hnqzz.top/gtwlyxaxjo.html

JS:   greet() { return this.name; }
来源：http://hz.hywenlv.cn/gtoovzpcwl.html

TS:   greet(): string { return this.name; }
来源：http://hz.svipenyu.cn/gtegzqfasn.html

Java: String greet() { return name; }
来源：http://hz.redwolf501.top/gtnaroqhjk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.iojbl.cn/gtqigpznwo.html

Ruby: def greet; @name; end
来源：http://hz.meibo888.top/gtkhacazbi.html

C#:   public string Greet() => Name;
来源：http://hz.zhijiandao.cn/gtsdyktarm.html

[G05] 继承
来源：http://hz.gaohongyu789.top/gtjtwgxjef.html

Py:   class Admin(User): pass
来源：http://hz.fengsongda.top/gtvqmhtfrd.html

PHP:  class Admin extends User {}
来源：http://hz.ybcxt.top/gteeyryhzp.html

JS:   class Admin extends User {}
来源：http://hz.birdmap.top/gtqrdbypnq.html

TS:   class Admin extends User {}
来源：http://hz.snrcjt.cn/gtnfosipwb.html

Java: class Admin extends User {}
来源：http://hz.yongpay.top/gtaghmcpys.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yj20258888.top/gtevfikedz.html

Ruby: class Admin < User; end
来源：http://hz.guannengcc.top/gtffqwvssi.html

C#:   class Admin : User {}
来源：http://hz.shanyushiyangtech.top/gtyxiyeuus.html

[G06] 重写方法
来源：http://hz.cucudq.cn/gtlfouurir.html

Py:   def greet(self): return "admin"
来源：http://hz.jianghu66.top/gtsnzzqxty.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.shuidangran.top/gthtxxofjk.html

JS:   greet() { return "admin"; }
来源：http://hz.guowangkeji.top/gtvnlfmgug.html

TS:   greet(): string { return "admin"; }
来源：http://hz.vqdsnc.cn/gtgyvtyqbs.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.cucudq.cn/gtecqsvirb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.shzxlz.cn/gtuspoedde.html

Ruby: def greet; "admin"; end
来源：http://hz.zhoulong.xyz/gtigotjjnh.html


<!-- 参考信息 -->