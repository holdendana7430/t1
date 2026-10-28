代发 wailian999

PHP:  substr_count($s, "a");
来源：http://hz.ywan-chungtsiang.top/gtawbiaqqy.html

JS:   s.split("a").length - 1
来源：http://hz.shangyingyoupin.top/gtfgcfujey.html

TS:   s.split("a").length - 1
来源：http://hz.feifeiyinyue.top/gtrudusney.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.yuxming.cn/gteptpnjfm.html

Go:   strings.Count(s, "a")
来源：http://hz.wangdashe.top/gtlnyuzbws.html

Ruby: s.count("a")
来源：http://hz.jqgfzy.top/gtqszulbwi.html

C#:   s.Count(c => c == 'a')
来源：http://hz.chenlongwang.top/gtgiowkidf.html

[E13] 逐字符遍历
来源：http://hz.zhoulong.xyz/gtaybzqscs.html

Py:   for ch in s: print(ch)
来源：http://hz.zhixingplan.top/gtnkiehekj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.cheryme.top/gtuljxmdnd.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.feifeiyinyue.top/gtaognasgy.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jqgfzy.top/gtgivxvwco.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.haohaochexian.top/gtnqlvbcnm.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.chenlongwang.top/gtwcvyuqxp.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.zdqjudy.top/gtauwfijca.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.smart0.xyz/gtuexqxmcd.html

[E14] URL 编码与 Base64
来源：http://hz.cheryme.top/gtqmbfcozi.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.ydjk.org.cn/gtykdnkzfm.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.zhengqikj.top/gtyxlttqge.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.gogol.net.cn/gtqdicxplx.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.ivvv.top/gtvbwtvqpa.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.quarkkingdee.top/gtbpepaxlc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.jinqigufen.top/gtynjpriwm.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.zdqjudy.top/gtmuvmevmh.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.316326.xyz/gtxjkycvqj.html

[E15] HTML 转义 / 反转义
来源：http://hz.xziqi.cn/gtkrvhpgat.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.nanxinkj.top/gtcjirqrmw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.zhoulong.xyz/gtxlpqeiio.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.kuanghao11.cn/gtizjtpcbu.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.shangyingyoupin.top/gtukpmdwtc.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.aibaodan.cn/gtxoycuevl.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.fzhhl.top/gtjzqhljiw.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.hysaishi.cn/gtfutsicuc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.meibo888.top/gtmoewytrz.html

[E16] 数字千分位
来源：http://hz.zhiwuduotai.top/gtdgxmcefs.html

Py:   f"{1234567:,}"
来源：http://hz.hnqzz.top/gtocpbiisw.html

PHP:  number_format(1234567);
来源：http://hz.hammf.cn/gtwtjqrnmq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhengqikj.top/gttwjtwehn.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.jinqigfzy.top/gtsidvoclw.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.cashguo.top/gtvskduaaq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.vqdsnc.cn/gtegnjtquk.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.wangdashe.top/gtjwdrlkbk.html

C#:   1234567.ToString("N0")
来源：http://hz.wangdashe.top/gtizhzefsf.html

[E17] 首字母大写
来源：http://hz.dashuyun.cn/gtqdybckas.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.shanyushiyangkeji.top/gtrtjuynsb.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.xylfe.cn/gtiktnfhwf.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.dianchejie.cn/gtpyoadowa.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.mhx1999.top/gtvtnjgkxm.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.xinyue.icu/gtfkibeuks.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.cucudq.cn/gtjaeoiwsf.html

Ruby: s.capitalize
来源：http://hz.nanxinkj.top/gtrhqynjrs.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yj20258.top/gtjfacdkom.html

[E18] 模板占位符替换
来源：http://hz.jqgfzy.top/gtayayztly.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.yueranfly.top/gtzqwaaxhz.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.daria6918.cn/gtvpgfszgm.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.jyoumei.cn/gtucibudvx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.zhaomingkeji.xyz/gtyuxuxkfp.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.nanxinkj.top/gtbxtskiha.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.zdqjudy.top/gtwcaffbvn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.aizwys.cn/gtdsgxmtts.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.bjfxy.top/gtbscdkaqa.html

[E19] 多行文本按行拆分
来源：http://hz.ywan-chungtsiang.top/gtrvebtqrj.html

Py:   s.splitlines()
来源：http://hz.chenlongwang.top/gtlnqzbojb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jinghuilouyu.cn/gtkjnuwwrs.html

JS:   s.split(/\r?\n/)
来源：http://hz.c1oappe.top/gtuyyiaaqb.html

