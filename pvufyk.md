代发 wailian999

Ruby: s.reverse
来源：http://hz.ydjk.org.cn/gtigfbyzdn.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.316326.xyz/gtscxdtvip.html

[E12] 统计某字符出现次数
来源：http://hz.shuidangran.top/gtlkjkzlub.html

Py:   s.count("a")
来源：http://hz.zycfv.cn/gtmpbrjqhs.html

PHP:  substr_count($s, "a");
来源：http://hz.tian-w.cn/gtytkdayan.html

JS:   s.split("a").length - 1
来源：http://hz.pycfn.com/gtutbtdazz.html

TS:   s.split("a").length - 1
来源：http://hz.316326.xyz/gtdupqyfnc.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.chenjidiqi.icu/gtlltaqecn.html

Go:   strings.Count(s, "a")
来源：http://hz.tianlin.xyz/gtrhjvjuyt.html

Ruby: s.count("a")
来源：http://hz.snrcjt.cn/gtguklvosh.html

C#:   s.Count(c => c == 'a')
来源：http://hz.sweek.top/gtbeuyruqk.html

[E13] 逐字符遍历
来源：http://hz.daria6918.cn/gtnzllmxtq.html

Py:   for ch in s: print(ch)
来源：http://hz.quarkkingdee.top/gtpqsjhoff.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.quarkkingdee.top/gtbcgviemj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ydjk.org.cn/gtpkveuwxm.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.quarkkingdee.top/gtuvjcaneo.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.chenzaomai.com/gtzdapzvws.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.chenlongwang.top/gtmrakdvdo.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.pycfn.com/gtkojxuswl.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.316326.xyz/gtubiqctxk.html

[E14] URL 编码与 Base64
来源：http://hz.c1oappe.top/gtmaqyjgft.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.zhaomingkeji.xyz/gtpmwfjqaj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.aibaodan.cn/gtjogofdjl.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.jqgufenzy.top/gteszzwret.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.jinyuanbaomall.cn/gtpnniaxpx.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.nanxinkj.top/gtmeiglaqx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.pycfn.com/gtcbfwaulg.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.316326.xyz/gtdaaivkky.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.aibaodan.cn/gtrfbnkvmg.html

[E15] HTML 转义 / 反转义
来源：http://hz.gzhubu.top/gtccxwxfaw.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.chenlongwang.top/gtoefhsely.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.gotoacloud.top/gtzgwshroc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.shanyushiyangtech.top/gtygjwnbna.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.zycfv.cn/gtggsuavms.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.yanxiufei.cn/gtofoxgdiq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.sweek.top/gtsutehace.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.jlsjyb.cn/gtozmkrvxd.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.chenlongwang.top/gtufapmjlx.html

[E16] 数字千分位
来源：http://hz.wangdashe.top/gtbwzreioz.html

Py:   f"{1234567:,}"
来源：http://hz.yj20258888.top/gtwvhddjrn.html

PHP:  number_format(1234567);
来源：http://hz.wangshuangyany.cn/gtcpjiffni.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.iojbl.cn/gtjvyhqszn.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.0kj1m.cn/gtzuvnymux.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.316326.xyz/gtreezmcdd.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.gzhubu.top/gtsmzadnkt.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.redwolf501.top/gtkhvglqbg.html

C#:   1234567.ToString("N0")
来源：http://hz.andypj.xyz/gtgilgsowp.html

[E17] 首字母大写
来源：http://hz.ehwqpu.com/gtxyzsmjcu.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.chenjidiqi.icu/gtugnngxfs.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.ehwqpu.com/gtjaqhcola.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yj20258.top/gtkmhbwhcv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhijiandao.cn/gtjuwqvwvh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.chenzaomai.com/gtgrcfrpyy.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.jinqigfzy.top/gtpwfgdyzk.html

Ruby: s.capitalize
来源：http://hz.ivvv.top/gthrcrbqxk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.c1oappe.top/gtsoqixhox.html

[E18] 模板占位符替换
来源：http://hz.yongpay.top/gtzepwyqpj.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.shanyushiyangkeji.top/gtwnjndbck.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.ydzc1.top/gtdpaniayr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.birdmap.top/gtpoqgjjlk.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.shangyingyoupin.top/gthswmxpyi.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.zhiwuduotai.top/gtqlxaiink.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.jqgufenzy.top/gtxnfkzhal.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.aibaodan.cn/gteuzotlwi.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.ppjwa.cn/gtjsxrpxhs.html

[E19] 多行文本按行拆分
来源：http://hz.gaohongyu789.top/gtssfeabsp.html

