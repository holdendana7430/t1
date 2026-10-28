代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.zycfv.cn/gtjybzwody.html

[E11] 反转字符串
来源：http://hz.jinyuanbaomall.cn/gtfgkknbdw.html

Py:   s[::-1]
来源：http://hz.xinyue.icu/gtbvsrfftd.html

PHP:  strrev($s);
来源：http://hz.hysaishi.cn/gtyebbphgi.html

JS:   [...s].reverse().join("")
来源：http://hz.gzhubu.top/gtgzzvpurr.html

TS:   [...s].reverse().join("")
来源：http://hz.pycfn.com/gtxnyomixo.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.pycfn.com/gtswloeyyn.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.xuanzx.com/gtkrsfzvqk.html

Ruby: s.reverse
来源：http://hz.gzhubu.top/gtabrnlwsp.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.yj20258888.top/gtscaefawh.html

[E12] 统计某字符出现次数
来源：http://hz.316326.xyz/gtqdyduozd.html

Py:   s.count("a")
来源：http://hz.chenlongwang.top/gtmeyabdvq.html

PHP:  substr_count($s, "a");
来源：http://hz.gzhubu.top/gtrebgivmt.html

JS:   s.split("a").length - 1
来源：http://hz.jlsjyb.cn/gtcvofqrsu.html

TS:   s.split("a").length - 1
来源：http://hz.pycfn.com/gtkqgccklo.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.wangdashe.top/gtnghcuwco.html

Go:   strings.Count(s, "a")
来源：http://hz.316326.xyz/gtkakzqifq.html

Ruby: s.count("a")
来源：http://hz.fengsongda.top/gtkwgxbgqp.html

C#:   s.Count(c => c == 'a')
来源：http://hz.dashuyun.cn/gtytiwmdfq.html

[E13] 逐字符遍历
来源：http://hz.wangshuangyany.cn/gtwaahmthc.html

Py:   for ch in s: print(ch)
来源：http://hz.sufxvd.cn/gtpvvhntrt.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.haohaochexian.top/gtbgqfzzbk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.bjfxy.top/gtjufesdig.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.hnxiangtu.top/gtlkglxkbc.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.yangfankeji.com/gtnngjbrph.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.9152youxi.cn/gtixpuktcs.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.meibo888.top/gtcdikkifb.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.feifeiyinyue.top/gtwesrwccv.html

[E14] URL 编码与 Base64
来源：http://hz.aibaodan.cn/gtetnomfpj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.ivvv.top/gtwsjshhst.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.gogol.net.cn/gtqzrhetue.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.mhx1999.top/gtqhastrrt.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.chenzaomai.com/gtjehzoefx.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.guowangkeji.top/gtywvurtso.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.wangdashe.top/gtztotzlxi.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.daxiang520.top/gtimflexcn.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.xuetiantiany.cn/gtzcmxtbgz.html

[E15] HTML 转义 / 反转义
来源：http://hz.zhijiandao.cn/gtlwkidunv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.ywan-chungtsiang.top/gtcwqlftwz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.cashguo.top/gtznbrmtpc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.daria6918.cn/gtofhldamm.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.shanyushiyangtech.top/gtbsixmqoj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.cqqwz.cn/gthqseqykf.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.iojbl.cn/gtaxlukako.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.hysaishi.cn/gtzhxkuqik.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.jyoumei.cn/gtmxjptytq.html

[E16] 数字千分位
来源：http://hz.sysykeji.top/gtjcfatrxp.html

Py:   f"{1234567:,}"
来源：http://hz.shangyingyoupin.top/gtarpmpbai.html

PHP:  number_format(1234567);
来源：http://hz.meibo888.top/gtcijwnwbc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.xylfe.cn/gtrovsndaa.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.cdnleiting.top/gtfdskclot.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.redwolf501.top/gthipfoltb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.hnqzz.top/gtasxjjdqn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.ywan-chungtsiang.top/gtdlriucfs.html

C#:   1234567.ToString("N0")
来源：http://hz.dashuyun.cn/gtmandquco.html

[E17] 首字母大写
来源：http://hz.snrcjt.cn/gtacrztyqf.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.cqqwz.cn/gtazybjfvf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.ivvv.top/gtocebycns.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.52xcode.cn/gtvgiogztc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jinqigfzy.top/gtqbjlsvxt.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.shangyingyoupin.top/gtxbojiese.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.zycfv.cn/gtiadxwbka.html

Ruby: s.capitalize
来源：http://hz.ywan-chungtsiang.top/gtabkdeify.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.gaohongyu789.top/gtjbahbghk.html

