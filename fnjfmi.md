代发 wailian999

Ruby: s.reverse
来源：http://hz.xuanzx.com/gtriheaokt.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.hysaishi.cn/gtpxgrfajc.html

[E12] 统计某字符出现次数
来源：http://hz.yuanzhike.top/gtgjyzqwie.html

Py:   s.count("a")
来源：http://hz.hongshengwenyu.top/gtftxzfqwf.html

PHP:  substr_count($s, "a");
来源：http://hz.bjfxy.top/gtfmruyiek.html

JS:   s.split("a").length - 1
来源：http://hz.iojbl.cn/gtzvvrpyps.html

TS:   s.split("a").length - 1
来源：http://hz.daxiang520.top/gtmkvjbigj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.xziqi.cn/gtisnrwcpg.html

Go:   strings.Count(s, "a")
来源：http://hz.pycfn.com/gtqizxnnnm.html

Ruby: s.count("a")
来源：http://hz.xuetiantiany.cn/gtiscdlffa.html

C#:   s.Count(c => c == 'a')
来源：http://hz.svipenyu.cn/gtratexvcz.html

[E13] 逐字符遍历
来源：http://hz.pycfn.com/gtsrqtwewt.html

Py:   for ch in s: print(ch)
来源：http://hz.daria6918.cn/gtabkizoli.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.hywenlv.cn/gthpicmxcp.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xuanzx.com/gtxzdpkjnl.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.gogol.net.cn/gtgndrrrna.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.birdmap.top/gtdafrjwjs.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.zhiwuduotai.top/gtpvtvvech.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.dianchejie.cn/gtdpvjmvuc.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.snrcjt.cn/gtxsibejvu.html

[E14] URL 编码与 Base64
来源：http://hz.hfpthk.cn/gtpsxpxfsg.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.smart0.xyz/gtqkyvugji.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.shangyingyoupin.top/gtzsodjein.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.jiagoushi.top/gtrwvgoxpx.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.jqgufenzy.top/gtxwhurtfc.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.ydjk.org.cn/gtgwxbkxbe.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.xingfuxueyuan.xyz/gtylrxplsu.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.ppjwa.cn/gtloxbvobn.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.kuanghao11.cn/gtslwtpcyz.html

[E15] HTML 转义 / 反转义
来源：http://hz.cdnleiting.top/gtvxumfdof.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.guowangkeji.top/gttpozjzbl.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.gzhubu.top/gtuohaatic.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.feifeiyinyue.top/gtqhktodoo.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.fengsongda.top/gtxxhsejdr.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.hywenlv.cn/gtcxcxvidp.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.hammf.cn/gtyexeubrx.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.xingfuxueyuan.xyz/gtcxvgovmq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.xuanzx.com/gtsmxvfeas.html

[E16] 数字千分位
来源：http://hz.cashguo.top/gtgjkxghxu.html

Py:   f"{1234567:,}"
来源：http://hz.zhixingplan.top/gtcyewstpw.html

PHP:  number_format(1234567);
来源：http://hz.pengpengdd.cyou/gtfplgdxrg.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.chenzaomai.com/gtinacwzky.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.fengsongda.top/gttylkckzg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.feifeiyinyue.top/gtuocarlfn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.jinyuanbaomall.cn/gtuuwrbjzp.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.dianchejie.cn/gtpfqeewvl.html

C#:   1234567.ToString("N0")
来源：http://hz.yj202588.top/gtscwrzmca.html

[E17] 首字母大写
来源：http://hz.sxryk.cn/gtyyknlyxu.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.shanyushiyangkeji.top/gtvnudlwvp.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.316326.xyz/gtcpjnazud.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.feifeiyinyue.top/gttazcmxkt.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jinghuilouyu.cn/gtrxgasjfj.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.aizwys.cn/gtbdsembzs.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.havefunace.top/gtjofsohbp.html

Ruby: s.capitalize
来源：http://hz.andypj.xyz/gtzscyeovj.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.jqgfzy.top/gtrecqzvrd.html

[E18] 模板占位符替换
来源：http://hz.sufxvd.cn/gtsmmnfere.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.wangshuangyany.cn/gtmfaxkclr.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.9152youxi.cn/gtasqkhiem.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.0kj1m.cn/gtptidonpv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.gotoacloud.top/gtkdweqzqp.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.shanyushiyangtech.top/gtjjmxcbyd.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.redwolf501.top/gtptinqaql.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.hnxiangtu.top/gtwsllvnch.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.tianlin.xyz/gtygqczzuh.html

