代发 wailian999

Ruby: s.reverse
来源：http://hz.quarkkingdee.top/gtuxkxdtlw.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.gotoacloud.top/gtvswkciui.html

[E12] 统计某字符出现次数
来源：http://hz.hnxiangtu.top/gtwnkzxemd.html

Py:   s.count("a")
来源：http://hz.fengsongda.top/gthskyayem.html

PHP:  substr_count($s, "a");
来源：http://hz.jianghu66.top/gtltziychz.html

JS:   s.split("a").length - 1
来源：http://hz.ydzc1.top/gtfsuzkgyc.html

TS:   s.split("a").length - 1
来源：http://hz.yanxiufei.cn/gtaxlgmkrc.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.hfpthk.cn/gtuadovvfc.html

Go:   strings.Count(s, "a")
来源：http://hz.xinyue.icu/gtcjekzhxf.html

Ruby: s.count("a")
来源：http://hz.52xcode.cn/gtxbvmvrfn.html

C#:   s.Count(c => c == 'a')
来源：http://hz.smart0.xyz/gtlgnduqnj.html

[E13] 逐字符遍历
来源：http://hz.jqgufenzy.top/gtjkcqlxtj.html

Py:   for ch in s: print(ch)
来源：http://hz.mhx1999.top/gtwukwqrtw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.yonumen.top/gtznphpixb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xuetiantiany.cn/gtpgizxpya.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.chenlongwang.top/gtkajwjsvz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.ybcxt.top/gtxrisowst.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.hfpthk.cn/gttmgupkuw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.zhoulong.xyz/gtjlhoapqb.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.zhengqikj.top/gtidbihyij.html

[E14] URL 编码与 Base64
来源：http://hz.ppjwa.cn/gtrqscllas.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.fengsongda.top/gtvwbljnlx.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.cqqwz.cn/gtxsutkzhw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.aizwys.cn/gtgurvpukz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.wangdashe.top/gthfqfzqyd.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.jqgfzy.top/gtomjseish.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.jianghu66.top/gtibsacoot.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.havefunace.top/gthcpmgaor.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.wangdashe.top/gtaeasefwk.html

[E15] HTML 转义 / 反转义
来源：http://hz.sysykeji.top/gtnoqwrpwh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.mhx1999.top/gtfelzgsxy.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.daria6918.cn/gtanniljmt.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.aibaodan.cn/gtdktpzmks.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.pengpengdd.cyou/gtvzxdnkqr.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.yvedp.cn/gtdgilhpwb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.fengsongda.top/gttpemigkv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.jyoumei.cn/gtnvdbkitm.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.meibo888.top/gtzzgzaumm.html

[E16] 数字千分位
来源：http://hz.52xcode.cn/gtsoaqdluh.html

Py:   f"{1234567:,}"
来源：http://hz.chenlongwang.top/gtfxfulhig.html

PHP:  number_format(1234567);
来源：http://hz.jinyuanbaomall.cn/gtmjdpfeny.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.ydjk.org.cn/gtzrslglrr.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.wangshuangyany.cn/gtspxfjinr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.jlsjyb.cn/gtvlxcpnuu.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.hnxiangtu.top/gtrgwiudby.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.zhijiandao.cn/gttuatacaq.html

C#:   1234567.ToString("N0")
来源：http://hz.jinqigufen.top/gteetxhznl.html

[E17] 首字母大写
来源：http://hz.ybcxt.top/gtolvnumxk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.jyoumei.cn/gtovmxzjyt.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.0kj1m.cn/gtrtsqplsp.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.guannengcc.top/gtcbraubiu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.hongshengwenyu.top/gtfwmdvdyb.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.yuxming.cn/gtsewdthou.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.meibo888.top/gtmxglswnu.html

Ruby: s.capitalize
来源：http://hz.chenzaomai.com/gtwjuiudcz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.pycfn.com/gtitpodije.html

[E18] 模板占位符替换
来源：http://hz.xingfuxueyuan.xyz/gtqxwujrpy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.ehwqpu.com/gtalrigcef.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.yj20258888.top/gtvbaaopbu.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.cheryme.top/gtbxslyenc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.xuanzx.com/gtxewwkdcr.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.jinghuilouyu.cn/gtzwsdvjhd.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.wangshuangyany.cn/gtldsparqh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.yuxming.cn/gtuhrstpot.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.zhiwuduotai.top/gtkcogucsw.html

[E19] 多行文本按行拆分
来源：http://hz.birdmap.top/gtbrwthfbm.html

