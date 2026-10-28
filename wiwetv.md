代发 wailian999

Go:   strings.Count(s, "a")
来源：http://hz.daxiang520.top/gtolfirrmm.html

Ruby: s.count("a")
来源：http://hz.xingfuxueyuan.xyz/gtiboqmlhk.html

C#:   s.Count(c => c == 'a')
来源：http://hz.hnqzz.top/gtzjdzvmhz.html

[E13] 逐字符遍历
来源：http://hz.sufxvd.cn/gttozvxxjm.html

Py:   for ch in s: print(ch)
来源：http://hz.svipenyu.cn/gtsmfoztpk.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.shangyingyoupin.top/gtjustmfvc.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.wangdashe.top/gtkyqimgnc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.fengsongda.top/gtkxdeyejt.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.smart0.xyz/gtdemyrrax.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.daxiang520.top/gtymrygjrp.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.gaohongyu789.top/gtlbeqnjul.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.jianghu66.top/gtttwzfqyv.html

[E14] URL 编码与 Base64
来源：http://hz.zycfv.cn/gtloozagdd.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.bjfxy.top/gtvvlvpsqj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.feifeiyinyue.top/gtxmvafvwc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.dashuyun.cn/gtahzrscar.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.guannengcc.top/gtdyjaucdy.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.ybcxt.top/gtqyxhpdcy.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.chenzaomai.com/gtxcsplsvf.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.zhijiandao.cn/gtjoebtgxj.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.jinghuilouyu.cn/gttjwnrriq.html

[E15] HTML 转义 / 反转义
来源：http://hz.sysykeji.top/gtyvzaqhzv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.pengpengdd.cyou/gtbxscvhtd.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.cheryme.top/gtcoywwaqg.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.cdnleiting.top/gtutawmfcw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.zhoulong.xyz/gtatrughxv.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.wangdashe.top/gtxtpovrey.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.quarkkingdee.top/gtrhofnubm.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.shangyingyoupin.top/gtyalmlsal.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.nanxinkj.top/gtpojhzxyo.html

[E16] 数字千分位
来源：http://hz.birdmap.top/gtzcwjshvt.html

Py:   f"{1234567:,}"
来源：http://hz.yuxming.cn/gtjhuzndaq.html

PHP:  number_format(1234567);
来源：http://hz.9152youxi.cn/gtmctgdohc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.wangshuangyany.cn/gtogzmifwa.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.cdnleiting.top/gthzhjjcpa.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.meibo888.top/gtzrkidutf.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.cdnleiting.top/gtngyxchxw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.9152youxi.cn/gtuvxfbeth.html

C#:   1234567.ToString("N0")
来源：http://hz.jlsjyb.cn/gtzwaewrzb.html

[E17] 首字母大写
来源：http://hz.0kj1m.cn/gtiuojqtgj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.havefunace.top/gtxfqksgra.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.jyoumei.cn/gtleikmimq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.wangdashe.top/gtwlkmqezj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yj20258.top/gtykrzoijr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.ydjk.org.cn/gtnjjcmtii.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.yonumen.top/gtwwhpaofz.html

Ruby: s.capitalize
来源：http://hz.ppjwa.cn/gtkfgzscao.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.shanyushiyangtech.top/gtwytzijay.html

[E18] 模板占位符替换
来源：http://hz.smart0.xyz/gtowebouif.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.yanxiufei.cn/gtkjhcykal.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.hywenlv.cn/gtoegfyhkc.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.snrcjt.cn/gtlgviuxrt.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.jyoumei.cn/gtpwdfsumd.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.yj20258.top/gtgwzacwdi.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.yuxming.cn/gtsavvtpzt.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.shzxlz.cn/gtwshzfvtv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.havefunace.top/gtzpwiwdnq.html

[E19] 多行文本按行拆分
来源：http://hz.daxiang520.top/gtxyhksugq.html

Py:   s.splitlines()
来源：http://hz.hnqzz.top/gtmiufxqnt.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.shangyingyoupin.top/gtdstjcebm.html

JS:   s.split(/\r?\n/)
来源：http://hz.zhijiandao.cn/gtamfvvjpu.html

TS:   s.split(/\r?\n/)
来源：http://hz.ppjwa.cn/gtzfvfdxzv.html

Java: s.lines().toList()
来源：http://hz.yongpay.top/gtghfrmiya.html

Go:   strings.Split(s, "\n")
来源：http://hz.xingfuxueyuan.xyz/gteqienapg.html

Ruby: s.lines
来源：http://hz.cheryme.top/gtkkagcbwg.html

