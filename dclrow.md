代发 wailian999

PHP:  substr_count($s, "a");
来源：http://hz.vqdsnc.cn/gtrbyvtwjf.html

JS:   s.split("a").length - 1
来源：http://hz.yj20258.top/gttwctkcgg.html

TS:   s.split("a").length - 1
来源：http://hz.guannengcc.top/gtebzaxlbm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.aizwys.cn/gtzcqowmdm.html

Go:   strings.Count(s, "a")
来源：http://hz.smart0.xyz/gtyzcwyyuj.html

Ruby: s.count("a")
来源：http://hz.gotoacloud.top/gtpvzujxkn.html

C#:   s.Count(c => c == 'a')
来源：http://hz.cheryme.top/gtydpskvtp.html

[E13] 逐字符遍历
来源：http://hz.yuanzhike.top/gtatatnigu.html

Py:   for ch in s: print(ch)
来源：http://hz.yvedp.cn/gtbueyumfh.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.tanke756.top/gtqubmvrzo.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ehwqpu.com/gtniihmfny.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.mhx1999.top/gtnxnnicme.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.quarkkingdee.top/gtrkkbrpci.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.svipenyu.cn/gtxhukwbcx.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.sxryk.cn/gtczzwrtyg.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.aibaodan.cn/gtfgajiduj.html

[E14] URL 编码与 Base64
来源：http://hz.bjfxy.top/gtwanyddcu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.feifeiyinyue.top/gtktbuqtxm.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.gzhubu.top/gtqqaklypx.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.xuetiantiany.cn/gtdtzaelct.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.sxryk.cn/gtaezuasgn.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.havefunace.top/gtcxukkqmp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.guannengcc.top/gtnmnzdxsn.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.ywan-chungtsiang.top/gtsdoobxmv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.cashguo.top/gtzxxkwtmq.html

[E15] HTML 转义 / 反转义
来源：http://hz.hfpthk.cn/gtbvdlfpvz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.zhaomingkeji.xyz/gtlwgnhmqi.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.aibaodan.cn/gthseakbrp.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.zhixingplan.top/gtinthvcmy.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.zhongyouzk.top/gtjlmawpnu.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.yj202588.top/gtjswilhnz.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.xuanzx.com/gtipbhlvpo.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.yvedp.cn/gtfekbvdmp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.gzhubu.top/gtqoirkjuh.html

[E16] 数字千分位
来源：http://hz.zhixingplan.top/gtimtbwxly.html

Py:   f"{1234567:,}"
来源：http://hz.xuanzx.com/gtwhaxogkr.html

PHP:  number_format(1234567);
来源：http://hz.iojbl.cn/gtkgsquhhd.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.meibo888.top/gtunwudjlh.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.cqqwz.cn/gtslbbivac.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.yonumen.top/gtwxlaompt.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.zycfv.cn/gtslrwjdiu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.yongpay.top/gtqmasccxz.html

C#:   1234567.ToString("N0")
来源：http://hz.nwbrower.top/gtmkgycult.html

[E17] 首字母大写
来源：http://hz.yongpay.top/gtigrbgfct.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.cqqwz.cn/gtbuhezisv.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.mhx1999.top/gtobxwbrrs.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.cqqwz.cn/gtbkbhbzsa.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.havefunace.top/gtcklzzbzl.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.sufxvd.cn/gtoldqxaqh.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.birdmap.top/gtmfovbute.html

Ruby: s.capitalize
来源：http://hz.tanke756.top/gtxugjatsm.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yongpay.top/gtjtkqqxnc.html

[E18] 模板占位符替换
来源：http://hz.hammf.cn/gtgvgcaolb.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.gotoacloud.top/gtefmlccbw.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.guowangkeji.top/gtbwtaqnjl.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.zdqjudy.top/gtnyuyxtxu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.jinghuilouyu.cn/gtxhsochbb.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.birdmap.top/gtscbneawx.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.shanyushiyangkeji.top/gtysvxpneb.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.shanyushiyangtech.top/gtxrllbmpp.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.jqgfzy.top/gtnemzwmkv.html

[E19] 多行文本按行拆分
来源：http://hz.snrcjt.cn/gtpucgkxlf.html

Py:   s.splitlines()
来源：http://hz.kuanghao11.cn/gtshsqvagr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.tianlin.xyz/gtsjgqpdye.html

JS:   s.split(/\r?\n/)
来源：http://hz.zhixingplan.top/gtzecamtxw.html

TS:   s.split(/\r?\n/)
来源：http://hz.tian-w.cn/gtioqzouum.html

