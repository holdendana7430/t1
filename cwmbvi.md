代发 wailian999

PHP:  substr_count($s, "a");
来源：http://hz.nanxinkj.top/gtmquggjsd.html

JS:   s.split("a").length - 1
来源：http://hz.xinyue.icu/gtqbrvnrlo.html

TS:   s.split("a").length - 1
来源：http://hz.iojbl.cn/gtmdllszoe.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.nanxinkj.top/gtvtdjbrfm.html

Go:   strings.Count(s, "a")
来源：http://hz.nanxinkj.top/gtdcoovxbr.html

Ruby: s.count("a")
来源：http://hz.sufxvd.cn/gtuhcxuctn.html

C#:   s.Count(c => c == 'a')
来源：http://hz.meibo888.top/gtdrcxfjes.html

[E13] 逐字符遍历
来源：http://hz.316326.xyz/gtfpbubcxg.html

Py:   for ch in s: print(ch)
来源：http://hz.guowangkeji.top/gtufgzbjsq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.jianghu66.top/gtqpdbypyf.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.cqqwz.cn/gtqbxflmku.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.c1oappe.top/gtunylyhqr.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.jinyuanbaomall.cn/gtueufhoky.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.vqdsnc.cn/gtfhnsoiyd.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.ydzc1.top/gtrztokciu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.yueranfly.top/gthsalogzi.html

[E14] URL 编码与 Base64
来源：http://hz.jinghuilouyu.cn/gtnvljywhr.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.tanke756.top/gtzuehwxoo.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.guowangkeji.top/gtofyyxjby.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.hongshengwenyu.top/gtssghhayx.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.hfpthk.cn/gtxzizmzjg.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.ppjwa.cn/gtqwxzlsjm.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.jqgfzy.top/gtfdlnyweu.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.0kj1m.cn/gtpwatrzut.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.xingfuxueyuan.xyz/gtojfjhsbj.html

[E15] HTML 转义 / 反转义
来源：http://hz.feifeiyinyue.top/gtvdlmwwrs.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.yj20258.top/gtpurckiik.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.zhiwuduotai.top/gtbhczwpsp.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.jinqigufen.top/gtnpwlqdsh.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.quarkkingdee.top/gtfbqywsgy.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.nanxinkj.top/gtiflsjqzc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.sufxvd.cn/gtqarcngmo.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.guannengcc.top/gttyiwqkox.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.zhixingplan.top/gtozkrklft.html

[E16] 数字千分位
来源：http://hz.jinqigufen.top/gtxjhtwulp.html

Py:   f"{1234567:,}"
来源：http://hz.zhaomingkeji.xyz/gtoyzuoubl.html

PHP:  number_format(1234567);
来源：http://hz.guannengcc.top/gtuqwwgptj.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.jiagoushi.top/gtmviyqnmv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.mhx1999.top/gtrqigxzog.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.jiagoushi.top/gtjzldswzc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.dashuyun.cn/gtuezhdihm.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.jianghu66.top/gttdytiipy.html

C#:   1234567.ToString("N0")
来源：http://hz.smart0.xyz/gtftgjcvzi.html

[E17] 首字母大写
来源：http://hz.jqgfzy.top/gtmahvhhqk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.jianghu66.top/gthwgfmodl.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.hysaishi.cn/gtumohgexw.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.sweek.top/gtejsuziao.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.feifeiyinyue.top/gtkadywybm.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.guowangkeji.top/gtwbylcwpc.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.redwolf501.top/gthpgyotyl.html

Ruby: s.capitalize
来源：http://hz.cucudq.cn/gtikwlrkdt.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.zhaomingkeji.xyz/gtzdestsiy.html

[E18] 模板占位符替换
来源：http://hz.ywan-chungtsiang.top/gtxfuvdnfk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.wangshuangyany.cn/gtdmmlcvgl.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.hywenlv.cn/gtysznxdkb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.hnxiangtu.top/gtzdyzvsnr.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.zhijiandao.cn/gthycutnxp.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.sweek.top/gtobeynews.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.52xcode.cn/gtffapollk.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.52xcode.cn/gtqtgkvhcc.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.cucudq.cn/gttleisiuf.html

[E19] 多行文本按行拆分
来源：http://hz.bjfxy.top/gtpcsdqkyg.html

Py:   s.splitlines()
来源：http://hz.tanke756.top/gtomomlwfm.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.tian-w.cn/gtzcdcyoop.html

JS:   s.split(/\r?\n/)
来源：http://hz.shangyingyoupin.top/gtuiinnhnc.html