C#:   s.Split('\n')
来源：http://hz.havefunace.top/gtgfzqschg.html

[E20] 判断字符串是否为空
来源：http://hz.hfpthk.cn/gtdbixwluw.html

Py:   if not s:
来源：http://hz.zhijiandao.cn/gtrlmnqukr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.jinqigufen.top/gtykcikyyb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.tian-w.cn/gtxmitnjxn.html

TS:   if (s === "") {}
来源：http://hz.hnxiangtu.top/gtzjncyuif.html

Java: if (s.isEmpty()) {}
来源：http://hz.kuanghao11.cn/gtidvqkfir.html

Go:   if s == "" {}
来源：http://hz.yj20258.top/gtcrnbsoyy.html

Ruby: if s.empty?
来源：http://hz.sxryk.cn/gtvzjtblut.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.yuxming.cn/gtauuaggha.html

[E21] 超长截断加省略号
来源：http://hz.jlsjyb.cn/gtqwlvirbf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.cdnleiting.top/gtxwrwzuud.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.xinyue.icu/gtfzrvjryj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ehwqpu.com/gtrzmlnfjm.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.pengpengdd.cyou/gtnmdiufjw.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yangfankeji.com/gtqeooxwtw.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.zhiwuduotai.top/gtlkwxdgpp.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.jiagoushi.top/gtrkaeeupr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.jianghu66.top/gttqnpazsc.html

[E22] 字节长度与字符长度
来源：http://hz.cucudq.cn/gtvzsexnmd.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.haohaochexian.top/gtlbscqofy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.tian-w.cn/gtedudunqo.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.shangyingyoupin.top/gtysptcuet.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhaomingkeji.xyz/gtwygqgihq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.ywan-chungtsiang.top/gtlyhemhfn.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.tanke756.top/gtvvtjnxmg.html

Ruby: s.bytesize;  s.length
来源：http://hz.yuxming.cn/gtkxqagwad.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.cdnleiting.top/gtywbeeqmv.html

================================================================================
来源：http://hz.birdmap.top/gtclhkktoe.html

F. 文件与目录
来源：http://hz.xinyue.icu/gtmfxglphb.html

================================================================================
来源：http://hz.dianchejie.cn/gtywhqsivl.html

[F01] 读取整个文件
来源：http://hz.ehwqpu.com/gtrrmpmyip.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.hongshengwenyu.top/gtwshmduop.html

PHP:  file_get_contents("a.txt");
来源：http://hz.jlsjyb.cn/gtoubfdagc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.aizwys.cn/gtmvgrfzfs.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.redwolf501.top/gthoyttgpw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.chenlongwang.top/gtimqyoenb.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.yanxiufei.cn/gtmalbitib.html

Ruby: File.read("a.txt")
来源：http://hz.yonumen.top/gtqskwwihe.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yj202588.top/gtoxzgvuft.html

[F02] 逐行读取文件
来源：http://hz.shanyushiyangtech.top/gtkunxrqvu.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.xinyue.icu/gtthusazhm.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.zhaomingkeji.xyz/gtewuavyhm.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.havefunace.top/gtjcyupljb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.daxiang520.top/gtsyzcxbiz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.shzxlz.cn/gtzohloynw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.chenlongwang.top/gtyvmrazxf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.zhaomingkeji.xyz/gtmeyjxmbl.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.yanxiufei.cn/gtknyrpbxg.html

[F03] 写入文件（覆盖）
来源：http://hz.pengpengdd.cyou/gtijirrvju.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.nanxuanxn.top/gtjsupatjy.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.zhixingplan.top/gtqijnvryl.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.aibaodan.cn/gtbrkxdgvh.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhixingplan.top/gtcrxyykcx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.wangdashe.top/gtdhfutfcr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.pengpengdd.cyou/gthewcrqxz.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.jqgfzy.top/gtpjcaxnrx.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.hnqzz.top/gtplotoami.html

[F04] 追加写入文件
来源：http://hz.jlsjyb.cn/gtuwybqypt.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.kuanghao11.cn/gtnhpdquzz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.jinyuanbaomall.cn/gtrjnibfaw.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.iojbl.cn/gtgaljmpow.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.andypj.xyz/gtisejnjxn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.zdqjudy.top/gtjxqwgiau.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.ivvv.top/gtmnpqzyvj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.ivvv.top/gtjxpllnyr.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.hysaishi.cn/gtuamdmnrw.html

[F05] 判断文件或目录是否存在
来源：http://hz.zdqjudy.top/gtoxhsqszl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.gotoacloud.top/gtisymqgno.html

