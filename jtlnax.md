代发 wailian999

PHP:  substr_count($s, "a");
来源：http://hz.jiagoushi.top/gtegllciyd.html

JS:   s.split("a").length - 1
来源：http://hz.nanxinkj.top/gtpwlymypu.html

TS:   s.split("a").length - 1
来源：http://hz.shangyingyoupin.top/gtajhbavpq.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.c1oappe.top/gturphgyau.html

Go:   strings.Count(s, "a")
来源：http://hz.cashguo.top/gtknwfqdht.html

Ruby: s.count("a")
来源：http://hz.ydjk.org.cn/gtatrhqawh.html

C#:   s.Count(c => c == 'a')
来源：http://hz.nanxuanxn.top/gtqttoehoy.html

[E13] 逐字符遍历
来源：http://hz.xuetiantiany.cn/gtgxrpileh.html

Py:   for ch in s: print(ch)
来源：http://hz.hongshengwenyu.top/gtiyfouldx.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.gzhubu.top/gtdglozixt.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zdqjudy.top/gtprwesbie.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ydjk.org.cn/gtcminasov.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.guowangkeji.top/gtojlcbltx.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.jinqigfzy.top/gtzwrkuinr.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.yonumen.top/gtbcwofigs.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.jianghu66.top/gtbkyhhmid.html

[E14] URL 编码与 Base64
来源：http://hz.ehwqpu.com/gtujjwqeai.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.yanxiufei.cn/gtklnuhlgr.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.shangyingyoupin.top/gteexenqlp.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.shanyushiyangkeji.top/gtbnfurmhw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.birdmap.top/gtreshvwcv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.hfpthk.cn/gtbttsiryy.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.jinghuilouyu.cn/gtdkaqrzux.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.sufxvd.cn/gtrdyaxtdd.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.tianlin.xyz/gtgiivdpma.html

[E15] HTML 转义 / 反转义
来源：http://hz.smart0.xyz/gtdwhndqpr.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.shzxlz.cn/gtbkggwuyy.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.feifeiyinyue.top/gttelcahcw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.xziqi.cn/gtdpqayyfc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.chenlongwang.top/gttwzqstxz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.shuidangran.top/gtznwibstw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.pengpengdd.cyou/gtcpbsrqej.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.vqdsnc.cn/gtftdzwmmm.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.yanxiufei.cn/gtomnvwcid.html

[E16] 数字千分位
来源：http://hz.yj202588.top/gttbrvtpyq.html

Py:   f"{1234567:,}"
来源：http://hz.52xcode.cn/gtihvkllnh.html

PHP:  number_format(1234567);
来源：http://hz.yvedp.cn/gtoxvvuwsh.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.tianlin.xyz/gtywgvxahh.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.xuanzx.com/gtyzgnobtx.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.xziqi.cn/gtrncbwbmp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.zdqjudy.top/gtrjrhiejp.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.chenjidiqi.icu/gtcayiubsr.html

C#:   1234567.ToString("N0")
来源：http://hz.gaohongyu789.top/gtvjefszmq.html

[E17] 首字母大写
来源：http://hz.pengpengdd.cyou/gtxvgjnocn.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.zhixingplan.top/gtejldoiwv.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.zdqjudy.top/gtaznnphtz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jinghuilouyu.cn/gtrrdhowec.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.gotoacloud.top/gtyyfkuwtc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.daria6918.cn/gtiiyvzttk.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.xylfe.cn/gttnyasikn.html

Ruby: s.capitalize
来源：http://hz.chenzaomai.com/gtlrppfmal.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.0kj1m.cn/gtjzxtsflt.html

[E18] 模板占位符替换
来源：http://hz.guannengcc.top/gtkbvoeirr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.gaohongyu789.top/gtunhlfvuz.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.shuidangran.top/gtsxlirxrs.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.jinqigufen.top/gtmrkptyfg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.cqqwz.cn/gtxhiultol.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.jinqigufen.top/gtqpcisvya.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.jyoumei.cn/gtvusbavwm.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.xuetiantiany.cn/gtmrscuasu.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.chenjidiqi.icu/gtoxugvici.html

[E19] 多行文本按行拆分
来源：http://hz.tian-w.cn/gtcgteohet.html

Py:   s.splitlines()
来源：http://hz.pycfn.com/gtrfxdpgbg.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jlsjyb.cn/gtoasyohjq.html

JS:   s.split(/\r?\n/)
来源：http://hz.cdnleiting.top/gtpbwsuwkk.html