Java: s.lines().toList()
来源：http://hz.hnqzz.top/gtktvfjkar.html

Go:   strings.Split(s, "\n")
来源：http://hz.aibaodan.cn/gtbagxrqqz.html

Ruby: s.lines
来源：http://hz.yonumen.top/gtviwlahha.html

C#:   s.Split('\n')
来源：http://hz.cashguo.top/gtclcisscc.html

[E20] 判断字符串是否为空
来源：http://hz.yueranfly.top/gtebfuixqg.html

Py:   if not s:
来源：http://hz.tanke756.top/gtnbrxxbqc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.dashuyun.cn/gtsbnihazz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.yueranfly.top/gttjysuvud.html

TS:   if (s === "") {}
来源：http://hz.iojbl.cn/gtqbbajyau.html

Java: if (s.isEmpty()) {}
来源：http://hz.yuanzhike.top/gtrujhpiab.html

Go:   if s == "" {}
来源：http://hz.fzhhl.top/gttswnbiwn.html

Ruby: if s.empty?
来源：http://hz.cheryme.top/gtjkjznimi.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.smart0.xyz/gtevlcvmtv.html

[E21] 超长截断加省略号
来源：http://hz.yongpay.top/gthvxxbctj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.9152youxi.cn/gtewtzonwd.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.yvedp.cn/gtwjdrlrms.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.pengpengdd.cyou/gtrnadiwtz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yonumen.top/gtahzfxujj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.meibo888.top/gtburjenym.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.hywenlv.cn/gtletnogmo.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.iojbl.cn/gtpsoqrqjf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.mhx1999.top/gtnkbxkqld.html

[E22] 字节长度与字符长度
来源：http://hz.haohaochexian.top/gtwbdqsmmt.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.ywan-chungtsiang.top/gtfvpgwspq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yj202588.top/gtzccciezm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.aizwys.cn/gtavstmpxx.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yj20258888.top/gtmgjpgclq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.yj20258.top/gthiokucmk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.xuanzx.com/gteaotdrko.html

Ruby: s.bytesize;  s.length
来源：http://hz.jinghuilouyu.cn/gtpmchmtxz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.andypj.xyz/gthwedddlo.html

================================================================================
来源：http://hz.jqgufenzy.top/gtkblovmno.html

F. 文件与目录
来源：http://hz.ywan-chungtsiang.top/gttnfvdbgf.html

================================================================================
来源：http://hz.sufxvd.cn/gtkvcmjtdo.html

[F01] 读取整个文件
来源：http://hz.aibaodan.cn/gtphbbgceo.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.hammf.cn/gtzsboqhqg.html

PHP:  file_get_contents("a.txt");
来源：http://hz.xuanzx.com/gtxukpdvaq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.chenlongwang.top/gtljhyahgb.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.gaohongyu789.top/gtrvuvsutm.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.snrcjt.cn/gtyaqfnbqe.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.shuidangran.top/gtqqkljkyo.html

Ruby: File.read("a.txt")
来源：http://hz.feifeiyinyue.top/gthwntciqe.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.gzhubu.top/gtrbyksqek.html

[F02] 逐行读取文件
来源：http://hz.hongshengwenyu.top/gtubnyomdk.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.shanyushiyangtech.top/gtsdhxrjzw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.fzhhl.top/gthgbtkeld.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.shanyushiyangkeji.top/gtrfearhss.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jqgfzy.top/gtynpmqhbd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.havefunace.top/gtsyinaylm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.jianghu66.top/gtibptnlvy.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.cqqwz.cn/gtaoldypic.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.nanxuanxn.top/gtgazubsak.html

[F03] 写入文件（覆盖）
来源：http://hz.kuanghao11.cn/gtynsxkwtx.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.nanxuanxn.top/gthktbqzbq.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.sxryk.cn/gtstrdslwv.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.guowangkeji.top/gtajxkgdmq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.cashguo.top/gttbzosbpg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.shuidangran.top/gtnhalgmbf.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.52xcode.cn/gtunxxgror.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.dianchejie.cn/gtxawnllgw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.havefunace.top/gtdhqrjuna.html

[F04] 追加写入文件
来源：http://hz.zhengqikj.top/gtuwupfsnn.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.xingfuxueyuan.xyz/gtjrqtbiqj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.zdqjudy.top/gtsbdraagt.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.nanxuanxn.top/gteristtcw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.nanxuanxn.top/gtwmlnqrrh.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.yuanzhike.top/gtffixpjmd.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.nanxuanxn.top/gtdzwznpgk.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.xinyue.icu/gtybdksjzf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.yonumen.top/gtdlnceptn.html

