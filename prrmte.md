代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.daria6918.cn/gtpsnbaiev.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.vqdsnc.cn/gtuelytukc.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.havefunace.top/gtdbsupyfx.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.yonumen.top/gtepfxxdqr.html

[E14] URL 编码与 Base64
来源：http://hz.gzhubu.top/gtdwfnnvjh.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.jiagoushi.top/gtdzahxmau.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.dashuyun.cn/gtmxpdvbnq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.iojbl.cn/gtfdexwkfy.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.yueranfly.top/gtmkmcrksd.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.nanxinkj.top/gtqkxqkoje.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.ehwqpu.com/gtckiicpip.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.yuxming.cn/gthmxhzczw.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.daria6918.cn/gtddkmnvdb.html

[E15] HTML 转义 / 反转义
来源：http://hz.jinqigfzy.top/gtpkftqhuc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.fengsongda.top/gtucmojxnk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.aibaodan.cn/gtoqwwlvpk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yvedp.cn/gthprirpth.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.yuxming.cn/gtsptlfyps.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.cashguo.top/gtqpnhqkhu.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.ydzc1.top/gtqssduhca.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.andypj.xyz/gtmjtjmveu.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.0kj1m.cn/gtwwoenwvb.html

[E16] 数字千分位
来源：http://hz.xylfe.cn/gtmktbragw.html

Py:   f"{1234567:,}"
来源：http://hz.jlsjyb.cn/gtabgwoyni.html

PHP:  number_format(1234567);
来源：http://hz.yanxiufei.cn/gtqdqxahqs.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.sysykeji.top/gtjogmuimb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.xinyue.icu/gtdqwustgd.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.52xcode.cn/gtenlwtoyx.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.yuxming.cn/gtyexbsafc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.yj202588.top/gtioidsbpv.html

C#:   1234567.ToString("N0")
来源：http://hz.zhijiandao.cn/gtdbrydxjf.html

[E17] 首字母大写
来源：http://hz.ybcxt.top/gtsopfzrhz.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.9152youxi.cn/gtwfznowfc.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.mhx1999.top/gtgghebmru.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhoulong.xyz/gtvucewuwc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhoulong.xyz/gtlavswntk.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.yj202588.top/gtrvkcovtl.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.jiagoushi.top/gteyvgcifi.html

Ruby: s.capitalize
来源：http://hz.havefunace.top/gtgyudbmyz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.hnqzz.top/gtndmyhmyl.html

[E18] 模板占位符替换
来源：http://hz.sweek.top/gtlsudstsf.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.tianlin.xyz/gtfewrmpue.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.ydzc1.top/gtpgsxdvyf.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.xziqi.cn/gtqsqdxvgq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.shuidangran.top/gttcuishmw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.jinyuanbaomall.cn/gtauvdzkog.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.vqdsnc.cn/gtqkgicxfm.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.chenzaomai.com/gtatalwghw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.c1oappe.top/gtokltqxzh.html

[E19] 多行文本按行拆分
来源：http://hz.ehwqpu.com/gtzqeucvve.html

Py:   s.splitlines()
来源：http://hz.dashuyun.cn/gtrhaehryy.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.pengpengdd.cyou/gtxizubdvc.html

JS:   s.split(/\r?\n/)
来源：http://hz.fzhhl.top/gtrzeihthm.html

TS:   s.split(/\r?\n/)
来源：http://hz.gotoacloud.top/gtzgfiyoln.html

Java: s.lines().toList()
来源：http://hz.cdnleiting.top/gtnunqhipp.html

Go:   strings.Split(s, "\n")
来源：http://hz.zhengqikj.top/gtdwegyxpn.html

Ruby: s.lines
来源：http://hz.yuxming.cn/gttgxparvk.html

C#:   s.Split('\n')
来源：http://hz.hongshengwenyu.top/gtdgzynvoh.html

[E20] 判断字符串是否为空
来源：http://hz.yuxming.cn/gthakqoild.html

Py:   if not s:
来源：http://hz.iojbl.cn/gtkmspfret.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.tanke756.top/gtqhadhsdc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.chenzaomai.com/gtxqzamtnj.html

TS:   if (s === "") {}
来源：http://hz.cqqwz.cn/gtikshcewe.html

Java: if (s.isEmpty()) {}
来源：http://hz.zhiwuduotai.top/gtowdfwdve.html

Go:   if s == "" {}
来源：http://hz.xuetiantiany.cn/gtaydsaroo.html