TS:   s.split(/\r?\n/)
来源：http://hz.yanxiufei.cn/gthjlgibnv.html

Java: s.lines().toList()
来源：http://hz.hnqzz.top/gtdqvoatxg.html

Go:   strings.Split(s, "\n")
来源：http://hz.sysykeji.top/gtygwcvsky.html

Ruby: s.lines
来源：http://hz.zhiwuduotai.top/gtthlnayqm.html

C#:   s.Split('\n')
来源：http://hz.sufxvd.cn/gtjgbmmgyt.html

[E20] 判断字符串是否为空
来源：http://hz.jinghuilouyu.cn/gtfbadfkpz.html

Py:   if not s:
来源：http://hz.zhengqikj.top/gtnvlnngkk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.yongpay.top/gtbfjsxnyb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.jqgfzy.top/gtpjyckpbf.html

TS:   if (s === "") {}
来源：http://hz.c1oappe.top/gtvdenoycc.html

Java: if (s.isEmpty()) {}
来源：http://hz.yanxiufei.cn/gtwphnzdky.html

Go:   if s == "" {}
来源：http://hz.yanxiufei.cn/gteonpdsni.html

Ruby: if s.empty?
来源：http://hz.ehwqpu.com/gtihehnzub.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.quarkkingdee.top/gttsgocgmw.html

[E21] 超长截断加省略号
来源：http://hz.sweek.top/gttpyrbasf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.gotoacloud.top/gtzvvcskpe.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.jqgufenzy.top/gteavafeba.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.xziqi.cn/gteilbsttd.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.haohaochexian.top/gtwwilercm.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.feifeiyinyue.top/gtsmutisok.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.jinyuanbaomall.cn/gtkasaemuy.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.gogol.net.cn/gtybhxuthe.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.hnxiangtu.top/gtjahvfmds.html

[E22] 字节长度与字符长度
来源：http://hz.9152youxi.cn/gtjulddgtt.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.jinghuilouyu.cn/gtxolzndjl.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.shuidangran.top/gtarxvuamu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.iojbl.cn/gtbmtgnllv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.andypj.xyz/gtxpiwdgdf.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.sufxvd.cn/gthncecpcd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.xinyue.icu/gtvtsfccyk.html

Ruby: s.bytesize;  s.length
来源：http://hz.316326.xyz/gtqlgwyqyd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.ydzc1.top/gtmleelwul.html

================================================================================
来源：http://hz.zhengqikj.top/gtvqufocgz.html

F. 文件与目录
来源：http://hz.hywenlv.cn/gttiyjgnkn.html

================================================================================
来源：http://hz.shuidangran.top/gtyprpgjrc.html

[F01] 读取整个文件
来源：http://hz.yvedp.cn/gtgtngqwcn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.daria6918.cn/gtkevrazom.html

PHP:  file_get_contents("a.txt");
来源：http://hz.zhixingplan.top/gtknigwseh.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.jqgfzy.top/gtpfzpqjkh.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.iojbl.cn/gtxomyfamj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.zhiwuduotai.top/gtyepwmhzz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.gaohongyu789.top/gtczuqwjqm.html

Ruby: File.read("a.txt")
来源：http://hz.tianlin.xyz/gtohjuoywd.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.316326.xyz/gtgklfigwz.html

[F02] 逐行读取文件
来源：http://hz.xylfe.cn/gtcpimigcd.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.yuxming.cn/gtcmjwlqyl.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.ehwqpu.com/gthwcytjvy.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.aizwys.cn/gtcqaetygs.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hnxiangtu.top/gtwsiambla.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.xuanzx.com/gtvodkegcn.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.gotoacloud.top/gtxysmiazn.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.redwolf501.top/gtnxjfubrh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.zhixingplan.top/gtmuwosiis.html

[F03] 写入文件（覆盖）
来源：http://hz.sufxvd.cn/gtwyfmyhui.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.xziqi.cn/gtvgnecujq.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.dashuyun.cn/gtznmftnmx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhongyouzk.top/gtwuiqlyop.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ydzc1.top/gtjsxwgqgo.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.meibo888.top/gtegjzukmi.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.jinqigufen.top/gtlustqujm.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.shzxlz.cn/gtmcrcelek.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.yuanzhike.top/gttborfmzv.html

[F04] 追加写入文件
来源：http://hz.0kj1m.cn/gtrjkxrhvx.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.bjfxy.top/gtpcirujbf.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.ybcxt.top/gtwbqtidgj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yuanzhike.top/gtrpichhff.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.316326.xyz/gttqrojppb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.52xcode.cn/gtwxyzqcvw.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.yj202588.top/gtbuyogoao.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.zdqjudy.top/gtjbpvftdn.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.gotoacloud.top/gtzbrmtdpm.html

