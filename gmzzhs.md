代发 wailian999

Ruby: s.reverse
来源：http://hz.cqqwz.cn/gtabxodpel.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.yuanzhike.top/gtdzizlsum.html

[E12] 统计某字符出现次数
来源：http://hz.aizwys.cn/gttkmrqsvn.html

Py:   s.count("a")
来源：http://hz.svipenyu.cn/gtfxdusdhu.html

PHP:  substr_count($s, "a");
来源：http://hz.iojbl.cn/gtkflbbtzn.html

JS:   s.split("a").length - 1
来源：http://hz.smart0.xyz/gtslozokpk.html

TS:   s.split("a").length - 1
来源：http://hz.xylfe.cn/gtgaeccbvo.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.jqgfzy.top/gthzvtvtud.html

Go:   strings.Count(s, "a")
来源：http://hz.hongshengwenyu.top/gtftvsmtlg.html

Ruby: s.count("a")
来源：http://hz.shanyushiyangkeji.top/gtaveulmoi.html

C#:   s.Count(c => c == 'a')
来源：http://hz.sxryk.cn/gtvhumqehq.html

[E13] 逐字符遍历
来源：http://hz.nanxuanxn.top/gtzqaqxsgw.html

Py:   for ch in s: print(ch)
来源：http://hz.aibaodan.cn/gtcgbthbrx.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.svipenyu.cn/gthkfkvfot.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jyoumei.cn/gtzwmhyxyc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.quarkkingdee.top/gtlduyfcsb.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.gotoacloud.top/gtbqvmdtcg.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.dashuyun.cn/gtpddcfvwf.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.dashuyun.cn/gtiqjwnnnx.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.hysaishi.cn/gtvwzbeznt.html

[E14] URL 编码与 Base64
来源：http://hz.zhengqikj.top/gtmcnoyhjz.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.yj202588.top/gtcfbhvigj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.guannengcc.top/gtxbkueaxg.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.hfpthk.cn/gtxlzbefhu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.52xcode.cn/gtadrrtkeo.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.havefunace.top/gtqcuslwoz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.andypj.xyz/gtemkpqqkh.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.cucudq.cn/gtdwiuiuvq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.sufxvd.cn/gtladrofli.html

[E15] HTML 转义 / 反转义
来源：http://hz.chenjidiqi.icu/gtttfmhaqj.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.jiagoushi.top/gtwvynsnsc.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.zhengqikj.top/gtwlhedsml.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.jinyuanbaomall.cn/gtsjszwcrq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.yj20258888.top/gtexjtwjsy.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.hfpthk.cn/gtdlsinfpj.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.zhengqikj.top/gtpfziztcy.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.jyoumei.cn/gtnwjaosyq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.zdqjudy.top/gtcxavjswc.html

[E16] 数字千分位
来源：http://hz.chenzaomai.com/gthdjcwjbk.html

Py:   f"{1234567:,}"
来源：http://hz.hywenlv.cn/gtoksrcpyu.html

PHP:  number_format(1234567);
来源：http://hz.316326.xyz/gthmmcdaud.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhixingplan.top/gtznehcyit.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.vqdsnc.cn/gthwpglouz.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.hammf.cn/gtisoydliz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.jinyuanbaomall.cn/gtydweopwl.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.cdnleiting.top/gtiesieyfy.html

C#:   1234567.ToString("N0")
来源：http://hz.vqdsnc.cn/gtyjtbtqjc.html

[E17] 首字母大写
来源：http://hz.jqgfzy.top/gtrettgxor.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.mhx1999.top/gtjuwjfnfx.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.hfpthk.cn/gtiamvpiqt.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.shangyingyoupin.top/gtuxlvrdkt.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.gotoacloud.top/gtqvsacwsa.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.tian-w.cn/gttffiucuk.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.andypj.xyz/gthjhkpaxy.html

Ruby: s.capitalize
来源：http://hz.pycfn.com/gtfaywebvu.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yangfankeji.com/gtbwkavvkl.html

[E18] 模板占位符替换
来源：http://hz.c1oappe.top/gttmrrfgux.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.vqdsnc.cn/gtmvlbbjzf.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.yueranfly.top/gtzkwxgeks.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.jyoumei.cn/gtqcmqubzz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.vqdsnc.cn/gtwsismukt.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.yanxiufei.cn/gtigjhohso.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.cashguo.top/gtositsfmu.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.daxiang520.top/gtvwcsflsv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.jianghu66.top/gtwekulwly.html

[E19] 多行文本按行拆分
来源：http://hz.zycfv.cn/gtodxlvltp.html