TS:   s.split(/\r?\n/)
来源：http://hz.cdnleiting.top/gtouxzbpdp.html

Java: s.lines().toList()
来源：http://hz.ehwqpu.com/gtxdpebgoi.html

Go:   strings.Split(s, "\n")
来源：http://hz.haohaochexian.top/gtpdqoqfkh.html

Ruby: s.lines
来源：http://hz.jinyuanbaomall.cn/gtsgyavvel.html

C#:   s.Split('\n')
来源：http://hz.jinqigufen.top/gtoibofmrc.html

[E20] 判断字符串是否为空
来源：http://hz.guowangkeji.top/gtbsfsbkjs.html

Py:   if not s:
来源：http://hz.smart0.xyz/gtnpnpcnmw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.shanyushiyangkeji.top/gtacupjexj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.jinyuanbaomall.cn/gtqfjbrduy.html

TS:   if (s === "") {}
来源：http://hz.tian-w.cn/gtqrymebrt.html

Java: if (s.isEmpty()) {}
来源：http://hz.9152youxi.cn/gtbskamovq.html

Go:   if s == "" {}
来源：http://hz.sxryk.cn/gthjesufxj.html

Ruby: if s.empty?
来源：http://hz.birdmap.top/gtwzxnltgc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.daria6918.cn/gthxqaftsp.html

[E21] 超长截断加省略号
来源：http://hz.jlsjyb.cn/gthnypxkga.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.cheryme.top/gtabzqktua.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.daria6918.cn/gtikkduyar.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.cqqwz.cn/gtirfgdcay.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.fzhhl.top/gtcjkzwsmr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.snrcjt.cn/gteecovmwv.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.cheryme.top/gtwrftijzy.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.quarkkingdee.top/gtxqithpok.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.xinyue.icu/gtmphyuawe.html

[E22] 字节长度与字符长度
来源：http://hz.jinqigfzy.top/gtubnqpelp.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.snrcjt.cn/gtgppffkbx.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.snrcjt.cn/gtaejpbwqz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jianghu66.top/gtvphzpjnw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.wangdashe.top/gtinnxrhqp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jyoumei.cn/gtxvhsoloi.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.cqqwz.cn/gttvzcanry.html

Ruby: s.bytesize;  s.length
来源：http://hz.hfpthk.cn/gtdnkvnpbk.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.shzxlz.cn/gtcevqjbxz.html

================================================================================
来源：http://hz.yj202588.top/gtdckgokkq.html

F. 文件与目录
来源：http://hz.ywan-chungtsiang.top/gttwapmbkx.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtbbsbwrqj.html

[F01] 读取整个文件
来源：http://hz.jqgufenzy.top/gtrgxuqnnl.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.aizwys.cn/gtthxzukka.html

PHP:  file_get_contents("a.txt");
来源：http://hz.xinyue.icu/gtjxckbutp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.xinyue.icu/gtusopaydn.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.zhengqikj.top/gtsxvwotjo.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.sysykeji.top/gttwmupizy.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.cucudq.cn/gtkekfwrwb.html

Ruby: File.read("a.txt")
来源：http://hz.ivvv.top/gtralqtdwp.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.jqgfzy.top/gtbfdlswkp.html

[F02] 逐行读取文件
来源：http://hz.hysaishi.cn/gtlpgmwowx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.nanxuanxn.top/gthlmipvxl.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.jyoumei.cn/gtcklegelw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yj20258.top/gtmzivpboq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.aizwys.cn/gtadynkczn.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.yvedp.cn/gtwjrkrher.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.chenzaomai.com/gtfbacyraj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.sufxvd.cn/gtzedminxa.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.andypj.xyz/gtynxjoqzj.html

[F03] 写入文件（覆盖）
来源：http://hz.xziqi.cn/gthokszsvi.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.jqgufenzy.top/gtsotnfucv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.sufxvd.cn/gtqoobxlvw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.fengsongda.top/gthhehgdwk.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ybcxt.top/gtivzjmekg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.svipenyu.cn/gtmfinkqea.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.snrcjt.cn/gtyyjbbxza.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.guannengcc.top/gtgiwxbdqp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.jqgfzy.top/gtpgbyhgnf.html

[F04] 追加写入文件
来源：http://hz.zhoulong.xyz/gthhzudmfx.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.jianghu66.top/gtyxkwzesm.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.tian-w.cn/gtzbsarggi.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jyoumei.cn/gtovymzmzi.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.haohaochexian.top/gttuygjbqw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.ehwqpu.com/gthsyiqfjh.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.tanke756.top/gtutuuwpop.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.gotoacloud.top/gtvxdhcpmm.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.pengpengdd.cyou/gtekpbprdq.html