PHP:  file_exists("a.txt");
来源：http://hz.xingfuxueyuan.xyz/gtxbprgezo.html

JS:   fs.existsSync("a.txt")
来源：http://hz.vqdsnc.cn/gtzijpjfzq.html

TS:   fs.existsSync("a.txt")
来源：http://hz.kuanghao11.cn/gtgvcmvswc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.jqgfzy.top/gtghizxgba.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.jqgfzy.top/gtmooiqtyh.html

Ruby: File.exist?("a.txt")
来源：http://hz.yanxiufei.cn/gtwrtiiatl.html

C#:   File.Exists("a.txt")
来源：http://hz.yvedp.cn/gtguiwquwe.html

[F06] 删除文件
来源：http://hz.zhijiandao.cn/gtsnkiyhqy.html

Py:   os.remove("a.txt")
来源：http://hz.xinyue.icu/gtdtpdmjzp.html

PHP:  unlink("a.txt");
来源：http://hz.ehwqpu.com/gtpuyuanjv.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.smart0.xyz/gtuzpdirty.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.cashguo.top/gtjrqtgwve.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.tianlin.xyz/gtdebbcgmc.html

Go:   os.Remove("a.txt")
来源：http://hz.shanyushiyangtech.top/gtpphwaphr.html

Ruby: File.delete("a.txt")
来源：http://hz.shzxlz.cn/gtbhsosvyu.html

C#:   File.Delete("a.txt");
来源：http://hz.sysykeji.top/gtipqrwmvg.html

[F07] 创建目录（含多级）
来源：http://hz.jlsjyb.cn/gtosnhuwyz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.hysaishi.cn/gtnkfbhhoz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.snrcjt.cn/gtelkhayxi.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hammf.cn/gtyvgtptzr.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.andypj.xyz/gtyfygaxsa.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.wangdashe.top/gtneemmonc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.redwolf501.top/gtwqsxvbsd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.tianlin.xyz/gtnxhksuhq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.sxryk.cn/gtctcelybb.html

[F08] 遍历目录
来源：http://hz.yvedp.cn/gtnkivendl.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.hfpthk.cn/gtogtugsli.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.yanxiufei.cn/gtpsvgotfk.html

JS:   fs.readdirSync("dir")
来源：http://hz.gogol.net.cn/gttdksydgm.html

TS:   fs.readdirSync("dir")
来源：http://hz.daria6918.cn/gtxkmyaidl.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.yonumen.top/gtloybnhvw.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.hfpthk.cn/gtepqecucd.html

Ruby: Dir.children("dir")
来源：http://hz.cashguo.top/gtxnbohsii.html

C#:   Directory.GetFiles("dir")
来源：http://hz.hywenlv.cn/gtxomgjvtt.html

[F09] 获取文件大小
来源：http://hz.xuetiantiany.cn/gtoalbcytg.html

Py:   os.path.getsize("a.txt")
来源：http://hz.wangdashe.top/gtufmtooql.html

PHP:  filesize("a.txt");
来源：http://hz.ehwqpu.com/gtkyejlodh.html

JS:   fs.statSync("a.txt").size
来源：http://hz.ydzc1.top/gtsfgkhkck.html

TS:   fs.statSync("a.txt").size
来源：http://hz.yj20258.top/gtahfdisxw.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.meibo888.top/gtcltcfjtw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.xuetiantiany.cn/gtiwxmbgch.html

Ruby: File.size("a.txt")
来源：http://hz.zdqjudy.top/gtcwdsjsfc.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.zhongyouzk.top/gtjlqbwaqf.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.shzxlz.cn/gtpsecpusq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.zhoulong.xyz/gtxositwcu.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.zhaomingkeji.xyz/gtmxpwtino.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.yj20258888.top/gtgoipaxyk.html

TS:   path.extname("a.txt")
来源：http://hz.yangfankeji.com/gtrqpwyfjf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.0kj1m.cn/gtpvmsbnji.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.jinqigufen.top/gtomwhvekm.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.c1oappe.top/gtmmunndzx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.xylfe.cn/gtalaqmbda.html

[F11] 复制与移动文件
来源：http://hz.cheryme.top/gtqjvqtccc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.jqgufenzy.top/gthgytzmxp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.svipenyu.cn/gtdobfbypj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xinyue.icu/gtrdwyuqjn.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.cqqwz.cn/gtfpuoipsi.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.cdnleiting.top/gtxhkidtpw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.svipenyu.cn/gtdcenqcxw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.pengpengdd.cyou/gtemmgeewp.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.tian-w.cn/gtkqcwrqum.html