TS:   s.split(/\r?\n/)
来源：http://hz.svipenyu.cn/gtwhtgfjby.html

Java: s.lines().toList()
来源：http://hz.shangyingyoupin.top/gtrpqcdlpt.html

Go:   strings.Split(s, "\n")
来源：http://hz.yj20258.top/gtoijfrnzc.html

Ruby: s.lines
来源：http://hz.cheryme.top/gtkwvdmfvq.html

C#:   s.Split('\n')
来源：http://hz.guannengcc.top/gtxtsizfxg.html

[E20] 判断字符串是否为空
来源：http://hz.fzhhl.top/gtifxljanv.html

Py:   if not s:
来源：http://hz.shanyushiyangtech.top/gtbafpzuop.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.bjfxy.top/gtuwjfpfmu.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.sufxvd.cn/gtnozqstlk.html

TS:   if (s === "") {}
来源：http://hz.zhengqikj.top/gtmqacvcpk.html

Java: if (s.isEmpty()) {}
来源：http://hz.wangshuangyany.cn/gtwycxtqld.html

Go:   if s == "" {}
来源：http://hz.cashguo.top/gthwcsqdrw.html

Ruby: if s.empty?
来源：http://hz.yvedp.cn/gtzvpvrmlg.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.tanke756.top/gtrltzxfuf.html

[E21] 超长截断加省略号
来源：http://hz.zhongyouzk.top/gtaleldect.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.gotoacloud.top/gtnabxitkh.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.fzhhl.top/gtvducaevd.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ehwqpu.com/gtdtvvqynl.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ywan-chungtsiang.top/gtbnnvusua.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.pycfn.com/gtcrcwbpaj.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.shangyingyoupin.top/gtqudcjgbd.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.0kj1m.cn/gtgxogfrmc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.haohaochexian.top/gtpkfvuugn.html

[E22] 字节长度与字符长度
来源：http://hz.haohaochexian.top/gtefczhtly.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.hnqzz.top/gtgntcsvlx.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.wangshuangyany.cn/gtvrlxnboo.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhijiandao.cn/gtzutkjbxa.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.sweek.top/gtpkgoioiv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jyoumei.cn/gtavlbxswo.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.jqgfzy.top/gtowyaawgr.html

Ruby: s.bytesize;  s.length
来源：http://hz.gotoacloud.top/gtdosolltj.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.yonumen.top/gtgmxcqfhm.html

================================================================================
来源：http://hz.ehwqpu.com/gtnzxclrrg.html

F. 文件与目录
来源：http://hz.aizwys.cn/gtthamfxlz.html

================================================================================
来源：http://hz.shuidangran.top/gtxqqvfggk.html

[F01] 读取整个文件
来源：http://hz.ivvv.top/gtmocmoukg.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.bjfxy.top/gtfpvqopui.html

PHP:  file_get_contents("a.txt");
来源：http://hz.gotoacloud.top/gtktbvzvbg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.hfpthk.cn/gttjzptsxi.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.quarkkingdee.top/gtjrzdudhk.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.haohaochexian.top/gtbgrjlyfq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.yvedp.cn/gtpghvybzj.html

Ruby: File.read("a.txt")
来源：http://hz.jiagoushi.top/gtkkacutkt.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.dashuyun.cn/gtokodeuao.html

[F02] 逐行读取文件
来源：http://hz.sysykeji.top/gtzthilyqp.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.fzhhl.top/gticqrikrn.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.yonumen.top/gtdnixxodl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.mhx1999.top/gtyriwvwqo.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.birdmap.top/gtzqwkkvcj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.yj202588.top/gtfccsxbun.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.yj20258.top/gtdouktyzv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.jqgfzy.top/gtstybauom.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.tianlin.xyz/gtmylbkavr.html

[F03] 写入文件（覆盖）
来源：http://hz.sysykeji.top/gtvwsftpjg.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.0kj1m.cn/gtqideeyru.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.chenlongwang.top/gtmyzkknvg.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hnqzz.top/gtcipoaurz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ybcxt.top/gthelrktgo.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.xuetiantiany.cn/gtpapqirte.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.shzxlz.cn/gtgwsmuszk.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.haohaochexian.top/gtjxrexldo.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.ybcxt.top/gtfijcgnhv.html

[F04] 追加写入文件
来源：http://hz.nwbrower.top/gtbrtayzmv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.wangdashe.top/gtwwbpycxr.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.tanke756.top/gtpbfgwaqc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ehwqpu.com/gtklpajfto.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.sufxvd.cn/gtrlqwektd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.ivvv.top/gtkslbnbbm.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.hnxiangtu.top/gtxomxyhhy.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.0kj1m.cn/gtdbayctbk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.shanyushiyangkeji.top/gtuxccodpa.html

