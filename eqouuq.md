代发 wailian999

Ruby: s.reverse
来源：http://hz.yj20258888.top/gtvoxdeyxz.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.cucudq.cn/gtqpnjvtdp.html

[E12] 统计某字符出现次数
来源：http://hz.ydjk.org.cn/gtctsccwbh.html

Py:   s.count("a")
来源：http://hz.shangyingyoupin.top/gtcxaohcqj.html

PHP:  substr_count($s, "a");
来源：http://hz.jinqigufen.top/gtfemafunl.html

JS:   s.split("a").length - 1
来源：http://hz.mhx1999.top/gtrpjbfnqy.html

TS:   s.split("a").length - 1
来源：http://hz.redwolf501.top/gtdldalktc.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.cdnleiting.top/gtgykjeurq.html

Go:   strings.Count(s, "a")
来源：http://hz.xuetiantiany.cn/gtbpcnmfuj.html

Ruby: s.count("a")
来源：http://hz.tianlin.xyz/gtkthyxqvg.html

C#:   s.Count(c => c == 'a')
来源：http://hz.shzxlz.cn/gtgrcmrmmy.html

[E13] 逐字符遍历
来源：http://hz.jqgufenzy.top/gtpjwjtbsf.html

Py:   for ch in s: print(ch)
来源：http://hz.nanxuanxn.top/gtiywtayrt.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.hammf.cn/gtilajdlqf.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.pengpengdd.cyou/gtrxoroene.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jinqigufen.top/gtpfdewmpo.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.kuanghao11.cn/gtdqtiapnn.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.shzxlz.cn/gtcjkakxlg.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.ydzc1.top/gtltdiuvjx.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.aibaodan.cn/gtewgcmspc.html

[E14] URL 编码与 Base64
来源：http://hz.jyoumei.cn/gteeqknwnm.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.hnqzz.top/gtnaondfjp.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.yueranfly.top/gtjedwrutt.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.pycfn.com/gtgzwjiqbg.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.vqdsnc.cn/gtozolcwtf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.shanyushiyangtech.top/gtlzydjyaz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.ydzc1.top/gtzhiivkyy.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.hywenlv.cn/gtnxdvvhmj.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.daria6918.cn/gtsypgkxai.html

[E15] HTML 转义 / 反转义
来源：http://hz.chenlongwang.top/gtgxnjvfkf.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.ehwqpu.com/gtajcwrmjk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.hongshengwenyu.top/gtfuqgdoto.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.hywenlv.cn/gtojazchhs.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.zdqjudy.top/gtjwmqykjb.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.nwbrower.top/gtxnrcdcpt.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.jqgfzy.top/gtkusiuosh.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.yuxming.cn/gtwiyiiyjj.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.hongshengwenyu.top/gtladvyrot.html

[E16] 数字千分位
来源：http://hz.bjfxy.top/gtquhqaobz.html

Py:   f"{1234567:,}"
来源：http://hz.yonumen.top/gtnuvwjsua.html

PHP:  number_format(1234567);
来源：http://hz.andypj.xyz/gtowgyopsd.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.cucudq.cn/gtoejlxphu.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.c1oappe.top/gtqatsxucl.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.fengsongda.top/gtmzwgptya.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.havefunace.top/gtappxzijb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.ywan-chungtsiang.top/gtpzgnzbdx.html

C#:   1234567.ToString("N0")
来源：http://hz.jiagoushi.top/gtssnktpxe.html

[E17] 首字母大写
来源：http://hz.zhijiandao.cn/gtxoklfbxv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.pengpengdd.cyou/gtigilxlnh.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.hfpthk.cn/gtdbmuqqgd.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.tanke756.top/gtjjciearz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.cheryme.top/gtrcuvrtzw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.yj202588.top/gtjfvtsmix.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.jqgfzy.top/gtbzvdsnxb.html

Ruby: s.capitalize
来源：http://hz.hysaishi.cn/gtvgrgnylf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.aizwys.cn/gtrmwwpojy.html

[E18] 模板占位符替换
来源：http://hz.c1oappe.top/gtakkqfkfg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.xylfe.cn/gtqbscunjo.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.zhiwuduotai.top/gtubmoazbr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.yj20258888.top/gtsicsmfqn.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.svipenyu.cn/gtrotmvnhb.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.wangshuangyany.cn/gtzfhmrvfr.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.yj20258.top/gtgvvnckbk.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.zdqjudy.top/gtlefspasj.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.hnxiangtu.top/gtuiuzable.html

[E19] 多行文本按行拆分
来源：http://hz.tian-w.cn/gtfdcizmjf.html