Py:   s.splitlines()
来源：http://hz.meibo888.top/gthtffyrcw.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.fengsongda.top/gtdwwvhamo.html

JS:   s.split(/\r?\n/)
来源：http://hz.ppjwa.cn/gtlcbaogkn.html

TS:   s.split(/\r?\n/)
来源：http://hz.zycfv.cn/gtgbufayad.html

Java: s.lines().toList()
来源：http://hz.yangfankeji.com/gthnrehtzl.html

Go:   strings.Split(s, "\n")
来源：http://hz.jianghu66.top/gtqnfwieiq.html

Ruby: s.lines
来源：http://hz.shzxlz.cn/gtyotqyxjr.html

C#:   s.Split('\n')
来源：http://hz.0kj1m.cn/gtsbjokxvu.html

[E20] 判断字符串是否为空
来源：http://hz.gzhubu.top/gtvarykqec.html

Py:   if not s:
来源：http://hz.jiagoushi.top/gttgcpcwfv.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.zhoulong.xyz/gtysajyzzr.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.chenlongwang.top/gtgalfukmg.html

TS:   if (s === "") {}
来源：http://hz.nanxinkj.top/gtnxmqsaow.html

Java: if (s.isEmpty()) {}
来源：http://hz.xinyue.icu/gtigbkevya.html

Go:   if s == "" {}
来源：http://hz.yj202588.top/gtvwqqpsow.html

Ruby: if s.empty?
来源：http://hz.shanyushiyangkeji.top/gtalmjvdvp.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.bjfxy.top/gtyfxspgcn.html

[E21] 超长截断加省略号
来源：http://hz.aibaodan.cn/gteolpcyvp.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.quarkkingdee.top/gtliynzrdz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.sweek.top/gtfjlsdsbw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.chenzaomai.com/gtotrjklaa.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.haohaochexian.top/gtmzjnasbu.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.redwolf501.top/gthdwhguvw.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.aizwys.cn/gtbaxfvjkq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.jinqigfzy.top/gttgtriykj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.xziqi.cn/gtojzijbxk.html

[E22] 字节长度与字符长度
来源：http://hz.hnxiangtu.top/gtipmtmolp.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.jinghuilouyu.cn/gtyrzhdueh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jinqigufen.top/gtfawpoihc.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yuanzhike.top/gtpnfzosax.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jyoumei.cn/gtistzcica.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.feifeiyinyue.top/gtrtrqsncg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.yj202588.top/gtyuqwfern.html

Ruby: s.bytesize;  s.length
来源：http://hz.hywenlv.cn/gtbyitvhpf.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.316326.xyz/gtfakkldfb.html

================================================================================
来源：http://hz.yj20258888.top/gtmovczzjg.html

F. 文件与目录
来源：http://hz.zhoulong.xyz/gtpxqeviaj.html

================================================================================
来源：http://hz.dianchejie.cn/gtimrgexck.html

[F01] 读取整个文件
来源：http://hz.shuidangran.top/gttylfwqci.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.hammf.cn/gtvzedtwnp.html

PHP:  file_get_contents("a.txt");
来源：http://hz.0kj1m.cn/gtgjcxqmrr.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.iojbl.cn/gtxsacuhrk.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.9152youxi.cn/gtyqgjjtqt.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.redwolf501.top/gtpfgovmwr.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.xuanzx.com/gtxqxogrkr.html

Ruby: File.read("a.txt")
来源：http://hz.bjfxy.top/gtylnvsycl.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.zhongyouzk.top/gtpwkxfhas.html

[F02] 逐行读取文件
来源：http://hz.shanyushiyangtech.top/gtaoylzmbg.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.sysykeji.top/gteynfavfm.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.jiagoushi.top/gtudrjglml.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.aizwys.cn/gtxfusbegs.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zycfv.cn/gteytwpzye.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.sxryk.cn/gtonnwmkqk.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.yueranfly.top/gtkjysozii.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yueranfly.top/gtulszuuzg.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.hnqzz.top/gtyisbmirz.html

[F03] 写入文件（覆盖）
来源：http://hz.fengsongda.top/gtnaczetbv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.sufxvd.cn/gtljwfcari.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.zhiwuduotai.top/gtkxkwzeuw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.cashguo.top/gtcchnwvns.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.wangshuangyany.cn/gtwwmfaxfl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.xuetiantiany.cn/gtlgchebib.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.zhixingplan.top/gthalmzugn.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.cqqwz.cn/gtnzrntqub.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.hfpthk.cn/gtzisbvqtb.html