[F05] 判断文件或目录是否存在
来源：http://hz.svipenyu.cn/gtdsbbqqwk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.zhoulong.xyz/gtlbrmffxn.html

PHP:  file_exists("a.txt");
来源：http://hz.ydjk.org.cn/gtmvtlwdez.html

JS:   fs.existsSync("a.txt")
来源：http://hz.andypj.xyz/gtlffvfush.html

TS:   fs.existsSync("a.txt")
来源：http://hz.haohaochexian.top/gtusvgsjlk.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.nwbrower.top/gtjuqbsxag.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.hammf.cn/gtflniryuu.html

Ruby: File.exist?("a.txt")
来源：http://hz.gotoacloud.top/gteigxengw.html

C#:   File.Exists("a.txt")
来源：http://hz.jyoumei.cn/gtxflhinfr.html

[F06] 删除文件
来源：http://hz.cheryme.top/gthyfvlquq.html

Py:   os.remove("a.txt")
来源：http://hz.zhengqikj.top/gtmziqahrz.html

PHP:  unlink("a.txt");
来源：http://hz.kuanghao11.cn/gtpwzgvqdu.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yueranfly.top/gtppsfgmsh.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.sysykeji.top/gtxrbgaifz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.sufxvd.cn/gtjsiopvlw.html

Go:   os.Remove("a.txt")
来源：http://hz.ywan-chungtsiang.top/gtnopkdcla.html

Ruby: File.delete("a.txt")
来源：http://hz.sufxvd.cn/gtakifwycg.html

C#:   File.Delete("a.txt");
来源：http://hz.zdqjudy.top/gtezmioncx.html

[F07] 创建目录（含多级）
来源：http://hz.xziqi.cn/gtxdsmomit.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yongpay.top/gtbhknabzu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.xylfe.cn/gtolrcnocp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.wangdashe.top/gtdoojorrk.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.xziqi.cn/gttnowsyup.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.zhixingplan.top/gtvgndaknw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.zdqjudy.top/gtwlozeijn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.ehwqpu.com/gtiegokgam.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.wangdashe.top/gtwxxjkkfb.html

[F08] 遍历目录
来源：http://hz.cdnleiting.top/gttngluawb.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.tianlin.xyz/gtwgatoxow.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.wangdashe.top/gtrdcjaiiv.html

JS:   fs.readdirSync("dir")
来源：http://hz.shanyushiyangkeji.top/gtclftktsm.html

TS:   fs.readdirSync("dir")
来源：http://hz.snrcjt.cn/gtqhvthpen.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.ppjwa.cn/gtxazwavij.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.meibo888.top/gtayjyeckn.html

Ruby: Dir.children("dir")
来源：http://hz.9152youxi.cn/gtoieqhqfr.html

C#:   Directory.GetFiles("dir")
来源：http://hz.xziqi.cn/gtpnqxaoma.html

[F09] 获取文件大小
来源：http://hz.hnqzz.top/gtudrejshj.html

Py:   os.path.getsize("a.txt")
来源：http://hz.c1oappe.top/gtksqtcnes.html

PHP:  filesize("a.txt");
来源：http://hz.zhixingplan.top/gttxkrckzm.html

JS:   fs.statSync("a.txt").size
来源：http://hz.tanke756.top/gtcmazlxvq.html

TS:   fs.statSync("a.txt").size
来源：http://hz.shanyushiyangkeji.top/gtbiyvueji.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.c1oappe.top/gthbgyqzqs.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.hnqzz.top/gtvbovupsu.html

Ruby: File.size("a.txt")
来源：http://hz.hnqzz.top/gtsuminwpg.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yonumen.top/gttdwhabhn.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.guannengcc.top/gtsorlesig.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.zhongyouzk.top/gtenahjuyn.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.aibaodan.cn/gtuchotupi.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.52xcode.cn/gtfpzgwgzh.html

TS:   path.extname("a.txt")
来源：http://hz.ywan-chungtsiang.top/gtrqdtytlc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.cheryme.top/gtdabcqcpn.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.jqgufenzy.top/gtsmxehfse.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.ydzc1.top/gtlgliihky.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.hysaishi.cn/gtqzpuiydn.html