[F05] 判断文件或目录是否存在
来源：http://hz.fzhhl.top/gtsaednqff.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.meibo888.top/gtyqcmzpzf.html

PHP:  file_exists("a.txt");
来源：http://hz.shuidangran.top/gtavugtrlt.html

JS:   fs.existsSync("a.txt")
来源：http://hz.cdnleiting.top/gtsvulgnko.html

TS:   fs.existsSync("a.txt")
来源：http://hz.jinqigufen.top/gtuoajebxy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.iojbl.cn/gtjqrribfv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.xinyue.icu/gtrxnojyzk.html

Ruby: File.exist?("a.txt")
来源：http://hz.tanke756.top/gtwtfyqfjz.html

C#:   File.Exists("a.txt")
来源：http://hz.ppjwa.cn/gtiorxazzq.html

[F06] 删除文件
来源：http://hz.52xcode.cn/gtifekyxtd.html

Py:   os.remove("a.txt")
来源：http://hz.shanyushiyangtech.top/gtqgswvymt.html

PHP:  unlink("a.txt");
来源：http://hz.jyoumei.cn/gtdeqvlkks.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.shzxlz.cn/gtminhpcms.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.yangfankeji.com/gtftmzjmso.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.chenjidiqi.icu/gtolxsmtne.html

Go:   os.Remove("a.txt")
来源：http://hz.jqgfzy.top/gtxwowdrer.html

Ruby: File.delete("a.txt")
来源：http://hz.shuidangran.top/gtwcrmmtxl.html

C#:   File.Delete("a.txt");
来源：http://hz.316326.xyz/gtcfmiydmj.html

[F07] 创建目录（含多级）
来源：http://hz.sxryk.cn/gtzqjxefrs.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.wangdashe.top/gtalocxzdv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.jinqigfzy.top/gtwtbtzptj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhaomingkeji.xyz/gtagacdigo.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ppjwa.cn/gtrhfrmyzd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.xziqi.cn/gtbnfxrakt.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.yj20258.top/gtuofnidmw.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.zhoulong.xyz/gtnyfkihlx.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.hammf.cn/gtqxoipamd.html

[F08] 遍历目录
来源：http://hz.ivvv.top/gthqeelsxx.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.birdmap.top/gtuxsenqvo.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.daria6918.cn/gtjlpmsqwb.html

JS:   fs.readdirSync("dir")
来源：http://hz.xingfuxueyuan.xyz/gtlntkhwnc.html

TS:   fs.readdirSync("dir")
来源：http://hz.hysaishi.cn/gtwhztzdkv.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.zycfv.cn/gtjasjchko.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.smart0.xyz/gtmsccpdmm.html

Ruby: Dir.children("dir")
来源：http://hz.smart0.xyz/gtjvwogyks.html

C#:   Directory.GetFiles("dir")
来源：http://hz.meibo888.top/gtsmnfqyot.html

[F09] 获取文件大小
来源：http://hz.wangdashe.top/gtrkstpglv.html

Py:   os.path.getsize("a.txt")
来源：http://hz.shzxlz.cn/gtvmqwejir.html

PHP:  filesize("a.txt");
来源：http://hz.hfpthk.cn/gttegnejui.html

JS:   fs.statSync("a.txt").size
来源：http://hz.0kj1m.cn/gttjxfvlyf.html

TS:   fs.statSync("a.txt").size
来源：http://hz.sufxvd.cn/gtpudhzzjw.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.nwbrower.top/gtmxnhvmrq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.hnqzz.top/gtspouanua.html

Ruby: File.size("a.txt")
来源：http://hz.yangfankeji.com/gtbdeavztu.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.xziqi.cn/gtkizjqsch.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.tanke756.top/gtxqhpjqof.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.zhoulong.xyz/gtipbacygm.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.fengsongda.top/gtpljyvsgp.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.jqgufenzy.top/gtvwzroxid.html

TS:   path.extname("a.txt")
来源：http://hz.cheryme.top/gtxdkwrnzc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.ydzc1.top/gtirniibdl.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.daria6918.cn/gtkganbynn.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.sxryk.cn/gttjkqgnoe.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.ybcxt.top/gtofzlhqpv.html