Ruby: if s.empty?
来源：http://hz.yanxiufei.cn/gtqrgmllpx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.dashuyun.cn/gtegnecole.html

[E21] 超长截断加省略号
来源：http://hz.jianghu66.top/gtzreoumvv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.jinghuilouyu.cn/gtkcyiyilk.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.jinqigufen.top/gtnjgwedqe.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.wangdashe.top/gtzfwqbzxm.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.fzhhl.top/gtlonkqnim.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yj202588.top/gtiibyxuey.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.guannengcc.top/gtlbrwnsyw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.hywenlv.cn/gtbookqexb.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.sufxvd.cn/gtozvctlci.html

[E22] 字节长度与字符长度
来源：http://hz.meibo888.top/gtwcurkcvf.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.svipenyu.cn/gtrrrmycff.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhijiandao.cn/gtablqpjfy.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.fengsongda.top/gtrdgduupq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhijiandao.cn/gtikntlusm.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.redwolf501.top/gtnthilils.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.nanxuanxn.top/gtybrsucsd.html

Ruby: s.bytesize;  s.length
来源：http://hz.ydzc1.top/gtnhbkysoe.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.jinqigfzy.top/gtigddmlas.html

================================================================================
来源：http://hz.zhoulong.xyz/gtzoysomho.html

F. 文件与目录
来源：http://hz.gaohongyu789.top/gtadildtuq.html

================================================================================
来源：http://hz.ybcxt.top/gtzshpealo.html

[F01] 读取整个文件
来源：http://hz.shanyushiyangtech.top/gtxxfhdmks.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.bjfxy.top/gtbyrtkhoj.html

PHP:  file_get_contents("a.txt");
来源：http://hz.snrcjt.cn/gtrobuqblb.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.c1oappe.top/gtgvwqqwvl.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.zhengqikj.top/gtkshoysur.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.gaohongyu789.top/gtapcccocz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.xinyue.icu/gtptbibodh.html

Ruby: File.read("a.txt")
来源：http://hz.ydzc1.top/gtagakfelg.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.sweek.top/gtbyqqhutl.html

[F02] 逐行读取文件
来源：http://hz.zhixingplan.top/gtcbylurjo.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.cqqwz.cn/gtarlyjjuk.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.chenzaomai.com/gtnqevehjc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.gotoacloud.top/gtwxicurnk.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hfpthk.cn/gtuoliombg.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.0kj1m.cn/gtsmalghzs.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.chenzaomai.com/gtifgoooqf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.pycfn.com/gtuctsnwpu.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.hongshengwenyu.top/gtnjhxhxhb.html

[F03] 写入文件（覆盖）
来源：http://hz.xuetiantiany.cn/gtqdwbepih.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.yj20258888.top/gtovragiyz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.52xcode.cn/gtlsaqzwpt.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yvedp.cn/gtdgykkbpx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hywenlv.cn/gtkgbgujqs.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.chenlongwang.top/gtriubcjxt.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.quarkkingdee.top/gtkylkhhal.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.ppjwa.cn/gtlcprrryz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.shangyingyoupin.top/gtdhjlxksk.html

[F04] 追加写入文件
来源：http://hz.cheryme.top/gtkwlbdlyn.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.zdqjudy.top/gtodmfkgcm.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.cdnleiting.top/gtkbdgfaxb.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.shuidangran.top/gtruzogjoq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jqgufenzy.top/gtxlewmwyh.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.hnxiangtu.top/gtfmrwqmwr.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.jiagoushi.top/gtaehmaflg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.andypj.xyz/gthossxzcm.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.mhx1999.top/gtmpgkluvr.html

[F05] 判断文件或目录是否存在
来源：http://hz.shanyushiyangkeji.top/gtgbfpdqqv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.wangshuangyany.cn/gtfdpwbheh.html

PHP:  file_exists("a.txt");
来源：http://hz.xuetiantiany.cn/gtkhwdyttr.html

JS:   fs.existsSync("a.txt")
来源：http://hz.cdnleiting.top/gtcseeknix.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yuanzhike.top/gtgjgcphlm.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.yj202588.top/gtglvzbgax.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.hysaishi.cn/gtspdcedmq.html

Ruby: File.exist?("a.txt")
来源：http://hz.cucudq.cn/gtggduaosv.html

C#:   File.Exists("a.txt")
来源：http://hz.xuetiantiany.cn/gtzlljysjs.html

[F06] 删除文件
来源：http://hz.52xcode.cn/gttjxdxbue.html

