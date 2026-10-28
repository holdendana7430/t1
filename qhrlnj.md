代发 wailian999

JS:   [...s].reverse().join("")
来源：http://hz.dashuyun.cn/gtixkwxwfe.html

TS:   [...s].reverse().join("")
来源：http://hz.9152youxi.cn/gtnkfjidqu.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.yuanzhike.top/gtqdpefmkx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.wangdashe.top/gtjuiqowjw.html

Ruby: s.reverse
来源：http://hz.shangyingyoupin.top/gtmuqovohh.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.xuetiantiany.cn/gtyfptthfn.html

[E12] 统计某字符出现次数
来源：http://hz.jinghuilouyu.cn/gtzjqpemmm.html

Py:   s.count("a")
来源：http://hz.xziqi.cn/gtiicgiesi.html

PHP:  substr_count($s, "a");
来源：http://hz.zhaomingkeji.xyz/gtxtdudkzo.html

JS:   s.split("a").length - 1
来源：http://hz.havefunace.top/gtwsgbpkza.html

TS:   s.split("a").length - 1
来源：http://hz.yuxming.cn/gtxdpvpkak.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.guowangkeji.top/gtbeoxpnxb.html

Go:   strings.Count(s, "a")
来源：http://hz.zycfv.cn/gtycdbawhd.html

Ruby: s.count("a")
来源：http://hz.zhoulong.xyz/gtuwlglwmt.html

C#:   s.Count(c => c == 'a')
来源：http://hz.zhaomingkeji.xyz/gtgwkhlloo.html

[E13] 逐字符遍历
来源：http://hz.sysykeji.top/gtbeotkelx.html

Py:   for ch in s: print(ch)
来源：http://hz.xuetiantiany.cn/gtvnvrpkgh.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.feifeiyinyue.top/gtatduflrm.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.quarkkingdee.top/gtevqvmzog.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.feifeiyinyue.top/gtlplhqhut.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.tian-w.cn/gtxzycayvj.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.gotoacloud.top/gtjyaahidx.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.sweek.top/gtbevigwck.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.jqgufenzy.top/gtnumokktq.html

[E14] URL 编码与 Base64
来源：http://hz.tianlin.xyz/gtzcplszkx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.guannengcc.top/gtyvooeztb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.aizwys.cn/gtypwfupeh.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.tianlin.xyz/gtqvzvgijz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.iojbl.cn/gtmwsqcapx.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.sweek.top/gthfwoumep.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.wangshuangyany.cn/gtnurvtilb.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.vqdsnc.cn/gtuorijbzh.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yangfankeji.com/gttikdxdja.html

[E15] HTML 转义 / 反转义
来源：http://hz.yj20258.top/gtbbracgto.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.sufxvd.cn/gtvmulxfrx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.cashguo.top/gtydrpobtw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.52xcode.cn/gtbjiijamk.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.jyoumei.cn/gtbcinrrik.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.ehwqpu.com/gtgxlritlj.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.shangyingyoupin.top/gtrvvuoncs.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.yangfankeji.com/gtzwtiugbi.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.jlsjyb.cn/gtxvvzgvpt.html

[E16] 数字千分位
来源：http://hz.zhongyouzk.top/gtmmzqhrlx.html

Py:   f"{1234567:,}"
来源：http://hz.aizwys.cn/gtnxiqqljw.html

PHP:  number_format(1234567);
来源：http://hz.andypj.xyz/gtxazffevl.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.ydzc1.top/gtvpwmfcat.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.xuetiantiany.cn/gtkewvdqdq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.gzhubu.top/gtncsrzcdn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.zhiwuduotai.top/gtygcswobd.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.zhiwuduotai.top/gthqxieevi.html

C#:   1234567.ToString("N0")
来源：http://hz.yongpay.top/gtcfwtpsbv.html

[E17] 首字母大写
来源：http://hz.jqgfzy.top/gtwyikosnj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.yonumen.top/gtuqspqsbj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.yuanzhike.top/gtswshcjjr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.xylfe.cn/gtupabkuog.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.shanyushiyangtech.top/gteiigdfrv.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.daria6918.cn/gtskwdqyek.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.xingfuxueyuan.xyz/gtqfcmormo.html

Ruby: s.capitalize
来源：http://hz.yueranfly.top/gtggemqlxm.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.hfpthk.cn/gtplwboexp.html