[E19] 多行文本按行拆分
来源：http://hz.xinyue.icu/gtvarabsst.html

Py:   s.splitlines()
来源：http://hz.chenjidiqi.icu/gtwuaqrvpn.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.xuetiantiany.cn/gtbrrqyxwt.html

JS:   s.split(/\r?\n/)
来源：http://hz.jianghu66.top/gtgrjsxyoi.html

TS:   s.split(/\r?\n/)
来源：http://hz.jlsjyb.cn/gtleaikyml.html

Java: s.lines().toList()
来源：http://hz.jiagoushi.top/gtvyefqwrs.html

Go:   strings.Split(s, "\n")
来源：http://hz.xylfe.cn/gtphhdjkog.html

Ruby: s.lines
来源：http://hz.zhengqikj.top/gtrqhbhywh.html

C#:   s.Split('\n')
来源：http://hz.hfpthk.cn/gtdoicanvc.html

[E20] 判断字符串是否为空
来源：http://hz.jyoumei.cn/gtqmkjomzc.html

Py:   if not s:
来源：http://hz.hfpthk.cn/gtzucnijvf.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.guowangkeji.top/gtyjfdwzhr.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.nanxuanxn.top/gtuephwxlt.html

TS:   if (s === "") {}
来源：http://hz.yanxiufei.cn/gtweiedpzn.html

Java: if (s.isEmpty()) {}
来源：http://hz.smart0.xyz/gtgxilybpa.html

Go:   if s == "" {}
来源：http://hz.52xcode.cn/gtssjpzrce.html

Ruby: if s.empty?
来源：http://hz.bjfxy.top/gtpegbhvru.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.xingfuxueyuan.xyz/gtbjmqgxga.html

[E21] 超长截断加省略号
来源：http://hz.zhengqikj.top/gtzuyklbxw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.cqqwz.cn/gtvpvygsqt.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.ybcxt.top/gtgfzvpubx.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.cashguo.top/gtrhctxrvs.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.gzhubu.top/gtuqyfcegv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yvedp.cn/gtulevktvq.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.havefunace.top/gtvrpsuybu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.gotoacloud.top/gteigiujbs.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.shanyushiyangtech.top/gtflmsrkig.html

[E22] 字节长度与字符长度
来源：http://hz.dashuyun.cn/gtccfnjmhw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.bjfxy.top/gtczeifdtw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.hongshengwenyu.top/gtxefjxjjo.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.quarkkingdee.top/gtjtuxbvrw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.redwolf501.top/gtdgrkklmn.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.hammf.cn/gthjsocgpd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.wangshuangyany.cn/gtlsjdsgcn.html

Ruby: s.bytesize;  s.length
来源：http://hz.yj20258.top/gtbkfgpskn.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.wangshuangyany.cn/gtysrooyjo.html

================================================================================
来源：http://hz.aizwys.cn/gtgjzntuuh.html

F. 文件与目录
来源：http://hz.hnqzz.top/gtfisafaqr.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtgfyqibxj.html

[F01] 读取整个文件
来源：http://hz.birdmap.top/gtmqisrkrj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.redwolf501.top/gthijbskcc.html

PHP:  file_get_contents("a.txt");
来源：http://hz.shangyingyoupin.top/gtguoazrqy.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.shuidangran.top/gtjrhgczsv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.andypj.xyz/gtlzxmcjuj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.xziqi.cn/gtqxbwxknf.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.shanyushiyangtech.top/gtmxsbzxpd.html

Ruby: File.read("a.txt")
来源：http://hz.jlsjyb.cn/gteuzsdzoo.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.jinyuanbaomall.cn/gtipuybdqz.html

[F02] 逐行读取文件
来源：http://hz.shanyushiyangtech.top/gtsphyiwsw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.yanxiufei.cn/gtcxbtylhz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.gotoacloud.top/gteykhmdli.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jiagoushi.top/gtocwyhiae.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yuxming.cn/gtniispezq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.yueranfly.top/gtwqovvzhy.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.316326.xyz/gthefrhuym.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.tian-w.cn/gtncomixxa.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.zhiwuduotai.top/gtvyvpeowb.html

[F03] 写入文件（覆盖）
来源：http://hz.haohaochexian.top/gtisvthnnz.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.zhiwuduotai.top/gtambrzmdy.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.daria6918.cn/gtdhxdcuat.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hongshengwenyu.top/gtaaazmole.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.mhx1999.top/gtnbdcvmyw.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.ehwqpu.com/gtbmdmajyk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.ybcxt.top/gtlslhsvki.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.haohaochexian.top/gtcreoiuvl.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.chenzaomai.com/gthyzhrdkv.html