Py:   os.remove("a.txt")
来源：http://hz.zhiwuduotai.top/gtxhsztnek.html

PHP:  unlink("a.txt");
来源：http://hz.redwolf501.top/gtisfjykgb.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yj20258.top/gtpumhxhth.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.smart0.xyz/gtsepdjrlw.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.nanxinkj.top/gtefgvhect.html

Go:   os.Remove("a.txt")
来源：http://hz.yangfankeji.com/gtshwngdzu.html

Ruby: File.delete("a.txt")
来源：http://hz.ppjwa.cn/gtkrmncrmk.html

C#:   File.Delete("a.txt");
来源：http://hz.yanxiufei.cn/gtiopfsyqi.html

[F07] 创建目录（含多级）
来源：http://hz.mhx1999.top/gtbaslfuly.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.wangdashe.top/gtbkmfwkhi.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.redwolf501.top/gtaexkabaz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.vqdsnc.cn/gtavtnwzal.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.dashuyun.cn/gtfnadcvyf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.jyoumei.cn/gtpvrykkib.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.ybcxt.top/gtxbyajzeo.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.fzhhl.top/gtstvyyzqw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.svipenyu.cn/gtlphnpsib.html

[F08] 遍历目录
来源：http://hz.ywan-chungtsiang.top/gtlekxdlpk.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.chenjidiqi.icu/gtyootdqsm.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.hysaishi.cn/gtkmsfkydg.html

JS:   fs.readdirSync("dir")
来源：http://hz.shzxlz.cn/gtiwckbcvz.html

TS:   fs.readdirSync("dir")
来源：http://hz.yj202588.top/gtqcribczy.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.aizwys.cn/gtiwuovpnx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.hammf.cn/gtvrlbxyfd.html

Ruby: Dir.children("dir")
来源：http://hz.ppjwa.cn/gtslywnqhz.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yueranfly.top/gtbnxmzqrb.html

[F09] 获取文件大小
来源：http://hz.jianghu66.top/gtlxegsihp.html

Py:   os.path.getsize("a.txt")
来源：http://hz.andypj.xyz/gtmizflhwx.html

PHP:  filesize("a.txt");
来源：http://hz.birdmap.top/gtvjhehqze.html

JS:   fs.statSync("a.txt").size
来源：http://hz.tianlin.xyz/gtkmceoarm.html

TS:   fs.statSync("a.txt").size
来源：http://hz.ybcxt.top/gtgfhipnmr.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.wangdashe.top/gtbjsanmjz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.xuanzx.com/gtjyhvifdk.html

Ruby: File.size("a.txt")
来源：http://hz.tanke756.top/gtbfvbwuwc.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.wangdashe.top/gtajrfzquf.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.sysykeji.top/gtatwbuwtx.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.sweek.top/gtfhdhftcs.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.ybcxt.top/gtpiqpwxlw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.jinghuilouyu.cn/gtupcdfuwt.html

TS:   path.extname("a.txt")
来源：http://hz.wangdashe.top/gtakhfnkar.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.yj20258.top/gtaiknthyk.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.jianghu66.top/gtsgvctqql.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.sweek.top/gtheinglbs.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.jiagoushi.top/gtnotasodd.html

[F11] 复制与移动文件
来源：http://hz.chenjidiqi.icu/gtysevpzqn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.xinyue.icu/gtjevqlork.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.chenjidiqi.icu/gtybilpnmf.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ydzc1.top/gtlccojtka.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.sufxvd.cn/gtrjsynkds.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.iojbl.cn/gtzotrcsij.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.gaohongyu789.top/gtfiswsevx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.quarkkingdee.top/gtappnzjhx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.pengpengdd.cyou/gtrdszgbga.html

[F12] CSV 读写
来源：http://hz.chenzaomai.com/gtrasuqewj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.yonumen.top/gttxsimaxs.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.bjfxy.top/gtkykfezyj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.c1oappe.top/gtzxfhswnb.html

TS:   // 同上
来源：http://hz.hnxiangtu.top/gtxbvhqial.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.bjfxy.top/gtnlsqxeys.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.daria6918.cn/gtzfrrrvvn.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.gzhubu.top/gtzscyskjd.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.sxryk.cn/gtwtouwvwl.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtxksjhotq.html

G. 面向对象
来源：http://hz.52xcode.cn/gtjescanjy.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtdcuquqct.html

[G01] 定义类
来源：http://hz.haohaochexian.top/gtoaoqwajl.html

Py:   class User: pass
来源：http://hz.birdmap.top/gtyuiezdwe.html

