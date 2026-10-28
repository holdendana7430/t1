代发 wailian999

Py:   for ch in s: print(ch)
来源：http://hz.jianghu66.top/gtyylhcjwj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.gotoacloud.top/gtadxuyduc.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.tianlin.xyz/gtmphojlye.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.gzhubu.top/gtzgnwwdsu.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.yuanzhike.top/gtmciuxutv.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.yueranfly.top/gtctvykdrp.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.zhongyouzk.top/gtmfqygmqk.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.quarkkingdee.top/gtuonjmcll.html

[E14] URL 编码与 Base64
来源：http://hz.sysykeji.top/gtnqivdyoe.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.hnqzz.top/gteysjvwrj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.nanxuanxn.top/gtzweajgpb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.dianchejie.cn/gtjjoqybkl.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.smart0.xyz/gtwxzdkykr.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.nanxuanxn.top/gtohatytre.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.jqgfzy.top/gtypzpkedu.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.jinyuanbaomall.cn/gthoqtvfiv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.snrcjt.cn/gtoeaoeijo.html

[E15] HTML 转义 / 反转义
来源：http://hz.yj202588.top/gtgqsdrmkp.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.aibaodan.cn/gtrnekbxbd.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.chenlongwang.top/gtjvvlzhhm.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.pycfn.com/gtsilaurko.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.tianlin.xyz/gtxenxlreg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.aizwys.cn/gteovindia.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.vqdsnc.cn/gttfjouwxx.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.gaohongyu789.top/gtaostwvrj.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.yongpay.top/gtjakrydix.html

[E16] 数字千分位
来源：http://hz.zdqjudy.top/gtiuztlezf.html

Py:   f"{1234567:,}"
来源：http://hz.xziqi.cn/gtxobzaxtl.html

PHP:  number_format(1234567);
来源：http://hz.bjfxy.top/gtlakigzch.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.chenjidiqi.icu/gtfhosjogg.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.guannengcc.top/gtoobshebj.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.hywenlv.cn/gtilumapuk.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.yj202588.top/gtedhprjtf.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.xylfe.cn/gtuilekrbz.html

C#:   1234567.ToString("N0")
来源：http://hz.meibo888.top/gtiouxqgpy.html

[E17] 首字母大写
来源：http://hz.sweek.top/gtoamhgihg.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.jianghu66.top/gtncflqguz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.ppjwa.cn/gtnovrcins.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.wangshuangyany.cn/gtltaavaxi.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.shzxlz.cn/gtpexallds.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.jyoumei.cn/gteuoadbjd.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.ivvv.top/gtsoiusanx.html

Ruby: s.capitalize
来源：http://hz.nanxinkj.top/gtunabdghq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yj202588.top/gtnzuciefm.html

[E18] 模板占位符替换
来源：http://hz.chenlongwang.top/gtawwpcvod.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.andypj.xyz/gtagbetqmq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.shzxlz.cn/gtixiemypc.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.cucudq.cn/gtiworihue.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.jinqigfzy.top/gtnaysofnz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.yueranfly.top/gtofemgooc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.sxryk.cn/gttujvslgj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.pengpengdd.cyou/gtrdmskkrm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.daxiang520.top/gtemfstpyy.html

[E19] 多行文本按行拆分
来源：http://hz.jinqigufen.top/gtlpdmflcs.html

Py:   s.splitlines()
来源：http://hz.cqqwz.cn/gtmaazsuam.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.nanxinkj.top/gtkdsabvnr.html

JS:   s.split(/\r?\n/)
来源：http://hz.xuetiantiany.cn/gtazcgnuco.html

TS:   s.split(/\r?\n/)
来源：http://hz.cheryme.top/gtxbcyzvrk.html

Java: s.lines().toList()
来源：http://hz.hnqzz.top/gtcjzfogqc.html

Go:   strings.Split(s, "\n")
来源：http://hz.meibo888.top/gtdwefjjyp.html

Ruby: s.lines
来源：http://hz.zhijiandao.cn/gtkiojqind.html

C#:   s.Split('\n')
来源：http://hz.gzhubu.top/gtgahukjzs.html

[E20] 判断字符串是否为空
来源：http://hz.fengsongda.top/gtvpxjsuuy.html

Py:   if not s:
来源：http://hz.yueranfly.top/gtxvmufikd.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.kuanghao11.cn/gtbbilmgcq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.yonumen.top/gttdmofoqp.html

TS:   if (s === "") {}
来源：http://hz.zhongyouzk.top/gtkdlrqpwf.html