Py:   s.splitlines()
来源：http://hz.xingfuxueyuan.xyz/gtmlefelac.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jiagoushi.top/gtcmlcbcdo.html

JS:   s.split(/\r?\n/)
来源：http://hz.dashuyun.cn/gtdfchsgfp.html

TS:   s.split(/\r?\n/)
来源：http://hz.cashguo.top/gtuxctgysf.html

Java: s.lines().toList()
来源：http://hz.hnxiangtu.top/gtcpodbtsn.html

Go:   strings.Split(s, "\n")
来源：http://hz.sxryk.cn/gtserxjwcq.html

Ruby: s.lines
来源：http://hz.hnxiangtu.top/gtfpexalma.html

C#:   s.Split('\n')
来源：http://hz.zhiwuduotai.top/gteviagxkm.html

[E20] 判断字符串是否为空
来源：http://hz.xziqi.cn/gtcmamdhwi.html

Py:   if not s:
来源：http://hz.zhongyouzk.top/gtaicgluwj.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.wangshuangyany.cn/gtrljlaotq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.ivvv.top/gtfsufdbqr.html

TS:   if (s === "") {}
来源：http://hz.yangfankeji.com/gtixnzvipb.html

Java: if (s.isEmpty()) {}
来源：http://hz.chenlongwang.top/gtiisjmokr.html

Go:   if s == "" {}
来源：http://hz.guowangkeji.top/gtiylpfsow.html

Ruby: if s.empty?
来源：http://hz.vqdsnc.cn/gtreoecohr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.xuanzx.com/gtvdbvieef.html

[E21] 超长截断加省略号
来源：http://hz.yuxming.cn/gtftmnfjiw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.andypj.xyz/gtvdxruxvi.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.yuxming.cn/gtwvppiosr.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.shangyingyoupin.top/gtkmisfyhd.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.tianlin.xyz/gtxfgwzqwr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.dianchejie.cn/gtemshoefw.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.shangyingyoupin.top/gtobaltnab.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.tian-w.cn/gtfgxovqvv.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.nwbrower.top/gtsdwabyzy.html

[E22] 字节长度与字符长度
来源：http://hz.shangyingyoupin.top/gtvfwjwqar.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.shangyingyoupin.top/gtojxqglze.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jinqigfzy.top/gttfzabaot.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.wangshuangyany.cn/gtjlkesonz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.smart0.xyz/gtfcfjmrie.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.daxiang520.top/gtzmbxjhmm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.bjfxy.top/gtdcuxnoqg.html

Ruby: s.bytesize;  s.length
来源：http://hz.9152youxi.cn/gthxboxyvf.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.cqqwz.cn/gtesvwutqe.html

================================================================================
来源：http://hz.fengsongda.top/gtcdukfzlh.html

F. 文件与目录
来源：http://hz.zhiwuduotai.top/gtmiygncnf.html

================================================================================
来源：http://hz.chenlongwang.top/gtbqndhwlr.html

[F01] 读取整个文件
来源：http://hz.c1oappe.top/gtrskxtgbj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.ywan-chungtsiang.top/gtskdmnvul.html

PHP:  file_get_contents("a.txt");
来源：http://hz.wangshuangyany.cn/gtxmjrhvyc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.ybcxt.top/gtxewouiyv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.tanke756.top/gtcpercelu.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.yanxiufei.cn/gtqohlamhl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.shanyushiyangkeji.top/gtbtcvhdlr.html

Ruby: File.read("a.txt")
来源：http://hz.jqgfzy.top/gtsdvfgszq.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yongpay.top/gtuybzxiwu.html

[F02] 逐行读取文件
来源：http://hz.guowangkeji.top/gtctvhwcrz.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.meibo888.top/gtbkbfxsrv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.fengsongda.top/gtfkvnsnpw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ydzc1.top/gtiznkwjex.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.gogol.net.cn/gtiwpgvnta.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.shzxlz.cn/gtmrzismgs.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.zhengqikj.top/gtcrocorhj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.nwbrower.top/gttqkoiger.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.vqdsnc.cn/gtgqbewuua.html

[F03] 写入文件（覆盖）
来源：http://hz.vqdsnc.cn/gtklujzalm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.pycfn.com/gtvmldlkli.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.yanxiufei.cn/gtxqbcytpo.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.redwolf501.top/gtinzrpdbw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.gogol.net.cn/gtlcooicmz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.52xcode.cn/gtxavjgxwv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.svipenyu.cn/gtcjzdlztv.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.quarkkingdee.top/gtngnwkqzj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.yuanzhike.top/gtgayipfku.html

