代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.cdnleiting.top/gtdcvlcdow.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.gotoacloud.top/gtelnjvyou.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.yj202588.top/gtfyjhtnpg.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.jinqigufen.top/gtbebzagtw.html

[E14] URL 编码与 Base64
来源：http://hz.zhongyouzk.top/gttjelqdxx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.tianlin.xyz/gtnlarrsrz.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.c1oappe.top/gtcoeeachg.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.hongshengwenyu.top/gtkimemhmz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.zhengqikj.top/gtnolmkliu.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.aizwys.cn/gtkamejjtw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.shzxlz.cn/gtbchecruj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.ydjk.org.cn/gteqqcxpdy.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.hongshengwenyu.top/gtvwwosjel.html

[E15] HTML 转义 / 反转义
来源：http://hz.hammf.cn/gtjpccmxpf.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.shangyingyoupin.top/gtnijosuzh.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.chenzaomai.com/gtdvaraaqe.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.xylfe.cn/gtjmwqamye.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.zhoulong.xyz/gtrshunsns.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.cqqwz.cn/gtcsjefvut.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.ivvv.top/gtkidfblxh.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.jqgufenzy.top/gtnkhdltlk.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.shanyushiyangkeji.top/gtqvvespjn.html

[E16] 数字千分位
来源：http://hz.shzxlz.cn/gtxpnnxsim.html

Py:   f"{1234567:,}"
来源：http://hz.jqgufenzy.top/gtenekkfjw.html

PHP:  number_format(1234567);
来源：http://hz.aibaodan.cn/gtgfijjqll.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.cqqwz.cn/gtpcjfjmwi.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.yvedp.cn/gtqtvbgebf.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.sxryk.cn/gtrohxymsz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.yueranfly.top/gtuiwjgyiy.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.chenlongwang.top/gtnakjlron.html

C#:   1234567.ToString("N0")
来源：http://hz.yonumen.top/gtejozyrit.html

[E17] 首字母大写
来源：http://hz.fengsongda.top/gtcrvlemfl.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.hongshengwenyu.top/gtmnwubpfk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.xylfe.cn/gthutlrzxy.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yj20258.top/gtsautfbqv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.52xcode.cn/gtwysqquxx.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.zhiwuduotai.top/gtdkcupreu.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.bjfxy.top/gtdlggukzo.html

Ruby: s.capitalize
来源：http://hz.sysykeji.top/gtoyrwfhko.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.ivvv.top/gtprmaogmt.html

[E18] 模板占位符替换
来源：http://hz.zhengqikj.top/gtxxjdnfrl.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.zycfv.cn/gteqztcnwr.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.yj20258888.top/gtmrpjtgyw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.xingfuxueyuan.xyz/gtfrbcmryz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.0kj1m.cn/gtdiusdjim.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.jinqigfzy.top/gtrhoebklp.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.chenzaomai.com/gtkqbvmkkq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.jqgfzy.top/gttfiwagta.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.svipenyu.cn/gtagfeythz.html

[E19] 多行文本按行拆分
来源：http://hz.cqqwz.cn/gtskpxvbie.html

Py:   s.splitlines()
来源：http://hz.zdqjudy.top/gtqlxwjman.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.zhoulong.xyz/gtpdobbqna.html

JS:   s.split(/\r?\n/)
来源：http://hz.shangyingyoupin.top/gtsesqmpbc.html

TS:   s.split(/\r?\n/)
来源：http://hz.wangshuangyany.cn/gtlhxwzgys.html

Java: s.lines().toList()
来源：http://hz.zhixingplan.top/gthidhchsy.html

Go:   strings.Split(s, "\n")
来源：http://hz.tanke756.top/gtowrgepay.html

Ruby: s.lines
来源：http://hz.sxryk.cn/gtgluzuccb.html

C#:   s.Split('\n')
来源：http://hz.nanxinkj.top/gtwhxthvbz.html

[E20] 判断字符串是否为空
来源：http://hz.ydjk.org.cn/gtkrvjbixs.html

Py:   if not s:
来源：http://hz.zhaomingkeji.xyz/gttsasvpef.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.xylfe.cn/gtyjuyxtfx.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.jqgufenzy.top/gtohidsphx.html

TS:   if (s === "") {}
来源：http://hz.yj202588.top/gtxkmtvqzv.html

Java: if (s.isEmpty()) {}
来源：http://hz.ehwqpu.com/gturdwfcaq.html

Go:   if s == "" {}
来源：http://hz.svipenyu.cn/gtaodwgujw.html