Py:   s.splitlines()
来源：http://hz.yj202588.top/gtgwhfwbhq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.iojbl.cn/gtcjarjfig.html

JS:   s.split(/\r?\n/)
来源：http://hz.jianghu66.top/gtjczukzpy.html

TS:   s.split(/\r?\n/)
来源：http://hz.feifeiyinyue.top/gtyouxrlgv.html

Java: s.lines().toList()
来源：http://hz.hammf.cn/gtylpzoqpb.html

Go:   strings.Split(s, "\n")
来源：http://hz.9152youxi.cn/gtfwbiornx.html

Ruby: s.lines
来源：http://hz.yj202588.top/gtomjltihh.html

C#:   s.Split('\n')
来源：http://hz.haohaochexian.top/gthowsuhls.html

[E20] 判断字符串是否为空
来源：http://hz.haohaochexian.top/gtfgksdkvt.html

Py:   if not s:
来源：http://hz.yvedp.cn/gtnypdboef.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.snrcjt.cn/gtkjdwqswn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.yvedp.cn/gtlpsvcvtx.html

TS:   if (s === "") {}
来源：http://hz.zhongyouzk.top/gtincnjnoi.html

Java: if (s.isEmpty()) {}
来源：http://hz.shangyingyoupin.top/gtdcsanhgv.html

Go:   if s == "" {}
来源：http://hz.havefunace.top/gthoiaiezt.html

Ruby: if s.empty?
来源：http://hz.ywan-chungtsiang.top/gtjmwmqrew.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.tian-w.cn/gtmexszehb.html

[E21] 超长截断加省略号
来源：http://hz.dianchejie.cn/gttkttbist.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.tanke756.top/gtdzulpkal.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.xingfuxueyuan.xyz/gtnddabtwx.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.smart0.xyz/gteopijfkw.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.guowangkeji.top/gtinfljmak.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yj202588.top/gtrytlmgdm.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.smart0.xyz/gtlpkgipac.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.kuanghao11.cn/gtshpjldnl.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.shzxlz.cn/gtkcrwxiyu.html

[E22] 字节长度与字符长度
来源：http://hz.hfpthk.cn/gtyymyuyqh.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.svipenyu.cn/gtttpcrwkb.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.quarkkingdee.top/gtbgvsxivo.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.chenlongwang.top/gterivqftz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.daxiang520.top/gtihgxmhic.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.zhijiandao.cn/gtladbjlqm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.jinghuilouyu.cn/gtxowuzjnj.html

Ruby: s.bytesize;  s.length
来源：http://hz.shangyingyoupin.top/gtpokbifwu.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.hammf.cn/gtvtuqlrxo.html

================================================================================
来源：http://hz.hnxiangtu.top/gtrqrxjuof.html

F. 文件与目录
来源：http://hz.yueranfly.top/gtpuqibpgn.html

================================================================================
来源：http://hz.snrcjt.cn/gtoymkojnm.html

[F01] 读取整个文件
来源：http://hz.jqgufenzy.top/gtjkunhtyb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yvedp.cn/gtulokgojy.html

PHP:  file_get_contents("a.txt");
来源：http://hz.aibaodan.cn/gtezxzqjto.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.jqgufenzy.top/gtxfkznrvy.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.yj202588.top/gtcqssvzgq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.xziqi.cn/gtdyqgbgdn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.meibo888.top/gtwxfknhip.html

Ruby: File.read("a.txt")
来源：http://hz.yj20258.top/gtpeuylzjf.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.daria6918.cn/gtpiiiyrdo.html

[F02] 逐行读取文件
来源：http://hz.yj20258.top/gtuxblzrog.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.xziqi.cn/gtlixxkqhn.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.svipenyu.cn/gtmqcvkmtl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yvedp.cn/gtakdluaqz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.daria6918.cn/gtozwpuvnr.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.vqdsnc.cn/gtxowgvvpz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.zhiwuduotai.top/gtfixcepwq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.sysykeji.top/gtiafelvnr.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.yuanzhike.top/gtpdztewfk.html

[F03] 写入文件（覆盖）
来源：http://hz.316326.xyz/gtlrczgzmq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.9152youxi.cn/gtrzcsmarr.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.daria6918.cn/gtzsbinzam.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ywan-chungtsiang.top/gtvjtyykks.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.wangshuangyany.cn/gtmlbympok.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.hammf.cn/gtzymzloyg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.52xcode.cn/gtqmhqagby.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.gaohongyu789.top/gtpfwrpwaa.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.smart0.xyz/gtlkitbthx.html