[F05] 判断文件或目录是否存在
来源：http://hz.shuidangran.top/gttdbbltjc.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.jinghuilouyu.cn/gtzhauqokx.html

PHP:  file_exists("a.txt");
来源：http://hz.jyoumei.cn/gtxsldghol.html

JS:   fs.existsSync("a.txt")
来源：http://hz.tianlin.xyz/gtmrwgefjh.html

TS:   fs.existsSync("a.txt")
来源：http://hz.aizwys.cn/gtjhzezhpm.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.52xcode.cn/gtwpfxbkbu.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.hnxiangtu.top/gtxqrrosdm.html

Ruby: File.exist?("a.txt")
来源：http://hz.wangshuangyany.cn/gthxoxlbic.html

C#:   File.Exists("a.txt")
来源：http://hz.cqqwz.cn/gtyntcrnix.html

[F06] 删除文件
来源：http://hz.guowangkeji.top/gtegqmlepc.html

Py:   os.remove("a.txt")
来源：http://hz.chenzaomai.com/gtpsmqryxv.html

PHP:  unlink("a.txt");
来源：http://hz.gaohongyu789.top/gtomivgwba.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.shuidangran.top/gtqkizcajr.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.kuanghao11.cn/gtgpvvkrsa.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.xingfuxueyuan.xyz/gtotsgqern.html

Go:   os.Remove("a.txt")
来源：http://hz.pengpengdd.cyou/gtzpkmtdmo.html

Ruby: File.delete("a.txt")
来源：http://hz.daxiang520.top/gtwnwzsexu.html

C#:   File.Delete("a.txt");
来源：http://hz.xziqi.cn/gtuwmmyzvo.html

[F07] 创建目录（含多级）
来源：http://hz.xylfe.cn/gtbsshesoh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.shangyingyoupin.top/gtuixplmwg.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.hongshengwenyu.top/gtbetonsyq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.havefunace.top/gtzbjumvho.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.gotoacloud.top/gtpcovznan.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.sufxvd.cn/gtqrvcivto.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jianghu66.top/gtzdgwnfjh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.xylfe.cn/gtbdilynmf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.jqgufenzy.top/gtnbnlnosr.html

[F08] 遍历目录
来源：http://hz.meibo888.top/gtannmmpma.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.jinghuilouyu.cn/gthwdbemci.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.daria6918.cn/gtosziixix.html

JS:   fs.readdirSync("dir")
来源：http://hz.kuanghao11.cn/gtlmnrprch.html

TS:   fs.readdirSync("dir")
来源：http://hz.yonumen.top/gtbtpcozpv.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.zhongyouzk.top/gtzgzfsijx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.guowangkeji.top/gtrftdjrby.html

Ruby: Dir.children("dir")
来源：http://hz.jqgufenzy.top/gtbvjogxhr.html

C#:   Directory.GetFiles("dir")
来源：http://hz.c1oappe.top/gtcebzexry.html

[F09] 获取文件大小
来源：http://hz.ivvv.top/gtjpbgmkla.html

Py:   os.path.getsize("a.txt")
来源：http://hz.yj20258888.top/gtrfzpzsnd.html

PHP:  filesize("a.txt");
来源：http://hz.guowangkeji.top/gtvbgkhtgc.html

JS:   fs.statSync("a.txt").size
来源：http://hz.zhengqikj.top/gtrbltinwz.html

TS:   fs.statSync("a.txt").size
来源：http://hz.nanxuanxn.top/gtmcelizei.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.nanxuanxn.top/gtvmkhbdlg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.yongpay.top/gtitbpuitm.html

Ruby: File.size("a.txt")
来源：http://hz.jqgfzy.top/gthkcpkrio.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.fengsongda.top/gtivkumshu.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.zhijiandao.cn/gtbcnblpzv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.feifeiyinyue.top/gtadbpvnqt.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.daxiang520.top/gtiejbjavs.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.9152youxi.cn/gtjazdhtnt.html

TS:   path.extname("a.txt")
来源：http://hz.mhx1999.top/gthquetzxe.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.yuanzhike.top/gtrhjwwqlh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.guannengcc.top/gtitmeihor.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.cqqwz.cn/gtvumxckec.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.fzhhl.top/gtntyjxmqf.html

