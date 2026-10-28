代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.smart0.xyz/gtputbdxkw.html

[E11] 反转字符串
来源：http://hz.ywan-chungtsiang.top/gtyghmufhi.html

Py:   s[::-1]
来源：http://hz.xingfuxueyuan.xyz/gtfjclmpyp.html

PHP:  strrev($s);
来源：http://hz.cdnleiting.top/gtyrgbiryb.html

JS:   [...s].reverse().join("")
来源：http://hz.hysaishi.cn/gtzlqugnyg.html

TS:   [...s].reverse().join("")
来源：http://hz.aibaodan.cn/gtuklicanb.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.hywenlv.cn/gtltzpaurm.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.andypj.xyz/gthxnzsbmr.html

Ruby: s.reverse
来源：http://hz.xuanzx.com/gtobmsnjnh.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.nwbrower.top/gtuzkucrqr.html

[E12] 统计某字符出现次数
来源：http://hz.jinyuanbaomall.cn/gtfyybyqrq.html

Py:   s.count("a")
来源：http://hz.cashguo.top/gtkonuczkd.html

PHP:  substr_count($s, "a");
来源：http://hz.cucudq.cn/gtezftsvxn.html

JS:   s.split("a").length - 1
来源：http://hz.snrcjt.cn/gtgtnygrnl.html

TS:   s.split("a").length - 1
来源：http://hz.xziqi.cn/gtzqclksyd.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.jinghuilouyu.cn/gtidljlgcn.html

Go:   strings.Count(s, "a")
来源：http://hz.cqqwz.cn/gtgvvejzir.html

Ruby: s.count("a")
来源：http://hz.9152youxi.cn/gtwzajwooh.html

C#:   s.Count(c => c == 'a')
来源：http://hz.snrcjt.cn/gtaporiwbu.html

[E13] 逐字符遍历
来源：http://hz.quarkkingdee.top/gttobvczop.html

Py:   for ch in s: print(ch)
来源：http://hz.shzxlz.cn/gtjefkmjpj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.dianchejie.cn/gtpjoglost.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.vqdsnc.cn/gtlpdgygjk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zhiwuduotai.top/gtaqqdylxq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.shzxlz.cn/gtqjgmyzix.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.fzhhl.top/gtsiosdrmg.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.chenlongwang.top/gtwtegsogu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.ydzc1.top/gtwhkfkvvx.html

[E14] URL 编码与 Base64
来源：http://hz.yuxming.cn/gtmdumnymx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.gzhubu.top/gtvgdrrfsr.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.hnxiangtu.top/gttbeivtmr.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.jinghuilouyu.cn/gtdxdwhban.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.xuetiantiany.cn/gtsmzgvvof.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.daxiang520.top/gtvzopuruy.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.havefunace.top/gtdheybnik.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.zhiwuduotai.top/gtqjvueyfr.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.ybcxt.top/gtufgxvrpd.html

[E15] HTML 转义 / 反转义
来源：http://hz.shanyushiyangkeji.top/gtmigunsad.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.andypj.xyz/gtsllhaeiu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.gogol.net.cn/gtrvorxhmj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.zhoulong.xyz/gtgwuxpxtq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.cqqwz.cn/gtgjymcxub.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.shuidangran.top/gtitdyjwkr.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.daria6918.cn/gtamddbjbe.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.bjfxy.top/gtitbhewpr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.daria6918.cn/gtpkinuzie.html

[E16] 数字千分位
来源：http://hz.yonumen.top/gtgttjpbse.html

Py:   f"{1234567:,}"
来源：http://hz.redwolf501.top/gtqadlmruy.html

PHP:  number_format(1234567);
来源：http://hz.xuanzx.com/gtwdicokam.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.jinghuilouyu.cn/gtvoqwwmrz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.wangdashe.top/gturadcwac.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.yanxiufei.cn/gtlatsycbv.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.jianghu66.top/gtopaetiyx.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.smart0.xyz/gtxlpvkoaz.html

C#:   1234567.ToString("N0")
来源：http://hz.xylfe.cn/gtrfnlsbdj.html

[E17] 首字母大写
来源：http://hz.tianlin.xyz/gtgonuseur.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.bjfxy.top/gtfrehlljy.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.nanxuanxn.top/gtohbovmsq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.316326.xyz/gtheujptxd.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhixingplan.top/gthmurgsui.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.chenlongwang.top/gtjtyudmov.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.mhx1999.top/gtpkxobpid.html

Ruby: s.capitalize
来源：http://hz.jianghu66.top/gtmghdgdoz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.sweek.top/gtwdpabdnd.html