Ruby: if s.empty?
来源：http://hz.ehwqpu.com/gtbkfjmmey.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.haohaochexian.top/gtgcvxzwhg.html

[E21] 超长截断加省略号
来源：http://hz.ppjwa.cn/gtjqfvyxgz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.yonumen.top/gtubtctexk.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.yj20258888.top/gtjiypclwj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhongyouzk.top/gtgkjqxmvk.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.mhx1999.top/gtwiljfetr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.jqgufenzy.top/gtqgcrnnav.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.xylfe.cn/gtgevtderw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.svipenyu.cn/gtcwirvrvb.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.gogol.net.cn/gtpoazzamh.html

[E22] 字节长度与字符长度
来源：http://hz.sysykeji.top/gtswxwtbsd.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.cucudq.cn/gtfsmieuce.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zycfv.cn/gtykcmjgzl.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yangfankeji.com/gtbrlfeqgy.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jqgufenzy.top/gtxvledshx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.zhixingplan.top/gtiuojczaw.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.hysaishi.cn/gtjvvducra.html

Ruby: s.bytesize;  s.length
来源：http://hz.jyoumei.cn/gtvyancjgg.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.cheryme.top/gtzjuvyhpa.html

================================================================================
来源：http://hz.gaohongyu789.top/gtmrpenpyo.html

F. 文件与目录
来源：http://hz.52xcode.cn/gtnfgfjcyo.html

================================================================================
来源：http://hz.daria6918.cn/gtqulcbbrm.html

[F01] 读取整个文件
来源：http://hz.xylfe.cn/gtvpmlsgeb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.zdqjudy.top/gtclienocr.html

PHP:  file_get_contents("a.txt");
来源：http://hz.0kj1m.cn/gtielaujxj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.gotoacloud.top/gtjvipxofo.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.gaohongyu789.top/gtruvfxuvt.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.daria6918.cn/gtcjzhalst.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.yangfankeji.com/gtblvijrkt.html

Ruby: File.read("a.txt")
来源：http://hz.andypj.xyz/gtzjnchjos.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.shzxlz.cn/gtlrtwkfau.html

[F02] 逐行读取文件
来源：http://hz.yj20258.top/gtuyuzukwu.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.52xcode.cn/gtvbiomgbm.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.chenzaomai.com/gtxdtgqpfz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhixingplan.top/gtrmogqexc.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yuanzhike.top/gttfozxbtm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.gotoacloud.top/gtrpyzashy.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.jinyuanbaomall.cn/gtlcgncviu.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.jiagoushi.top/gtywymoezl.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.ehwqpu.com/gtqsbyemqt.html

[F03] 写入文件（覆盖）
来源：http://hz.hysaishi.cn/gtzehpwayp.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.wangshuangyany.cn/gtikpizsgc.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.cucudq.cn/gtzssafqfc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jyoumei.cn/gtpljrrjre.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.cdnleiting.top/gtfsahekhy.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.0kj1m.cn/gtfigcaxfb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.zhoulong.xyz/gtkfwztzbi.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.nwbrower.top/gtdgtjzfit.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.wangdashe.top/gtombjkxun.html

[F04] 追加写入文件
来源：http://hz.gaohongyu789.top/gtcbjpbqxz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.gaohongyu789.top/gtvcjogrxm.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.mhx1999.top/gtgkmtxxyq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.9152youxi.cn/gtanckfgxu.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jinghuilouyu.cn/gtblhxwqug.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.ydzc1.top/gtiayktyma.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.sysykeji.top/gtnkfmeboo.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yuanzhike.top/gtwrybxvfy.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.cdnleiting.top/gtojrwnnxj.html

[F05] 判断文件或目录是否存在
来源：http://hz.chenjidiqi.icu/gtkvongpic.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.zhongyouzk.top/gtmgiwkyxz.html

PHP:  file_exists("a.txt");
来源：http://hz.jinyuanbaomall.cn/gtpmtzsrph.html

JS:   fs.existsSync("a.txt")
来源：http://hz.fzhhl.top/gtmcaqffbi.html

TS:   fs.existsSync("a.txt")
来源：http://hz.nwbrower.top/gtfkdsmtbx.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.ydzc1.top/gtrjdpwcux.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.shanyushiyangkeji.top/gtmubmymif.html

Ruby: File.exist?("a.txt")
来源：http://hz.9152youxi.cn/gtfrfmfgub.html

C#:   File.Exists("a.txt")
来源：http://hz.feifeiyinyue.top/gtqofyzvoh.html

[F06] 删除文件
来源：http://hz.shangyingyoupin.top/gtjsheswpp.html