[F04] 追加写入文件
来源：http://hz.shuidangran.top/gtirbizmlp.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.birdmap.top/gtggzqlrkw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.xuanzx.com/gtaavcvogl.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jlsjyb.cn/gtozlneymn.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.gaohongyu789.top/gthbstcsuw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.sufxvd.cn/gtrzvbhdnj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.wangshuangyany.cn/gtdhoshwtg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.ehwqpu.com/gteknomguh.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.xingfuxueyuan.xyz/gtnwlqcxci.html

[F05] 判断文件或目录是否存在
来源：http://hz.zdqjudy.top/gtlcpmzvvj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.zhaomingkeji.xyz/gthsktzksg.html

PHP:  file_exists("a.txt");
来源：http://hz.jqgufenzy.top/gtoixhafhj.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yonumen.top/gthdfamhyf.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zycfv.cn/gtllayziob.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.jianghu66.top/gthtntxupl.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.nwbrower.top/gtnoiwzasb.html

Ruby: File.exist?("a.txt")
来源：http://hz.xziqi.cn/gtqhiesywz.html

C#:   File.Exists("a.txt")
来源：http://hz.zdqjudy.top/gtlotrxahj.html

[F06] 删除文件
来源：http://hz.dashuyun.cn/gtaiveowrm.html

Py:   os.remove("a.txt")
来源：http://hz.52xcode.cn/gtbygqditr.html

PHP:  unlink("a.txt");
来源：http://hz.chenzaomai.com/gtnexflneo.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.jinyuanbaomall.cn/gtmlvbqrcz.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.zhongyouzk.top/gtgjdhevvc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.feifeiyinyue.top/gtajmwkqqc.html

Go:   os.Remove("a.txt")
来源：http://hz.ybcxt.top/gtboprrwis.html

Ruby: File.delete("a.txt")
来源：http://hz.aizwys.cn/gtzjwdyxnt.html

C#:   File.Delete("a.txt");
来源：http://hz.zhijiandao.cn/gtasncpebh.html

[F07] 创建目录（含多级）
来源：http://hz.bjfxy.top/gtpxzrkrer.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.fzhhl.top/gtjxbbckbe.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.pycfn.com/gterqtdwwj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhiwuduotai.top/gtlrbrrnjm.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.xuetiantiany.cn/gtkldbyrjf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.yueranfly.top/gtwcostaub.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.cucudq.cn/gtkmdofyhu.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.dashuyun.cn/gttdobdgar.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.tanke756.top/gtfanikasr.html

[F08] 遍历目录
来源：http://hz.hfpthk.cn/gtmesdqasc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.xuanzx.com/gtrnpimztl.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.ydjk.org.cn/gterwjvpid.html

JS:   fs.readdirSync("dir")
来源：http://hz.tanke756.top/gtwizgirmx.html

TS:   fs.readdirSync("dir")
来源：http://hz.hnxiangtu.top/gtcgkiioai.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.tanke756.top/gtiqowagtc.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.xuanzx.com/gtugclnxie.html

Ruby: Dir.children("dir")
来源：http://hz.zdqjudy.top/gtvgpffgjb.html

C#:   Directory.GetFiles("dir")
来源：http://hz.ivvv.top/gtprvztesh.html

[F09] 获取文件大小
来源：http://hz.zdqjudy.top/gtphsjdjka.html

Py:   os.path.getsize("a.txt")
来源：http://hz.yanxiufei.cn/gtidararir.html

PHP:  filesize("a.txt");
来源：http://hz.yvedp.cn/gtjjurnrrc.html

JS:   fs.statSync("a.txt").size
来源：http://hz.zhengqikj.top/gtagnnpnxl.html

TS:   fs.statSync("a.txt").size
来源：http://hz.zhiwuduotai.top/gtudqovpev.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.sufxvd.cn/gtteceqwky.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.shanyushiyangtech.top/gtxgmijqaj.html

Ruby: File.size("a.txt")
来源：http://hz.jyoumei.cn/gtmykmficz.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yueranfly.top/gtrqtufvie.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.jqgfzy.top/gtveoejvty.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.xinyue.icu/gtgfroqjmb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.yangfankeji.com/gtuxqwxfsd.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.shanyushiyangkeji.top/gtwjtdjtcg.html

TS:   path.extname("a.txt")
来源：http://hz.ydzc1.top/gtneluqpva.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.zhaomingkeji.xyz/gtzvjxjhoi.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.aibaodan.cn/gtyydxbcfl.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.9152youxi.cn/gtadujbhno.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.vqdsnc.cn/gtpjmgmalp.html

