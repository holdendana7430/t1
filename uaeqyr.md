代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://hz.hysaishi.cn/gtgzmajudn.html

Java: String.format("%03d", 7)
来源：http://hz.ydzc1.top/gtkdcfgolq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.yuxming.cn/gtglbubbrd.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.aibaodan.cn/gtgrtjoqcn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.fengsongda.top/gtvjxqzvhg.html

[E11] 反转字符串
来源：http://hz.gzhubu.top/gtnepbqrem.html

Py:   s[::-1]
来源：http://hz.yj202588.top/gtcdnyemdg.html

PHP:  strrev($s);
来源：http://hz.gzhubu.top/gtrfpntrrv.html

JS:   [...s].reverse().join("")
来源：http://hz.52xcode.cn/gtfefserje.html

TS:   [...s].reverse().join("")
来源：http://hz.yueranfly.top/gttuaabnrv.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.meibo888.top/gtbicdgrav.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.yangfankeji.com/gtvhqmcwwy.html

Ruby: s.reverse
来源：http://hz.havefunace.top/gtcyzjrzfj.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.nanxinkj.top/gtvtisrhwb.html

[E12] 统计某字符出现次数
来源：http://hz.zhongyouzk.top/gtbesyhkdy.html

Py:   s.count("a")
来源：http://hz.gaohongyu789.top/gtnyblusss.html

PHP:  substr_count($s, "a");
来源：http://hz.fengsongda.top/gttkkxdmqc.html

JS:   s.split("a").length - 1
来源：http://hz.hfpthk.cn/gtzbdyymbh.html

TS:   s.split("a").length - 1
来源：http://hz.andypj.xyz/gtgfvbdigu.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.redwolf501.top/gtasmdkfpb.html

Go:   strings.Count(s, "a")
来源：http://hz.chenlongwang.top/gtrhedxwdr.html

Ruby: s.count("a")
来源：http://hz.xuetiantiany.cn/gtukyhufny.html

C#:   s.Count(c => c == 'a')
来源：http://hz.yueranfly.top/gtvjiaywcz.html

[E13] 逐字符遍历
来源：http://hz.zycfv.cn/gtpcduzbyi.html

Py:   for ch in s: print(ch)
来源：http://hz.shanyushiyangkeji.top/gtmnbyalwg.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.gogol.net.cn/gtjmrwpvjd.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yuanzhike.top/gtcvxaxxti.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xuetiantiany.cn/gtlqiqakig.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.yongpay.top/gtrdndelny.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.feifeiyinyue.top/gtusdulhom.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.jinyuanbaomall.cn/gtdplasxva.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.guannengcc.top/gtmdtmrvwr.html

[E14] URL 编码与 Base64
来源：http://hz.pycfn.com/gtgxsnncyb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.mhx1999.top/gtyhhmhlsy.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.yuanzhike.top/gtxifivugm.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.c1oappe.top/gtlttfkwui.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.chenjidiqi.icu/gtihxhvnez.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.hywenlv.cn/gtomidzkvn.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.nanxinkj.top/gtnwsswmgf.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.dashuyun.cn/gtfoulpent.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.jinyuanbaomall.cn/gtfswptjce.html

[E15] HTML 转义 / 反转义
来源：http://hz.gogol.net.cn/gtsljqidyj.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.jinghuilouyu.cn/gtqeiyakfc.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.sysykeji.top/gtsxxvgqrk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.sufxvd.cn/gtjgejngtj.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.tanke756.top/gtngytfaip.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.daria6918.cn/gtnmyxulpe.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.chenzaomai.com/gtugnerovi.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.snrcjt.cn/gtfmszrwvx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.yj20258.top/gtmhjzavou.html

[E16] 数字千分位
来源：http://hz.xingfuxueyuan.xyz/gtuneouyvw.html

Py:   f"{1234567:,}"
来源：http://hz.snrcjt.cn/gtzaeuqrgl.html

PHP:  number_format(1234567);
来源：http://hz.gaohongyu789.top/gtqtuudyzh.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.chenlongwang.top/gtlumtpyxi.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.feifeiyinyue.top/gtiqvoalqu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.fzhhl.top/gtopsxwmqu.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.fengsongda.top/gtmrrvteyf.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.cqqwz.cn/gtdxmsuywz.html

C#:   1234567.ToString("N0")
来源：http://hz.shanyushiyangtech.top/gtrntvfkhu.html