Java: if (s.isEmpty()) {}
来源：http://hz.zhoulong.xyz/gtqahidair.html

Go:   if s == "" {}
来源：http://hz.sufxvd.cn/gtfkwhtnug.html

Ruby: if s.empty?
来源：http://hz.yongpay.top/gtrypspoeq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.zhijiandao.cn/gtqqoqzeab.html

[E21] 超长截断加省略号
来源：http://hz.guannengcc.top/gtdwkyfmff.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.tian-w.cn/gtavgttsbq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.ehwqpu.com/gtzuvehwnd.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.xuetiantiany.cn/gtracpqxlo.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.wangshuangyany.cn/gtnhhnrrkd.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.52xcode.cn/gtnqfhpifj.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.zhixingplan.top/gtoauispbc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.quarkkingdee.top/gtmpytfdwf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.redwolf501.top/gtsdpehqas.html

[E22] 字节长度与字符长度
来源：http://hz.ydjk.org.cn/gtujkkwtev.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.xingfuxueyuan.xyz/gtsciyxxex.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.hywenlv.cn/gtbxulsgoq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hammf.cn/gtxoadgkml.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.chenlongwang.top/gtaiufbpyf.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.hywenlv.cn/gtgygpdyhp.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.xinyue.icu/gtqrzskauo.html

Ruby: s.bytesize;  s.length
来源：http://hz.kuanghao11.cn/gtxqlwpiwx.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.gotoacloud.top/gtlxhcwasq.html

================================================================================
来源：http://hz.tanke756.top/gtamjssxyp.html

F. 文件与目录
来源：http://hz.ydjk.org.cn/gtdstducvp.html

================================================================================
来源：http://hz.jinqigufen.top/gtimaxczey.html

[F01] 读取整个文件
来源：http://hz.pengpengdd.cyou/gtppewycly.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yanxiufei.cn/gtvfimncwd.html

PHP:  file_get_contents("a.txt");
来源：http://hz.sxryk.cn/gtmafffwlh.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.nanxuanxn.top/gtvtaiqgun.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.xuetiantiany.cn/gtiubigcdq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.ivvv.top/gtcygsccaj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.chenzaomai.com/gtssjbsswc.html

Ruby: File.read("a.txt")
来源：http://hz.tanke756.top/gtyypbtbsw.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.guowangkeji.top/gtxutwzoph.html

[F02] 逐行读取文件
来源：http://hz.shangyingyoupin.top/gtkpplbryy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.ydzc1.top/gtotkqtshl.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.wangdashe.top/gttuqqdxqq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.gotoacloud.top/gtotaepldr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yj202588.top/gtykyenuaz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.chenlongwang.top/gtfamgqurq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.nanxuanxn.top/gtwncusrsm.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.zhengqikj.top/gtcrybowfr.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.gzhubu.top/gtgxxshddt.html

[F03] 写入文件（覆盖）
来源：http://hz.ppjwa.cn/gtxdygvduk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.aibaodan.cn/gtinmeshve.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.mhx1999.top/gtgyzqkmdk.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.mhx1999.top/gttfbihcyq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.shanyushiyangtech.top/gtjsxpdzzy.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.hnqzz.top/gtwoxxacqs.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.jlsjyb.cn/gtfzmdwceq.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.shanyushiyangkeji.top/gtbneduheq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.jyoumei.cn/gtttxmhtbw.html

[F04] 追加写入文件
来源：http://hz.shangyingyoupin.top/gthakicfay.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yangfankeji.com/gtwltsfklw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.zhongyouzk.top/gtbwbecsei.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.fzhhl.top/gtwymkgonh.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ywan-chungtsiang.top/gtmdipvzhg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.zycfv.cn/gtblpzhtpw.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.tianlin.xyz/gttscubger.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yuanzhike.top/gtffbicomf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.jinqigufen.top/gtgsfztifm.html

[F05] 判断文件或目录是否存在
来源：http://hz.daria6918.cn/gtfenoggnz.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.andypj.xyz/gtevlssfcp.html

PHP:  file_exists("a.txt");
来源：http://hz.andypj.xyz/gthrnpepvm.html

JS:   fs.existsSync("a.txt")
来源：http://hz.cqqwz.cn/gtumaplypt.html

TS:   fs.existsSync("a.txt")
来源：http://hz.hnxiangtu.top/gtvdtecxns.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.chenlongwang.top/gtlodwgbjh.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.cashguo.top/gtfzkjmixz.html

Ruby: File.exist?("a.txt")
来源：http://hz.feifeiyinyue.top/gtqvulvmbp.html