[E18] 模板占位符替换
来源：http://hz.pengpengdd.cyou/gtsbokjsvv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.ywan-chungtsiang.top/gttkbvrqqm.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.chenlongwang.top/gtczorhgtr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.ybcxt.top/gtkwflonhg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.jinghuilouyu.cn/gtpebiknfh.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.meibo888.top/gtfzhuvlen.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.yangfankeji.com/gtunhkzdas.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.yj20258.top/gtzrsmkqny.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.yuanzhike.top/gtrjyvrjqx.html

[E19] 多行文本按行拆分
来源：http://hz.hywenlv.cn/gttsxsufle.html

Py:   s.splitlines()
来源：http://hz.9152youxi.cn/gtydfobvkg.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.hnqzz.top/gtkxrzsand.html

JS:   s.split(/\r?\n/)
来源：http://hz.ppjwa.cn/gteawupyte.html

TS:   s.split(/\r?\n/)
来源：http://hz.nanxinkj.top/gtkbiedkhe.html

Java: s.lines().toList()
来源：http://hz.svipenyu.cn/gtypgbdakw.html

Go:   strings.Split(s, "\n")
来源：http://hz.hnxiangtu.top/gtmhruapky.html

Ruby: s.lines
来源：http://hz.haohaochexian.top/gtkbaochff.html

C#:   s.Split('\n')
来源：http://hz.fzhhl.top/gtzqotqpsi.html

[E20] 判断字符串是否为空
来源：http://hz.snrcjt.cn/gtuhthzlwt.html

Py:   if not s:
来源：http://hz.zhixingplan.top/gtxdufwure.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.ivvv.top/gtfznloqig.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.sufxvd.cn/gthuvxdccu.html

TS:   if (s === "") {}
来源：http://hz.dashuyun.cn/gtxujtzybv.html

Java: if (s.isEmpty()) {}
来源：http://hz.xingfuxueyuan.xyz/gtvnfsluuy.html

Go:   if s == "" {}
来源：http://hz.iojbl.cn/gtonmrlvlo.html

Ruby: if s.empty?
来源：http://hz.hnqzz.top/gtoushtccv.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.ppjwa.cn/gtbwbbjwmd.html

[E21] 超长截断加省略号
来源：http://hz.sweek.top/gtkdxqfedf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.52xcode.cn/gtkpumspip.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.zhongyouzk.top/gtoxdthapd.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.fzhhl.top/gtkwrsqzmo.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.kuanghao11.cn/gtsmkrgrne.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.aizwys.cn/gtxzfvbqii.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.xuanzx.com/gtihsqrdrm.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.xuetiantiany.cn/gtmqgjsjjz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.ppjwa.cn/gtrykxuwki.html

[E22] 字节长度与字符长度
来源：http://hz.fzhhl.top/gtwcsouvra.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.shanyushiyangtech.top/gtajffqagi.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.nanxuanxn.top/gthhueerrl.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ywan-chungtsiang.top/gtadmqhwjd.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhengqikj.top/gtpaohflnc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.ppjwa.cn/gtsgnzvcro.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.daxiang520.top/gtbxrtmqcv.html

Ruby: s.bytesize;  s.length
来源：http://hz.nwbrower.top/gtivlnwvdw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.yj20258.top/gtmfilcmop.html

================================================================================
来源：http://hz.dashuyun.cn/gteprmeyjd.html

F. 文件与目录
来源：http://hz.iojbl.cn/gtkgzfntjg.html

================================================================================
来源：http://hz.ydjk.org.cn/gtxgatinba.html

[F01] 读取整个文件
来源：http://hz.jqgfzy.top/gtmburtjud.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.ydjk.org.cn/gtqybvjeor.html

PHP:  file_get_contents("a.txt");
来源：http://hz.xuanzx.com/gtcgjfdlmu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.316326.xyz/gthddfgdnn.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.xuanzx.com/gtnxsvmuvv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.0kj1m.cn/gtrtelldoi.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.xziqi.cn/gtsxhmpqaz.html

Ruby: File.read("a.txt")
来源：http://hz.gaohongyu789.top/gttmbgcjqj.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.tian-w.cn/gtigaolzbc.html

[F02] 逐行读取文件
来源：http://hz.yuxming.cn/gtkeyfbiag.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.jinghuilouyu.cn/gtnlcaqpjr.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.meibo888.top/gtknzksrpp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.guowangkeji.top/gtwtdwclbi.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.quarkkingdee.top/gtmoobeipj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.nanxuanxn.top/gtucktjoiv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.yuanzhike.top/gtwgmbmhim.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yanxiufei.cn/gtxakqjeea.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.jinqigufen.top/gtkvuencls.html