[E17] 首字母大写
来源：http://hz.zycfv.cn/gtbvlplghi.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.guannengcc.top/gtaqoecfmq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.havefunace.top/gtcmswaylc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.cdnleiting.top/gtblhmtzkq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ydzc1.top/gtwgveimag.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.shzxlz.cn/gtkvlfdzib.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.fzhhl.top/gtdqxazkzh.html

Ruby: s.capitalize
来源：http://hz.zhengqikj.top/gtcxdehpxf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.shuidangran.top/gtjomwdwew.html

[E18] 模板占位符替换
来源：http://hz.chenlongwang.top/gtqnvvgjqw.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.ydzc1.top/gtjfkcgmme.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.cashguo.top/gtchzxckiv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.andypj.xyz/gtaofzhxnd.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.tian-w.cn/gtapzhgypp.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.mhx1999.top/gtrhqgohnt.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.wangdashe.top/gtlzpbwvgl.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.gogol.net.cn/gtyztqggtl.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.jyoumei.cn/gtgvxtsfun.html

[E19] 多行文本按行拆分
来源：http://hz.gzhubu.top/gtgaqgooug.html

Py:   s.splitlines()
来源：http://hz.sysykeji.top/gtvehrrzyr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.zhaomingkeji.xyz/gtdgbthzkq.html

JS:   s.split(/\r?\n/)
来源：http://hz.yvedp.cn/gtxinodfka.html

TS:   s.split(/\r?\n/)
来源：http://hz.chenjidiqi.icu/gtohmppmfm.html

Java: s.lines().toList()
来源：http://hz.ywan-chungtsiang.top/gtwpbnnrfv.html

Go:   strings.Split(s, "\n")
来源：http://hz.hnxiangtu.top/gtqpydvjav.html

Ruby: s.lines
来源：http://hz.sysykeji.top/gtvqdbrldf.html

C#:   s.Split('\n')
来源：http://hz.cheryme.top/gtogalpjpr.html

[E20] 判断字符串是否为空
来源：http://hz.cheryme.top/gtydzzkycp.html

Py:   if not s:
来源：http://hz.316326.xyz/gtdwohloqi.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.vqdsnc.cn/gtrrthilwl.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.jlsjyb.cn/gtemkfttth.html

TS:   if (s === "") {}
来源：http://hz.xziqi.cn/gtzutjaoyr.html

Java: if (s.isEmpty()) {}
来源：http://hz.ydjk.org.cn/gtihywzhbd.html

Go:   if s == "" {}
来源：http://hz.iojbl.cn/gtzwyyjouc.html

Ruby: if s.empty?
来源：http://hz.yongpay.top/gtugmamnad.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.jqgufenzy.top/gthsetisaj.html

[E21] 超长截断加省略号
来源：http://hz.ydzc1.top/gtahzcteuq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.zhongyouzk.top/gtegngixkw.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.ydzc1.top/gtypjksukf.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhongyouzk.top/gtazpqytwz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.fzhhl.top/gtamcedxhk.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.xingfuxueyuan.xyz/gtesdjlaff.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.yongpay.top/gtxosvzkru.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.hammf.cn/gtmwyqxpto.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.zhengqikj.top/gtbzujalrc.html

[E22] 字节长度与字符长度
来源：http://hz.0kj1m.cn/gtzxutpcuo.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.meibo888.top/gtqdrbkfqn.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.aibaodan.cn/gtpaynrhws.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hnqzz.top/gtjzhwjgpj.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.shanyushiyangtech.top/gtcbrufudl.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.fengsongda.top/gtgmyairmy.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.haohaochexian.top/gtxxqiheop.html

Ruby: s.bytesize;  s.length
来源：http://hz.aibaodan.cn/gtwrsehnzm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.daxiang520.top/gtjrtktfat.html

================================================================================
来源：http://hz.jlsjyb.cn/gtaudvvmzn.html

F. 文件与目录
来源：http://hz.guannengcc.top/gtxjrysedh.html

================================================================================
来源：http://hz.9152youxi.cn/gtpuxlzmlh.html

[F01] 读取整个文件
来源：http://hz.fzhhl.top/gtkmrfnfid.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.jinyuanbaomall.cn/gtrncerijz.html

PHP:  file_get_contents("a.txt");
来源：http://hz.hnxiangtu.top/gtxtarynmr.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.cqqwz.cn/gtoobjiyhj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.zhoulong.xyz/gtjtgnbusz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.yonumen.top/gtlqaxllmq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.cdnleiting.top/gtnawsvbkm.html

Ruby: File.read("a.txt")
来源：http://hz.bjfxy.top/gtoaomumzv.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.xuetiantiany.cn/gtsjytmdwi.html