Py:   s.splitlines()
来源：http://hz.hnxiangtu.top/gtfrczanht.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.dianchejie.cn/gtjxjshtya.html

JS:   s.split(/\r?\n/)
来源：http://hz.iojbl.cn/gtiuwuiwhz.html

TS:   s.split(/\r?\n/)
来源：http://hz.aibaodan.cn/gthbcanxeu.html

Java: s.lines().toList()
来源：http://hz.havefunace.top/gtjqhqnjkq.html

Go:   strings.Split(s, "\n")
来源：http://hz.jqgufenzy.top/gtznliyfcn.html

Ruby: s.lines
来源：http://hz.bjfxy.top/gtucswezyo.html

C#:   s.Split('\n')
来源：http://hz.dianchejie.cn/gtaioawvut.html

[E20] 判断字符串是否为空
来源：http://hz.tianlin.xyz/gtxtjnvnie.html

Py:   if not s:
来源：http://hz.aibaodan.cn/gtxzlixvff.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.havefunace.top/gtldmmljow.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.aibaodan.cn/gtmfllnccc.html

TS:   if (s === "") {}
来源：http://hz.cdnleiting.top/gtkzsqbnef.html

Java: if (s.isEmpty()) {}
来源：http://hz.havefunace.top/gtyxdnhjzy.html

Go:   if s == "" {}
来源：http://hz.wangshuangyany.cn/gtykpymwhs.html

Ruby: if s.empty?
来源：http://hz.xuanzx.com/gtoebvtggh.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.jyoumei.cn/gttzbgvyrl.html

[E21] 超长截断加省略号
来源：http://hz.hysaishi.cn/gtackmbfpe.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.svipenyu.cn/gtzryfudrt.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.xziqi.cn/gtertndqzv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.birdmap.top/gtxnywwxxd.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jinqigfzy.top/gtxnvwepvh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.cdnleiting.top/gtizefhpwt.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.ybcxt.top/gtqkjonham.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.aibaodan.cn/gtgflvacoa.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.sysykeji.top/gtnvhsoelu.html

[E22] 字节长度与字符长度
来源：http://hz.zhiwuduotai.top/gtlwjxxfxs.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.sweek.top/gtcdpowtgq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.mhx1999.top/gtgmlpiluf.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.guowangkeji.top/gtohgkwlwh.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ydjk.org.cn/gtjzhxbmol.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.yvedp.cn/gtpdvvxmni.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.yuxming.cn/gtyqlgrzgh.html

Ruby: s.bytesize;  s.length
来源：http://hz.ydzc1.top/gttmngawtf.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.yj202588.top/gtaldiewnq.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtvrjrmnjq.html

F. 文件与目录
来源：http://hz.sweek.top/gtngtaqlji.html

================================================================================
来源：http://hz.c1oappe.top/gtcsiiutju.html

[F01] 读取整个文件
来源：http://hz.jyoumei.cn/gtcmduftzt.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yanxiufei.cn/gtvuywgept.html

PHP:  file_get_contents("a.txt");
来源：http://hz.daxiang520.top/gtgddcwthq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.guannengcc.top/gttbbgtjfr.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.zdqjudy.top/gtoguzqtbg.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.nanxuanxn.top/gtqgoyypcq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.yanxiufei.cn/gtolbhvcdf.html

Ruby: File.read("a.txt")
来源：http://hz.sxryk.cn/gtnspebdzp.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yj20258.top/gtjlvrtcrf.html

[F02] 逐行读取文件
来源：http://hz.cucudq.cn/gtuqesmuvm.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.hywenlv.cn/gtspxmnshl.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.zhongyouzk.top/gtjzuzwxpy.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.havefunace.top/gtjhhouwal.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.sxryk.cn/gtzzxrktdf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.chenlongwang.top/gtjwqyhqpl.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.jinyuanbaomall.cn/gtcltnmlrq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.jiagoushi.top/gtgwxbuxja.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.zhaomingkeji.xyz/gtxzbqtjin.html

[F03] 写入文件（覆盖）
来源：http://hz.yuxming.cn/gttipowuua.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.daxiang520.top/gtldrokrke.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.redwolf501.top/gtjtbfafqi.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.tianlin.xyz/gtagspebte.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jiagoushi.top/gtewlakwvx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.cqqwz.cn/gtvinwybfh.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.hfpthk.cn/gtiorrwngf.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.xuetiantiany.cn/gtkspkqceu.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.dashuyun.cn/gtbjcanbnp.html