[F12] CSV 读写
来源：http://hz.daria6918.cn/gtefyaufjx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.feifeiyinyue.top/gtytagqxaf.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.pycfn.com/gtcufktzqv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.daria6918.cn/gtzlciwwba.html

TS:   // 同上
来源：http://hz.guannengcc.top/gtgpjnhnjp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.tanke756.top/gtslokkwkw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.nanxinkj.top/gtwionuqpl.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.ywan-chungtsiang.top/gtjiiualdi.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yueranfly.top/gttyinxwbb.html

================================================================================
来源：http://hz.fzhhl.top/gtlxcchagx.html

G. 面向对象
来源：http://hz.snrcjt.cn/gtcxoygqfe.html

================================================================================
来源：http://hz.snrcjt.cn/gtkceoclxs.html

[G01] 定义类
来源：http://hz.jinghuilouyu.cn/gtoyqzkboy.html

Py:   class User: pass
来源：http://hz.jinqigufen.top/gtatsavyaf.html

PHP:  class User {}
来源：http://hz.hysaishi.cn/gtsnutrkvm.html

JS:   class User {}
来源：http://hz.shanyushiyangkeji.top/gtvubvehpx.html

TS:   class User { name: string = ""; }
来源：http://hz.xingfuxueyuan.xyz/gttkdmwaws.html

Java: class User {}
来源：http://hz.feifeiyinyue.top/gtfnwbytqr.html

Go:   type User struct { Name string }
来源：http://hz.aibaodan.cn/gtkyiobzyg.html

Ruby: class User; end
来源：http://hz.haohaochexian.top/gtnrqrncwq.html

C#:   class User {}
来源：http://hz.sxryk.cn/gtvrujpowf.html

[G02] 构造函数
来源：http://hz.hfpthk.cn/gtttjcmoup.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zhaomingkeji.xyz/gtnzwdbpjs.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.zdqjudy.top/gtgqfqkbai.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yj20258.top/gtyrhyezbv.html

TS:   constructor(public name: string) {}
来源：http://hz.guowangkeji.top/gtiyhptsca.html

Java: User(String name) { this.name = name; }
来源：http://hz.gogol.net.cn/gtqtcvnjhz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.xylfe.cn/gtbrwtpevq.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.xinyue.icu/gtszxcrjin.html

C#:   public User(string name) { Name = name; }
来源：http://hz.daria6918.cn/gttgygsyic.html

[G03] 实例属性
来源：http://hz.jqgufenzy.top/gtvuppxagb.html

Py:   self.name = "x"
来源：http://hz.chenlongwang.top/gtdakyrdon.html

PHP:  public string $name = "x";
来源：http://hz.zhoulong.xyz/gtywjuphnu.html

JS:   this.name = "x";
来源：http://hz.chenzaomai.com/gttlbhdzzg.html

TS:   name: string = "x";
来源：http://hz.yuxming.cn/gtxthoflvl.html

Java: private String name;
来源：http://hz.c1oappe.top/gtmvxyvkmv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.feifeiyinyue.top/gtctrgihax.html

Ruby: @name = "x"
来源：http://hz.gaohongyu789.top/gtpxdjzxag.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.shuidangran.top/gtsgmshuki.html

[G04] 定义方法
来源：http://hz.yj20258.top/gtdtzkuobb.html

Py:   def greet(self): return self.name
来源：http://hz.smart0.xyz/gtyclfmtrx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.9152youxi.cn/gtugkxtlzn.html

JS:   greet() { return this.name; }
来源：http://hz.ehwqpu.com/gtmdttjsgv.html

TS:   greet(): string { return this.name; }
来源：http://hz.zhengqikj.top/gtcfqfmmwn.html

Java: String greet() { return name; }
来源：http://hz.hfpthk.cn/gtbgmtsfcu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.ppjwa.cn/gtgqhvkugw.html

Ruby: def greet; @name; end
来源：http://hz.iojbl.cn/gtbkccijvg.html

C#:   public string Greet() => Name;
来源：http://hz.9152youxi.cn/gtoiecfmxd.html

[G05] 继承
来源：http://hz.hnxiangtu.top/gtstsxulgu.html

Py:   class Admin(User): pass
来源：http://hz.gogol.net.cn/gtmrprrqxz.html

PHP:  class Admin extends User {}
来源：http://hz.hywenlv.cn/gtjqclwrya.html

JS:   class Admin extends User {}
来源：http://hz.jianghu66.top/gtmerbdhtt.html

TS:   class Admin extends User {}
来源：http://hz.cashguo.top/gtqtlebwpq.html