[F11] 复制与移动文件
来源：http://hz.gzhubu.top/gtrrbiqylc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.kuanghao11.cn/gtrosiftsm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.sxryk.cn/gtiwnbmjit.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.nwbrower.top/gtxeaprcjw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhongyouzk.top/gtrtbjmvct.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.yj202588.top/gthcriwijj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.nanxinkj.top/gtbpfwptvk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.havefunace.top/gtsbcqxyrn.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.yueranfly.top/gtwuelegyy.html

[F12] CSV 读写
来源：http://hz.zhoulong.xyz/gtcqvtgnje.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.pycfn.com/gtcxqesife.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.tianlin.xyz/gtwspyfhai.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.fengsongda.top/gtbwyblihr.html

TS:   // 同上
来源：http://hz.sweek.top/gtkerngzgk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.52xcode.cn/gtaoeovoil.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.chenjidiqi.icu/gtaugesazc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.cdnleiting.top/gtzzfpkfct.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.gzhubu.top/gtgizbhvqd.html

================================================================================
来源：http://hz.hfpthk.cn/gtrqnhxyhb.html

G. 面向对象
来源：http://hz.hywenlv.cn/gtvfoirupx.html

================================================================================
来源：http://hz.dianchejie.cn/gtdsajksrb.html

[G01] 定义类
来源：http://hz.jinqigufen.top/gtdyvtwepi.html

Py:   class User: pass
来源：http://hz.c1oappe.top/gtryeiickq.html

PHP:  class User {}
来源：http://hz.9152youxi.cn/gtbyttghqt.html

JS:   class User {}
来源：http://hz.cashguo.top/gtnibjejlk.html

TS:   class User { name: string = ""; }
来源：http://hz.yj202588.top/gtsyfcrkpu.html

Java: class User {}
来源：http://hz.haohaochexian.top/gtkytxvubf.html

Go:   type User struct { Name string }
来源：http://hz.yanxiufei.cn/gtyknhbpmi.html

Ruby: class User; end
来源：http://hz.andypj.xyz/gthvamjzxn.html

C#:   class User {}
来源：http://hz.9152youxi.cn/gtuotjgfch.html

[G02] 构造函数
来源：http://hz.ywan-chungtsiang.top/gtorgbnwua.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yj202588.top/gtzdgbmdku.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.feifeiyinyue.top/gtozcdhtzq.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.bjfxy.top/gtekfkgvaz.html

TS:   constructor(public name: string) {}
来源：http://hz.yonumen.top/gtnnscirqw.html

Java: User(String name) { this.name = name; }
来源：http://hz.andypj.xyz/gtnhzhrsdk.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.aizwys.cn/gtuitzykac.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.mhx1999.top/gtycakarjb.html

C#:   public User(string name) { Name = name; }
来源：http://hz.xylfe.cn/gtudcvwerb.html

[G03] 实例属性
来源：http://hz.xuetiantiany.cn/gtfjadfmdo.html

Py:   self.name = "x"
来源：http://hz.birdmap.top/gtubqnojdr.html

PHP:  public string $name = "x";
来源：http://hz.guowangkeji.top/gtsfncbthh.html

JS:   this.name = "x";
来源：http://hz.tian-w.cn/gtencifnry.html

TS:   name: string = "x";
来源：http://hz.nanxinkj.top/gticzqramj.html

Java: private String name;
来源：http://hz.xziqi.cn/gticncxbqk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.bjfxy.top/gtovzagxww.html

Ruby: @name = "x"
来源：http://hz.shanyushiyangtech.top/gtdhrrersh.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.guannengcc.top/gtpvmhzhib.html

[G04] 定义方法
来源：http://hz.xylfe.cn/gtidrskmax.html

Py:   def greet(self): return self.name
来源：http://hz.jlsjyb.cn/gtpjnehqvi.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.cucudq.cn/gtzfcpmvzv.html

JS:   greet() { return this.name; }
来源：http://hz.guowangkeji.top/gtryecrbtk.html

TS:   greet(): string { return this.name; }
来源：http://hz.smart0.xyz/gtoqamjyhw.html

Java: String greet() { return name; }
来源：http://hz.zdqjudy.top/gtwccflauc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.redwolf501.top/gtyfhvqdpb.html

Ruby: def greet; @name; end
来源：http://hz.zhixingplan.top/gtyenugyrs.html

C#:   public string Greet() => Name;
来源：http://hz.sufxvd.cn/gtclhvlrzd.html

[G05] 继承
来源：http://hz.xziqi.cn/gteglqfavv.html

Py:   class Admin(User): pass
来源：http://hz.shanyushiyangtech.top/gtsmecbrsr.html