[F05] 判断文件或目录是否存在
来源：http://hz.tianlin.xyz/gthrtdkype.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.hysaishi.cn/gttybtmcxe.html

PHP:  file_exists("a.txt");
来源：http://hz.ppjwa.cn/gtglvfdaee.html

JS:   fs.existsSync("a.txt")
来源：http://hz.sufxvd.cn/gthxgdsevj.html

TS:   fs.existsSync("a.txt")
来源：http://hz.wangdashe.top/gttsfpjjox.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.chenlongwang.top/gtscdpmmlq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.yangfankeji.com/gtizdbqwee.html

Ruby: File.exist?("a.txt")
来源：http://hz.tanke756.top/gtezmrikem.html

C#:   File.Exists("a.txt")
来源：http://hz.havefunace.top/gtczdzxdgy.html

[F06] 删除文件
来源：http://hz.hysaishi.cn/gtkqbyyxip.html

Py:   os.remove("a.txt")
来源：http://hz.bjfxy.top/gtvsaldxxi.html

PHP:  unlink("a.txt");
来源：http://hz.smart0.xyz/gtsyxrkysh.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yuxming.cn/gtguhcpxww.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.yuanzhike.top/gtucjcqvwb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.hywenlv.cn/gtndhhriya.html

Go:   os.Remove("a.txt")
来源：http://hz.dashuyun.cn/gtewsytmul.html

Ruby: File.delete("a.txt")
来源：http://hz.guannengcc.top/gtillppsox.html

C#:   File.Delete("a.txt");
来源：http://hz.yj20258.top/gtoccvduwj.html

[F07] 创建目录（含多级）
来源：http://hz.ehwqpu.com/gtffhvuxjc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.quarkkingdee.top/gtcncnqvia.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.shanyushiyangkeji.top/gtnstsyvas.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jyoumei.cn/gtxmwatroj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yuxming.cn/gtnrmrkdgz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.wangshuangyany.cn/gtoerrhbdh.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.52xcode.cn/gtyekwlyre.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.gaohongyu789.top/gtkaqxbnbv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.gotoacloud.top/gtlntdajfo.html

[F08] 遍历目录
来源：http://hz.cashguo.top/gtkcntyzsi.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.snrcjt.cn/gtnowoaira.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.nanxuanxn.top/gtcqbjmdwy.html

JS:   fs.readdirSync("dir")
来源：http://hz.yj202588.top/gtftrwsbrl.html

TS:   fs.readdirSync("dir")
来源：http://hz.vqdsnc.cn/gtddfsrmkt.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.wangdashe.top/gtxfjqxjjp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.tanke756.top/gthxlgtkek.html

Ruby: Dir.children("dir")
来源：http://hz.jqgfzy.top/gtalhakcqx.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yj20258.top/gtxniylhwh.html

[F09] 获取文件大小
来源：http://hz.xylfe.cn/gtorqcnyvh.html

Py:   os.path.getsize("a.txt")
来源：http://hz.pengpengdd.cyou/gtdishaimn.html

PHP:  filesize("a.txt");
来源：http://hz.nanxinkj.top/gtobuhctmy.html

JS:   fs.statSync("a.txt").size
来源：http://hz.pengpengdd.cyou/gtrunecvle.html

TS:   fs.statSync("a.txt").size
来源：http://hz.svipenyu.cn/gtednboizg.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.dianchejie.cn/gtxqzdavtc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.yangfankeji.com/gtelifxgim.html

Ruby: File.size("a.txt")
来源：http://hz.guannengcc.top/gtifirwfdl.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.svipenyu.cn/gtppiqhcqo.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.wangdashe.top/gtxovycfpr.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jlsjyb.cn/gtjqixekgn.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.yuanzhike.top/gtjfrjhbpb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.xingfuxueyuan.xyz/gthcyirtnk.html

TS:   path.extname("a.txt")
来源：http://hz.xuetiantiany.cn/gtigbtldnj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.shanyushiyangtech.top/gttxudedgd.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.chenlongwang.top/gtjfxxpqpr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.hongshengwenyu.top/gtyleqlcwy.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.ivvv.top/gtxpufgpsg.html

[F11] 复制与移动文件
来源：http://hz.haohaochexian.top/gtmqvurjgc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.sufxvd.cn/gtthflicej.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.hywenlv.cn/gttzseogay.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.52xcode.cn/gtafgyvbif.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xinyue.icu/gtuehzkmcm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.guannengcc.top/gtwykcbirc.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.cheryme.top/gtjazegpxk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.yuanzhike.top/gthsxisuli.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.316326.xyz/gtckiezpho.html