[E18] 模板占位符替换
来源：http://hz.zhengqikj.top/gtrkfvhylp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.tianlin.xyz/gtubhyoqkd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.hywenlv.cn/gtohedokml.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.shanyushiyangkeji.top/gtwdcywoaj.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.yonumen.top/gteivtwlcz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.yanxiufei.cn/gtqszgwbwg.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.kuanghao11.cn/gtdmrhpxex.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.jinqigufen.top/gtlzpkssak.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.zycfv.cn/gtumffzcfz.html

[E19] 多行文本按行拆分
来源：http://hz.xinyue.icu/gtxwyyuxnt.html

Py:   s.splitlines()
来源：http://hz.yuxming.cn/gtkamnilba.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.haohaochexian.top/gtfjajwgyl.html

JS:   s.split(/\r?\n/)
来源：http://hz.aizwys.cn/gtodwgnwrf.html

TS:   s.split(/\r?\n/)
来源：http://hz.mhx1999.top/gtcadolpac.html

Java: s.lines().toList()
来源：http://hz.svipenyu.cn/gtvspabqgu.html

Go:   strings.Split(s, "\n")
来源：http://hz.fzhhl.top/gtzbpjnzyi.html

Ruby: s.lines
来源：http://hz.jinqigufen.top/gtizpqyhuj.html

C#:   s.Split('\n')
来源：http://hz.jinghuilouyu.cn/gtshgahwcz.html

[E20] 判断字符串是否为空
来源：http://hz.jqgfzy.top/gtkfrgctlw.html

Py:   if not s:
来源：http://hz.cheryme.top/gtsfbemkzy.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.sxryk.cn/gtshecfhuy.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.shangyingyoupin.top/gtkwntmmit.html

TS:   if (s === "") {}
来源：http://hz.dashuyun.cn/gtfirtcmud.html

Java: if (s.isEmpty()) {}
来源：http://hz.hnqzz.top/gtwebrfwsi.html

Go:   if s == "" {}
来源：http://hz.dashuyun.cn/gtlgsbvteu.html

Ruby: if s.empty?
来源：http://hz.yj20258.top/gttenxhqvi.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.feifeiyinyue.top/gtabkbzube.html

[E21] 超长截断加省略号
来源：http://hz.yueranfly.top/gtmpfsqecq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.jinyuanbaomall.cn/gthrmxwuzx.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.aibaodan.cn/gttoicmwhf.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jiagoushi.top/gteksztnif.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.pengpengdd.cyou/gttazwrxnb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.gotoacloud.top/gtsjhpzety.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.bjfxy.top/gtgssmddns.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.jlsjyb.cn/gtsmeyzjjs.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.tian-w.cn/gtljxibdfp.html

[E22] 字节长度与字符长度
来源：http://hz.yuxming.cn/gtnliuhrkv.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.havefunace.top/gtrdbzpvuw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.guannengcc.top/gtwzhpqfdm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.nanxinkj.top/gtekvgpqbm.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jinyuanbaomall.cn/gttftokezm.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.shanyushiyangkeji.top/gtlcanhhvq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.52xcode.cn/gtiumccyjt.html

Ruby: s.bytesize;  s.length
来源：http://hz.shuidangran.top/gtbccixpdu.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.cucudq.cn/gtlgxqzjun.html

================================================================================
来源：http://hz.yuanzhike.top/gtqdsqkqey.html

F. 文件与目录
来源：http://hz.redwolf501.top/gtnhkedvdu.html

================================================================================
来源：http://hz.jinqigfzy.top/gtkfncuvis.html

[F01] 读取整个文件
来源：http://hz.fzhhl.top/gtjtbzstwu.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.jinyuanbaomall.cn/gtqhslhmna.html

PHP:  file_get_contents("a.txt");
来源：http://hz.yonumen.top/gtwpzjnajt.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.smart0.xyz/gtwjedtebz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.zhiwuduotai.top/gtozabckfd.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.52xcode.cn/gttjdkieam.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.shanyushiyangtech.top/gtvhjucnla.html

Ruby: File.read("a.txt")
来源：http://hz.zycfv.cn/gtgqtusjpb.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.birdmap.top/gtagqvazid.html

[F02] 逐行读取文件
来源：http://hz.hfpthk.cn/gtqgygmsdx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.ppjwa.cn/gtywnrglrx.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.birdmap.top/gtactugetd.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.dashuyun.cn/gtleqjtbfn.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.nanxuanxn.top/gtfcfrkzky.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.havefunace.top/gtkemkduge.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.cashguo.top/gtprxavpoz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yj202588.top/gtplvqlszp.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.nwbrower.top/gtxfgzggcv.html