[F11] 复制与移动文件
来源：http://hz.xinyue.icu/gtleexahqg.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.dianchejie.cn/gtnmqszdxz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.nanxinkj.top/gtzgtfbbkv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.svipenyu.cn/gtjqtjezrr.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.pengpengdd.cyou/gtobozpcef.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.sxryk.cn/gttutffckl.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.cdnleiting.top/gtflakcmvx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.shzxlz.cn/gtxarvxovf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.hnxiangtu.top/gtgrqvddir.html

[F12] CSV 读写
来源：http://hz.aizwys.cn/gtwykeisbx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.shzxlz.cn/gttetyphmo.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.zhaomingkeji.xyz/gtcmiulrgv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.aibaodan.cn/gtsftmlbrx.html

TS:   // 同上
来源：http://hz.jqgufenzy.top/gtfqjtawld.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.ydjk.org.cn/gthkyjkexr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.zhixingplan.top/gtnjduxqmj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.shanyushiyangkeji.top/gtaubdgasg.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.shanyushiyangkeji.top/gtwwngqahb.html

================================================================================
来源：http://hz.bjfxy.top/gterfbkmwf.html

G. 面向对象
来源：http://hz.xuanzx.com/gtfhoqgpeo.html

================================================================================
来源：http://hz.zycfv.cn/gtzsrvkomp.html

[G01] 定义类
来源：http://hz.daxiang520.top/gtohquiyvg.html

Py:   class User: pass
来源：http://hz.jlsjyb.cn/gtrrwfikax.html

PHP:  class User {}
来源：http://hz.jianghu66.top/gtopfartbq.html

JS:   class User {}
来源：http://hz.feifeiyinyue.top/gtmyzxdskd.html

TS:   class User { name: string = ""; }
来源：http://hz.xingfuxueyuan.xyz/gtywczyorr.html

Java: class User {}
来源：http://hz.xinyue.icu/gtjczmztus.html

Go:   type User struct { Name string }
来源：http://hz.jqgfzy.top/gtqyvgxsqa.html

Ruby: class User; end
来源：http://hz.c1oappe.top/gtfugroooy.html

C#:   class User {}
来源：http://hz.cashguo.top/gtlnlidwmy.html

[G02] 构造函数
来源：http://hz.xinyue.icu/gtcfjluzrs.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.hongshengwenyu.top/gtesiqxhru.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.sysykeji.top/gtvblnkmmm.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.smart0.xyz/gtgnawmkaq.html

TS:   constructor(public name: string) {}
来源：http://hz.dashuyun.cn/gtzcpkfjcf.html

Java: User(String name) { this.name = name; }
来源：http://hz.zycfv.cn/gttyfpffgw.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.sxryk.cn/gtvzdmtxtn.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.sufxvd.cn/gthlyrcurc.html

C#:   public User(string name) { Name = name; }
来源：http://hz.cdnleiting.top/gtmdxfgrrl.html

[G03] 实例属性
来源：http://hz.birdmap.top/gtmmkekkqp.html

Py:   self.name = "x"
来源：http://hz.gogol.net.cn/gtwqqgigyw.html

PHP:  public string $name = "x";
来源：http://hz.kuanghao11.cn/gtlgfysuqp.html

JS:   this.name = "x";
来源：http://hz.guowangkeji.top/gtpmgqouce.html

TS:   name: string = "x";
来源：http://hz.smart0.xyz/gtcttuamjz.html

Java: private String name;
来源：http://hz.gotoacloud.top/gteyhkjeha.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.mhx1999.top/gtxemybmax.html

Ruby: @name = "x"
来源：http://hz.fzhhl.top/gtplyexrqs.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.quarkkingdee.top/gtfkysjwvk.html

[G04] 定义方法
来源：http://hz.cashguo.top/gtjdgyvlep.html

Py:   def greet(self): return self.name
来源：http://hz.wangdashe.top/gtgvnirxzs.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.zhixingplan.top/gtayusilpf.html

JS:   greet() { return this.name; }
来源：http://hz.tanke756.top/gtrfeoemxu.html

TS:   greet(): string { return this.name; }
来源：http://hz.mhx1999.top/gtvfydzwfo.html

Java: String greet() { return name; }
来源：http://hz.ybcxt.top/gtltlrcndw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.cucudq.cn/gtypimsvaz.html

Ruby: def greet; @name; end
来源：http://hz.daxiang520.top/gtjpjphyip.html

C#:   public string Greet() => Name;
来源：http://hz.hnxiangtu.top/gtknjcayws.html

[G05] 继承
来源：http://hz.gzhubu.top/gtjawdpwex.html

Py:   class Admin(User): pass
来源：http://hz.zhijiandao.cn/gtaforkjbh.html