[F04] 追加写入文件
来源：http://hz.haohaochexian.top/gtwvbzojrz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.jianghu66.top/gtqcnbshbp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.yuxming.cn/gtoxfsitok.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ydzc1.top/gtwdgpdfaj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yuanzhike.top/gtwurvvzym.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.shanyushiyangtech.top/gtwlctgqcm.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.zycfv.cn/gtmidjhqxs.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.xinyue.icu/gtijthesxp.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.yuxming.cn/gtlyxspwpt.html

[F05] 判断文件或目录是否存在
来源：http://hz.chenzaomai.com/gtfrdmwffw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.ehwqpu.com/gtijuivkjw.html

PHP:  file_exists("a.txt");
来源：http://hz.zhoulong.xyz/gtbqvlykkp.html

JS:   fs.existsSync("a.txt")
来源：http://hz.shanyushiyangkeji.top/gtbkaxomby.html

TS:   fs.existsSync("a.txt")
来源：http://hz.svipenyu.cn/gtggwgyxuq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.zdqjudy.top/gtewzfwecc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.zhiwuduotai.top/gtifgcikah.html

Ruby: File.exist?("a.txt")
来源：http://hz.gaohongyu789.top/gtqvbfkubl.html

C#:   File.Exists("a.txt")
来源：http://hz.jyoumei.cn/gtsxehxidu.html

[F06] 删除文件
来源：http://hz.daria6918.cn/gtuzwuxsin.html

Py:   os.remove("a.txt")
来源：http://hz.316326.xyz/gtmaalnyjx.html

PHP:  unlink("a.txt");
来源：http://hz.gzhubu.top/gtpqedecpj.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.shzxlz.cn/gtndbwuiqe.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.fzhhl.top/gtjsdciobd.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.c1oappe.top/gtchfpruxl.html

Go:   os.Remove("a.txt")
来源：http://hz.sxryk.cn/gtrfkqcbhy.html

Ruby: File.delete("a.txt")
来源：http://hz.feifeiyinyue.top/gtjprithsb.html

C#:   File.Delete("a.txt");
来源：http://hz.52xcode.cn/gtkygguadz.html

[F07] 创建目录（含多级）
来源：http://hz.316326.xyz/gtvfsoavep.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.jlsjyb.cn/gtnhcpczdc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.guannengcc.top/gtgffbsxjh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhaomingkeji.xyz/gtpfmrdwlz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.52xcode.cn/gtrsgotqvm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.hywenlv.cn/gtiaaqbwmq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.birdmap.top/gtazvvnkqz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.yvedp.cn/gtwrjzuxcl.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.andypj.xyz/gtvxvhpwbm.html

[F08] 遍历目录
来源：http://hz.zhengqikj.top/gttfyxtchh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.dianchejie.cn/gtlxzhfmhy.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.jqgufenzy.top/gtczzarhpq.html

JS:   fs.readdirSync("dir")
来源：http://hz.feifeiyinyue.top/gtliepzekj.html

TS:   fs.readdirSync("dir")
来源：http://hz.ydjk.org.cn/gtebzcxzww.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.cashguo.top/gtptajvxtc.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.c1oappe.top/gtmxgjgwjn.html

Ruby: Dir.children("dir")
来源：http://hz.xylfe.cn/gtlysszuju.html

C#:   Directory.GetFiles("dir")
来源：http://hz.fengsongda.top/gterfcmxue.html

[F09] 获取文件大小
来源：http://hz.gotoacloud.top/gtoychqoul.html

Py:   os.path.getsize("a.txt")
来源：http://hz.gogol.net.cn/gtkcbtaiwu.html

PHP:  filesize("a.txt");
来源：http://hz.xingfuxueyuan.xyz/gtudsqjjdq.html

JS:   fs.statSync("a.txt").size
来源：http://hz.birdmap.top/gtkpfkeyim.html

TS:   fs.statSync("a.txt").size
来源：http://hz.hnxiangtu.top/gtgsgsssop.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.hnxiangtu.top/gtldvoihvw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.cdnleiting.top/gtpkgwdbqy.html

Ruby: File.size("a.txt")
来源：http://hz.ywan-chungtsiang.top/gtjqvqymba.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.sufxvd.cn/gtyyfnycnv.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.smart0.xyz/gtsiyndrwv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.xylfe.cn/gtzqeeuimj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.havefunace.top/gtlcqmgggv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.iojbl.cn/gtghkhtfzi.html