[F02] 逐行读取文件
来源：http://hz.ywan-chungtsiang.top/gtniafqrle.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.jinqigfzy.top/gtvuzkohxk.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.chenzaomai.com/gtuahtwxyp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xuanzx.com/gtrupnattv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xuanzx.com/gtxaxljuie.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.yuxming.cn/gtbgscgidz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.shanyushiyangkeji.top/gtqbokzecv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.hfpthk.cn/gtjbjndozd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.snrcjt.cn/gtoqmumfqg.html

[F03] 写入文件（覆盖）
来源：http://hz.fengsongda.top/gtpygrqfke.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.jinqigfzy.top/gtuzdwcqff.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.shangyingyoupin.top/gtltngvncj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ybcxt.top/gtfnsmvaeh.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yj20258888.top/gttttnnnmj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.cucudq.cn/gtntmsutxf.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.shangyingyoupin.top/gtxpeqtiub.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.feifeiyinyue.top/gtfmtnkfyo.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.ywan-chungtsiang.top/gtdsgfhjrx.html

[F04] 追加写入文件
来源：http://hz.birdmap.top/gthftneuer.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yuxming.cn/gtohgbfrwu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.yj20258888.top/gtkgfbneuy.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ppjwa.cn/gtztgcmxdo.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yonumen.top/gtiixdwixk.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.yuanzhike.top/gtzeiugtno.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.bjfxy.top/gtovodiadp.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.redwolf501.top/gtkdpfuipx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.hammf.cn/gtnmlpjlpw.html

[F05] 判断文件或目录是否存在
来源：http://hz.nwbrower.top/gtupboiaaf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.jinghuilouyu.cn/gtgdaxyfrl.html

PHP:  file_exists("a.txt");
来源：http://hz.yvedp.cn/gtezkayfxu.html

JS:   fs.existsSync("a.txt")
来源：http://hz.dashuyun.cn/gtbnwwremq.html

TS:   fs.existsSync("a.txt")
来源：http://hz.c1oappe.top/gtycswzazy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.xingfuxueyuan.xyz/gtzljgrxku.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.haohaochexian.top/gtrknkvhaq.html

Ruby: File.exist?("a.txt")
来源：http://hz.xinyue.icu/gtesvbnatb.html

C#:   File.Exists("a.txt")
来源：http://hz.mhx1999.top/gtarcuahgs.html

[F06] 删除文件
来源：http://hz.ivvv.top/gtyonvgfrp.html

Py:   os.remove("a.txt")
来源：http://hz.xinyue.icu/gtfxsgmfkv.html

PHP:  unlink("a.txt");
来源：http://hz.jyoumei.cn/gthbpddnxy.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.birdmap.top/gtaksdpckj.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.chenjidiqi.icu/gtqwoepqgf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.yvedp.cn/gtcrvyramw.html

Go:   os.Remove("a.txt")
来源：http://hz.yangfankeji.com/gtihrmwpiy.html

Ruby: File.delete("a.txt")
来源：http://hz.sufxvd.cn/gtjfxmpmuf.html

C#:   File.Delete("a.txt");
来源：http://hz.xylfe.cn/gtqgsfgsuc.html

[F07] 创建目录（含多级）
来源：http://hz.bjfxy.top/gtmqtxnjuo.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.gotoacloud.top/gtshqjqjni.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.zhoulong.xyz/gtvynqzlbu.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhijiandao.cn/gtpwrbudkp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.c1oappe.top/gthzcpoaaz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.quarkkingdee.top/gtepxfcnpx.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.hongshengwenyu.top/gtopgeqsyd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.ppjwa.cn/gtlxsuzmvf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.tian-w.cn/gtumpqecva.html

[F08] 遍历目录
来源：http://hz.birdmap.top/gtsqnuclke.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.wangdashe.top/gtnltvjhgg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.redwolf501.top/gtkljdtkhx.html

JS:   fs.readdirSync("dir")
来源：http://hz.snrcjt.cn/gtvxqyeorh.html

TS:   fs.readdirSync("dir")
来源：http://hz.c1oappe.top/gtheapgump.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.cqqwz.cn/gtaqezryml.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.ywan-chungtsiang.top/gtwlirdpuh.html

Ruby: Dir.children("dir")
来源：http://hz.cqqwz.cn/gteoycojse.html

C#:   Directory.GetFiles("dir")
来源：http://hz.daxiang520.top/gtfhngvzfi.html

[F09] 获取文件大小
来源：http://hz.jqgufenzy.top/gtyswmcwvh.html

Py:   os.path.getsize("a.txt")
来源：http://hz.52xcode.cn/gtmfcmauny.html