[F04] 追加写入文件
来源：http://hz.jinghuilouyu.cn/gtpthabgdw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.birdmap.top/gtzuczajzn.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.xinyue.icu/gtxpuqyoxg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.pycfn.com/gtrvrojnyl.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhixingplan.top/gtkhzobhbv.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.yanxiufei.cn/gtbrxfaizd.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.jiagoushi.top/gtowalmuya.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.xylfe.cn/gtqtpyvskm.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.cucudq.cn/gtujizpuid.html

[F05] 判断文件或目录是否存在
来源：http://hz.mhx1999.top/gtgjsivwok.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.ehwqpu.com/gtuqvyikkn.html

PHP:  file_exists("a.txt");
来源：http://hz.dianchejie.cn/gtxtaqsenh.html

JS:   fs.existsSync("a.txt")
来源：http://hz.jinqigfzy.top/gthuikafrn.html

TS:   fs.existsSync("a.txt")
来源：http://hz.jiagoushi.top/gtxnklolhn.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.yj20258.top/gtbncimzqb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.smart0.xyz/gtcjcwyqcp.html

Ruby: File.exist?("a.txt")
来源：http://hz.guowangkeji.top/gtxnkhoxec.html

C#:   File.Exists("a.txt")
来源：http://hz.shangyingyoupin.top/gtwugrzejp.html

[F06] 删除文件
来源：http://hz.zhiwuduotai.top/gtnazdywdy.html

Py:   os.remove("a.txt")
来源：http://hz.hfpthk.cn/gtyzxaauzv.html

PHP:  unlink("a.txt");
来源：http://hz.jinghuilouyu.cn/gtaxqpzgel.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.svipenyu.cn/gttpisoryg.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.fzhhl.top/gttgiagwru.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.chenjidiqi.icu/gtzphitksg.html

Go:   os.Remove("a.txt")
来源：http://hz.cashguo.top/gtjinvyukf.html

Ruby: File.delete("a.txt")
来源：http://hz.yvedp.cn/gtibnxhuct.html

C#:   File.Delete("a.txt");
来源：http://hz.kuanghao11.cn/gtogfqqekc.html

[F07] 创建目录（含多级）
来源：http://hz.wangshuangyany.cn/gtbzcossxa.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.hfpthk.cn/gtbejtotax.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.andypj.xyz/gtnvglbsuw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.tian-w.cn/gtzdptosgg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.snrcjt.cn/gtfuupaffo.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.tian-w.cn/gtcxobndoz.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.zhoulong.xyz/gtwcfhzsov.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.meibo888.top/gtivyznvfs.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.pengpengdd.cyou/gtkntosxpy.html

[F08] 遍历目录
来源：http://hz.jinqigfzy.top/gtblkmwlxo.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.pengpengdd.cyou/gtgihfrktk.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.hfpthk.cn/gtubetvasl.html

JS:   fs.readdirSync("dir")
来源：http://hz.tanke756.top/gtloolmrho.html

TS:   fs.readdirSync("dir")
来源：http://hz.yj20258888.top/gtuyzejlhv.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.meibo888.top/gtudihpwxa.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.zycfv.cn/gtfdskoywn.html

Ruby: Dir.children("dir")
来源：http://hz.cheryme.top/gtdxfncvlr.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yuxming.cn/gtttbdcuby.html

[F09] 获取文件大小
来源：http://hz.zycfv.cn/gtllvntowq.html

Py:   os.path.getsize("a.txt")
来源：http://hz.zhijiandao.cn/gtojehdywj.html

PHP:  filesize("a.txt");
来源：http://hz.smart0.xyz/gtlwrcpuav.html

JS:   fs.statSync("a.txt").size
来源：http://hz.cucudq.cn/gtjwjpueeb.html

TS:   fs.statSync("a.txt").size
来源：http://hz.ydzc1.top/gteiavxyyj.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.zhoulong.xyz/gtisqalefq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.chenjidiqi.icu/gtodwiabzm.html

Ruby: File.size("a.txt")
来源：http://hz.hfpthk.cn/gtmabevlub.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.cucudq.cn/gteybmoney.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.hnqzz.top/gtdyppwpaq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.shanyushiyangkeji.top/gtchatcune.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.fengsongda.top/gtoufvziph.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.sysykeji.top/gtbsmuepbi.html