[F11] 复制与移动文件
来源：http://hz.vqdsnc.cn/gtgvbrgxuh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.haohaochexian.top/gtykkpfkbb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.bjfxy.top/gtleeceroa.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zdqjudy.top/gtvdiisfeg.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.nwbrower.top/gtsachphjk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.zhoulong.xyz/gtubeqnmxw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.redwolf501.top/gtdwcolipf.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.yj202588.top/gttbtxccqp.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.ppjwa.cn/gtrahhrmye.html

[F12] CSV 读写
来源：http://hz.xinyue.icu/gtzfqvqozy.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.hysaishi.cn/gtjiakggpa.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.nanxuanxn.top/gthbowvrqo.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.kuanghao11.cn/gtkzzskvak.html

TS:   // 同上
来源：http://hz.yuanzhike.top/gtzrjkrgkd.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.quarkkingdee.top/gtqzzcilmp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.chenlongwang.top/gtjelatjgg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.nanxuanxn.top/gtltjotfez.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yj202588.top/gtenlrhnij.html

================================================================================
来源：http://hz.fzhhl.top/gtlyumlhpp.html

G. 面向对象
来源：http://hz.hnqzz.top/gtgugupgnj.html

================================================================================
来源：http://hz.fengsongda.top/gtguastbav.html

[G01] 定义类
来源：http://hz.wangdashe.top/gtgvgsblfz.html

Py:   class User: pass
来源：http://hz.yvedp.cn/gtaeuarrud.html

PHP:  class User {}
来源：http://hz.0kj1m.cn/gtmrykgemj.html

JS:   class User {}
来源：http://hz.0kj1m.cn/gtlpwolcua.html

TS:   class User { name: string = ""; }
来源：http://hz.cdnleiting.top/gtqwxricyr.html

Java: class User {}
来源：http://hz.zdqjudy.top/gttmvecmmp.html

Go:   type User struct { Name string }
来源：http://hz.xingfuxueyuan.xyz/gtmvtlwmrx.html

Ruby: class User; end
来源：http://hz.jqgfzy.top/gtyvclpswm.html

C#:   class User {}
来源：http://hz.jianghu66.top/gtpdqotqda.html

[G02] 构造函数
来源：http://hz.yonumen.top/gtmazcrbch.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.nanxuanxn.top/gtemjshawf.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.jinqigufen.top/gtwporogyc.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.zhaomingkeji.xyz/gtizttlhuv.html

TS:   constructor(public name: string) {}
来源：http://hz.birdmap.top/gtgvzqmlva.html

Java: User(String name) { this.name = name; }
来源：http://hz.jiagoushi.top/gtxwzqnyjp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.shuidangran.top/gtqndjdiuj.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yueranfly.top/gtsyiarojx.html

C#:   public User(string name) { Name = name; }
来源：http://hz.hfpthk.cn/gtpxxqchae.html

[G03] 实例属性
来源：http://hz.shangyingyoupin.top/gteqyfwcwu.html

Py:   self.name = "x"
来源：http://hz.shuidangran.top/gtdjrvadlk.html

PHP:  public string $name = "x";
来源：http://hz.dashuyun.cn/gtolzxztog.html

JS:   this.name = "x";
来源：http://hz.xylfe.cn/gtwmpasfzx.html

TS:   name: string = "x";
来源：http://hz.yuxming.cn/gtdpirahxf.html

Java: private String name;
来源：http://hz.xingfuxueyuan.xyz/gtgkznegct.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.daxiang520.top/gtrdegywzp.html

Ruby: @name = "x"
来源：http://hz.gzhubu.top/gtzanwskrv.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yvedp.cn/gttpfkhtcr.html

[G04] 定义方法
来源：http://hz.hnxiangtu.top/gtnojxauyk.html

Py:   def greet(self): return self.name
来源：http://hz.ydjk.org.cn/gtpblngyzy.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.nwbrower.top/gtfgsfhlvm.html

JS:   greet() { return this.name; }
来源：http://hz.gaohongyu789.top/gtfkngywvo.html

TS:   greet(): string { return this.name; }
来源：http://hz.shanyushiyangkeji.top/gtrrmpqnfi.html

Java: String greet() { return name; }
来源：http://hz.xinyue.icu/gtldoarbta.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.ybcxt.top/gtippcuwka.html

Ruby: def greet; @name; end
来源：http://hz.mhx1999.top/gtqnzurzgw.html