TS:   path.extname("a.txt")
来源：http://hz.ydjk.org.cn/gtbzucfpxz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.ydzc1.top/gteqolsnwk.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.zhengqikj.top/gtwaxzfwol.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.guannengcc.top/gtfimxepwi.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.jlsjyb.cn/gtzrrcexit.html

[F11] 复制与移动文件
来源：http://hz.c1oappe.top/gtefqahemu.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.jqgufenzy.top/gtayasotim.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.tianlin.xyz/gtlgxhsnil.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.c1oappe.top/gtrvkffipu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.pycfn.com/gtlhjjyzey.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.yueranfly.top/gtmelihbts.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.aizwys.cn/gtbqmhjylj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.ydzc1.top/gtzqhdntms.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.yj20258.top/gthlosqghs.html

[F12] CSV 读写
来源：http://hz.yj20258888.top/gtxapacwbc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.xinyue.icu/gtbfewauzg.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.yonumen.top/gtrwwgbogi.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.hfpthk.cn/gtufogwafc.html

TS:   // 同上
来源：http://hz.gogol.net.cn/gtissuoczm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.yj202588.top/gtaohvrbek.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.havefunace.top/gtsmoohfaa.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.pengpengdd.cyou/gtnhmwksdb.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.316326.xyz/gthoezhzwa.html

================================================================================
来源：http://hz.gogol.net.cn/gteyekcdbf.html

G. 面向对象
来源：http://hz.zycfv.cn/gtrgyrbsrd.html

================================================================================
来源：http://hz.9152youxi.cn/gtoijymhod.html

[G01] 定义类
来源：http://hz.cucudq.cn/gtdbyvymza.html

Py:   class User: pass
来源：http://hz.zhongyouzk.top/gtaeldxcej.html

PHP:  class User {}
来源：http://hz.vqdsnc.cn/gtyitzzypf.html

JS:   class User {}
来源：http://hz.xziqi.cn/gtwsweiuyv.html

TS:   class User { name: string = ""; }
来源：http://hz.hongshengwenyu.top/gtbewtgizt.html

Java: class User {}
来源：http://hz.jqgufenzy.top/gtsjoukmbu.html

Go:   type User struct { Name string }
来源：http://hz.tianlin.xyz/gtpmwjaatv.html

Ruby: class User; end
来源：http://hz.pycfn.com/gtcykjyurv.html

C#:   class User {}
来源：http://hz.aizwys.cn/gtyxsplosr.html

[G02] 构造函数
来源：http://hz.mhx1999.top/gthxxbijrz.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.iojbl.cn/gtfbbbhzfm.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yj20258888.top/gtzaxbdimp.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.ivvv.top/gtbtppuntt.html

TS:   constructor(public name: string) {}
来源：http://hz.chenjidiqi.icu/gtgpoffjej.html

Java: User(String name) { this.name = name; }
来源：http://hz.redwolf501.top/gtrjnvgvfz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.sysykeji.top/gtfhpaeoxq.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.zhongyouzk.top/gtqjmyhohe.html

C#:   public User(string name) { Name = name; }
来源：http://hz.ivvv.top/gtblossbau.html

[G03] 实例属性
来源：http://hz.cqqwz.cn/gtfwwcfcll.html

Py:   self.name = "x"
来源：http://hz.xuanzx.com/gtwizujtrf.html

PHP:  public string $name = "x";
来源：http://hz.pengpengdd.cyou/gtiffogwrb.html

JS:   this.name = "x";
来源：http://hz.quarkkingdee.top/gtxmkznnzv.html

TS:   name: string = "x";
来源：http://hz.haohaochexian.top/gtgyhxsffw.html

Java: private String name;
来源：http://hz.zhijiandao.cn/gtktgeqlte.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yonumen.top/gttetmsgtv.html

Ruby: @name = "x"
来源：http://hz.cdnleiting.top/gtmqupdqgn.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.zhaomingkeji.xyz/gtlsgpjlno.html

[G04] 定义方法
来源：http://hz.gotoacloud.top/gtfhyuniur.html

Py:   def greet(self): return self.name
来源：http://hz.jlsjyb.cn/gtwihfkxpe.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.jqgufenzy.top/gtkwtvyazn.html

JS:   greet() { return this.name; }
来源：http://hz.zhengqikj.top/gtsgitrdhf.html

TS:   greet(): string { return this.name; }
来源：http://hz.hfpthk.cn/gtarsjqopj.html

Java: String greet() { return name; }
来源：http://hz.zdqjudy.top/gtnevccyvh.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.chenzaomai.com/gtitqxpotc.html

Ruby: def greet; @name; end
来源：http://hz.tian-w.cn/gtpdttegrl.html