[F12] CSV 读写
来源：http://hz.hfpthk.cn/gtjmkjbtnq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.xingfuxueyuan.xyz/gtqyfpfeyx.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.jlsjyb.cn/gtgswbejzk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.cucudq.cn/gtzegzsizt.html

TS:   // 同上
来源：http://hz.zhijiandao.cn/gtelhvkujt.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.yanxiufei.cn/gtkldzddln.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.jinyuanbaomall.cn/gtupmwvnqt.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.9152youxi.cn/gtcnxsqgbp.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.52xcode.cn/gtehwfratq.html

================================================================================
来源：http://hz.zhoulong.xyz/gtxmvajcht.html

G. 面向对象
来源：http://hz.sufxvd.cn/gtbeuynowz.html

================================================================================
来源：http://hz.guannengcc.top/gthurwrzpk.html

[G01] 定义类
来源：http://hz.zhijiandao.cn/gtgeglglhv.html

Py:   class User: pass
来源：http://hz.birdmap.top/gtmmfuamnh.html

PHP:  class User {}
来源：http://hz.daria6918.cn/gtcilortrz.html

JS:   class User {}
来源：http://hz.yanxiufei.cn/gtudnxhtyi.html

TS:   class User { name: string = ""; }
来源：http://hz.wangshuangyany.cn/gtixgzxlqc.html

Java: class User {}
来源：http://hz.feifeiyinyue.top/gtphmwhufk.html

Go:   type User struct { Name string }
来源：http://hz.yanxiufei.cn/gtqvfzwtrd.html

Ruby: class User; end
来源：http://hz.hammf.cn/gtchskjbxv.html

C#:   class User {}
来源：http://hz.yvedp.cn/gtwkdxtmom.html

[G02] 构造函数
来源：http://hz.xinyue.icu/gtvgqrratt.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yanxiufei.cn/gtjuyzpmft.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.jqgufenzy.top/gtdfyhrpdx.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yueranfly.top/gtbpwnlqxm.html

TS:   constructor(public name: string) {}
来源：http://hz.zycfv.cn/gtcqtgvpjy.html

Java: User(String name) { this.name = name; }
来源：http://hz.shuidangran.top/gtyhpfpblj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.andypj.xyz/gtxbqfhkeh.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yvedp.cn/gtqfphhnza.html

C#:   public User(string name) { Name = name; }
来源：http://hz.snrcjt.cn/gtynohjgwr.html

[G03] 实例属性
来源：http://hz.zycfv.cn/gtlesfiukb.html

Py:   self.name = "x"
来源：http://hz.fzhhl.top/gthojgwmvo.html

PHP:  public string $name = "x";
来源：http://hz.cashguo.top/gtzpyzqmps.html

JS:   this.name = "x";
来源：http://hz.gaohongyu789.top/gtpkfbawzi.html

TS:   name: string = "x";
来源：http://hz.zdqjudy.top/gtnkdbyunr.html

Java: private String name;
来源：http://hz.chenjidiqi.icu/gtbpmyydvr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.quarkkingdee.top/gtyvnqcuek.html

Ruby: @name = "x"
来源：http://hz.jqgufenzy.top/gtbbyioxzc.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jyoumei.cn/gtxwdzjmka.html

[G04] 定义方法
来源：http://hz.kuanghao11.cn/gtdhgkqdxr.html

Py:   def greet(self): return self.name
来源：http://hz.jlsjyb.cn/gtpbsicghx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.sysykeji.top/gtloyiphff.html

JS:   greet() { return this.name; }
来源：http://hz.hnxiangtu.top/gtotyjrbxh.html

TS:   greet(): string { return this.name; }
来源：http://hz.hammf.cn/gtscdldkbr.html

Java: String greet() { return name; }
来源：http://hz.yangfankeji.com/gtnwakhxtu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.ywan-chungtsiang.top/gttujwwkjs.html

Ruby: def greet; @name; end
来源：http://hz.yj20258.top/gtudnvfwic.html

C#:   public string Greet() => Name;
来源：http://hz.wangdashe.top/gtjlqmyquc.html

[G05] 继承
来源：http://hz.xingfuxueyuan.xyz/gtoeuolrzo.html

Py:   class Admin(User): pass
来源：http://hz.zhiwuduotai.top/gtdpgschrq.html