[F04] 追加写入文件
来源：http://hz.yongpay.top/gtmopyogaf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.jinqigfzy.top/gtkhoyyyqk.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.zhijiandao.cn/gteoxiumyr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.xinyue.icu/gtvvtkumju.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.hnxiangtu.top/gtjzwuiyue.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.yangfankeji.com/gtxubdvdrl.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.dianchejie.cn/gtrpcxstnv.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.ehwqpu.com/gtiwrqbljs.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.yj20258.top/gtjgwoxppa.html

[F05] 判断文件或目录是否存在
来源：http://hz.aizwys.cn/gthrqiswqm.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.yuxming.cn/gtnjgmvfjy.html

PHP:  file_exists("a.txt");
来源：http://hz.vqdsnc.cn/gtmslekdtv.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yangfankeji.com/gtfqavybax.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zycfv.cn/gtymussszv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.sweek.top/gtzylkaxqk.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.gzhubu.top/gtfeijljji.html

Ruby: File.exist?("a.txt")
来源：http://hz.yvedp.cn/gtewdqtkjt.html

C#:   File.Exists("a.txt")
来源：http://hz.ivvv.top/gtzjcyesoz.html

[F06] 删除文件
来源：http://hz.jqgfzy.top/gtseigtisy.html

Py:   os.remove("a.txt")
来源：http://hz.havefunace.top/gtclvrnsll.html

PHP:  unlink("a.txt");
来源：http://hz.xingfuxueyuan.xyz/gtuxpdhueu.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.c1oappe.top/gtrvblvdrk.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.gaohongyu789.top/gtqnywifkg.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.ywan-chungtsiang.top/gtvogleggk.html

Go:   os.Remove("a.txt")
来源：http://hz.jyoumei.cn/gtjutbdsus.html

Ruby: File.delete("a.txt")
来源：http://hz.shanyushiyangtech.top/gtvhbcecnr.html

C#:   File.Delete("a.txt");
来源：http://hz.sysykeji.top/gtrgbzazpb.html

[F07] 创建目录（含多级）
来源：http://hz.c1oappe.top/gtgqbqkawo.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.ydjk.org.cn/gtulktxxzg.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.wangshuangyany.cn/gtiyucfaot.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hammf.cn/gtlgrrhxlq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.daria6918.cn/gttffallft.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.ppjwa.cn/gtvzpdtaob.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jqgufenzy.top/gtfgtdqvmp.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.havefunace.top/gtqnzbqkwq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.xingfuxueyuan.xyz/gthaigppyg.html

[F08] 遍历目录
来源：http://hz.dianchejie.cn/gtmgtlypqv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.vqdsnc.cn/gthyldzqbw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.jyoumei.cn/gtmaedzppz.html

JS:   fs.readdirSync("dir")
来源：http://hz.hywenlv.cn/gtfcqotiuv.html

TS:   fs.readdirSync("dir")
来源：http://hz.cheryme.top/gtwemrbbeb.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.sxryk.cn/gtlapabyxy.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.hysaishi.cn/gttjsbjane.html

Ruby: Dir.children("dir")
来源：http://hz.bjfxy.top/gtwykaomfq.html

C#:   Directory.GetFiles("dir")
来源：http://hz.jyoumei.cn/gtcxqckmub.html

[F09] 获取文件大小
来源：http://hz.ehwqpu.com/gtlegeoaem.html

Py:   os.path.getsize("a.txt")
来源：http://hz.svipenyu.cn/gtdufavsmy.html

PHP:  filesize("a.txt");
来源：http://hz.cucudq.cn/gtnyegoizs.html

JS:   fs.statSync("a.txt").size
来源：http://hz.cashguo.top/gtodxxxzps.html

TS:   fs.statSync("a.txt").size
来源：http://hz.jinghuilouyu.cn/gtesogmykv.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.hongshengwenyu.top/gtydmqsxfx.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.shzxlz.cn/gtfdhbmxgr.html

Ruby: File.size("a.txt")
来源：http://hz.guowangkeji.top/gtojwkwgct.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.quarkkingdee.top/gtdjklgbml.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.jinqigufen.top/gtwlsxpaxs.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.tianlin.xyz/gtnmyjylsa.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.nwbrower.top/gtishgqrjn.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.pycfn.com/gtnsywldyr.html

TS:   path.extname("a.txt")
来源：http://hz.ivvv.top/gtwuyytybn.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.jiagoushi.top/gtupmedomp.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.fzhhl.top/gtzzccapul.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jyoumei.cn/gtumnvwizv.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.redwolf501.top/gtqdyzxmnm.html