C#:   public string Greet() => Name;
来源：http://hz.xuetiantiany.cn/gteypswlts.html

[G05] 继承
来源：http://hz.kuanghao11.cn/gtrsbzyump.html

Py:   class Admin(User): pass
来源：http://hz.sweek.top/gthyfopoej.html

PHP:  class Admin extends User {}
来源：http://hz.yj202588.top/gtwudtkagp.html

JS:   class Admin extends User {}
来源：http://hz.52xcode.cn/gtmmjiojhq.html

TS:   class Admin extends User {}
来源：http://hz.jyoumei.cn/gtqshokhej.html

Java: class Admin extends User {}
来源：http://hz.cqqwz.cn/gtiinfpunh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.dianchejie.cn/gtedadnjww.html

Ruby: class Admin < User; end
来源：http://hz.zhaomingkeji.xyz/gtnzbwzdvl.html

C#:   class Admin : User {}
来源：http://hz.yj202588.top/gthyuqrwbx.html

[G06] 重写方法
来源：http://hz.guowangkeji.top/gtxppuangk.html

Py:   def greet(self): return "admin"
来源：http://hz.zhaomingkeji.xyz/gttvmcppod.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.ivvv.top/gtkpeicmsr.html

JS:   greet() { return "admin"; }
来源：http://hz.cqqwz.cn/gthpgdeyuk.html

TS:   greet(): string { return "admin"; }
来源：http://hz.yj202588.top/gtgsxgwpmr.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.pycfn.com/gtmgfhucua.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.yj20258888.top/gtqtxloisb.html

Ruby: def greet; "admin"; end
来源：http://hz.fzhhl.top/gtxdiievfp.html

C#:   public override string Greet() => "admin";
来源：http://hz.shzxlz.cn/gtsvqdhqvj.html

[G07] 调用父类方法
来源：http://hz.zhijiandao.cn/gtdotnlmvz.html

Py:   super().greet()
来源：http://hz.xylfe.cn/gtiqwzompz.html

PHP:  parent::greet();
来源：http://hz.jlsjyb.cn/gtgjlokzlq.html

JS:   super.greet();
来源：http://hz.tianlin.xyz/gtjntcwkmv.html

TS:   super.greet();
来源：http://hz.zhaomingkeji.xyz/gtmxicprjy.html

Java: super.greet();
来源：http://hz.yuxming.cn/gtqxsbctxt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yangfankeji.com/gtjwmdsynl.html

Ruby: super
来源：http://hz.jinqigufen.top/gtqkqinfjl.html

C#:   base.Greet();
来源：http://hz.zhoulong.xyz/gtnxgwyknv.html

[G08] 静态方法与属性
来源：http://hz.jyoumei.cn/gtqzylqnrl.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.hnxiangtu.top/gtsnfqgfsr.html

PHP:  public static function f() {}
来源：http://hz.yj202588.top/gtiucxjvly.html

JS:   static f() {}
来源：http://hz.aibaodan.cn/gtldiflrkg.html

TS:   static f(): void {}
来源：http://hz.zhaomingkeji.xyz/gtpidxeqgr.html

Java: static void f() {}
来源：http://hz.zhiwuduotai.top/gtrufwhxqn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.xinyue.icu/gtlbnyhofa.html

Ruby: def self.f; end
来源：http://hz.cheryme.top/gtvgyunwmv.html

C#:   public static void F() {}
来源：http://hz.kuanghao11.cn/gtmhrzoyel.html

[G09] 接口 / 抽象类
来源：http://hz.sweek.top/gtrdirieto.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.cashguo.top/gtmxubddlu.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.sxryk.cn/gtjfpysaty.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.yj20258888.top/gtdwtovpgd.html

TS:   interface Shape { area(): number; }
来源：http://hz.kuanghao11.cn/gtrbrvqeyf.html

Java: interface Shape { double area(); }
来源：http://hz.zhixingplan.top/gtrjijuvva.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.aizwys.cn/gtdjzpkbzp.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.sweek.top/gtwroeowtd.html

C#:   interface IShape { double Area(); }
来源：http://hz.meibo888.top/gtivbmkals.html

[G10] 访问控制
来源：http://hz.yongpay.top/gtfuesznpa.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.9152youxi.cn/gtuhjcwitb.html

PHP:  public / protected / private
来源：http://hz.guowangkeji.top/gtgasocrpu.html

JS:   #private 字段；其余公开
来源：http://hz.aizwys.cn/gtlbhrxldq.html


<!-- 参考信息 -->