[F11] 复制与移动文件
来源：http://hz.gaohongyu789.top/gtyzcsmerh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.yangfankeji.com/gtswfuocfa.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.vqdsnc.cn/gtnyxjwhmd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hnqzz.top/gtdzvmwwan.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ybcxt.top/gtbrwzzufh.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.jinyuanbaomall.cn/gtmrcvgvkh.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.snrcjt.cn/gtxfeznekd.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.xingfuxueyuan.xyz/gtzhpijjcr.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.yanxiufei.cn/gtiscpkthe.html

[F12] CSV 读写
来源：http://hz.zhengqikj.top/gtycocmimr.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.yuxming.cn/gtoggneids.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.mhx1999.top/gtflggzvvn.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.shanyushiyangtech.top/gtsclcdett.html

TS:   // 同上
来源：http://hz.shanyushiyangtech.top/gtobvcgtvg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.jinyuanbaomall.cn/gtdmagcigd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.snrcjt.cn/gtlcxvmvuf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.sysykeji.top/gticwwezpw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.tanke756.top/gtrfhoomyk.html

================================================================================
来源：http://hz.shzxlz.cn/gtcuiydrrw.html

G. 面向对象
来源：http://hz.wangdashe.top/gtizspxihd.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtvoosuhkd.html

[G01] 定义类
来源：http://hz.hfpthk.cn/gtguyktmjq.html

Py:   class User: pass
来源：http://hz.jinyuanbaomall.cn/gthdjuzqdu.html

PHP:  class User {}
来源：http://hz.cucudq.cn/gtiyngisvg.html

JS:   class User {}
来源：http://hz.316326.xyz/gthkndkpue.html

TS:   class User { name: string = ""; }
来源：http://hz.xziqi.cn/gtiambkvhy.html

Java: class User {}
来源：http://hz.chenzaomai.com/gtgadhgjrl.html

Go:   type User struct { Name string }
来源：http://hz.xingfuxueyuan.xyz/gtmrefhsou.html

Ruby: class User; end
来源：http://hz.feifeiyinyue.top/gtwkirpfbh.html

C#:   class User {}
来源：http://hz.jinqigufen.top/gtekmodwzw.html

[G02] 构造函数
来源：http://hz.vqdsnc.cn/gtjytzdnql.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zhongyouzk.top/gtjsoluftg.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.nwbrower.top/gtzmiyrmat.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.jianghu66.top/gtlyqgxiny.html

TS:   constructor(public name: string) {}
来源：http://hz.ywan-chungtsiang.top/gtlxptmbai.html

Java: User(String name) { this.name = name; }
来源：http://hz.wangshuangyany.cn/gtquwhuisk.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.fengsongda.top/gtxepuhmte.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.zhaomingkeji.xyz/gtozpapphv.html

C#:   public User(string name) { Name = name; }
来源：http://hz.c1oappe.top/gtukhupkso.html

[G03] 实例属性
来源：http://hz.haohaochexian.top/gtobyuinyg.html

Py:   self.name = "x"
来源：http://hz.xuetiantiany.cn/gtfpbzjxli.html

PHP:  public string $name = "x";
来源：http://hz.tian-w.cn/gtsapnrbcg.html

JS:   this.name = "x";
来源：http://hz.shanyushiyangkeji.top/gthujzdegl.html

TS:   name: string = "x";
来源：http://hz.52xcode.cn/gthafjzzgn.html

Java: private String name;
来源：http://hz.bjfxy.top/gtrimevlok.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.aibaodan.cn/gtvvwjbjcu.html

Ruby: @name = "x"
来源：http://hz.aizwys.cn/gtkxqueorq.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.sysykeji.top/gtxqdezorp.html

[G04] 定义方法
来源：http://hz.yonumen.top/gtqdekrxxv.html

Py:   def greet(self): return self.name
来源：http://hz.zhiwuduotai.top/gtxqelcfru.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.jqgfzy.top/gtksimepqm.html

JS:   greet() { return this.name; }
来源：http://hz.yj202588.top/gtemesoqsf.html

TS:   greet(): string { return this.name; }
来源：http://hz.c1oappe.top/gtdnxsugux.html

Java: String greet() { return name; }
来源：http://hz.xylfe.cn/gtvraqwrgr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.kuanghao11.cn/gtemxxugjc.html

Ruby: def greet; @name; end
来源：http://hz.meibo888.top/gtmygeilcz.html

C#:   public string Greet() => Name;
来源：http://hz.hnqzz.top/gtvskquikw.html

[G05] 继承
来源：http://hz.xziqi.cn/gtecljiwwi.html

Py:   class Admin(User): pass
来源：http://hz.guannengcc.top/gtlurqrwbx.html