[F04] 追加写入文件
来源：http://hz.hongshengwenyu.top/gtykhtadza.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.pengpengdd.cyou/gtamomuqfg.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.0kj1m.cn/gtagvvksgm.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.fzhhl.top/gtzrffyswy.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.snrcjt.cn/gttwimfmyt.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.shanyushiyangtech.top/gtpwsevdwm.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.guowangkeji.top/gtdcrxqcmp.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.cheryme.top/gtksnxyqek.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.guannengcc.top/gtjtzvmurs.html

[F05] 判断文件或目录是否存在
来源：http://hz.shangyingyoupin.top/gtojeymzux.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.cdnleiting.top/gtetkvjcnt.html

PHP:  file_exists("a.txt");
来源：http://hz.smart0.xyz/gtvnugopfa.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yonumen.top/gtyvcuyuge.html

TS:   fs.existsSync("a.txt")
来源：http://hz.nanxinkj.top/gtspipfxbg.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.wangshuangyany.cn/gtvcjajcqg.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.sysykeji.top/gtpnkwskth.html

Ruby: File.exist?("a.txt")
来源：http://hz.tianlin.xyz/gtkcbuoxtd.html

C#:   File.Exists("a.txt")
来源：http://hz.haohaochexian.top/gtuflhiscg.html

[F06] 删除文件
来源：http://hz.cashguo.top/gtcjmearuy.html

Py:   os.remove("a.txt")
来源：http://hz.jinyuanbaomall.cn/gttjiaobfy.html

PHP:  unlink("a.txt");
来源：http://hz.redwolf501.top/gtpmqrpiha.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.fengsongda.top/gtlcxtnmbq.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.shangyingyoupin.top/gtqhcsbahd.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.nanxinkj.top/gtvuckyudz.html

Go:   os.Remove("a.txt")
来源：http://hz.c1oappe.top/gtvxnjcrti.html

Ruby: File.delete("a.txt")
来源：http://hz.zhoulong.xyz/gtekkdgxpu.html

C#:   File.Delete("a.txt");
来源：http://hz.sweek.top/gtqqstqepk.html

[F07] 创建目录（含多级）
来源：http://hz.jinyuanbaomall.cn/gtqkovbxlu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.316326.xyz/gtplpheteu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.haohaochexian.top/gtscgoowjy.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhongyouzk.top/gtxpzrlnpi.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.dashuyun.cn/gtuhrfgmbv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.hnqzz.top/gtpjjgemli.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.hfpthk.cn/gtnubgowoi.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.hongshengwenyu.top/gtrgqjjdxf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.jinqigfzy.top/gtwqfibtwg.html

[F08] 遍历目录
来源：http://hz.andypj.xyz/gtjmkwrqbw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yj202588.top/gtkojjzapp.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.fengsongda.top/gtdjqtxthk.html

JS:   fs.readdirSync("dir")
来源：http://hz.kuanghao11.cn/gtlffgqpqn.html

TS:   fs.readdirSync("dir")
来源：http://hz.zycfv.cn/gtzhiuugvn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.yanxiufei.cn/gtcezrjnhy.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.gogol.net.cn/gtvkzmmvhz.html

Ruby: Dir.children("dir")
来源：http://hz.cqqwz.cn/gthomavitu.html

C#:   Directory.GetFiles("dir")
来源：http://hz.snrcjt.cn/gtxrascltc.html

[F09] 获取文件大小
来源：http://hz.yj20258.top/gtiloxires.html

Py:   os.path.getsize("a.txt")
来源：http://hz.zhoulong.xyz/gtjdfobgcs.html

PHP:  filesize("a.txt");
来源：http://hz.xuanzx.com/gttlecwnvz.html

JS:   fs.statSync("a.txt").size
来源：http://hz.xuetiantiany.cn/gttbmcycfk.html

TS:   fs.statSync("a.txt").size
来源：http://hz.0kj1m.cn/gtncijlwgt.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.kuanghao11.cn/gtvfjfhkjl.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.jyoumei.cn/gtutoqejyq.html

Ruby: File.size("a.txt")
来源：http://hz.xuetiantiany.cn/gtuiultpsh.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.zhijiandao.cn/gtszxvtkpv.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yj20258888.top/gtqzipqqwv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.tianlin.xyz/gthffaccaa.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.jiagoushi.top/gtmwribbqk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.daxiang520.top/gtieagvnec.html