[F03] 写入文件（覆盖）
来源：http://hz.hongshengwenyu.top/gthzcmlnjm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.jinqigfzy.top/gtcdqftodv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.hongshengwenyu.top/gtarzdcepa.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.tianlin.xyz/gtbqoxhofz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yanxiufei.cn/gtzzmdodzu.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.daxiang520.top/gthjwaanix.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.sxryk.cn/gtncbxowkm.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.meibo888.top/gtobsfexep.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.jinqigufen.top/gtnkojtaxc.html

[F04] 追加写入文件
来源：http://hz.zhongyouzk.top/gtcdbixwjo.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.aizwys.cn/gtnbndlelc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.chenzaomai.com/gtzxwrrdrv.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.meibo888.top/gtmkooyzoa.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.cucudq.cn/gtievpzgql.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.jqgufenzy.top/gtgvjorxxf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.yangfankeji.com/gttzvsonex.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.haohaochexian.top/gtvsicvvev.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.chenjidiqi.icu/gtckguzhvf.html

[F05] 判断文件或目录是否存在
来源：http://hz.jiagoushi.top/gtqxelscqq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.tian-w.cn/gtwugriyiu.html

PHP:  file_exists("a.txt");
来源：http://hz.gogol.net.cn/gtwvkuqslb.html

JS:   fs.existsSync("a.txt")
来源：http://hz.zhijiandao.cn/gtzrhmxjpt.html

TS:   fs.existsSync("a.txt")
来源：http://hz.sxryk.cn/gtritzntsr.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.jinqigfzy.top/gtltwoxhfw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.gotoacloud.top/gtkmqhioog.html

Ruby: File.exist?("a.txt")
来源：http://hz.tian-w.cn/gtwvkfcsdd.html

C#:   File.Exists("a.txt")
来源：http://hz.feifeiyinyue.top/gtpugcdryf.html

[F06] 删除文件
来源：http://hz.hfpthk.cn/gtjmgroraf.html

Py:   os.remove("a.txt")
来源：http://hz.daxiang520.top/gtnawibsoj.html

PHP:  unlink("a.txt");
来源：http://hz.52xcode.cn/gtytvrfbhr.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.fzhhl.top/gtquacqwly.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.nwbrower.top/gtnyxpdxwu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.jianghu66.top/gtffkpzpor.html

Go:   os.Remove("a.txt")
来源：http://hz.xuetiantiany.cn/gtnhxcgzvn.html

Ruby: File.delete("a.txt")
来源：http://hz.meibo888.top/gtmrsuvzfs.html

C#:   File.Delete("a.txt");
来源：http://hz.hysaishi.cn/gttzxnkwmx.html

[F07] 创建目录（含多级）
来源：http://hz.hammf.cn/gtmcnezypw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.sxryk.cn/gtprilkgxp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.yangfankeji.com/gtxejwwapi.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.daxiang520.top/gtuazjulzf.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.vqdsnc.cn/gtciiocsiq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.haohaochexian.top/gtyaeruzsi.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jinghuilouyu.cn/gtxeqxttpe.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.hammf.cn/gtmvctqmcm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yuanzhike.top/gtjrojnnhn.html

[F08] 遍历目录
来源：http://hz.aibaodan.cn/gtiirjxlby.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.xuetiantiany.cn/gtzclkwyvm.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.yvedp.cn/gtwkazsjcn.html

JS:   fs.readdirSync("dir")
来源：http://hz.dashuyun.cn/gteexkqdgi.html

TS:   fs.readdirSync("dir")
来源：http://hz.tianlin.xyz/gtlebobsrb.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.jlsjyb.cn/gtsfkbjsnl.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.tianlin.xyz/gtteqlptqa.html

Ruby: Dir.children("dir")
来源：http://hz.hnqzz.top/gtciwinxed.html

C#:   Directory.GetFiles("dir")
来源：http://hz.dashuyun.cn/gtmpsabxyv.html

[F09] 获取文件大小
来源：http://hz.pycfn.com/gttdkbdovm.html

Py:   os.path.getsize("a.txt")
来源：http://hz.hongshengwenyu.top/gttlnzuvht.html

PHP:  filesize("a.txt");
来源：http://hz.xingfuxueyuan.xyz/gtroulhzir.html

JS:   fs.statSync("a.txt").size
来源：http://hz.sysykeji.top/gtywvgotcp.html