[E18] 模板占位符替换
来源：http://hz.tanke756.top/gtlaxkketv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.vqdsnc.cn/gtuddcspyz.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.chenjidiqi.icu/gtycuttzzv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.0kj1m.cn/gtqztxrnrq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.zhixingplan.top/gtdhzffnkf.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.meibo888.top/gtdalqhkmf.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.guannengcc.top/gtflciziwr.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.snrcjt.cn/gtdibxrvpp.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.fengsongda.top/gtqadyhmbq.html

[E19] 多行文本按行拆分
来源：http://hz.ehwqpu.com/gtsbyjwfwg.html

Py:   s.splitlines()
来源：http://hz.xziqi.cn/gtvfrewvup.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.hnxiangtu.top/gtkbmrqqqq.html

JS:   s.split(/\r?\n/)
来源：http://hz.52xcode.cn/gtmyhalcnc.html

TS:   s.split(/\r?\n/)
来源：http://hz.svipenyu.cn/gteewwskve.html

Java: s.lines().toList()
来源：http://hz.jlsjyb.cn/gtnfkzruca.html

Go:   strings.Split(s, "\n")
来源：http://hz.ehwqpu.com/gtmtdnlkzn.html

Ruby: s.lines
来源：http://hz.zhongyouzk.top/gtswzzwcpx.html

C#:   s.Split('\n')
来源：http://hz.tianlin.xyz/gtualberva.html

[E20] 判断字符串是否为空
来源：http://hz.pengpengdd.cyou/gttmfxxwom.html

Py:   if not s:
来源：http://hz.hongshengwenyu.top/gtbloqnkpj.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.chenlongwang.top/gtpdtrvawz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.ydjk.org.cn/gtlwkztaai.html

TS:   if (s === "") {}
来源：http://hz.9152youxi.cn/gtzpsrulmv.html

Java: if (s.isEmpty()) {}
来源：http://hz.shangyingyoupin.top/gthmjzoazh.html

Go:   if s == "" {}
来源：http://hz.tian-w.cn/gtsnfnizil.html

Ruby: if s.empty?
来源：http://hz.havefunace.top/gtqaovypkv.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.snrcjt.cn/gtogiyoyed.html

[E21] 超长截断加省略号
来源：http://hz.iojbl.cn/gtkykwbjdc.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.kuanghao11.cn/gtefwmhnqd.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.wangshuangyany.cn/gtklczbucw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.xingfuxueyuan.xyz/gtxpfllzwd.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.havefunace.top/gtyvvgqzln.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.9152youxi.cn/gtccppmmnc.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.ydzc1.top/gtdnhdlxnh.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.yvedp.cn/gthuxpopsj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.yj20258.top/gtjxntqqmu.html

[E22] 字节长度与字符长度
来源：http://hz.havefunace.top/gtyuosvuis.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.52xcode.cn/gtycuablec.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.chenzaomai.com/gtsuvvgrue.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hammf.cn/gthdbdtnrb.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jqgufenzy.top/gtjvyizqrw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.cdnleiting.top/gtsaobrnpm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.andypj.xyz/gtyabrtnio.html

Ruby: s.bytesize;  s.length
来源：http://hz.dashuyun.cn/gtkvyllwwu.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.zhengqikj.top/gtmtstxxns.html

================================================================================
来源：http://hz.iojbl.cn/gtzpogdgec.html

F. 文件与目录
来源：http://hz.ehwqpu.com/gtblscnkdf.html

================================================================================
来源：http://hz.yuanzhike.top/gtlttnboqi.html

[F01] 读取整个文件
来源：http://hz.hfpthk.cn/gttlgwmoxt.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yuxming.cn/gtjrhogsop.html

PHP:  file_get_contents("a.txt");
来源：http://hz.gogol.net.cn/gtkfqrxvau.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.nanxinkj.top/gtgpwgsryh.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.sweek.top/gtxrdtbaxj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.xuetiantiany.cn/gtxvifocxm.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.guowangkeji.top/gtujiehbyl.html

Ruby: File.read("a.txt")
来源：http://hz.pycfn.com/gtyvkmbhrz.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yueranfly.top/gtnsobandn.html

[F02] 逐行读取文件
来源：http://hz.c1oappe.top/gtyituxjdx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.yuxming.cn/gtqfjxfqpi.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.ydzc1.top/gtnpziluyu.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jianghu66.top/gtwacqnklq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.shzxlz.cn/gtdijwlclb.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.sysykeji.top/gtmoxkgzxp.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.zhoulong.xyz/gtxucdogjs.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.fengsongda.top/gtjarhzrds.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.zhijiandao.cn/gtwcbtiqzi.html