PHP:  class User {}
来源：http://hz.yonumen.top/gtcqzenmxh.html

JS:   class User {}
来源：http://hz.sysykeji.top/gtiutmjblk.html

TS:   class User { name: string = ""; }
来源：http://hz.yangfankeji.com/gttnqydiet.html

Java: class User {}
来源：http://hz.52xcode.cn/gtsnpwmzwl.html

Go:   type User struct { Name string }
来源：http://hz.zhengqikj.top/gtnrzrsqgi.html

Ruby: class User; end
来源：http://hz.sufxvd.cn/gtqippwrle.html

C#:   class User {}
来源：http://hz.shzxlz.cn/gtawgxyuff.html

[G02] 构造函数
来源：http://hz.sufxvd.cn/gtdhgupovx.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.hysaishi.cn/gthgwfqqxu.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yuxming.cn/gtfdddgtve.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.gotoacloud.top/gtagbdgcyn.html

TS:   constructor(public name: string) {}
来源：http://hz.ivvv.top/gtkbjrooll.html

Java: User(String name) { this.name = name; }
来源：http://hz.aibaodan.cn/gtbukgeqby.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yanxiufei.cn/gtncbnxtvz.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.redwolf501.top/gtwfbrynau.html

C#:   public User(string name) { Name = name; }
来源：http://hz.yj20258888.top/gtceipslag.html

[G03] 实例属性
来源：http://hz.fzhhl.top/gtjwughblb.html

Py:   self.name = "x"
来源：http://hz.fengsongda.top/gtljhvxeeh.html

PHP:  public string $name = "x";
来源：http://hz.feifeiyinyue.top/gtxyecdivn.html

JS:   this.name = "x";
来源：http://hz.xinyue.icu/gtsckcrceb.html

TS:   name: string = "x";
来源：http://hz.zhoulong.xyz/gtjccllrru.html

Java: private String name;
来源：http://hz.jlsjyb.cn/gtozlsrjyh.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.havefunace.top/gtwrgklfbd.html

Ruby: @name = "x"
来源：http://hz.nwbrower.top/gtheyhgfqz.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.ybcxt.top/gtfleybrin.html

[G04] 定义方法
来源：http://hz.jinqigufen.top/gtoifylmmm.html

Py:   def greet(self): return self.name
来源：http://hz.vqdsnc.cn/gtlyxviehd.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.ybcxt.top/gtivefnqom.html

JS:   greet() { return this.name; }
来源：http://hz.hfpthk.cn/gtnwliqghs.html

TS:   greet(): string { return this.name; }
来源：http://hz.jiagoushi.top/gtwjuxevtn.html

Java: String greet() { return name; }
来源：http://hz.havefunace.top/gtkrzzhmdy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.hysaishi.cn/gtvnbuwrtr.html

Ruby: def greet; @name; end
来源：http://hz.ivvv.top/gtwpjgzlew.html

C#:   public string Greet() => Name;
来源：http://hz.jianghu66.top/gtxmauxpzz.html

[G05] 继承
来源：http://hz.sysykeji.top/gtydmdghxq.html

Py:   class Admin(User): pass
来源：http://hz.shzxlz.cn/gtxapocxig.html

PHP:  class Admin extends User {}
来源：http://hz.yanxiufei.cn/gtntxlahvw.html

JS:   class Admin extends User {}
来源：http://hz.vqdsnc.cn/gthspwjqhw.html

TS:   class Admin extends User {}
来源：http://hz.redwolf501.top/gtudqbtqyu.html

Java: class Admin extends User {}
来源：http://hz.svipenyu.cn/gtdcltrzmk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.shuidangran.top/gtledwgwdi.html

Ruby: class Admin < User; end
来源：http://hz.feifeiyinyue.top/gtfvdtafos.html

C#:   class Admin : User {}
来源：http://hz.gogol.net.cn/gtgvdlpzta.html

[G06] 重写方法
来源：http://hz.tanke756.top/gthrnmgxsw.html

Py:   def greet(self): return "admin"
来源：http://hz.ivvv.top/gtfbdxplnu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.haohaochexian.top/gtzskgydpm.html

JS:   greet() { return "admin"; }
来源：http://hz.yj20258.top/gtptiajoci.html

TS:   greet(): string { return "admin"; }
来源：http://hz.sysykeji.top/gtuqijagdi.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.nanxinkj.top/gtwqyuxzwt.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.xingfuxueyuan.xyz/gtovqhwweu.html