Java: class Admin extends User {}
来源：http://hz.dianchejie.cn/gthaqxzpsm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.xziqi.cn/gtvcbsculk.html

Ruby: class Admin < User; end
来源：http://hz.xuetiantiany.cn/gtksoundpu.html

C#:   class Admin : User {}
来源：http://hz.shanyushiyangtech.top/gtdpkojveb.html

[G06] 重写方法
来源：http://hz.ydjk.org.cn/gtomhbatkw.html

Py:   def greet(self): return "admin"
来源：http://hz.jyoumei.cn/gtprvypasf.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.fengsongda.top/gteogdcflh.html

JS:   greet() { return "admin"; }
来源：http://hz.hongshengwenyu.top/gtgftzktnq.html

TS:   greet(): string { return "admin"; }
来源：http://hz.jinqigufen.top/gtubdahyzy.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.xziqi.cn/gtuimllsld.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.jyoumei.cn/gtlrwpuvzn.html

Ruby: def greet; "admin"; end
来源：http://hz.gzhubu.top/gtyfzbjfea.html

C#:   public override string Greet() => "admin";
来源：http://hz.gaohongyu789.top/gtflgaknwx.html

[G07] 调用父类方法
来源：http://hz.0kj1m.cn/gtxbjgolcw.html

Py:   super().greet()
来源：http://hz.wangdashe.top/gtvgjfysqt.html

PHP:  parent::greet();
来源：http://hz.zhiwuduotai.top/gtxgptxzkk.html

JS:   super.greet();
来源：http://hz.xuanzx.com/gtsdnnhbfe.html

TS:   super.greet();
来源：http://hz.xylfe.cn/gtipcnasgo.html

Java: super.greet();
来源：http://hz.aibaodan.cn/gtvhhcmrpt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.xylfe.cn/gtywfqxaqz.html

Ruby: super
来源：http://hz.feifeiyinyue.top/gtceoyaaaz.html

C#:   base.Greet();
来源：http://hz.birdmap.top/gtagntyhfl.html

[G08] 静态方法与属性
来源：http://hz.wangdashe.top/gtrvejstkq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.xylfe.cn/gtorxiqwpq.html

PHP:  public static function f() {}
来源：http://hz.cucudq.cn/gttjzrmfhj.html

JS:   static f() {}
来源：http://hz.yj20258888.top/gtzlbhpijf.html

TS:   static f(): void {}
来源：http://hz.xinyue.icu/gtnaxixiva.html

Java: static void f() {}
来源：http://hz.wangshuangyany.cn/gtejdbksas.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.bjfxy.top/gtayvrvmji.html

Ruby: def self.f; end
来源：http://hz.ywan-chungtsiang.top/gtuumvgmqk.html

C#:   public static void F() {}
来源：http://hz.hongshengwenyu.top/gtdalaqvke.html

[G09] 接口 / 抽象类
来源：http://hz.redwolf501.top/gtvdpuuegc.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.xuetiantiany.cn/gtbqqkhgwa.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.svipenyu.cn/gtjhlgnrhn.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.zhoulong.xyz/gtxriefkec.html

TS:   interface Shape { area(): number; }
来源：http://hz.haohaochexian.top/gtvsfrmcen.html

Java: interface Shape { double area(); }
来源：http://hz.pengpengdd.cyou/gtordcnvth.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.shanyushiyangkeji.top/gtdhncbxth.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.meibo888.top/gtohrfzdet.html

C#:   interface IShape { double Area(); }
来源：http://hz.shangyingyoupin.top/gtapdmantx.html

[G10] 访问控制
来源：http://hz.jinghuilouyu.cn/gtgxmpzakw.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yj20258.top/gtytrfeorl.html

PHP:  public / protected / private
来源：http://hz.hfpthk.cn/gtpqkoctpi.html

JS:   #private 字段；其余公开
来源：http://hz.zhongyouzk.top/gtzpulqjmh.html

TS:   public / protected / private
来源：http://hz.sweek.top/gtbqzscers.html

Java: public / protected / private / 默认包级
来源：http://hz.mhx1999.top/gtidxrmgxj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yongpay.top/gtcmzaqkft.html

Ruby: public / protected / private
来源：http://hz.feifeiyinyue.top/gtuvuckqyt.html

C#:   public / protected / private / internal
来源：http://hz.jinqigfzy.top/gtgehtlylf.html

[G11] getter / setter
来源：http://hz.haohaochexian.top/gthcrjoxkg.html

Py:   @property 与 @x.setter
来源：http://hz.yonumen.top/gtddlfgitp.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.tian-w.cn/gtwbzqofqv.html


<!-- 参考信息 -->