[F03] 写入文件（覆盖）
来源：http://hz.aibaodan.cn/gtjsjqqgux.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.zhongyouzk.top/gtphywddyq.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.yonumen.top/gtqmbacret.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hongshengwenyu.top/gtgetgcbvs.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.redwolf501.top/gtgtfaziwe.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.birdmap.top/gtqwiauspo.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.dianchejie.cn/gtdrdtvkvj.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.nanxuanxn.top/gtmtxhisub.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.sysykeji.top/gthhkusukq.html

[F04] 追加写入文件
来源：http://hz.jiagoushi.top/gtjxsltrbp.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.zdqjudy.top/gtqdqcpnrb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.jinqigfzy.top/gtjtgvpsfk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ywan-chungtsiang.top/gtusawumxf.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.feifeiyinyue.top/gtrtkbdvgz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.tian-w.cn/gthamgmaki.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.gogol.net.cn/gtezoxmvmo.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.fzhhl.top/gtixpponjz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.aibaodan.cn/gtxroqrcze.html

[F05] 判断文件或目录是否存在
来源：http://hz.hongshengwenyu.top/gtmjgasccn.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.hnxiangtu.top/gtihykfaew.html

PHP:  file_exists("a.txt");
来源：http://hz.yj202588.top/gtbucoxpdg.html

JS:   fs.existsSync("a.txt")
来源：http://hz.ydzc1.top/gtyyoswikf.html

TS:   fs.existsSync("a.txt")
来源：http://hz.gaohongyu789.top/gtroawtito.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.tanke756.top/gtgexqidhx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.yueranfly.top/gtntozjsyo.html

Ruby: File.exist?("a.txt")
来源：http://hz.xinyue.icu/gtrtaeyeiz.html

C#:   File.Exists("a.txt")
来源：http://hz.c1oappe.top/gtmhhzbfzo.html

[F06] 删除文件
来源：http://hz.shanyushiyangkeji.top/gtlwzwxcdo.html

Py:   os.remove("a.txt")
来源：http://hz.zhiwuduotai.top/gtcuhldiqi.html

PHP:  unlink("a.txt");
来源：http://hz.hnqzz.top/gtpchowkgr.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.quarkkingdee.top/gtcscpjsfv.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.yj202588.top/gthamkctln.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.hnqzz.top/gtoijypdyc.html

Go:   os.Remove("a.txt")
来源：http://hz.9152youxi.cn/gttirjdpra.html

Ruby: File.delete("a.txt")
来源：http://hz.vqdsnc.cn/gtbwoyddxk.html

C#:   File.Delete("a.txt");
来源：http://hz.jqgfzy.top/gtmebcfcyq.html

[F07] 创建目录（含多级）
来源：http://hz.c1oappe.top/gtrrgoyibz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.chenjidiqi.icu/gtfrmfudhs.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.cashguo.top/gtllxqqlur.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yonumen.top/gtmllqulpe.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhaomingkeji.xyz/gtfdbvrmeb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.yj20258.top/gtoudvruoc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.pycfn.com/gtiycnziqg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.yangfankeji.com/gttcgfhsiu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.hysaishi.cn/gtsuhzpgxl.html

[F08] 遍历目录
来源：http://hz.yongpay.top/gtvjmrrquc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.vqdsnc.cn/gtvtljbvkm.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.yueranfly.top/gtvnrtpgdt.html

JS:   fs.readdirSync("dir")
来源：http://hz.gogol.net.cn/gtwfmjjpvz.html

TS:   fs.readdirSync("dir")
来源：http://hz.xylfe.cn/gtzpdzvznr.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.cucudq.cn/gtvrbbpisc.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.0kj1m.cn/gtbpafdflz.html

Ruby: Dir.children("dir")
来源：http://hz.tian-w.cn/gtqmnxhfyf.html

C#:   Directory.GetFiles("dir")
来源：http://hz.chenzaomai.com/gtwvmdbnbl.html

[F09] 获取文件大小
来源：http://hz.hysaishi.cn/gtcijtbpde.html

Py:   os.path.getsize("a.txt")
来源：http://hz.dashuyun.cn/gttcrpivqs.html

PHP:  filesize("a.txt");
来源：http://hz.redwolf501.top/gtxzgquseb.html

JS:   fs.statSync("a.txt").size
来源：http://hz.jianghu66.top/gtxvbpdcqg.html