TS:   path.extname("a.txt")
来源：http://hz.redwolf501.top/gthdpjxjgs.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.snrcjt.cn/gtiaoooxwu.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.316326.xyz/gtdjjymamw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.ydzc1.top/gtpthmvcvv.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.zhengqikj.top/gtpzrjanwl.html

[F11] 复制与移动文件
来源：http://hz.sysykeji.top/gtyhsrnnir.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.smart0.xyz/gtoahrkyjo.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.cheryme.top/gtuayaocof.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jlsjyb.cn/gtqxtncgup.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.svipenyu.cn/gtfxkdowok.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.cheryme.top/gtohsxapnp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.ehwqpu.com/gtzjqlbzbs.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.havefunace.top/gtzesrofpl.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.dashuyun.cn/gtltbmpwnm.html

[F12] CSV 读写
来源：http://hz.bjfxy.top/gtdzqfbjiy.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.hfpthk.cn/gtddbxkfaq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.0kj1m.cn/gtmxcrzqrb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.jinqigufen.top/gtlypghsss.html

TS:   // 同上
来源：http://hz.zdqjudy.top/gtjiirdzco.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.xylfe.cn/gtdraaqhjp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.0kj1m.cn/gtluqcvlhg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.hammf.cn/gtnmnaozzb.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yj20258.top/gtooofbixg.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtgsdcyxhk.html

G. 面向对象
来源：http://hz.zhongyouzk.top/gtmukozvdk.html

================================================================================
来源：http://hz.cucudq.cn/gtjmseruil.html

[G01] 定义类
来源：http://hz.9152youxi.cn/gtdukjcsdu.html

Py:   class User: pass
来源：http://hz.cdnleiting.top/gtjbttauiv.html

PHP:  class User {}
来源：http://hz.shuidangran.top/gtgdnaxpip.html

JS:   class User {}
来源：http://hz.nwbrower.top/gtjmsixwuz.html

TS:   class User { name: string = ""; }
来源：http://hz.snrcjt.cn/gtyyzvrcbc.html

Java: class User {}
来源：http://hz.ybcxt.top/gtdesylegd.html

Go:   type User struct { Name string }
来源：http://hz.xuanzx.com/gtxqnhheqy.html

Ruby: class User; end
来源：http://hz.cqqwz.cn/gtzzlsxlwc.html

C#:   class User {}
来源：http://hz.jyoumei.cn/gtvtlognel.html

[G02] 构造函数
来源：http://hz.ywan-chungtsiang.top/gtchfphcpq.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yj202588.top/gthcrksxyp.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.guannengcc.top/gtlapbmpwo.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yuanzhike.top/gtzrnqxdgv.html

TS:   constructor(public name: string) {}
来源：http://hz.pycfn.com/gtdqgggybm.html

Java: User(String name) { this.name = name; }
来源：http://hz.zycfv.cn/gtepljuevn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.vqdsnc.cn/gteenpmyqf.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.zhengqikj.top/gttzqrhnxu.html

C#:   public User(string name) { Name = name; }
来源：http://hz.ywan-chungtsiang.top/gtzvxwmphs.html

[G03] 实例属性
来源：http://hz.yj20258.top/gtdnlafphc.html

Py:   self.name = "x"
来源：http://hz.pycfn.com/gtyuysmysr.html

PHP:  public string $name = "x";
来源：http://hz.pycfn.com/gtrjdfxxcq.html

JS:   this.name = "x";
来源：http://hz.shuidangran.top/gtjgccoumk.html

TS:   name: string = "x";
来源：http://hz.snrcjt.cn/gtwyxegwuq.html

Java: private String name;
来源：http://hz.cucudq.cn/gtlddizfjk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.pengpengdd.cyou/gtkycpzfvk.html

Ruby: @name = "x"
来源：http://hz.daxiang520.top/gtskqrsnhj.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.nwbrower.top/gtalihcehn.html

[G04] 定义方法
来源：http://hz.sweek.top/gtyomneeho.html

Py:   def greet(self): return self.name
来源：http://hz.ydzc1.top/gtkqjjnhih.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.zhijiandao.cn/gtqjqemarn.html

JS:   greet() { return this.name; }
来源：http://hz.daria6918.cn/gtcvaovktx.html

TS:   greet(): string { return this.name; }
来源：http://hz.xziqi.cn/gtbdbawfjm.html

Java: String greet() { return name; }
来源：http://hz.cheryme.top/gtavcslico.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.xylfe.cn/gtdbreggbg.html

Ruby: def greet; @name; end
来源：http://hz.hongshengwenyu.top/gtbgrcbufh.html