Py:   os.remove("a.txt")
来源：http://hz.316326.xyz/gtnuavsevs.html

PHP:  unlink("a.txt");
来源：http://hz.0kj1m.cn/gtarxlhexc.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.jiagoushi.top/gtvwobknnz.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.nanxinkj.top/gtmsfhldsa.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.hnqzz.top/gtuvtowxrg.html

Go:   os.Remove("a.txt")
来源：http://hz.xinyue.icu/gtnftubtis.html

Ruby: File.delete("a.txt")
来源：http://hz.sufxvd.cn/gtzewbpsso.html

C#:   File.Delete("a.txt");
来源：http://hz.quarkkingdee.top/gtakpgqhvd.html

[F07] 创建目录（含多级）
来源：http://hz.hongshengwenyu.top/gttkcszces.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.shanyushiyangtech.top/gtutdllhfy.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.xziqi.cn/gtfpdpczgq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yj20258888.top/gtldpxsbjb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yuanzhike.top/gtgbuasukk.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.cheryme.top/gtplynjpdc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jlsjyb.cn/gtzjnsqoiy.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.shzxlz.cn/gtajbyvhkb.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.vqdsnc.cn/gtrlzreqod.html

[F08] 遍历目录
来源：http://hz.tianlin.xyz/gtqnlbrwbz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yj20258.top/gtvpygzowo.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.zhengqikj.top/gtokscgdgd.html

JS:   fs.readdirSync("dir")
来源：http://hz.chenjidiqi.icu/gtygqdlffg.html

TS:   fs.readdirSync("dir")
来源：http://hz.quarkkingdee.top/gtxuutgtbt.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.dianchejie.cn/gttfnytsuv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.wangdashe.top/gtjgxcaqje.html

Ruby: Dir.children("dir")
来源：http://hz.52xcode.cn/gthliruyrd.html

C#:   Directory.GetFiles("dir")
来源：http://hz.jlsjyb.cn/gtngzaawip.html

[F09] 获取文件大小
来源：http://hz.gaohongyu789.top/gtlybumiro.html

Py:   os.path.getsize("a.txt")
来源：http://hz.yangfankeji.com/gtfvvgactg.html

PHP:  filesize("a.txt");
来源：http://hz.jqgufenzy.top/gtfrnjtxto.html

JS:   fs.statSync("a.txt").size
来源：http://hz.ydzc1.top/gthzvhirxs.html

TS:   fs.statSync("a.txt").size
来源：http://hz.hammf.cn/gtgahrecsv.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.shangyingyoupin.top/gtbpyicaxa.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.guannengcc.top/gtgshcqbrn.html

Ruby: File.size("a.txt")
来源：http://hz.tian-w.cn/gtknbtxuiu.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.guowangkeji.top/gtydvzrpjv.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.quarkkingdee.top/gttmsugasm.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.kuanghao11.cn/gtjdqebtle.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.zhiwuduotai.top/gteichjjsc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.chenlongwang.top/gtrvellvsx.html