TS:   fs.statSync("a.txt").size
来源：http://hz.zhengqikj.top/gtbrqpykup.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.0kj1m.cn/gtkempzqhi.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.chenlongwang.top/gtepwljyvo.html

Ruby: File.size("a.txt")
来源：http://hz.meibo888.top/gttndovvan.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.smart0.xyz/gtpdnevkct.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.xuanzx.com/gtjdfljmwo.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.ydzc1.top/gthigrjnfz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.zhengqikj.top/gtjlfbcjqy.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.jqgufenzy.top/gtlsvqgcsc.html

TS:   path.extname("a.txt")
来源：http://hz.hfpthk.cn/gthibjuqpj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.tian-w.cn/gtakrmivfs.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.smart0.xyz/gtficgfrzu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.zhengqikj.top/gtcbdvbhkk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.cheryme.top/gtlhnkkmxy.html

[F11] 复制与移动文件
来源：http://hz.zhixingplan.top/gtpeptsaao.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.birdmap.top/gttyunhvvg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yvedp.cn/gtzhreiweu.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hfpthk.cn/gtimeuscnz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.nanxuanxn.top/gttbptwdgh.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.wangdashe.top/gtsgevflwz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jqgfzy.top/gtklawungk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.sufxvd.cn/gtfbqitven.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.kuanghao11.cn/gtnvyulfsx.html

[F12] CSV 读写
来源：http://hz.cdnleiting.top/gtcetxshqn.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.ydjk.org.cn/gtykwidqcz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.xingfuxueyuan.xyz/gtyzlfhnyz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.cqqwz.cn/gtotpxgsnx.html

TS:   // 同上
来源：http://hz.dashuyun.cn/gtkyhcsyur.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.ywan-chungtsiang.top/gtuolcqecb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.jqgfzy.top/gtjzhtwxlv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.ywan-chungtsiang.top/gtbpyapvjd.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.zhoulong.xyz/gtnmgpvzjt.html

================================================================================
来源：http://hz.jqgufenzy.top/gtpdvdsziq.html

G. 面向对象
来源：http://hz.aizwys.cn/gtodqfoxyl.html

================================================================================
来源：http://hz.ehwqpu.com/gtjappagbh.html

[G01] 定义类
来源：http://hz.jqgfzy.top/gtdgztqubf.html

Py:   class User: pass
来源：http://hz.cashguo.top/gtjuqtwpuo.html

PHP:  class User {}
来源：http://hz.guowangkeji.top/gtwhiycguo.html

JS:   class User {}
来源：http://hz.xuetiantiany.cn/gtkadztxsi.html

TS:   class User { name: string = ""; }
来源：http://hz.ydjk.org.cn/gtlacosjwt.html

Java: class User {}
来源：http://hz.9152youxi.cn/gtodwjplem.html

Go:   type User struct { Name string }
来源：http://hz.jyoumei.cn/gtdsocejtx.html

Ruby: class User; end
来源：http://hz.andypj.xyz/gttwpkbvql.html

C#:   class User {}
来源：http://hz.shzxlz.cn/gtvsixqpyp.html

[G02] 构造函数
来源：http://hz.zhengqikj.top/gtyoliqutu.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.andypj.xyz/gtecuosuxo.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yueranfly.top/gtesfqhuko.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.ivvv.top/gtqfdoctmq.html

TS:   constructor(public name: string) {}
来源：http://hz.zycfv.cn/gtdfujgccd.html

Java: User(String name) { this.name = name; }
来源：http://hz.quarkkingdee.top/gttngjkngw.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.zhijiandao.cn/gtsjkzldkv.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.aibaodan.cn/gtaizyfiwz.html

C#:   public User(string name) { Name = name; }
来源：http://hz.snrcjt.cn/gticradzkt.html

[G03] 实例属性
来源：http://hz.fengsongda.top/gtpqzawlov.html

Py:   self.name = "x"
来源：http://hz.ehwqpu.com/gtpgupkwda.html

PHP:  public string $name = "x";
来源：http://hz.nanxinkj.top/gtxcpcrepv.html

JS:   this.name = "x";
来源：http://hz.jianghu66.top/gthruqsuza.html

TS:   name: string = "x";
来源：http://hz.vqdsnc.cn/gtlwdmqzcq.html

Java: private String name;
来源：http://hz.zhixingplan.top/gtcxajfiqd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.daxiang520.top/gtoabznhao.html

Ruby: @name = "x"
来源：http://hz.yuanzhike.top/gtuoqqtsgw.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.hnxiangtu.top/gtzblahxfp.html