C#:   File.Exists("a.txt")
来源：http://hz.sysykeji.top/gthuuhmdhm.html

[F06] 删除文件
来源：http://hz.xziqi.cn/gtjxajgqtx.html

Py:   os.remove("a.txt")
来源：http://hz.yanxiufei.cn/gttcugkdtn.html

PHP:  unlink("a.txt");
来源：http://hz.jianghu66.top/gtjavfyiov.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.0kj1m.cn/gtesabbzkv.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.gogol.net.cn/gtvkolbxst.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.zhengqikj.top/gtjginmnbm.html

Go:   os.Remove("a.txt")
来源：http://hz.nwbrower.top/gtsgwsivyb.html

Ruby: File.delete("a.txt")
来源：http://hz.xuetiantiany.cn/gtbzqfwjib.html

C#:   File.Delete("a.txt");
来源：http://hz.ehwqpu.com/gtinffbvaj.html

[F07] 创建目录（含多级）
来源：http://hz.cdnleiting.top/gtvfxqcbnn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yj20258888.top/gturdirkjx.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.chenlongwang.top/gtqvpehtpd.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.feifeiyinyue.top/gtxrfrgwyu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ehwqpu.com/gtvplwpdqg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.wangdashe.top/gtuvjvoidn.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.yuxming.cn/gtadaaxcgo.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.hfpthk.cn/gtzkltarck.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.guannengcc.top/gtwojlrtif.html

[F08] 遍历目录
来源：http://hz.ydjk.org.cn/gtpykdgdst.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.fengsongda.top/gtbihedhbr.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.shuidangran.top/gtbtoqphii.html

JS:   fs.readdirSync("dir")
来源：http://hz.ivvv.top/gtbhfnurlz.html

TS:   fs.readdirSync("dir")
来源：http://hz.chenlongwang.top/gtotoaaeen.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.meibo888.top/gtdlhpemsr.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.jinqigufen.top/gtlwhhxjho.html

Ruby: Dir.children("dir")
来源：http://hz.wangshuangyany.cn/gtrhdmqzxy.html

C#:   Directory.GetFiles("dir")
来源：http://hz.cheryme.top/gtoettycuz.html

[F09] 获取文件大小
来源：http://hz.jianghu66.top/gtkviaooft.html

Py:   os.path.getsize("a.txt")
来源：http://hz.chenzaomai.com/gttioxbgvn.html

PHP:  filesize("a.txt");
来源：http://hz.c1oappe.top/gtprlevukl.html

JS:   fs.statSync("a.txt").size
来源：http://hz.svipenyu.cn/gtidhsycrv.html

TS:   fs.statSync("a.txt").size
来源：http://hz.hnxiangtu.top/gtqoqinpks.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.snrcjt.cn/gtuahnrbpa.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.xingfuxueyuan.xyz/gtuwcedafb.html

Ruby: File.size("a.txt")
来源：http://hz.wangshuangyany.cn/gtoxnaardz.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.ywan-chungtsiang.top/gthumqejwd.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.9152youxi.cn/gtewfepxel.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jlsjyb.cn/gtpcexpavi.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.ydzc1.top/gtvgjkiirt.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.shuidangran.top/gtqpqlqspe.html

TS:   path.extname("a.txt")
来源：http://hz.shzxlz.cn/gtsaicoosr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.yj20258.top/gtppppbohd.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.tanke756.top/gtklwffdmz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.ydzc1.top/gtwjccnavh.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.shangyingyoupin.top/gtndcxurov.html

[F11] 复制与移动文件
来源：http://hz.redwolf501.top/gtyeyoigxy.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.gotoacloud.top/gtsdnifhup.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.ehwqpu.com/gtewljfjdi.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.52xcode.cn/gtakxhclcs.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yj202588.top/gtcmekdaip.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.shangyingyoupin.top/gtytgvporo.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.sufxvd.cn/gtywsrbqkp.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.havefunace.top/gtlqeexhet.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.jiagoushi.top/gtiihcsnzg.html

[F12] CSV 读写
来源：http://hz.cashguo.top/gtraxrvidi.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.andypj.xyz/gtgksygbye.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.mhx1999.top/gtkdarxkcd.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.iojbl.cn/gtxpfvqwyh.html

TS:   // 同上
来源：http://hz.redwolf501.top/gtquvihwgh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.jinqigfzy.top/gtwwupvouc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.shanyushiyangtech.top/gtqbpqbjrd.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.fzhhl.top/gtlrreiwfi.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.svipenyu.cn/gtijirzlna.html