PHP:  class Admin extends User {}
来源：http://hz.iojbl.cn/gtmainracd.html

JS:   class Admin extends User {}
来源：http://hz.fzhhl.top/gtakrfoppo.html

TS:   class Admin extends User {}
来源：http://hz.shanyushiyangkeji.top/gtanrhxfxr.html

Java: class Admin extends User {}
来源：http://hz.jqgfzy.top/gthomcnfwb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.chenjidiqi.icu/gtbfwyxwdc.html

Ruby: class Admin < User; end
来源：http://hz.hysaishi.cn/gtajybstgh.html

C#:   class Admin : User {}
来源：http://hz.quarkkingdee.top/gtvyitvquk.html

[G06] 重写方法
来源：http://hz.fzhhl.top/gtyikztekv.html

Py:   def greet(self): return "admin"
来源：http://hz.52xcode.cn/gtwmrsrxda.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jinqigufen.top/gtcmpbajhk.html

JS:   greet() { return "admin"; }
来源：http://hz.snrcjt.cn/gtlkioutop.html

TS:   greet(): string { return "admin"; }
来源：http://hz.zhengqikj.top/gtlqjjqxlk.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.hongshengwenyu.top/gttmnjtrpq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.jqgufenzy.top/gtfcyfuvlz.html

Ruby: def greet; "admin"; end
来源：http://hz.jinqigfzy.top/gtkqyaadig.html

C#:   public override string Greet() => "admin";
来源：http://hz.zycfv.cn/gtzjitkhxr.html

[G07] 调用父类方法
来源：http://hz.xuanzx.com/gtokqoalpx.html

Py:   super().greet()
来源：http://hz.hysaishi.cn/gtuunlldlt.html

PHP:  parent::greet();
来源：http://hz.snrcjt.cn/gtpkymoipt.html

JS:   super.greet();
来源：http://hz.wangshuangyany.cn/gtytwdpuak.html

TS:   super.greet();
来源：http://hz.hnqzz.top/gtisxycgfq.html

Java: super.greet();
来源：http://hz.yj20258888.top/gtrnehjjhp.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.c1oappe.top/gtlgvcoltu.html

Ruby: super
来源：http://hz.0kj1m.cn/gtsbvjhaqx.html

C#:   base.Greet();
来源：http://hz.shangyingyoupin.top/gtxgbmrmcr.html

[G08] 静态方法与属性
来源：http://hz.zhiwuduotai.top/gtinpmsour.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jyoumei.cn/gtvtyggxnn.html

PHP:  public static function f() {}
来源：http://hz.sweek.top/gtugpvckef.html

JS:   static f() {}
来源：http://hz.316326.xyz/gtvvkgprsu.html

TS:   static f(): void {}
来源：http://hz.sufxvd.cn/gtasazqczs.html

Java: static void f() {}
来源：http://hz.hywenlv.cn/gthebctxuk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.hnxiangtu.top/gtovsqdeun.html

Ruby: def self.f; end
来源：http://hz.zhaomingkeji.xyz/gtnzffdaxz.html

C#:   public static void F() {}
来源：http://hz.ywan-chungtsiang.top/gtauodvfui.html

[G09] 接口 / 抽象类
来源：http://hz.gogol.net.cn/gtuvonzwwl.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.tianlin.xyz/gtknynxynw.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.gzhubu.top/gtwaoqjzvx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.hnqzz.top/gtjvjdhxue.html

TS:   interface Shape { area(): number; }
来源：http://hz.52xcode.cn/gtrkhqtljo.html

Java: interface Shape { double area(); }
来源：http://hz.pengpengdd.cyou/gtnrcwioej.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yongpay.top/gtsombihwe.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.xingfuxueyuan.xyz/gtahsriafg.html

C#:   interface IShape { double Area(); }
来源：http://hz.jianghu66.top/gtnljjndfb.html

[G10] 访问控制
来源：http://hz.yuxming.cn/gtntpxezri.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.gogol.net.cn/gtggklivsh.html

PHP:  public / protected / private
来源：http://hz.tianlin.xyz/gtgsamsyin.html

JS:   #private 字段；其余公开
来源：http://hz.andypj.xyz/gtnskfpyif.html

TS:   public / protected / private
来源：http://hz.ivvv.top/gtpaaafquk.html

Java: public / protected / private / 默认包级
来源：http://hz.guannengcc.top/gteyvvdhav.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.wangshuangyany.cn/gtauicumvu.html

Ruby: public / protected / private
来源：http://hz.snrcjt.cn/gtveohebir.html


<!-- 参考信息 -->