[G04] 定义方法
来源：http://hz.hfpthk.cn/gtkkgagspi.html

Py:   def greet(self): return self.name
来源：http://hz.yanxiufei.cn/gtufnabdpa.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.316326.xyz/gtvelzrmqd.html

JS:   greet() { return this.name; }
来源：http://hz.ehwqpu.com/gthssryjcq.html

TS:   greet(): string { return this.name; }
来源：http://hz.nanxuanxn.top/gtvrdiiuaw.html

Java: String greet() { return name; }
来源：http://hz.zhoulong.xyz/gtdfvdcqzt.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.meibo888.top/gtjggpoujv.html

Ruby: def greet; @name; end
来源：http://hz.hywenlv.cn/gtzgrcfwgt.html

C#:   public string Greet() => Name;
来源：http://hz.yueranfly.top/gtgkrljnpq.html

[G05] 继承
来源：http://hz.hnxiangtu.top/gteinmzcus.html

Py:   class Admin(User): pass
来源：http://hz.xinyue.icu/gtvmamffre.html

PHP:  class Admin extends User {}
来源：http://hz.dianchejie.cn/gtjutwgirl.html

JS:   class Admin extends User {}
来源：http://hz.birdmap.top/gtfbnpichp.html

TS:   class Admin extends User {}
来源：http://hz.sweek.top/gtpidjgdsj.html

Java: class Admin extends User {}
来源：http://hz.yonumen.top/gtdvakzxqp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.jinqigufen.top/gtmapdxhmm.html

Ruby: class Admin < User; end
来源：http://hz.havefunace.top/gtdjwosiuw.html

C#:   class Admin : User {}
来源：http://hz.iojbl.cn/gtaqbkhsxn.html

[G06] 重写方法
来源：http://hz.jianghu66.top/gtmjapptsw.html

Py:   def greet(self): return "admin"
来源：http://hz.jlsjyb.cn/gtiysffgda.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.sxryk.cn/gtkpcpvmig.html

JS:   greet() { return "admin"; }
来源：http://hz.zhaomingkeji.xyz/gtmajcuauj.html

TS:   greet(): string { return "admin"; }
来源：http://hz.shanyushiyangkeji.top/gtntxttmnq.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.shangyingyoupin.top/gtnpomdzks.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.yanxiufei.cn/gtwzaehugu.html

Ruby: def greet; "admin"; end
来源：http://hz.daria6918.cn/gtmcxddcfh.html

C#:   public override string Greet() => "admin";
来源：http://hz.iojbl.cn/gtzlkbhqdd.html

[G07] 调用父类方法
来源：http://hz.sxryk.cn/gtyypwqdnz.html

Py:   super().greet()
来源：http://hz.cheryme.top/gtzyktgfpu.html

PHP:  parent::greet();
来源：http://hz.ehwqpu.com/gtojxelpuc.html

JS:   super.greet();
来源：http://hz.zdqjudy.top/gtexllmpfp.html

TS:   super.greet();
来源：http://hz.jyoumei.cn/gtokpqzrpo.html

Java: super.greet();
来源：http://hz.chenzaomai.com/gtehovcqhz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.shzxlz.cn/gtcrexaehb.html

Ruby: super
来源：http://hz.ppjwa.cn/gtyfbjursz.html

C#:   base.Greet();
来源：http://hz.redwolf501.top/gtmymkzkwd.html

[G08] 静态方法与属性
来源：http://hz.yueranfly.top/gtbzkdndpf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.shanyushiyangtech.top/gtfppcpvaf.html

PHP:  public static function f() {}
来源：http://hz.gaohongyu789.top/gtpxpwokra.html

JS:   static f() {}
来源：http://hz.kuanghao11.cn/gtugfqlhgl.html

TS:   static f(): void {}
来源：http://hz.bjfxy.top/gtjmdxqikn.html

Java: static void f() {}
来源：http://hz.yj20258888.top/gtjiqjalzw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.zdqjudy.top/gtvbgmoazp.html

Ruby: def self.f; end
来源：http://hz.chenzaomai.com/gtoadmbeey.html

C#:   public static void F() {}
来源：http://hz.hfpthk.cn/gteunbwpam.html

[G09] 接口 / 抽象类
来源：http://hz.c1oappe.top/gtxqixpsso.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.c1oappe.top/gtzzzqnizr.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.kuanghao11.cn/gtsbkvdpqc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.gotoacloud.top/gtdtephqti.html

TS:   interface Shape { area(): number; }
来源：http://hz.hfpthk.cn/gtbifhzyev.html


<!-- 参考信息 -->