TS:   path.extname("a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtfzhqdpmd.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.zhijiandao.cn/gtokwrwgda.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.snrcjt.cn/gtgmdwcxkn.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.pycfn.com/gtlfzsxsii.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.bjfxy.top/gtlnxdfzlo.html

[F11] 复制与移动文件
来源：http://hz.zhiwuduotai.top/gtakjszqcn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.yongpay.top/gtsrcqsobz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.cdnleiting.top/gtycwhoarg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ydzc1.top/gtrcoabwwy.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.chenlongwang.top/gtbxbzpcdu.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.hysaishi.cn/gtmbhdyhjw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.haohaochexian.top/gtpxobjodr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.tian-w.cn/gtdgbxhbmj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.ybcxt.top/gtuyejazjm.html

[F12] CSV 读写
来源：http://hz.zhixingplan.top/gtipynblxo.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.hammf.cn/gtobgdniew.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.fzhhl.top/gtgefkhtpr.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.sxryk.cn/gthfpilfdb.html

TS:   // 同上
来源：http://hz.daria6918.cn/gtmkldejsb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.dianchejie.cn/gtekqqgvvi.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.bjfxy.top/gtgtciemrj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.c1oappe.top/gtdgwxbhiy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jinghuilouyu.cn/gttymnilxn.html

================================================================================
来源：http://hz.sxryk.cn/gtatvmmkgr.html

G. 面向对象
来源：http://hz.xinyue.icu/gtrlbnwlix.html

================================================================================
来源：http://hz.bjfxy.top/gtzzwiigls.html

[G01] 定义类
来源：http://hz.jinghuilouyu.cn/gtnreugikn.html

Py:   class User: pass
来源：http://hz.zdqjudy.top/gtxcnscjxr.html

PHP:  class User {}
来源：http://hz.wangdashe.top/gtyyoykxpj.html

JS:   class User {}
来源：http://hz.yj20258888.top/gtccrqopgk.html

TS:   class User { name: string = ""; }
来源：http://hz.cashguo.top/gtpokrgxkc.html

Java: class User {}
来源：http://hz.ehwqpu.com/gtbttkkvzi.html

Go:   type User struct { Name string }
来源：http://hz.kuanghao11.cn/gtznogfofp.html

Ruby: class User; end
来源：http://hz.shzxlz.cn/gtokajskbm.html

C#:   class User {}
来源：http://hz.tianlin.xyz/gtuesgpqlp.html

[G02] 构造函数
来源：http://hz.ehwqpu.com/gtnpgwhubx.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zhongyouzk.top/gtyivkvwfy.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.shzxlz.cn/gtxuflwmdx.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.zhaomingkeji.xyz/gtinabsuey.html

TS:   constructor(public name: string) {}
来源：http://hz.jinqigufen.top/gthyvqtrvm.html

Java: User(String name) { this.name = name; }
来源：http://hz.jinghuilouyu.cn/gtjwemvhsi.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.zhaomingkeji.xyz/gtrixpsaqn.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.sxryk.cn/gtryilstir.html

C#:   public User(string name) { Name = name; }
来源：http://hz.havefunace.top/gtxemvmnhv.html

[G03] 实例属性
来源：http://hz.redwolf501.top/gttufhhemg.html

Py:   self.name = "x"
来源：http://hz.chenzaomai.com/gtelwizuna.html

PHP:  public string $name = "x";
来源：http://hz.bjfxy.top/gtdeblvjyb.html

JS:   this.name = "x";
来源：http://hz.wangshuangyany.cn/gtdmvmaihr.html

TS:   name: string = "x";
来源：http://hz.guowangkeji.top/gtrjwlucxn.html

Java: private String name;
来源：http://hz.hfpthk.cn/gtgftvxqkd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.daxiang520.top/gtmojvlrcs.html

Ruby: @name = "x"
来源：http://hz.hywenlv.cn/gtkdvbptwh.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.dianchejie.cn/gtmfhwtjfe.html

[G04] 定义方法
来源：http://hz.xuetiantiany.cn/gtaxtvmzqf.html

Py:   def greet(self): return self.name
来源：http://hz.zhongyouzk.top/gtjtvsymyq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.xinyue.icu/gtxrmhutqo.html

JS:   greet() { return this.name; }
来源：http://hz.nanxinkj.top/gtifexzkpy.html

TS:   greet(): string { return this.name; }
来源：http://hz.shangyingyoupin.top/gtgrdwfdro.html

Java: String greet() { return name; }
来源：http://hz.jiagoushi.top/gtywbedvxc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.tian-w.cn/gtxtvxhizx.html

Ruby: def greet; @name; end
来源：http://hz.0kj1m.cn/gtqaqbwclq.html

C#:   public string Greet() => Name;
来源：http://hz.chenjidiqi.icu/gtsrqgasvn.html

[G05] 继承
来源：http://hz.hongshengwenyu.top/gtxrihatqn.html

Py:   class Admin(User): pass
来源：http://hz.cqqwz.cn/gtfxznexzh.html

PHP:  class Admin extends User {}
来源：http://hz.tianlin.xyz/gtetynqvfy.html

JS:   class Admin extends User {}
来源：http://hz.zhixingplan.top/gthvauzrna.html

TS:   class Admin extends User {}
来源：http://hz.gzhubu.top/gtfkzftyur.html

Java: class Admin extends User {}
来源：http://hz.xylfe.cn/gtzfvxwfir.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.zhoulong.xyz/gtqmisiirn.html

Ruby: class Admin < User; end
来源：http://hz.xinyue.icu/gtkisuwvxk.html

C#:   class Admin : User {}
来源：http://hz.xuetiantiany.cn/gtpoaodppz.html

[G06] 重写方法
来源：http://hz.zhongyouzk.top/gtghtpoxog.html

Py:   def greet(self): return "admin"
来源：http://hz.xuetiantiany.cn/gtumonlysu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.zdqjudy.top/gtdxhcgivq.html

JS:   greet() { return "admin"; }
来源：http://hz.shangyingyoupin.top/gtcnaxoqng.html

TS:   greet(): string { return "admin"; }
来源：http://hz.shanyushiyangkeji.top/gtcplqysfc.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.feifeiyinyue.top/gtxklnmwcy.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.xuanzx.com/gtehdkdsef.html

Ruby: def greet; "admin"; end
来源：http://hz.yj20258.top/gtqherqhlz.html

C#:   public override string Greet() => "admin";
来源：http://hz.daria6918.cn/gtyjhvomlc.html

[G07] 调用父类方法
来源：http://hz.xuanzx.com/gtnjlsjzfp.html

Py:   super().greet()
来源：http://hz.jiagoushi.top/gtfssuepnf.html

PHP:  parent::greet();
来源：http://hz.ydzc1.top/gtqfcqnwph.html

JS:   super.greet();
来源：http://hz.xylfe.cn/gtvrnqnuim.html

TS:   super.greet();
来源：http://hz.yj20258.top/gtbwpaswrj.html

Java: super.greet();
来源：http://hz.andypj.xyz/gtrjkexdmc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.quarkkingdee.top/gtafzulsbl.html

Ruby: super
来源：http://hz.vqdsnc.cn/gtkgiagtsk.html

C#:   base.Greet();
来源：http://hz.dashuyun.cn/gtorudtgld.html

[G08] 静态方法与属性
来源：http://hz.sufxvd.cn/gthmzhdoap.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.52xcode.cn/gtculyenkm.html

PHP:  public static function f() {}
来源：http://hz.hammf.cn/gtdxevhgae.html

JS:   static f() {}
来源：http://hz.hnxiangtu.top/gtkqmdvfql.html

TS:   static f(): void {}
来源：http://hz.ydjk.org.cn/gtglourmjk.html

Java: static void f() {}
来源：http://hz.sweek.top/gtdhbfrnmp.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.zhixingplan.top/gtajdraiqs.html

Ruby: def self.f; end
来源：http://hz.fengsongda.top/gtorjvhfzc.html

C#:   public static void F() {}
来源：http://hz.xingfuxueyuan.xyz/gtquxtrkop.html

[G09] 接口 / 抽象类
来源：http://hz.yuxming.cn/gtrxpsrtxq.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.xziqi.cn/gtwmpmnhqy.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jlsjyb.cn/gtjdbzigwe.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.haohaochexian.top/gtppnuitcb.html

TS:   interface Shape { area(): number; }
来源：http://hz.jinqigufen.top/gtkcokcrih.html

Java: interface Shape { double area(); }
来源：http://hz.wangshuangyany.cn/gtpewuqdqz.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.zhoulong.xyz/gtxehvycug.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.c1oappe.top/gtkqsbrpqd.html

C#:   interface IShape { double Area(); }
来源：http://hz.gzhubu.top/gtbjaovfth.html

[G10] 访问控制
来源：http://hz.zhiwuduotai.top/gtaqjtolnf.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.iojbl.cn/gtwzutlisv.html

PHP:  public / protected / private
来源：http://hz.jianghu66.top/gtfnikclrz.html

JS:   #private 字段；其余公开
来源：http://hz.xingfuxueyuan.xyz/gtgutktxcw.html

TS:   public / protected / private
来源：http://hz.zhengqikj.top/gtccfdmhwg.html

Java: public / protected / private / 默认包级
来源：http://hz.zhijiandao.cn/gtonznqkyo.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.shuidangran.top/gtmgbcypds.html

Ruby: public / protected / private
来源：http://hz.chenzaomai.com/gtlzyoeaof.html

C#:   public / protected / private / internal
来源：http://hz.52xcode.cn/gtiuoperoo.html

[G11] getter / setter
来源：http://hz.xinyue.icu/gtejeibysp.html

Py:   @property 与 @x.setter
来源：http://hz.yj202588.top/gtcqpgbaey.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.shuidangran.top/gteurbqqxh.html

JS:   get name() { return this._name; }
来源：http://hz.xuanzx.com/gtgogdxqyn.html

TS:   get name(): string { return this._name; }
来源：http://hz.jinyuanbaomall.cn/gtagtfhfup.html

Java: public String getName() { return name; }
来源：http://hz.zhengqikj.top/gtvmmfhexe.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.xinyue.icu/gtixyvjkip.html

Ruby: attr_accessor :name
来源：http://hz.fzhhl.top/gtytjwuddk.html

C#:   public string Name { get; set; }
来源：http://hz.daxiang520.top/gtxtpoekhl.html

[G12] 对象转字符串
来源：http://hz.hysaishi.cn/gtlucrijyk.html

Py:   def __str__(self): return self.name
来源：http://hz.haohaochexian.top/gtefvhrjxv.html


<!-- 参考信息 -->