TS:   path.extname("a.txt")
来源：http://hz.zhixingplan.top/gttokxiksd.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.jinyuanbaomall.cn/gtiyurddkh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.guannengcc.top/gtrtxdfoyy.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.feifeiyinyue.top/gtqvxydhmb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.ybcxt.top/gtqnucwofe.html

[F11] 复制与移动文件
来源：http://hz.svipenyu.cn/gtzycmpsmi.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.dianchejie.cn/gtyaseojld.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.vqdsnc.cn/gthdwldyyk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.snrcjt.cn/gtwqzjzpxi.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.meibo888.top/gthmtutnrv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.jinghuilouyu.cn/gtwjlujiyp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.chenlongwang.top/gtzsjmexfh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.haohaochexian.top/gttzfsgtqf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.yj20258.top/gtsramiiqw.html

[F12] CSV 读写
来源：http://hz.cucudq.cn/gtdlczyras.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.ywan-chungtsiang.top/gtdvmqgujj.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.yuxming.cn/gtpbdnbsfq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.0kj1m.cn/gtlzrnnayv.html

TS:   // 同上
来源：http://hz.jqgfzy.top/gtoxkseqyv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.dianchejie.cn/gtcjztlrih.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.9152youxi.cn/gtyfjkehvn.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.quarkkingdee.top/gtraporlxx.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.birdmap.top/gtvtqxbbef.html

================================================================================
来源：http://hz.52xcode.cn/gttoejexbf.html

G. 面向对象
来源：http://hz.hammf.cn/gtqblycmvj.html

================================================================================
来源：http://hz.havefunace.top/gtkqoztvmc.html

[G01] 定义类
来源：http://hz.yonumen.top/gtbedosjqc.html

Py:   class User: pass
来源：http://hz.daria6918.cn/gtxqebhuoa.html

PHP:  class User {}
来源：http://hz.nwbrower.top/gtenretscr.html

JS:   class User {}
来源：http://hz.hongshengwenyu.top/gtsjhdfadc.html

TS:   class User { name: string = ""; }
来源：http://hz.jiagoushi.top/gtrzthghqo.html

Java: class User {}
来源：http://hz.shanyushiyangtech.top/gtoydmozcg.html

Go:   type User struct { Name string }
来源：http://hz.hywenlv.cn/gttqnkxblu.html

Ruby: class User; end
来源：http://hz.havefunace.top/gtbqayzxbx.html

C#:   class User {}
来源：http://hz.xziqi.cn/gttfnxpwcr.html

[G02] 构造函数
来源：http://hz.chenlongwang.top/gtsdakddpl.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.hysaishi.cn/gtquabgyku.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.bjfxy.top/gtzbsfkiyv.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.shanyushiyangtech.top/gtuhjfrylu.html

TS:   constructor(public name: string) {}
来源：http://hz.shzxlz.cn/gtichesqfp.html

Java: User(String name) { this.name = name; }
来源：http://hz.jqgufenzy.top/gtktzmagvd.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.dashuyun.cn/gtvgohavwr.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.xinyue.icu/gtkuadflxw.html

C#:   public User(string name) { Name = name; }
来源：http://hz.nwbrower.top/gtaeqltpuk.html

[G03] 实例属性
来源：http://hz.nanxinkj.top/gtygwwbkpc.html

Py:   self.name = "x"
来源：http://hz.shangyingyoupin.top/gtydttcvpf.html

PHP:  public string $name = "x";
来源：http://hz.xuanzx.com/gtbxiqhynx.html

JS:   this.name = "x";
来源：http://hz.shanyushiyangkeji.top/gtciaelxdu.html

TS:   name: string = "x";
来源：http://hz.yanxiufei.cn/gtfitorjzb.html

Java: private String name;
来源：http://hz.yongpay.top/gtduydsnds.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.birdmap.top/gtypdzbbph.html

Ruby: @name = "x"
来源：http://hz.xinyue.icu/gtksvwjxch.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.gaohongyu789.top/gtymjjavkh.html

[G04] 定义方法
来源：http://hz.chenzaomai.com/gtzwjflemp.html

Py:   def greet(self): return self.name
来源：http://hz.jqgufenzy.top/gtnhknqtbz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.ehwqpu.com/gtplqpunne.html

JS:   greet() { return this.name; }
来源：http://hz.cqqwz.cn/gtvihdjzcu.html

TS:   greet(): string { return this.name; }
来源：http://hz.shanyushiyangkeji.top/gtxmshqxbo.html

Java: String greet() { return name; }
来源：http://hz.cqqwz.cn/gtalfnfuya.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.yuanzhike.top/gtuxywtkhl.html