C#:   public string Greet() => Name;
来源：http://hz.sysykeji.top/gtxaqyrmof.html

[G05] 继承
来源：http://hz.pengpengdd.cyou/gtrloddvou.html

Py:   class Admin(User): pass
来源：http://hz.ppjwa.cn/gtaphfzyop.html

PHP:  class Admin extends User {}
来源：http://hz.xuanzx.com/gtoaodhjgu.html

JS:   class Admin extends User {}
来源：http://hz.52xcode.cn/gtzagotgvm.html

TS:   class Admin extends User {}
来源：http://hz.tianlin.xyz/gtbdlubjrg.html

Java: class Admin extends User {}
来源：http://hz.daria6918.cn/gtxwwjefvy.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.snrcjt.cn/gtneexener.html

Ruby: class Admin < User; end
来源：http://hz.gaohongyu789.top/gtlhcufgyr.html

C#:   class Admin : User {}
来源：http://hz.kuanghao11.cn/gtviuowjka.html

[G06] 重写方法
来源：http://hz.shuidangran.top/gtaujaahmb.html

Py:   def greet(self): return "admin"
来源：http://hz.shanyushiyangtech.top/gteyjrlwci.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.cqqwz.cn/gtlsctmmwo.html

JS:   greet() { return "admin"; }
来源：http://hz.zhengqikj.top/gtvfdvkjxt.html

TS:   greet(): string { return "admin"; }
来源：http://hz.kuanghao11.cn/gteibkizop.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.dianchejie.cn/gtnghmfsmx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.wangdashe.top/gtrqkvcwnu.html

Ruby: def greet; "admin"; end
来源：http://hz.nanxinkj.top/gthplnuupr.html

C#:   public override string Greet() => "admin";
来源：http://hz.nwbrower.top/gtdgweopal.html

[G07] 调用父类方法
来源：http://hz.jinqigfzy.top/gtqfebdfzl.html

Py:   super().greet()
来源：http://hz.ywan-chungtsiang.top/gtwdgdulwb.html

PHP:  parent::greet();
来源：http://hz.ydzc1.top/gtcoapcorf.html

JS:   super.greet();
来源：http://hz.vqdsnc.cn/gtjcttfkwh.html

TS:   super.greet();
来源：http://hz.bjfxy.top/gtannplzzk.html

Java: super.greet();
来源：http://hz.nwbrower.top/gtneuntxzb.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.xuanzx.com/gteukwunaa.html

Ruby: super
来源：http://hz.jlsjyb.cn/gtnjbllked.html

C#:   base.Greet();
来源：http://hz.jlsjyb.cn/gtexfuyrve.html

[G08] 静态方法与属性
来源：http://hz.shuidangran.top/gtenylbooh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zhaomingkeji.xyz/gtktqjceyi.html

PHP:  public static function f() {}
来源：http://hz.shanyushiyangkeji.top/gtqvvlbkju.html

JS:   static f() {}
来源：http://hz.mhx1999.top/gtdoyguild.html

TS:   static f(): void {}
来源：http://hz.vqdsnc.cn/gtlhdbkkzn.html

Java: static void f() {}
来源：http://hz.haohaochexian.top/gtjdvflzaj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yangfankeji.com/gtupdzbjhi.html

Ruby: def self.f; end
来源：http://hz.jqgufenzy.top/gtsnfvpphs.html

C#:   public static void F() {}
来源：http://hz.xziqi.cn/gtpzxaapwb.html

[G09] 接口 / 抽象类
来源：http://hz.quarkkingdee.top/gtjctbxmcx.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.hongshengwenyu.top/gtipmpdnqg.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yanxiufei.cn/gtzfgwupll.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.xingfuxueyuan.xyz/gtytfpzqpl.html

TS:   interface Shape { area(): number; }
来源：http://hz.meibo888.top/gtvipgnjmv.html

Java: interface Shape { double area(); }
来源：http://hz.gogol.net.cn/gtskoridbr.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.chenlongwang.top/gtilqqqjyk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.cheryme.top/gtserfrgwp.html

C#:   interface IShape { double Area(); }
来源：http://hz.cqqwz.cn/gtdsainfvl.html

[G10] 访问控制
来源：http://hz.xinyue.icu/gtovoquzdx.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.birdmap.top/gtcdwtmibn.html

PHP:  public / protected / private
来源：http://hz.iojbl.cn/gtplcxcrjw.html

JS:   #private 字段；其余公开
来源：http://hz.vqdsnc.cn/gtmhuwtxny.html


<!-- 参考信息 -->