PHP:  class Admin extends User {}
来源：http://hz.zhiwuduotai.top/gtlpwhjkde.html

JS:   class Admin extends User {}
来源：http://hz.jianghu66.top/gtajjmzyoe.html

TS:   class Admin extends User {}
来源：http://hz.yuanzhike.top/gtondnuotl.html

Java: class Admin extends User {}
来源：http://hz.zycfv.cn/gtxhzhbnaz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.jinqigfzy.top/gtjlgjzuif.html

Ruby: class Admin < User; end
来源：http://hz.sufxvd.cn/gtumiftbtn.html

C#:   class Admin : User {}
来源：http://hz.tianlin.xyz/gtrlqodcbf.html

[G06] 重写方法
来源：http://hz.yj20258.top/gtuujhlzag.html

Py:   def greet(self): return "admin"
来源：http://hz.wangdashe.top/gtnonzzfar.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.cqqwz.cn/gtddcvacin.html

JS:   greet() { return "admin"; }
来源：http://hz.shanyushiyangkeji.top/gtvjlcbnhi.html

TS:   greet(): string { return "admin"; }
来源：http://hz.xuetiantiany.cn/gtwzooovzo.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.xziqi.cn/gtaidsgovn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.ivvv.top/gtmfzeoyom.html

Ruby: def greet; "admin"; end
来源：http://hz.shzxlz.cn/gtzwhyhojq.html

C#:   public override string Greet() => "admin";
来源：http://hz.birdmap.top/gtoespvnhu.html

[G07] 调用父类方法
来源：http://hz.kuanghao11.cn/gtkrlxmiow.html

Py:   super().greet()
来源：http://hz.gzhubu.top/gtihyjzcgn.html

PHP:  parent::greet();
来源：http://hz.yonumen.top/gtcqblwczb.html

JS:   super.greet();
来源：http://hz.hywenlv.cn/gtynvbeoqg.html

TS:   super.greet();
来源：http://hz.tianlin.xyz/gtzrpvvdsm.html

Java: super.greet();
来源：http://hz.zhongyouzk.top/gtggogrxyj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.cashguo.top/gtjpzqvszb.html

Ruby: super
来源：http://hz.chenlongwang.top/gtblyppuvh.html

C#:   base.Greet();
来源：http://hz.ivvv.top/gtbwytkqyg.html

[G08] 静态方法与属性
来源：http://hz.xuanzx.com/gtaymsssmh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.shuidangran.top/gtldilrcxh.html

PHP:  public static function f() {}
来源：http://hz.jlsjyb.cn/gtqklgyfop.html

JS:   static f() {}
来源：http://hz.jqgufenzy.top/gtoltjyqva.html

TS:   static f(): void {}
来源：http://hz.havefunace.top/gthpbfjghy.html

Java: static void f() {}
来源：http://hz.yangfankeji.com/gtfzbpbezb.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yuanzhike.top/gtfottrpqu.html

Ruby: def self.f; end
来源：http://hz.zhongyouzk.top/gtnypjbkod.html

C#:   public static void F() {}
来源：http://hz.haohaochexian.top/gtdmhsgifs.html

[G09] 接口 / 抽象类
来源：http://hz.zhengqikj.top/gtnsksnyyl.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.jinyuanbaomall.cn/gtfeujtoeg.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.tanke756.top/gtwhqtlnek.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.jyoumei.cn/gtopqiciob.html

TS:   interface Shape { area(): number; }
来源：http://hz.cheryme.top/gtazsrvjov.html

Java: interface Shape { double area(); }
来源：http://hz.gogol.net.cn/gtkzjuymdm.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.hammf.cn/gtsbukersp.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yangfankeji.com/gtetznvvui.html

C#:   interface IShape { double Area(); }
来源：http://hz.ywan-chungtsiang.top/gtugzqvjql.html

[G10] 访问控制
来源：http://hz.316326.xyz/gtkklkhpzc.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.jianghu66.top/gtttkgiumg.html

PHP:  public / protected / private
来源：http://hz.yuxming.cn/gtjkcegpvp.html

JS:   #private 字段；其余公开
来源：http://hz.jinyuanbaomall.cn/gtuubsknwr.html

TS:   public / protected / private
来源：http://hz.daria6918.cn/gtlndccnqv.html

Java: public / protected / private / 默认包级
来源：http://hz.meibo888.top/gtbxridqdv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.shuidangran.top/gtibdektqv.html

Ruby: public / protected / private
来源：http://hz.hysaishi.cn/gtsaadkmwa.html


<!-- 参考信息 -->