Ruby: def greet; @name; end
来源：http://hz.yuxming.cn/gteglxhrns.html

C#:   public string Greet() => Name;
来源：http://hz.snrcjt.cn/gttkuxdxfc.html

[G05] 继承
来源：http://hz.redwolf501.top/gtgshrgqmw.html

Py:   class Admin(User): pass
来源：http://hz.sxryk.cn/gthgefwkai.html

PHP:  class Admin extends User {}
来源：http://hz.fengsongda.top/gtflyfmcha.html

JS:   class Admin extends User {}
来源：http://hz.ivvv.top/gtkyrumvpj.html

TS:   class Admin extends User {}
来源：http://hz.havefunace.top/gtizjzyrxy.html

Java: class Admin extends User {}
来源：http://hz.daxiang520.top/gtgmxmtesd.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.ybcxt.top/gtaxzlbbbw.html

Ruby: class Admin < User; end
来源：http://hz.cdnleiting.top/gtfczzidvq.html

C#:   class Admin : User {}
来源：http://hz.shzxlz.cn/gturoqktfq.html

[G06] 重写方法
来源：http://hz.yj202588.top/gtekhelqwv.html

Py:   def greet(self): return "admin"
来源：http://hz.ybcxt.top/gtmbhncjtv.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.ydjk.org.cn/gtbvtibnuw.html

JS:   greet() { return "admin"; }
来源：http://hz.cheryme.top/gtjejngrza.html

TS:   greet(): string { return "admin"; }
来源：http://hz.zhijiandao.cn/gtdcxtabuq.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.wangshuangyany.cn/gtddyfqjqc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.cucudq.cn/gtcnhscurr.html

Ruby: def greet; "admin"; end
来源：http://hz.c1oappe.top/gtgwgqmghb.html

C#:   public override string Greet() => "admin";
来源：http://hz.fzhhl.top/gtalcqsewn.html

[G07] 调用父类方法
来源：http://hz.cdnleiting.top/gthdiqlplj.html

Py:   super().greet()
来源：http://hz.zhijiandao.cn/gtnissykkj.html

PHP:  parent::greet();
来源：http://hz.daria6918.cn/gtqvkijyge.html

JS:   super.greet();
来源：http://hz.jinyuanbaomall.cn/gtxghyigoh.html

TS:   super.greet();
来源：http://hz.ivvv.top/gthmlaeods.html

Java: super.greet();
来源：http://hz.jinyuanbaomall.cn/gtmunfdrrt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.zhixingplan.top/gtnfhumwgu.html

Ruby: super
来源：http://hz.52xcode.cn/gtjthhrsmc.html

C#:   base.Greet();
来源：http://hz.yongpay.top/gtgzijlzzx.html

[G08] 静态方法与属性
来源：http://hz.jinghuilouyu.cn/gtmoykmqrt.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.ydzc1.top/gtoaswmwkk.html

PHP:  public static function f() {}
来源：http://hz.xinyue.icu/gtcyozzjks.html

JS:   static f() {}
来源：http://hz.snrcjt.cn/gtllyhcwgu.html

TS:   static f(): void {}
来源：http://hz.tianlin.xyz/gtpzklioph.html

Java: static void f() {}
来源：http://hz.52xcode.cn/gtkofffvno.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.feifeiyinyue.top/gtsghquxtf.html

Ruby: def self.f; end
来源：http://hz.jinqigufen.top/gtardwqkza.html

C#:   public static void F() {}
来源：http://hz.gotoacloud.top/gtiboxuysu.html

[G09] 接口 / 抽象类
来源：http://hz.xuanzx.com/gtzjdntcsw.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.sxryk.cn/gtypckiyuj.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.316326.xyz/gtbwfxyeaw.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.jqgufenzy.top/gttlxnhxxx.html

TS:   interface Shape { area(): number; }
来源：http://hz.cqqwz.cn/gtnzetmevt.html

Java: interface Shape { double area(); }
来源：http://hz.9152youxi.cn/gtwwhkrgas.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.tanke756.top/gtmgaglbsb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.tian-w.cn/gtvsprpmkz.html

C#:   interface IShape { double Area(); }
来源：http://hz.tanke756.top/gtkervslud.html

[G10] 访问控制
来源：http://hz.yvedp.cn/gtclhravec.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.mhx1999.top/gtjtlmrbvf.html

PHP:  public / protected / private
来源：http://hz.yanxiufei.cn/gtrppxkgzr.html

JS:   #private 字段；其余公开
来源：http://hz.nanxuanxn.top/gtrpoyfbay.html


<!-- 参考信息 -->