PHP:  filesize("a.txt");
来源：http://hz.pycfn.com/gtbwvoqpst.html

JS:   fs.statSync("a.txt").size
来源：http://hz.shanyushiyangkeji.top/gtxoxlpelr.html

TS:   fs.statSync("a.txt").size
来源：http://hz.zycfv.cn/gtsaypncvf.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.meibo888.top/gtsjxymvyl.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.bjfxy.top/gtnchmumbq.html

Ruby: File.size("a.txt")
来源：http://hz.xylfe.cn/gtgcyjflze.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.pycfn.com/gtdohqpqnl.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yuanzhike.top/gtujsgtyhi.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.xziqi.cn/gtcwjrbhak.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.yuanzhike.top/gtxopwmrrx.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.nanxuanxn.top/gtebzntbty.html

TS:   path.extname("a.txt")
来源：http://hz.zhengqikj.top/gtxkzyzyst.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.jinqigfzy.top/gtcjpjuzil.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.zhongyouzk.top/gtmytbctlf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.feifeiyinyue.top/gtnsnimygw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.zhixingplan.top/gtekdrmmqm.html

[F11] 复制与移动文件
来源：http://hz.sufxvd.cn/gtuqfxudod.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.xylfe.cn/gtcgogqanh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yanxiufei.cn/gtrjwkfcxh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jianghu66.top/gtxeyefkac.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.kuanghao11.cn/gtlflbbntb.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.sufxvd.cn/gtqgsdccjv.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.cucudq.cn/gtybycvlbf.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.quarkkingdee.top/gtfwotpefb.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.smart0.xyz/gtqmyripsg.html

[F12] CSV 读写
来源：http://hz.tanke756.top/gtiegneqzm.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.zhaomingkeji.xyz/gtvaoirqwc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.gzhubu.top/gtrxkcsoba.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.sysykeji.top/gtnixihctc.html

TS:   // 同上
来源：http://hz.xingfuxueyuan.xyz/gtnbugcsvi.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.smart0.xyz/gtuptgxkry.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.cdnleiting.top/gtevczksel.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.svipenyu.cn/gttlwijbdm.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yangfankeji.com/gtioigrago.html

================================================================================
来源：http://hz.wangdashe.top/gtfammisjj.html

G. 面向对象
来源：http://hz.gaohongyu789.top/gttosnyzbu.html

================================================================================
来源：http://hz.smart0.xyz/gtoevdgzwr.html

[G01] 定义类
来源：http://hz.hammf.cn/gtcoohxhnh.html

Py:   class User: pass
来源：http://hz.chenlongwang.top/gtwwwlwklk.html

PHP:  class User {}
来源：http://hz.nanxuanxn.top/gteqawgfrz.html

JS:   class User {}
来源：http://hz.zhongyouzk.top/gtxsdiazit.html

TS:   class User { name: string = ""; }
来源：http://hz.xinyue.icu/gtgncnguaf.html

Java: class User {}
来源：http://hz.chenzaomai.com/gtgjiivgdx.html

Go:   type User struct { Name string }
来源：http://hz.cqqwz.cn/gtmwjszipm.html

Ruby: class User; end
来源：http://hz.cdnleiting.top/gtasvywypi.html

C#:   class User {}
来源：http://hz.birdmap.top/gtarxmfomg.html

[G02] 构造函数
来源：http://hz.yanxiufei.cn/gtyqjloyhu.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.hfpthk.cn/gtinyzwyct.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.zhixingplan.top/gtgrqibsyj.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.jqgufenzy.top/gtfriadcxk.html

TS:   constructor(public name: string) {}
来源：http://hz.jlsjyb.cn/gtxspknyus.html

Java: User(String name) { this.name = name; }
来源：http://hz.zhoulong.xyz/gtulyuqnud.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.gogol.net.cn/gtppuzzojm.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.jinqigfzy.top/gtduivarjk.html

C#:   public User(string name) { Name = name; }
来源：http://hz.ybcxt.top/gtkuwmqfiu.html

[G03] 实例属性
来源：http://hz.nanxinkj.top/gtlsnaoiur.html

Py:   self.name = "x"
来源：http://hz.xziqi.cn/gtyltlrgmc.html

PHP:  public string $name = "x";
来源：http://hz.hysaishi.cn/gtxmqkhgdm.html

JS:   this.name = "x";
来源：http://hz.guannengcc.top/gtcpxxplxv.html

TS:   name: string = "x";
来源：http://hz.chenlongwang.top/gtpccsonyg.html