================================================================================
来源：http://hz.xinyue.icu/gtivofponf.html

G. 面向对象
来源：http://hz.zhongyouzk.top/gtbrhphuip.html

================================================================================
来源：http://hz.zhixingplan.top/gtdtpxwybf.html

[G01] 定义类
来源：http://hz.xuetiantiany.cn/gthylprwez.html

Py:   class User: pass
来源：http://hz.yj20258888.top/gtxopgvjqi.html

PHP:  class User {}
来源：http://hz.zdqjudy.top/gtdgdnrgmu.html

JS:   class User {}
来源：http://hz.xuanzx.com/gtvfxohyhn.html

TS:   class User { name: string = ""; }
来源：http://hz.9152youxi.cn/gtejraojel.html

Java: class User {}
来源：http://hz.tanke756.top/gtjoihzqwi.html

Go:   type User struct { Name string }
来源：http://hz.aibaodan.cn/gtfaxigaeh.html

Ruby: class User; end
来源：http://hz.gaohongyu789.top/gtctrgmtgm.html

C#:   class User {}
来源：http://hz.wangdashe.top/gthznycblm.html

[G02] 构造函数
来源：http://hz.0kj1m.cn/gtydfwriqf.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.tianlin.xyz/gtbtzxbkcs.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.ivvv.top/gtbztashbb.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.guowangkeji.top/gtiktegysi.html

TS:   constructor(public name: string) {}
来源：http://hz.yuxming.cn/gtjyojqhev.html

Java: User(String name) { this.name = name; }
来源：http://hz.iojbl.cn/gtqlstwiug.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.52xcode.cn/gtsbiexjsu.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yongpay.top/gtkoddrlam.html

C#:   public User(string name) { Name = name; }
来源：http://hz.gzhubu.top/gthyhtfjgu.html

[G03] 实例属性
来源：http://hz.daxiang520.top/gtktybywwm.html

Py:   self.name = "x"
来源：http://hz.zhoulong.xyz/gtbluoofdr.html

PHP:  public string $name = "x";
来源：http://hz.cqqwz.cn/gtzekwbgeh.html

JS:   this.name = "x";
来源：http://hz.aibaodan.cn/gtujhwzymy.html

TS:   name: string = "x";
来源：http://hz.shzxlz.cn/gtulqfdlca.html

Java: private String name;
来源：http://hz.feifeiyinyue.top/gtgplzcdta.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.ydzc1.top/gtuffsmivi.html

Ruby: @name = "x"
来源：http://hz.pengpengdd.cyou/gtjfulqgcl.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jinqigufen.top/gtlrzphjxp.html

[G04] 定义方法
来源：http://hz.hnqzz.top/gtqlxlljmk.html

Py:   def greet(self): return self.name
来源：http://hz.dianchejie.cn/gtffntjrvu.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.sysykeji.top/gtyuasswbk.html

JS:   greet() { return this.name; }
来源：http://hz.ppjwa.cn/gtdgwktqtf.html

TS:   greet(): string { return this.name; }
来源：http://hz.yj20258888.top/gtkbgyvrvw.html

Java: String greet() { return name; }
来源：http://hz.hnxiangtu.top/gtzbhlqwkg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.hammf.cn/gtdixzafis.html

Ruby: def greet; @name; end
来源：http://hz.zycfv.cn/gtlqgxqvmm.html

C#:   public string Greet() => Name;
来源：http://hz.guowangkeji.top/gtnxtpwxek.html

[G05] 继承
来源：http://hz.ehwqpu.com/gtqsaqnolw.html

Py:   class Admin(User): pass
来源：http://hz.smart0.xyz/gtdhhpkage.html

PHP:  class Admin extends User {}
来源：http://hz.birdmap.top/gtortnzskm.html

JS:   class Admin extends User {}
来源：http://hz.zdqjudy.top/gtmnoapqbu.html

TS:   class Admin extends User {}
来源：http://hz.guannengcc.top/gtaylminmh.html

Java: class Admin extends User {}
来源：http://hz.guowangkeji.top/gtvhuegqec.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.gaohongyu789.top/gtttwrhwrx.html

Ruby: class Admin < User; end
来源：http://hz.jinghuilouyu.cn/gtgedpytpp.html

C#:   class Admin : User {}
来源：http://hz.gaohongyu789.top/gtbhqmcxzz.html

[G06] 重写方法
来源：http://hz.jinqigufen.top/gtserzokts.html