TS:   fs.statSync("a.txt").size
来源：http://hz.zhoulong.xyz/gtnhccqpla.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.9152youxi.cn/gtefopsnrb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.jqgufenzy.top/gtnzwlphit.html

Ruby: File.size("a.txt")
来源：http://hz.svipenyu.cn/gtsclmijtw.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.vqdsnc.cn/gtgterqrzx.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.shanyushiyangkeji.top/gtllolwjft.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.cqqwz.cn/gtauvloccj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.andypj.xyz/gtvrtndnsq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.sweek.top/gtdsxntfsp.html

TS:   path.extname("a.txt")
来源：http://hz.quarkkingdee.top/gtwepiahtt.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.yonumen.top/gtcxtduykv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.jinqigfzy.top/gtnnbrhmfb.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jinyuanbaomall.cn/gtjuozrpcm.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.hongshengwenyu.top/gtgzznvsbj.html

[F11] 复制与移动文件
来源：http://hz.shanyushiyangkeji.top/gttiuaaiwl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.daxiang520.top/gtrglljxuj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.chenjidiqi.icu/gtjvqdjddf.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.cucudq.cn/gtsckkrdap.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xuetiantiany.cn/gtyryxlikq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.hongshengwenyu.top/gtjbdqnhez.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.ivvv.top/gttgzehcze.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.jinqigfzy.top/gtzpzmcdhy.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.zhoulong.xyz/gtvmitpgls.html

[F12] CSV 读写
来源：http://hz.cheryme.top/gtejvnfcxx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.ppjwa.cn/gtvfagpuzf.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.aibaodan.cn/gtcayqsxgg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.sufxvd.cn/gtkultygel.html

TS:   // 同上
来源：http://hz.havefunace.top/gtuyhjgqus.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.zhaomingkeji.xyz/gtqeemionn.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.zhengqikj.top/gtsnvswudr.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.havefunace.top/gtbaazifjk.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yuxming.cn/gtliyobhcl.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtcldnzlol.html

G. 面向对象
来源：http://hz.feifeiyinyue.top/gtylpvibus.html

================================================================================
来源：http://hz.0kj1m.cn/gtalcvtsym.html

[G01] 定义类
来源：http://hz.ivvv.top/gtgudmgzni.html

Py:   class User: pass
来源：http://hz.9152youxi.cn/gtdwqeqjuh.html

PHP:  class User {}
来源：http://hz.hysaishi.cn/gtgrjemoli.html

JS:   class User {}
来源：http://hz.yj20258.top/gtekhhjiub.html

TS:   class User { name: string = ""; }
来源：http://hz.jianghu66.top/gtbmqzaghs.html

Java: class User {}
来源：http://hz.yongpay.top/gtxejrgilh.html

Go:   type User struct { Name string }
来源：http://hz.jianghu66.top/gtlkefinkz.html

Ruby: class User; end
来源：http://hz.sxryk.cn/gtcqtnvcso.html

C#:   class User {}
来源：http://hz.kuanghao11.cn/gtlglyiikj.html

[G02] 构造函数
来源：http://hz.yvedp.cn/gthyhawpwv.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yanxiufei.cn/gtpzlybarz.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.9152youxi.cn/gtaxzhvtcp.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.zhoulong.xyz/gtfjiuyaie.html

TS:   constructor(public name: string) {}
来源：http://hz.jinqigufen.top/gtfbolddqe.html

Java: User(String name) { this.name = name; }
来源：http://hz.zycfv.cn/gtzojsjkqu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jinghuilouyu.cn/gtrvplzvrh.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.shuidangran.top/gtagbwwydl.html

C#:   public User(string name) { Name = name; }
来源：http://hz.yonumen.top/gtdhwmspzu.html

[G03] 实例属性
来源：http://hz.yueranfly.top/gtpxodefjb.html

Py:   self.name = "x"
来源：http://hz.fengsongda.top/gtfcezggng.html

PHP:  public string $name = "x";
来源：http://hz.guowangkeji.top/gtrsmbsnua.html

JS:   this.name = "x";
来源：http://hz.jlsjyb.cn/gtuobafkdc.html

TS:   name: string = "x";
来源：http://hz.zycfv.cn/gtgrrfjprd.html

Java: private String name;
来源：http://hz.yangfankeji.com/gtqgcvlgoe.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yangfankeji.com/gtuxdewvob.html

Ruby: @name = "x"
来源：http://hz.wangshuangyany.cn/gtwwlnqpls.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.feifeiyinyue.top/gtptqehqvw.html