Java: private String name;
来源：http://hz.c1oappe.top/gtbaqizmtj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.cucudq.cn/gtmoxdauiz.html

Ruby: @name = "x"
来源：http://hz.tianlin.xyz/gtexjowbwq.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.xziqi.cn/gtuvtdyipz.html

[G04] 定义方法
来源：http://hz.sxryk.cn/gtyzvyatsf.html

Py:   def greet(self): return self.name
来源：http://hz.ybcxt.top/gtptlkiltn.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yuanzhike.top/gthdunuift.html

JS:   greet() { return this.name; }
来源：http://hz.guowangkeji.top/gtvhvkcjms.html

TS:   greet(): string { return this.name; }
来源：http://hz.nwbrower.top/gtcqmentwh.html

Java: String greet() { return name; }
来源：http://hz.hammf.cn/gtqxgkpmow.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.zhixingplan.top/gtzvwatkiv.html

Ruby: def greet; @name; end
来源：http://hz.xingfuxueyuan.xyz/gtmjyffiyo.html

C#:   public string Greet() => Name;
来源：http://hz.yangfankeji.com/gtbkezzhtb.html

[G05] 继承
来源：http://hz.ywan-chungtsiang.top/gtqsoaqbbp.html

Py:   class Admin(User): pass
来源：http://hz.hfpthk.cn/gtanshhqjl.html

PHP:  class Admin extends User {}
来源：http://hz.fzhhl.top/gtiscivnds.html

JS:   class Admin extends User {}
来源：http://hz.andypj.xyz/gthvsqqfwc.html

TS:   class Admin extends User {}
来源：http://hz.xylfe.cn/gtrvyamqqt.html

Java: class Admin extends User {}
来源：http://hz.yuanzhike.top/gtkytldzvo.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.aizwys.cn/gtvfijizem.html

Ruby: class Admin < User; end
来源：http://hz.sweek.top/gtsunxxeth.html

C#:   class Admin : User {}
来源：http://hz.tian-w.cn/gtzbslhana.html

[G06] 重写方法
来源：http://hz.gaohongyu789.top/gtpfozepwk.html

Py:   def greet(self): return "admin"
来源：http://hz.sufxvd.cn/gtvvhkgpqq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.dashuyun.cn/gtijfwypwl.html

JS:   greet() { return "admin"; }
来源：http://hz.nanxinkj.top/gtupejydba.html

TS:   greet(): string { return "admin"; }
来源：http://hz.xuanzx.com/gtnrqbbxup.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.zycfv.cn/gtsykgbqyj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.andypj.xyz/gtcetehwvv.html

Ruby: def greet; "admin"; end
来源：http://hz.sxryk.cn/gtwyyhctnx.html

C#:   public override string Greet() => "admin";
来源：http://hz.pycfn.com/gtxpctmyot.html

[G07] 调用父类方法
来源：http://hz.316326.xyz/gttlrqkcfc.html

Py:   super().greet()
来源：http://hz.ybcxt.top/gtlixcosim.html

PHP:  parent::greet();
来源：http://hz.sxryk.cn/gtogkorddp.html

JS:   super.greet();
来源：http://hz.tian-w.cn/gtprzmeawy.html

TS:   super.greet();
来源：http://hz.gaohongyu789.top/gtklpodkyh.html

Java: super.greet();
来源：http://hz.fengsongda.top/gtfwxqszrn.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.hongshengwenyu.top/gtiiwcnirs.html

Ruby: super
来源：http://hz.yuxming.cn/gtbmehtvtk.html

C#:   base.Greet();
来源：http://hz.zhixingplan.top/gtcywbjwaa.html

[G08] 静态方法与属性
来源：http://hz.sxryk.cn/gtcxnvzpdp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.wangdashe.top/gtwqovqclp.html

PHP:  public static function f() {}
来源：http://hz.ehwqpu.com/gttfcxnlpc.html

JS:   static f() {}
来源：http://hz.hongshengwenyu.top/gtrhalfzpe.html

TS:   static f(): void {}
来源：http://hz.jyoumei.cn/gthbkockxj.html

Java: static void f() {}
来源：http://hz.xingfuxueyuan.xyz/gttewkypfg.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.cheryme.top/gtazhehilj.html

Ruby: def self.f; end
来源：http://hz.hfpthk.cn/gtxhkjylrl.html

C#:   public static void F() {}
来源：http://hz.snrcjt.cn/gtxajbdkhx.html

[G09] 接口 / 抽象类
来源：http://hz.chenjidiqi.icu/gtohurfujg.html


<!-- 参考信息 -->