Ruby: def greet; "admin"; end
来源：http://hz.jianghu66.top/gtwcacmebt.html

C#:   public override string Greet() => "admin";
来源：http://hz.guowangkeji.top/gtkchluvgn.html

[G07] 调用父类方法
来源：http://hz.yanxiufei.cn/gtpffdldtc.html

Py:   super().greet()
来源：http://hz.sweek.top/gtbkekxlau.html

PHP:  parent::greet();
来源：http://hz.shangyingyoupin.top/gtkdmlagzk.html

JS:   super.greet();
来源：http://hz.shanyushiyangtech.top/gtzerpdseg.html

TS:   super.greet();
来源：http://hz.yongpay.top/gtbmaksfsi.html

Java: super.greet();
来源：http://hz.nanxuanxn.top/gtxyulokgf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.shuidangran.top/gtikpipiwe.html

Ruby: super
来源：http://hz.hammf.cn/gtdzrmweew.html

C#:   base.Greet();
来源：http://hz.guowangkeji.top/gtlvypoosd.html

[G08] 静态方法与属性
来源：http://hz.gotoacloud.top/gtojhklxpo.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.yj202588.top/gteqiykvdz.html

PHP:  public static function f() {}
来源：http://hz.cucudq.cn/gtihkyykxe.html

JS:   static f() {}
来源：http://hz.hongshengwenyu.top/gtqaowpffd.html

TS:   static f(): void {}
来源：http://hz.gaohongyu789.top/gtjclatwzd.html

Java: static void f() {}
来源：http://hz.quarkkingdee.top/gtjcvhejnk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.zhaomingkeji.xyz/gtumwbzuus.html

Ruby: def self.f; end
来源：http://hz.gotoacloud.top/gtodbeqrhp.html

C#:   public static void F() {}
来源：http://hz.daxiang520.top/gtoccpjmun.html

[G09] 接口 / 抽象类
来源：http://hz.yonumen.top/gtxduddspg.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.chenjidiqi.icu/gtkuceknvv.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jinyuanbaomall.cn/gtbmxiazca.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.chenjidiqi.icu/gtthyqqqqq.html

TS:   interface Shape { area(): number; }
来源：http://hz.dianchejie.cn/gtavvpwqxf.html

Java: interface Shape { double area(); }
来源：http://hz.gotoacloud.top/gtbwzeeuto.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.feifeiyinyue.top/gtwyqkqwwc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jyoumei.cn/gtlxtdfdma.html

C#:   interface IShape { double Area(); }
来源：http://hz.tianlin.xyz/gtlpumwfwa.html

[G10] 访问控制
来源：http://hz.ywan-chungtsiang.top/gthmpoljqo.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.cdnleiting.top/gttqvsvqvq.html

PHP:  public / protected / private
来源：http://hz.hfpthk.cn/gtqvezgtld.html

JS:   #private 字段；其余公开
来源：http://hz.chenlongwang.top/gtxyuifmon.html

TS:   public / protected / private
来源：http://hz.xinyue.icu/gtllfqjlfg.html

Java: public / protected / private / 默认包级
来源：http://hz.wangshuangyany.cn/gtudojoncd.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.chenzaomai.com/gtzcvepkhh.html

Ruby: public / protected / private
来源：http://hz.sxryk.cn/gtzlohaoia.html

C#:   public / protected / private / internal
来源：http://hz.hnxiangtu.top/gtgfsibept.html

[G11] getter / setter
来源：http://hz.iojbl.cn/gtcvlzjnau.html

Py:   @property 与 @x.setter
来源：http://hz.0kj1m.cn/gtmpztqhlz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.cqqwz.cn/gtsdyhtjpo.html

JS:   get name() { return this._name; }
来源：http://hz.pengpengdd.cyou/gtcxnrquww.html

TS:   get name(): string { return this._name; }
来源：http://hz.shanyushiyangkeji.top/gtzdshwbyr.html

Java: public String getName() { return name; }
来源：http://hz.wangdashe.top/gtvuwqnhcq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.sxryk.cn/gtqvahtlcp.html

Ruby: attr_accessor :name
来源：http://hz.hfpthk.cn/gtilvxdnab.html

C#:   public string Name { get; set; }
来源：http://hz.zhijiandao.cn/gtfwuuqdrh.html

[G12] 对象转字符串
来源：http://hz.hongshengwenyu.top/gtefwfutuk.html

Py:   def __str__(self): return self.name
来源：http://hz.tanke756.top/gttofhdvob.html


<!-- 参考信息 -->