[F11] 复制与移动文件
来源：http://hz.chenjidiqi.icu/gtksmxjdas.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.ywan-chungtsiang.top/gtztlivmfs.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.ybcxt.top/gtacfiiekv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhijiandao.cn/gtenasjanc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.tanke756.top/gtkvukbvih.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.jqgfzy.top/gtwwiissnu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.andypj.xyz/gtykxjmmov.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.yueranfly.top/gtytuobwnt.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.ydzc1.top/gtcvilnoyx.html

[F12] CSV 读写
来源：http://hz.fengsongda.top/gtamrdyjjg.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.chenzaomai.com/gtmcgcfiih.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.aibaodan.cn/gtzstrvocj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.snrcjt.cn/gtblnkelou.html

TS:   // 同上
来源：http://hz.zhijiandao.cn/gtvkxziksk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.yangfankeji.com/gtqfhvufhs.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.daxiang520.top/gtcxaxukxm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.chenlongwang.top/gtvufgyumu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jianghu66.top/gtasadfezw.html

================================================================================
来源：http://hz.jqgufenzy.top/gtwrtbayqw.html

G. 面向对象
来源：http://hz.dashuyun.cn/gtadjdwggx.html

================================================================================
来源：http://hz.xziqi.cn/gtfmvocdnj.html

[G01] 定义类
来源：http://hz.shzxlz.cn/gtpogqngrh.html

Py:   class User: pass
来源：http://hz.yanxiufei.cn/gttfsimjpf.html

PHP:  class User {}
来源：http://hz.yj20258.top/gtjssthecd.html

JS:   class User {}
来源：http://hz.52xcode.cn/gtrcohdvtk.html

TS:   class User { name: string = ""; }
来源：http://hz.gaohongyu789.top/gtjfmxoctd.html

Java: class User {}
来源：http://hz.sysykeji.top/gtigwfzurg.html

Go:   type User struct { Name string }
来源：http://hz.chenlongwang.top/gthldqnxgt.html

Ruby: class User; end
来源：http://hz.xuanzx.com/gtfzkwxkuv.html

C#:   class User {}
来源：http://hz.redwolf501.top/gtosxezxur.html

[G02] 构造函数
来源：http://hz.ybcxt.top/gtcqfovgnv.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.c1oappe.top/gtmfhxqvzu.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.snrcjt.cn/gtrmugkdsv.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.9152youxi.cn/gtkzotflsp.html

TS:   constructor(public name: string) {}
来源：http://hz.yuanzhike.top/gtustpnelc.html

Java: User(String name) { this.name = name; }
来源：http://hz.xziqi.cn/gteyhnxwrq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.tianlin.xyz/gttdypqzsw.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.nanxinkj.top/gttwcogabz.html

C#:   public User(string name) { Name = name; }
来源：http://hz.jqgfzy.top/gtogbvhdhr.html

[G03] 实例属性
来源：http://hz.sxryk.cn/gtzicxkzjk.html

Py:   self.name = "x"
来源：http://hz.smart0.xyz/gtfjkampbd.html

PHP:  public string $name = "x";
来源：http://hz.shanyushiyangkeji.top/gtrebrxcxl.html

JS:   this.name = "x";
来源：http://hz.smart0.xyz/gtyhgtjily.html

TS:   name: string = "x";
来源：http://hz.hfpthk.cn/gtkdafgcjg.html

Java: private String name;
来源：http://hz.jlsjyb.cn/gttnkwjihk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.hammf.cn/gtylioldas.html

Ruby: @name = "x"
来源：http://hz.cheryme.top/gtsdutgcdx.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.andypj.xyz/gtqfhnlvhd.html

[G04] 定义方法
来源：http://hz.hywenlv.cn/gtrtwyarlt.html

Py:   def greet(self): return self.name
来源：http://hz.ydjk.org.cn/gtoeonarlt.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yuxming.cn/gtmrmibjib.html

JS:   greet() { return this.name; }
来源：http://hz.cashguo.top/gteofdhimp.html

TS:   greet(): string { return this.name; }
来源：http://hz.ywan-chungtsiang.top/gtvngdnmfh.html

Java: String greet() { return name; }
来源：http://hz.birdmap.top/gtlnpawmzn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.hongshengwenyu.top/gtoohfiopy.html

Ruby: def greet; @name; end
来源：http://hz.pycfn.com/gttetjqbtd.html