[F03] 写入文件（覆盖）
来源：http://hz.andypj.xyz/gtnhsrohfm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.meibo888.top/gtxvxolwnk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.xingfuxueyuan.xyz/gtajwptikx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.xuanzx.com/gtidussakl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.cashguo.top/gtqbpdmeyt.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.yonumen.top/gtermhnpiu.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.jinqigufen.top/gtlsfabzpd.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.cdnleiting.top/gtvpvoyaph.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.sweek.top/gtgehceqzv.html

[F04] 追加写入文件
来源：http://hz.jqgfzy.top/gtwiqdwsos.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.ehwqpu.com/gtzneulvrf.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.shzxlz.cn/gtykmprfti.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yj20258.top/gtdfayvgyv.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.52xcode.cn/gtnbhqumyj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.birdmap.top/gtzsqovwex.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.shuidangran.top/gtgiyoxluh.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.jyoumei.cn/gtjfknqkiw.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.yuanzhike.top/gtjrxgcnxh.html

[F05] 判断文件或目录是否存在
来源：http://hz.svipenyu.cn/gtqdzxfkrg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.guannengcc.top/gtuwurixga.html

PHP:  file_exists("a.txt");
来源：http://hz.sufxvd.cn/gtqlwwljbl.html

JS:   fs.existsSync("a.txt")
来源：http://hz.kuanghao11.cn/gtxevskkcj.html

TS:   fs.existsSync("a.txt")
来源：http://hz.fzhhl.top/gtanoyscyn.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.yj20258888.top/gtfilsuuvz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.sufxvd.cn/gtmasnljkl.html

Ruby: File.exist?("a.txt")
来源：http://hz.yuxming.cn/gtjlptlqnp.html

C#:   File.Exists("a.txt")
来源：http://hz.316326.xyz/gtvsqhcgbo.html

[F06] 删除文件
来源：http://hz.yuanzhike.top/gtactlnhef.html

Py:   os.remove("a.txt")
来源：http://hz.redwolf501.top/gtaivnzzlz.html

PHP:  unlink("a.txt");
来源：http://hz.nanxinkj.top/gtgmufqbhz.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.kuanghao11.cn/gtpywmmszm.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.nwbrower.top/gtnsnumdch.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.xylfe.cn/gtxpqybgmi.html

Go:   os.Remove("a.txt")
来源：http://hz.mhx1999.top/gtsysrkuab.html

Ruby: File.delete("a.txt")
来源：http://hz.sysykeji.top/gtmjiqrrvm.html

C#:   File.Delete("a.txt");
来源：http://hz.yj20258888.top/gtmddrmrdd.html

[F07] 创建目录（含多级）
来源：http://hz.ivvv.top/gtbgozctsv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.zhengqikj.top/gtmqcizumd.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.chenlongwang.top/gtvdabpimo.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.pengpengdd.cyou/gtphbvtwlc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.svipenyu.cn/gtumyskkev.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.shanyushiyangtech.top/gtywxsxaid.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.sweek.top/gtsqscvhhf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.yuanzhike.top/gtlizsypxv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yuanzhike.top/gtgcuutrxc.html

[F08] 遍历目录
来源：http://hz.sysykeji.top/gtmrpfeqrv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.andypj.xyz/gtklttkkiu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.9152youxi.cn/gtkmjarfnv.html

JS:   fs.readdirSync("dir")
来源：http://hz.jlsjyb.cn/gtbvpgavte.html

TS:   fs.readdirSync("dir")
来源：http://hz.meibo888.top/gttefroioy.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.sysykeji.top/gtxuspicdc.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yvedp.cn/gtdvugidps.html

Ruby: Dir.children("dir")
来源：http://hz.gotoacloud.top/gtzuotgwqq.html

C#:   Directory.GetFiles("dir")
来源：http://hz.vqdsnc.cn/gtzusozpao.html

[F09] 获取文件大小
来源：http://hz.sufxvd.cn/gtmmscgrwq.html

Py:   os.path.getsize("a.txt")
来源：http://hz.9152youxi.cn/gtrzjoqguk.html

PHP:  filesize("a.txt");
来源：http://hz.sweek.top/gtcdgzovad.html

JS:   fs.statSync("a.txt").size
来源：http://hz.shanyushiyangtech.top/gtgvbvwvmf.html

TS:   fs.statSync("a.txt").size
来源：http://hz.zhaomingkeji.xyz/gttiuzarbb.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.zhixingplan.top/gtlwqwmokl.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.jianghu66.top/gtyoeslfpx.html