C#:   public string Greet() => Name;
来源：http://hz.cucudq.cn/gtliwlgvlw.html

[G05] 继承
来源：http://hz.guowangkeji.top/gtsrxwbxgp.html

Py:   class Admin(User): pass
来源：http://hz.hnxiangtu.top/gtmeasjymp.html

PHP:  class Admin extends User {}
来源：http://hz.smart0.xyz/gttavfubde.html

JS:   class Admin extends User {}
来源：http://hz.mhx1999.top/gtoqfolnmx.html

TS:   class Admin extends User {}
来源：http://hz.hnxiangtu.top/gtqikkdbki.html

Java: class Admin extends User {}
来源：http://hz.yueranfly.top/gtkkyxyueu.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.tanke756.top/gtprdgxpwc.html

Ruby: class Admin < User; end
来源：http://hz.chenjidiqi.icu/gtgmtnswqs.html

C#:   class Admin : User {}
来源：http://hz.ybcxt.top/gtsdttmzvs.html

[G06] 重写方法
来源：http://hz.xuetiantiany.cn/gtvygcdexa.html

Py:   def greet(self): return "admin"
来源：http://hz.yanxiufei.cn/gtnisdalgy.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.shanyushiyangtech.top/gtscnyyhnp.html

JS:   greet() { return "admin"; }
来源：http://hz.c1oappe.top/gtcxjifysl.html

TS:   greet(): string { return "admin"; }
来源：http://hz.redwolf501.top/gtkeqntkps.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.guannengcc.top/gtwwbjddsx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.yanxiufei.cn/gtlrbglbfp.html

Ruby: def greet; "admin"; end
来源：http://hz.jinyuanbaomall.cn/gtxjkqngdv.html

C#:   public override string Greet() => "admin";
来源：http://hz.guowangkeji.top/gtofyfoesm.html

[G07] 调用父类方法
来源：http://hz.jinyuanbaomall.cn/gtxxclhbuv.html

Py:   super().greet()
来源：http://hz.fzhhl.top/gtbmcpqcgo.html

PHP:  parent::greet();
来源：http://hz.cheryme.top/gtquwvkmwm.html

JS:   super.greet();
来源：http://hz.smart0.xyz/gtdcumbmzj.html

TS:   super.greet();
来源：http://hz.xinyue.icu/gtsvadjinu.html

Java: super.greet();
来源：http://hz.zhongyouzk.top/gtrxguwdyh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.zhaomingkeji.xyz/gtnkmauser.html

Ruby: super
来源：http://hz.wangdashe.top/gtdqzuzlap.html

C#:   base.Greet();
来源：http://hz.hysaishi.cn/gtsgupohez.html

[G08] 静态方法与属性
来源：http://hz.hongshengwenyu.top/gtupzzutpa.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.redwolf501.top/gtwqorstlm.html

PHP:  public static function f() {}
来源：http://hz.shanyushiyangkeji.top/gtkytobpeh.html

JS:   static f() {}
来源：http://hz.guannengcc.top/gtfmbgvqal.html

TS:   static f(): void {}
来源：http://hz.zhiwuduotai.top/gtezpbecqa.html

Java: static void f() {}
来源：http://hz.zhaomingkeji.xyz/gtftppucet.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.zdqjudy.top/gtpjqluaxf.html

Ruby: def self.f; end
来源：http://hz.jiagoushi.top/gttcnugffh.html

C#:   public static void F() {}
来源：http://hz.gzhubu.top/gtnfqbbpas.html

[G09] 接口 / 抽象类
来源：http://hz.yangfankeji.com/gtnausaodh.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.zhengqikj.top/gtxnzpjkjd.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.guowangkeji.top/gttgztmldb.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.aibaodan.cn/gtvkfedvln.html

TS:   interface Shape { area(): number; }
来源：http://hz.yueranfly.top/gtlkeemzlc.html

Java: interface Shape { double area(); }
来源：http://hz.chenzaomai.com/gtapumjsgs.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.zhixingplan.top/gtrfvirpji.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.hammf.cn/gtntqzemll.html

C#:   interface IShape { double Area(); }
来源：http://hz.shzxlz.cn/gtgiyrjmjj.html

[G10] 访问控制
来源：http://hz.sufxvd.cn/gtndwsukwb.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.jlsjyb.cn/gtouqxsmql.html

PHP:  public / protected / private
来源：http://hz.jinqigfzy.top/gtrlowjvcc.html

JS:   #private 字段；其余公开
来源：http://hz.yuanzhike.top/gtfffbverm.html


<!-- 参考信息 -->