PHP:  class Admin extends User {}
来源：http://hz.fzhhl.top/gtyrokhncm.html

JS:   class Admin extends User {}
来源：http://hz.yj202588.top/gtbkfajziv.html

TS:   class Admin extends User {}
来源：http://hz.jianghu66.top/gtydktrshz.html

Java: class Admin extends User {}
来源：http://hz.zdqjudy.top/gtjedqhnqi.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yuxming.cn/gttiyhgwzs.html

Ruby: class Admin < User; end
来源：http://hz.dianchejie.cn/gtcyfedkhv.html

C#:   class Admin : User {}
来源：http://hz.mhx1999.top/gttrtmjnay.html

[G06] 重写方法
来源：http://hz.aizwys.cn/gtoufoiplt.html

Py:   def greet(self): return "admin"
来源：http://hz.jqgufenzy.top/gtayvxpelt.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.chenzaomai.com/gtktqecxlh.html

JS:   greet() { return "admin"; }
来源：http://hz.xinyue.icu/gtubmyroby.html

TS:   greet(): string { return "admin"; }
来源：http://hz.yanxiufei.cn/gthlfptqmp.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.zhiwuduotai.top/gtohxwmjna.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.jyoumei.cn/gtyvjjvffr.html

Ruby: def greet; "admin"; end
来源：http://hz.fengsongda.top/gtrmnvrohv.html

C#:   public override string Greet() => "admin";
来源：http://hz.zhixingplan.top/gtcgwwhwvu.html

[G07] 调用父类方法
来源：http://hz.shzxlz.cn/gtyrbghhtp.html

Py:   super().greet()
来源：http://hz.jinghuilouyu.cn/gttjkdsaun.html

PHP:  parent::greet();
来源：http://hz.chenzaomai.com/gthusxyips.html

JS:   super.greet();
来源：http://hz.havefunace.top/gtbzblcxhu.html

TS:   super.greet();
来源：http://hz.nanxuanxn.top/gtepdmmeqr.html

Java: super.greet();
来源：http://hz.sysykeji.top/gtzzbzyltz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.nanxinkj.top/gthaiydcim.html

Ruby: super
来源：http://hz.aizwys.cn/gtzrvxhrta.html

C#:   base.Greet();
来源：http://hz.bjfxy.top/gtzlbmwkhc.html

[G08] 静态方法与属性
来源：http://hz.ydjk.org.cn/gtocqiehng.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.xuetiantiany.cn/gtwodbgwqi.html

PHP:  public static function f() {}
来源：http://hz.yuanzhike.top/gtmxgidvii.html

JS:   static f() {}
来源：http://hz.tanke756.top/gtfmzhrjbo.html

TS:   static f(): void {}
来源：http://hz.ivvv.top/gtimgkjsoj.html

Java: static void f() {}
来源：http://hz.wangshuangyany.cn/gttoxddykk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.snrcjt.cn/gtkzlsdexc.html

Ruby: def self.f; end
来源：http://hz.zhaomingkeji.xyz/gtgztxnbkb.html

C#:   public static void F() {}
来源：http://hz.wangshuangyany.cn/gttyhkahyp.html

[G09] 接口 / 抽象类
来源：http://hz.andypj.xyz/gtxpilhsyo.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.jinqigfzy.top/gtbiycjrva.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jyoumei.cn/gtrijyhtqu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.jinqigfzy.top/gtfkgovplb.html

TS:   interface Shape { area(): number; }
来源：http://hz.yongpay.top/gtzzpgkisn.html

Java: interface Shape { double area(); }
来源：http://hz.feifeiyinyue.top/gtakawuqzr.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.meibo888.top/gtjofnxmaf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yonumen.top/gtwxvuiakp.html

C#:   interface IShape { double Area(); }
来源：http://hz.yongpay.top/gtvbyhhhgw.html

[G10] 访问控制
来源：http://hz.fengsongda.top/gtfmrmocws.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.xylfe.cn/gtauomncow.html

PHP:  public / protected / private
来源：http://hz.quarkkingdee.top/gtooogebio.html

JS:   #private 字段；其余公开
来源：http://hz.snrcjt.cn/gtvhntdomz.html

TS:   public / protected / private
来源：http://hz.hysaishi.cn/gtnqvqtefy.html

Java: public / protected / private / 默认包级
来源：http://hz.birdmap.top/gtmlqqcpgj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.cashguo.top/gttsykbkrc.html

Ruby: public / protected / private
来源：http://hz.mhx1999.top/gtelxdhzak.html


<!-- 参考信息 -->