Ruby: File.size("a.txt")
来源：http://hz.nwbrower.top/gtmkaskyaw.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.c1oappe.top/gtxkxamcmj.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.xuetiantiany.cn/gtqqnybbxq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.zhijiandao.cn/gtrnaolipc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.birdmap.top/gtmwurgqni.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.gaohongyu789.top/gtzdobrvum.html

TS:   path.extname("a.txt")
来源：http://hz.ehwqpu.com/gtknqcohyg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.aibaodan.cn/gtugbmslwr.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.ppjwa.cn/gtnxwykjxy.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.sweek.top/gtacxgpqym.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.zhaomingkeji.xyz/gtlwcpauoy.html

[F11] 复制与移动文件
来源：http://hz.tanke756.top/gtlnighzae.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.yonumen.top/gthvulvpef.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.ywan-chungtsiang.top/gtbsnzejpl.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xylfe.cn/gtnfibjpfz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.wangdashe.top/gtasgmtjou.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.yj20258.top/gtuugslxth.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.sysykeji.top/gtyorhpcqe.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.ehwqpu.com/gtjbmxujmx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.fengsongda.top/gtmqjilusi.html

[F12] CSV 读写
来源：http://hz.aibaodan.cn/gtyattnaef.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.chenlongwang.top/gtzgbscgmd.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.yvedp.cn/gtspkcczsq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.zhijiandao.cn/gtoxooacfk.html

TS:   // 同上
来源：http://hz.snrcjt.cn/gtrlbocwez.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.yj20258.top/gtrgkgigdy.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.jinyuanbaomall.cn/gtleljgorr.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jinghuilouyu.cn/gtehrezuef.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.zhoulong.xyz/gtwlrsxzma.html

================================================================================
来源：http://hz.andypj.xyz/gtgmmmtvrk.html

G. 面向对象
来源：http://hz.ppjwa.cn/gtbnpxqrou.html

================================================================================
来源：http://hz.havefunace.top/gtrekeebro.html

[G01] 定义类
来源：http://hz.gzhubu.top/gtuzosmjuh.html

Py:   class User: pass
来源：http://hz.feifeiyinyue.top/gtbsjyizdd.html

PHP:  class User {}
来源：http://hz.aizwys.cn/gtegvuwxtb.html

JS:   class User {}
来源：http://hz.gzhubu.top/gttpzttlgu.html

TS:   class User { name: string = ""; }
来源：http://hz.yj20258.top/gtiglevlba.html

Java: class User {}
来源：http://hz.birdmap.top/gtmkgbkcbn.html

Go:   type User struct { Name string }
来源：http://hz.yuanzhike.top/gtlpoxktjo.html

Ruby: class User; end
来源：http://hz.yvedp.cn/gtsavdopay.html

C#:   class User {}
来源：http://hz.vqdsnc.cn/gtaphtkvrc.html

[G02] 构造函数
来源：http://hz.xuetiantiany.cn/gtsmgaozco.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yongpay.top/gteqiyjcam.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.wangshuangyany.cn/gtujwgsnmk.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yanxiufei.cn/gtuiylzvwf.html

TS:   constructor(public name: string) {}
来源：http://hz.guannengcc.top/gtvfqbwymr.html

Java: User(String name) { this.name = name; }
来源：http://hz.shangyingyoupin.top/gtitcrypte.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.zycfv.cn/gtdxyiifpf.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yanxiufei.cn/gtrqxgcugj.html

C#:   public User(string name) { Name = name; }
来源：http://hz.0kj1m.cn/gtuqxspyye.html

[G03] 实例属性
来源：http://hz.chenlongwang.top/gtnolkbjfo.html

Py:   self.name = "x"
来源：http://hz.ydzc1.top/gtwepomxwd.html

PHP:  public string $name = "x";
来源：http://hz.svipenyu.cn/gthskqaknf.html

JS:   this.name = "x";
来源：http://hz.shangyingyoupin.top/gtqrtvdofo.html

TS:   name: string = "x";
来源：http://hz.zhijiandao.cn/gtnggkmknc.html

Java: private String name;
来源：http://hz.cashguo.top/gtmbflbqxu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.cqqwz.cn/gtklrqyfbu.html

Ruby: @name = "x"
来源：http://hz.hammf.cn/gtfnvslwkz.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.zdqjudy.top/gtifrfpkkq.html

[G04] 定义方法
来源：http://hz.chenzaomai.com/gtgnnwabjk.html

Py:   def greet(self): return self.name
来源：http://hz.yuanzhike.top/gtxaqgythx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.jiagoushi.top/gtdbbpnexl.html