[G04] 定义方法
来源：http://hz.zhoulong.xyz/gtvidlapfv.html

Py:   def greet(self): return self.name
来源：http://hz.tanke756.top/gteqxzyrod.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.0kj1m.cn/gtsaoxwara.html

JS:   greet() { return this.name; }
来源：http://hz.yj20258.top/gtrwybucxa.html

TS:   greet(): string { return this.name; }
来源：http://hz.ydzc1.top/gtygjxdjof.html

Java: String greet() { return name; }
来源：http://hz.jqgfzy.top/gtrgsiquto.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.316326.xyz/gtowergdel.html

Ruby: def greet; @name; end
来源：http://hz.wangdashe.top/gtxyoysvcs.html

C#:   public string Greet() => Name;
来源：http://hz.cashguo.top/gtgqcxzfli.html

[G05] 继承
来源：http://hz.yuxming.cn/gtqwhqzguo.html

Py:   class Admin(User): pass
来源：http://hz.hammf.cn/gtulcahbli.html

PHP:  class Admin extends User {}
来源：http://hz.zhijiandao.cn/gtibdeylvd.html

JS:   class Admin extends User {}
来源：http://hz.shanyushiyangtech.top/gtzspqdler.html

TS:   class Admin extends User {}
来源：http://hz.bjfxy.top/gtwdblaolu.html

Java: class Admin extends User {}
来源：http://hz.cheryme.top/gtsvmjsqbz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.zdqjudy.top/gtgyhrdqvz.html

Ruby: class Admin < User; end
来源：http://hz.shuidangran.top/gtmqmsjvby.html

C#:   class Admin : User {}
来源：http://hz.shanyushiyangtech.top/gtwfzmcttk.html

[G06] 重写方法
来源：http://hz.fzhhl.top/gtixilafus.html

Py:   def greet(self): return "admin"
来源：http://hz.hongshengwenyu.top/gtvvmxwhvb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.wangdashe.top/gtprrlilpz.html

JS:   greet() { return "admin"; }
来源：http://hz.vqdsnc.cn/gtlztltgvs.html

TS:   greet(): string { return "admin"; }
来源：http://hz.yuanzhike.top/gtscrgpuvz.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.ehwqpu.com/gterwfumcc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.52xcode.cn/gtceyyyhbv.html

Ruby: def greet; "admin"; end
来源：http://hz.yj20258888.top/gtpnjilydh.html

C#:   public override string Greet() => "admin";
来源：http://hz.yangfankeji.com/gtnsugxgib.html

[G07] 调用父类方法
来源：http://hz.vqdsnc.cn/gtcaznpvtc.html

Py:   super().greet()
来源：http://hz.svipenyu.cn/gtneexbeop.html

PHP:  parent::greet();
来源：http://hz.zycfv.cn/gtphbharwo.html

JS:   super.greet();
来源：http://hz.pycfn.com/gthsyxzpzy.html

TS:   super.greet();
来源：http://hz.xinyue.icu/gtadtzxodp.html

Java: super.greet();
来源：http://hz.jinqigfzy.top/gticalnzfn.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.daxiang520.top/gtfywaehld.html

Ruby: super
来源：http://hz.cdnleiting.top/gtvaiomwrd.html

C#:   base.Greet();
来源：http://hz.c1oappe.top/gtidxlzydv.html

[G08] 静态方法与属性
来源：http://hz.yuxming.cn/gtmzamxseu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.pycfn.com/gtothqzsel.html

PHP:  public static function f() {}
来源：http://hz.feifeiyinyue.top/gtdgeobwxq.html

JS:   static f() {}
来源：http://hz.ehwqpu.com/gtokspfnro.html

TS:   static f(): void {}
来源：http://hz.jianghu66.top/gtgtzkjrah.html

Java: static void f() {}
来源：http://hz.nanxuanxn.top/gtzvfrhzzh.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.nwbrower.top/gtdhgkigct.html

Ruby: def self.f; end
来源：http://hz.xuanzx.com/gtkeqfwuhc.html

C#:   public static void F() {}
来源：http://hz.cqqwz.cn/gtiibtxoqw.html

[G09] 接口 / 抽象类
来源：http://hz.aibaodan.cn/gtbccidiwc.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.52xcode.cn/gtknzcmgmn.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.sweek.top/gtwrfxiobz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.chenjidiqi.icu/gtdescldss.html

TS:   interface Shape { area(): number; }
来源：http://hz.9152youxi.cn/gtklvxacpf.html


<!-- 参考信息 -->