C#:   public string Greet() => Name;
来源：http://hz.aibaodan.cn/gtxzjvvfme.html

[G05] 继承
来源：http://hz.jiagoushi.top/gtbxciwzxd.html

Py:   class Admin(User): pass
来源：http://hz.guannengcc.top/gtosjehnjr.html

PHP:  class Admin extends User {}
来源：http://hz.guannengcc.top/gtvravsmdg.html

JS:   class Admin extends User {}
来源：http://hz.yueranfly.top/gtqvepyspy.html

TS:   class Admin extends User {}
来源：http://hz.wangshuangyany.cn/gtdtmvniyu.html

Java: class Admin extends User {}
来源：http://hz.haohaochexian.top/gtqfypihyc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.jinghuilouyu.cn/gtsodfmmym.html

Ruby: class Admin < User; end
来源：http://hz.yangfankeji.com/gtcttnejte.html

C#:   class Admin : User {}
来源：http://hz.shuidangran.top/gtslfilnvf.html

[G06] 重写方法
来源：http://hz.meibo888.top/gtqkqqgmem.html

Py:   def greet(self): return "admin"
来源：http://hz.shzxlz.cn/gtoimpntwy.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.ydzc1.top/gtmzocxyjn.html

JS:   greet() { return "admin"; }
来源：http://hz.daria6918.cn/gtvguhpowx.html

TS:   greet(): string { return "admin"; }
来源：http://hz.shanyushiyangkeji.top/gtrxdceeks.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.nanxuanxn.top/gtdrnvhloi.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.yonumen.top/gtjbjfslsu.html

Ruby: def greet; "admin"; end
来源：http://hz.yj202588.top/gtxonatndn.html

C#:   public override string Greet() => "admin";
来源：http://hz.ppjwa.cn/gtefjmkxhd.html

[G07] 调用父类方法
来源：http://hz.daria6918.cn/gtodmoduvh.html

Py:   super().greet()
来源：http://hz.ywan-chungtsiang.top/gtcylcllrt.html

PHP:  parent::greet();
来源：http://hz.tianlin.xyz/gtyhnupmae.html

JS:   super.greet();
来源：http://hz.c1oappe.top/gtqmwqdhgg.html

TS:   super.greet();
来源：http://hz.xziqi.cn/gtczhcjoog.html

Java: super.greet();
来源：http://hz.kuanghao11.cn/gttecymgtr.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.ydzc1.top/gtbuutbkvu.html

Ruby: super
来源：http://hz.nanxuanxn.top/gtjebmelvx.html

C#:   base.Greet();
来源：http://hz.fengsongda.top/gtpghqabhp.html

[G08] 静态方法与属性
来源：http://hz.zycfv.cn/gtcexuatoj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.kuanghao11.cn/gttzqqsuev.html

PHP:  public static function f() {}
来源：http://hz.hywenlv.cn/gtskzaqnow.html

JS:   static f() {}
来源：http://hz.gzhubu.top/gtkygxojsq.html

TS:   static f(): void {}
来源：http://hz.cdnleiting.top/gtbqcnjcvs.html

Java: static void f() {}
来源：http://hz.yj202588.top/gtlqafwuwu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.snrcjt.cn/gtajpzhrbz.html

Ruby: def self.f; end
来源：http://hz.jlsjyb.cn/gtakbmyvbz.html

C#:   public static void F() {}
来源：http://hz.xuanzx.com/gttrnmajzd.html

[G09] 接口 / 抽象类
来源：http://hz.yanxiufei.cn/gtzbwwhdhc.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.shanyushiyangkeji.top/gtjebccclk.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.sweek.top/gtcrwddlbw.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.gzhubu.top/gtbadcqsyn.html

TS:   interface Shape { area(): number; }
来源：http://hz.yueranfly.top/gtfqudxtrw.html

Java: interface Shape { double area(); }
来源：http://hz.cdnleiting.top/gttezabjoe.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.daxiang520.top/gtlpdxnjlp.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.dianchejie.cn/gtsbdjzska.html

C#:   interface IShape { double Area(); }
来源：http://hz.guannengcc.top/gttemflefm.html

[G10] 访问控制
来源：http://hz.jqgfzy.top/gtcayabvtp.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.jlsjyb.cn/gtravkwtad.html

PHP:  public / protected / private
来源：http://hz.hnxiangtu.top/gtijnhrjxr.html

JS:   #private 字段；其余公开
来源：http://hz.feifeiyinyue.top/gttzgftipb.html


<!-- 参考信息 -->