JS:   greet() { return this.name; }
来源：http://hz.cucudq.cn/gttsxqeimh.html

TS:   greet(): string { return this.name; }
来源：http://hz.9152youxi.cn/gtxzzlfahr.html

Java: String greet() { return name; }
来源：http://hz.aizwys.cn/gtjipiphke.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.dashuyun.cn/gtxziakaey.html

Ruby: def greet; @name; end
来源：http://hz.tanke756.top/gtxpzbncat.html

C#:   public string Greet() => Name;
来源：http://hz.jianghu66.top/gttvebovyq.html

[G05] 继承
来源：http://hz.316326.xyz/gtiuakwzzq.html

Py:   class Admin(User): pass
来源：http://hz.snrcjt.cn/gtcvoiykkf.html

PHP:  class Admin extends User {}
来源：http://hz.jyoumei.cn/gtqbiehwyw.html

JS:   class Admin extends User {}
来源：http://hz.tianlin.xyz/gtckpbjtxo.html

TS:   class Admin extends User {}
来源：http://hz.zdqjudy.top/gtzhhilnki.html

Java: class Admin extends User {}
来源：http://hz.xuanzx.com/gtsdqmmmzz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.xylfe.cn/gtiopymykc.html

Ruby: class Admin < User; end
来源：http://hz.gaohongyu789.top/gtjyltrhbd.html

C#:   class Admin : User {}
来源：http://hz.cdnleiting.top/gthlkluakf.html

[G06] 重写方法
来源：http://hz.316326.xyz/gtahwdahzc.html

Py:   def greet(self): return "admin"
来源：http://hz.gaohongyu789.top/gtbmjzmhfg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.meibo888.top/gtkvjgognv.html

JS:   greet() { return "admin"; }
来源：http://hz.hongshengwenyu.top/gthreyqhhu.html

TS:   greet(): string { return "admin"; }
来源：http://hz.chenlongwang.top/gttmqjejkm.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.fengsongda.top/gtmjsbcubp.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.shanyushiyangtech.top/gtsnxkhlxo.html

Ruby: def greet; "admin"; end
来源：http://hz.xziqi.cn/gtmwpcboho.html

C#:   public override string Greet() => "admin";
来源：http://hz.hnqzz.top/gtuxickgxm.html

[G07] 调用父类方法
来源：http://hz.yj202588.top/gtegouhwru.html

Py:   super().greet()
来源：http://hz.cheryme.top/gtqjoxpnol.html

PHP:  parent::greet();
来源：http://hz.meibo888.top/gtgqulivcu.html

JS:   super.greet();
来源：http://hz.hysaishi.cn/gtgdnvzhxa.html

TS:   super.greet();
来源：http://hz.hnqzz.top/gtiqpribkd.html

Java: super.greet();
来源：http://hz.ybcxt.top/gtytwuyksa.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.daria6918.cn/gtvabclqwk.html

Ruby: super
来源：http://hz.yanxiufei.cn/gttbjyakzv.html

C#:   base.Greet();
来源：http://hz.sxryk.cn/gturqtwpyo.html

[G08] 静态方法与属性
来源：http://hz.meibo888.top/gtjevojsgd.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.iojbl.cn/gtcdubvryw.html

PHP:  public static function f() {}
来源：http://hz.pengpengdd.cyou/gtgafoznks.html

JS:   static f() {}
来源：http://hz.andypj.xyz/gtenygiyro.html

TS:   static f(): void {}
来源：http://hz.mhx1999.top/gtpotsekfk.html

Java: static void f() {}
来源：http://hz.jlsjyb.cn/gtjfkgxtpj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.daxiang520.top/gtfehknwey.html

Ruby: def self.f; end
来源：http://hz.316326.xyz/gtwlluvmja.html

C#:   public static void F() {}
来源：http://hz.aibaodan.cn/gthiflweml.html

[G09] 接口 / 抽象类
来源：http://hz.52xcode.cn/gtqipmyslg.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.hfpthk.cn/gtrqlyuqqp.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.tianlin.xyz/gtdkzcrijy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.zhiwuduotai.top/gtqtixdiuk.html

TS:   interface Shape { area(): number; }
来源：http://hz.sufxvd.cn/gtpnhqvoav.html

Java: interface Shape { double area(); }
来源：http://hz.cucudq.cn/gtdwfxlzfy.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yj202588.top/gtqelpngvh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.daria6918.cn/gtzicfrxss.html

C#:   interface IShape { double Area(); }
来源：http://hz.yj20258888.top/gthjyakhxj.html


<!-- 参考信息 -->