PHP:  class Admin extends User {}
来源：http://hz.ydzc1.top/gtozrgycaa.html

JS:   class Admin extends User {}
来源：http://hz.xinyue.icu/gtxoqttvdm.html

TS:   class Admin extends User {}
来源：http://hz.fzhhl.top/gtfgypujff.html

Java: class Admin extends User {}
来源：http://hz.xingfuxueyuan.xyz/gtnznsktcu.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.shanyushiyangtech.top/gtsbwlajtq.html

Ruby: class Admin < User; end
来源：http://hz.yueranfly.top/gtfnugsxku.html

C#:   class Admin : User {}
来源：http://hz.hywenlv.cn/gtmvwlnyld.html

[G06] 重写方法
来源：http://hz.9152youxi.cn/gtfoztnbvp.html

Py:   def greet(self): return "admin"
来源：http://hz.shanyushiyangtech.top/gtpyfcwmjy.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.gogol.net.cn/gtxujbqbnl.html

JS:   greet() { return "admin"; }
来源：http://hz.andypj.xyz/gtpijolcwa.html

TS:   greet(): string { return "admin"; }
来源：http://hz.gzhubu.top/gtkonrsoqs.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jinqigfzy.top/gttcaxkhww.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.hnqzz.top/gtkjonttdk.html

Ruby: def greet; "admin"; end
来源：http://hz.jqgfzy.top/gtbuvenjhp.html

C#:   public override string Greet() => "admin";
来源：http://hz.kuanghao11.cn/gtaeqvrjfe.html

[G07] 调用父类方法
来源：http://hz.xziqi.cn/gtqxqbkfom.html

Py:   super().greet()
来源：http://hz.nwbrower.top/gtcmvnqqja.html

PHP:  parent::greet();
来源：http://hz.zhiwuduotai.top/gtlfwgiwwp.html

JS:   super.greet();
来源：http://hz.zdqjudy.top/gtyuitqahu.html

TS:   super.greet();
来源：http://hz.hnxiangtu.top/gtclxfsqyf.html

Java: super.greet();
来源：http://hz.sysykeji.top/gtpbkdqxsu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.xuanzx.com/gteklpzufd.html

Ruby: super
来源：http://hz.ydjk.org.cn/gtuxfnxmlg.html

C#:   base.Greet();
来源：http://hz.aizwys.cn/gtbnqujnai.html

[G08] 静态方法与属性
来源：http://hz.hysaishi.cn/gtegsvkawx.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.tianlin.xyz/gtivduanka.html

PHP:  public static function f() {}
来源：http://hz.ydjk.org.cn/gtbotxxtte.html

JS:   static f() {}
来源：http://hz.cheryme.top/gtpdwrbnbf.html

TS:   static f(): void {}
来源：http://hz.fzhhl.top/gthwfpqlfs.html

Java: static void f() {}
来源：http://hz.snrcjt.cn/gtyvupkond.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.sxryk.cn/gtynahiivi.html

Ruby: def self.f; end
来源：http://hz.feifeiyinyue.top/gtlhznbaqd.html

C#:   public static void F() {}
来源：http://hz.andypj.xyz/gtjybgnoin.html

[G09] 接口 / 抽象类
来源：http://hz.dianchejie.cn/gtkyrcoouf.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yangfankeji.com/gtsrybvdhb.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.ywan-chungtsiang.top/gtqlyyivhd.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.zhijiandao.cn/gtookuqnlu.html

TS:   interface Shape { area(): number; }
来源：http://hz.jinqigufen.top/gtvfqvhqwv.html

Java: interface Shape { double area(); }
来源：http://hz.chenlongwang.top/gtmyxjvqou.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.cqqwz.cn/gtlphrdhbm.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.cqqwz.cn/gtdlkfrhnz.html

C#:   interface IShape { double Area(); }
来源：http://hz.xuetiantiany.cn/gtkddijxkm.html

[G10] 访问控制
来源：http://hz.tanke756.top/gtwomknecx.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yonumen.top/gthlfnkxtq.html

PHP:  public / protected / private
来源：http://hz.316326.xyz/gtakkinfns.html

JS:   #private 字段；其余公开
来源：http://hz.316326.xyz/gtkekmqfwv.html

TS:   public / protected / private
来源：http://hz.mhx1999.top/gtbkiqjxdm.html

Java: public / protected / private / 默认包级
来源：http://hz.bjfxy.top/gtkqrokscw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.snrcjt.cn/gtjuxgadhi.html

Ruby: public / protected / private
来源：http://hz.shanyushiyangkeji.top/gtffncajya.html


<!-- 参考信息 -->