Py:   def greet(self): return "admin"
来源：http://hz.sufxvd.cn/gtpnktiztx.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.sweek.top/gtpsvpjczq.html

JS:   greet() { return "admin"; }
来源：http://hz.smart0.xyz/gtklpwshds.html

TS:   greet(): string { return "admin"; }
来源：http://hz.cqqwz.cn/gtgbrfszwj.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.daxiang520.top/gtfkyyhxvr.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.gogol.net.cn/gtirciuqjh.html

Ruby: def greet; "admin"; end
来源：http://hz.xylfe.cn/gtkapsaqqn.html

C#:   public override string Greet() => "admin";
来源：http://hz.xinyue.icu/gtzvehucxu.html

[G07] 调用父类方法
来源：http://hz.ybcxt.top/gtqjjyqifh.html

Py:   super().greet()
来源：http://hz.52xcode.cn/gtfkfgkvmz.html

PHP:  parent::greet();
来源：http://hz.yonumen.top/gtkgvcrlpp.html

JS:   super.greet();
来源：http://hz.sysykeji.top/gtrwtfwtav.html

TS:   super.greet();
来源：http://hz.xuanzx.com/gtrpzrwakh.html

Java: super.greet();
来源：http://hz.jqgufenzy.top/gtdoajjxqk.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.aibaodan.cn/gttqeryamf.html

Ruby: super
来源：http://hz.jinghuilouyu.cn/gtaljbghxz.html

C#:   base.Greet();
来源：http://hz.ehwqpu.com/gtgjjdjepb.html

[G08] 静态方法与属性
来源：http://hz.hywenlv.cn/gtadincaci.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.shanyushiyangtech.top/gtcktoqzel.html

PHP:  public static function f() {}
来源：http://hz.cdnleiting.top/gtoqvsycks.html

JS:   static f() {}
来源：http://hz.cucudq.cn/gtvmzpswgv.html

TS:   static f(): void {}
来源：http://hz.birdmap.top/gtfnjrkixg.html

Java: static void f() {}
来源：http://hz.smart0.xyz/gtonvznqwh.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jqgufenzy.top/gtwjbwhjgu.html

Ruby: def self.f; end
来源：http://hz.shanyushiyangkeji.top/gtpbdfonit.html

C#:   public static void F() {}
来源：http://hz.yangfankeji.com/gtwtjcythh.html

[G09] 接口 / 抽象类
来源：http://hz.chenlongwang.top/gthzthkbin.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.feifeiyinyue.top/gtdaabiswh.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.tanke756.top/gtujjkwlgk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.vqdsnc.cn/gtdtdjapxk.html

TS:   interface Shape { area(): number; }
来源：http://hz.jinqigfzy.top/gtdnnkjlhi.html

Java: interface Shape { double area(); }
来源：http://hz.zhijiandao.cn/gtrgnlpgio.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yongpay.top/gtmekxcpsp.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yanxiufei.cn/gthgqdorgt.html

C#:   interface IShape { double Area(); }
来源：http://hz.wangdashe.top/gtaronkfct.html

[G10] 访问控制
来源：http://hz.bjfxy.top/gtesajlssy.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.hnxiangtu.top/gttoxbnbbg.html

PHP:  public / protected / private
来源：http://hz.tian-w.cn/gtijlppfen.html

JS:   #private 字段；其余公开
来源：http://hz.xuanzx.com/gtdvgzaayn.html

TS:   public / protected / private
来源：http://hz.shanyushiyangkeji.top/gtagiksvbg.html

Java: public / protected / private / 默认包级
来源：http://hz.andypj.xyz/gtsthgnaym.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.ywan-chungtsiang.top/gtzvmzupai.html

Ruby: public / protected / private
来源：http://hz.hammf.cn/gtgdglrlrp.html

C#:   public / protected / private / internal
来源：http://hz.jlsjyb.cn/gttwufjfkt.html

[G11] getter / setter
来源：http://hz.yonumen.top/gthbjyqnpo.html

Py:   @property 与 @x.setter
来源：http://hz.feifeiyinyue.top/gtuxkmrxlv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.smart0.xyz/gtjidgjpaw.html

JS:   get name() { return this._name; }
来源：http://hz.zhaomingkeji.xyz/gtybwfwqkn.html

TS:   get name(): string { return this._name; }
来源：http://hz.zhiwuduotai.top/gtpvosmkbj.html

Java: public String getName() { return name; }
来源：http://hz.jinghuilouyu.cn/gthwmulkvm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.nanxinkj.top/gtpuapvjuj.html


<!-- 参考信息 -->