代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.jinghuilouyu.cn/gtnwkulcbq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.gzhubu.top/gtpoceyrzv.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.hnqzz.top/gtxtnbvtnx.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.gzhubu.top/gtbnocdmnr.html

[E14] URL 编码与 Base64
来源：http://hz.svipenyu.cn/gtlrpcnwhe.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.shanyushiyangtech.top/gtntlpbbfe.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.xziqi.cn/gtnqandiir.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.pengpengdd.cyou/gtsezklkuv.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.gaohongyu789.top/gtkaekvaht.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.havefunace.top/gtbhqggazg.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.xuanzx.com/gtsusewviq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.yj20258.top/gtvoelzaxo.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.meibo888.top/gtdvrckzgp.html

[E15] HTML 转义 / 反转义
来源：http://hz.yuxming.cn/gtxwmbjtyo.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.yongpay.top/gtqnhimjkj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.tian-w.cn/gtdlrvulcb.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.hongshengwenyu.top/gtsaicazcz.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.hnqzz.top/gtgqtszenu.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.feifeiyinyue.top/gtoaftboxd.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.snrcjt.cn/gtgszttnyi.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.jlsjyb.cn/gtdngxsmvp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.c1oappe.top/gtltwsegef.html

[E16] 数字千分位
来源：http://hz.zhiwuduotai.top/gtuyykhcxf.html

Py:   f"{1234567:,}"
来源：http://hz.andypj.xyz/gtgxpokyxj.html

PHP:  number_format(1234567);
来源：http://hz.zycfv.cn/gtmydlbuir.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.hammf.cn/gtnurqedjp.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.nanxinkj.top/gtssgyznea.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.52xcode.cn/gtnvctmhlf.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.gogol.net.cn/gtaoocqums.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.jqgufenzy.top/gtbajwlvbe.html

C#:   1234567.ToString("N0")
来源：http://hz.ehwqpu.com/gtcmnhandq.html

[E17] 首字母大写
来源：http://hz.yj20258888.top/gtpssviuaf.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.cucudq.cn/gtpxymknse.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.feifeiyinyue.top/gthcsxystm.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhengqikj.top/gtptonjilk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.iojbl.cn/gtvvvhjcqn.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.hammf.cn/gttpwqblkt.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.fengsongda.top/gtxomdtxai.html

Ruby: s.capitalize
来源：http://hz.jqgfzy.top/gtqpnsjgem.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.zdqjudy.top/gtleiqlugc.html

[E18] 模板占位符替换
来源：http://hz.gogol.net.cn/gtdrcjlsmy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.fzhhl.top/gtzieypisb.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.chenzaomai.com/gttcjtttna.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.shuidangran.top/gthxapkett.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.sysykeji.top/gtctrrydtq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.yj20258888.top/gtgavldmjr.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.cdnleiting.top/gtksttyyvr.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.jinqigfzy.top/gtstcezlhv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.andypj.xyz/gtmuzfmmaz.html

[E19] 多行文本按行拆分
来源：http://hz.tian-w.cn/gtvogxntas.html

Py:   s.splitlines()
来源：http://hz.hammf.cn/gtrxndvdhf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.sweek.top/gttqlqglag.html

JS:   s.split(/\r?\n/)
来源：http://hz.tian-w.cn/gtrigzhnnm.html

TS:   s.split(/\r?\n/)
来源：http://hz.shuidangran.top/gtpowcppem.html

Java: s.lines().toList()
来源：http://hz.iojbl.cn/gtwgrkussy.html

Go:   strings.Split(s, "\n")
来源：http://hz.snrcjt.cn/gtuuvykign.html

Ruby: s.lines
来源：http://hz.zhongyouzk.top/gturkfcbcl.html

C#:   s.Split('\n')
来源：http://hz.gogol.net.cn/gtplbhagbf.html

[E20] 判断字符串是否为空
来源：http://hz.redwolf501.top/gtmlkipjfj.html

Py:   if not s:
来源：http://hz.chenzaomai.com/gtnbtvbhoq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.sysykeji.top/gtofcxhsgm.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.cqqwz.cn/gtgroiudpq.html

TS:   if (s === "") {}
来源：http://hz.shuidangran.top/gtvexviqyd.html

Java: if (s.isEmpty()) {}
来源：http://hz.cucudq.cn/gtkvggsetx.html

Go:   if s == "" {}
来源：http://hz.zhiwuduotai.top/gtvaimyomn.html

Ruby: if s.empty?
来源：http://hz.52xcode.cn/gtqdbofxwv.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.dashuyun.cn/gtlomisoxm.html

[E21] 超长截断加省略号
来源：http://hz.hysaishi.cn/gtgfuxzbsv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.chenzaomai.com/gtrpwxydjd.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.vqdsnc.cn/gtietcelve.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.fengsongda.top/gtmyhdlfsq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.snrcjt.cn/gtxeaxoppy.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.tian-w.cn/gtvmpicwxt.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.zdqjudy.top/gtlvfoixfk.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.daria6918.cn/gtzltdayfi.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.kuanghao11.cn/gtgessdvms.html

[E22] 字节长度与字符长度
来源：http://hz.meibo888.top/gteonycaqn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.shuidangran.top/gtgkjtjngh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.redwolf501.top/gtiualcwmd.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.cashguo.top/gtahzpwopi.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.nanxinkj.top/gtmsnopupa.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.cashguo.top/gtdlzvcndq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.yj202588.top/gtftizanep.html

Ruby: s.bytesize;  s.length
来源：http://hz.52xcode.cn/gtxfhxvvpm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.shuidangran.top/gtpbtqfqbv.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtvhmwoect.html

F. 文件与目录
来源：http://hz.xingfuxueyuan.xyz/gtxxfvjhqt.html

================================================================================
来源：http://hz.zhixingplan.top/gtfuhoclnf.html

[F01] 读取整个文件
来源：http://hz.cdnleiting.top/gtgfpivwic.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.gotoacloud.top/gttdmtrxzw.html

PHP:  file_get_contents("a.txt");
来源：http://hz.xingfuxueyuan.xyz/gtpapiqqhz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.dashuyun.cn/gtqnrhmxpe.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.sweek.top/gtdbfbhmsi.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.nanxuanxn.top/gtamhtjipi.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zhiwuduotai.top/gtobtlhgtm.html

Ruby: File.read("a.txt")
来源：http://hz.jinqigfzy.top/gtuezeftsl.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.jinqigfzy.top/gtsnwddeip.html

[F02] 逐行读取文件
来源：http://hz.gzhubu.top/gtjqjaqzed.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.zhaomingkeji.xyz/gtmttwyarn.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.jqgfzy.top/gtfsxobrga.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.cqqwz.cn/gtdxwskgbr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yuanzhike.top/gteryqtmap.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.nanxuanxn.top/gtsiqqodfi.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.nwbrower.top/gtzxwcvrrx.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.zhiwuduotai.top/gtpmkecsvv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.yuanzhike.top/gtiimfyfln.html

[F03] 写入文件（覆盖）
来源：http://hz.chenzaomai.com/gtwdkzxwel.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.chenlongwang.top/gtecjbaflw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.yj20258888.top/gtcevvmcwr.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.wangshuangyany.cn/gtkgaseocl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhoulong.xyz/gtfmgcqsab.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.316326.xyz/gtpnwnbsoq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.wangdashe.top/gtkahbqqba.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.haohaochexian.top/gtoptwvevl.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.yanxiufei.cn/gtpncbevik.html

[F04] 追加写入文件
来源：http://hz.nanxinkj.top/gtmgygxafr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.ehwqpu.com/gtbwxvxzvp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.9152youxi.cn/gtxqglyemh.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.mhx1999.top/gtdfgkrzhu.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yj20258.top/gtdqljsomg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.mhx1999.top/gtqepsaaue.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.xylfe.cn/gtxvciciqc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.dashuyun.cn/gtpyhgkmul.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.cqqwz.cn/gtuvgtoabi.html

[F05] 判断文件或目录是否存在
来源：http://hz.cashguo.top/gtebkbeqsa.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.jqgfzy.top/gtrjxqfnoq.html

PHP:  file_exists("a.txt");
来源：http://hz.iojbl.cn/gthawuieqm.html

JS:   fs.existsSync("a.txt")
来源：http://hz.gaohongyu789.top/gtmhthfdel.html

TS:   fs.existsSync("a.txt")
来源：http://hz.meibo888.top/gtwsarayhe.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.jinghuilouyu.cn/gtsfjbelml.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.c1oappe.top/gtugkxepob.html

Ruby: File.exist?("a.txt")
来源：http://hz.zhengqikj.top/gtdevktndy.html

C#:   File.Exists("a.txt")
来源：http://hz.jiagoushi.top/gtnowqvzfz.html

[F06] 删除文件
来源：http://hz.sysykeji.top/gthrfpbiza.html

Py:   os.remove("a.txt")
来源：http://hz.zhaomingkeji.xyz/gtbraphtat.html

PHP:  unlink("a.txt");
来源：http://hz.9152youxi.cn/gtmapfonfm.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.cashguo.top/gtwrbardek.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.nanxuanxn.top/gtfaytpcap.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.gaohongyu789.top/gtjtjlmusw.html

Go:   os.Remove("a.txt")
来源：http://hz.jlsjyb.cn/gtfkuqdkrj.html

Ruby: File.delete("a.txt")
来源：http://hz.chenlongwang.top/gtmbjqavob.html

C#:   File.Delete("a.txt");
来源：http://hz.ppjwa.cn/gthlsozxlc.html

[F07] 创建目录（含多级）
来源：http://hz.yuxming.cn/gtvymatojk.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.zhijiandao.cn/gtntyggzqx.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.chenjidiqi.icu/gtkmmrgnfs.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jlsjyb.cn/gtmuuqegzt.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yanxiufei.cn/gtntxevhhf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.yongpay.top/gtlxaqldcy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.tianlin.xyz/gtotvqmzjq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.pycfn.com/gtdgghvwjq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.snrcjt.cn/gtrbogjnog.html

[F08] 遍历目录
来源：http://hz.svipenyu.cn/gtngovkcmj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.aizwys.cn/gtripozuhy.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.svipenyu.cn/gtxiymxetu.html

JS:   fs.readdirSync("dir")
来源：http://hz.iojbl.cn/gtkcjtnyci.html

TS:   fs.readdirSync("dir")
来源：http://hz.pengpengdd.cyou/gtyzvkmscm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.xingfuxueyuan.xyz/gtipcthocs.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yj20258888.top/gtolvqabzt.html

Ruby: Dir.children("dir")
来源：http://hz.yuxming.cn/gtlyjewnud.html

C#:   Directory.GetFiles("dir")
来源：http://hz.svipenyu.cn/gtdwolqdlt.html

[F09] 获取文件大小
来源：http://hz.fzhhl.top/gtdnzvgkgs.html

Py:   os.path.getsize("a.txt")
来源：http://hz.meibo888.top/gtxtktpxgb.html

PHP:  filesize("a.txt");
来源：http://hz.yj20258888.top/gtiipwapvb.html

JS:   fs.statSync("a.txt").size
来源：http://hz.feifeiyinyue.top/gteosvsuwb.html

TS:   fs.statSync("a.txt").size
来源：http://hz.tianlin.xyz/gtkfkedtxy.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.shuidangran.top/gtxbdipmuw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.sxryk.cn/gtvlvtrxrk.html

Ruby: File.size("a.txt")
来源：http://hz.shuidangran.top/gtmxzhgcco.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.hongshengwenyu.top/gtckxwkfwx.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.haohaochexian.top/gtyxnmhnwt.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.xuetiantiany.cn/gtuobeeuyz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.shangyingyoupin.top/gtdtcjxbxh.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.nwbrower.top/gtthsghroe.html

TS:   path.extname("a.txt")
来源：http://hz.xylfe.cn/gtbfmzbjrg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.zhoulong.xyz/gtpuijrjjj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.birdmap.top/gtzshdyojk.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.cucudq.cn/gtyythiafe.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.daria6918.cn/gtmnbtoyxd.html

[F11] 复制与移动文件
来源：http://hz.gzhubu.top/gtwnzxlfcv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.quarkkingdee.top/gtrkgsqdpt.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.pengpengdd.cyou/gtdlhynhlu.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xinyue.icu/gtskldevrh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.fzhhl.top/gtcavrcice.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.xuetiantiany.cn/gtgwpfuxtg.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.redwolf501.top/gttsiohnpd.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.shzxlz.cn/gtilmblyds.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.chenzaomai.com/gtxkzslgnr.html

[F12] CSV 读写
来源：http://hz.zhongyouzk.top/gtfabjqbhk.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.haohaochexian.top/gtrxtkzmkm.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.yuanzhike.top/gtiuufompm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.gaohongyu789.top/gtkvvirlxz.html

TS:   // 同上
来源：http://hz.zhengqikj.top/gttlijuuod.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.yonumen.top/gtgdurztmu.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.gotoacloud.top/gtcdsjwoyl.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.gogol.net.cn/gtfjswdiyb.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yj20258888.top/gtqwddqmcv.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtnhczvqrc.html

G. 面向对象
来源：http://hz.ppjwa.cn/gtoykmanbi.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtgmgizjxr.html

[G01] 定义类
来源：http://hz.hysaishi.cn/gtigsqguzz.html

Py:   class User: pass
来源：http://hz.zhoulong.xyz/gtdsqinouk.html

PHP:  class User {}
来源：http://hz.jlsjyb.cn/gtsiuvgzyv.html

JS:   class User {}
来源：http://hz.ppjwa.cn/gtpynfmntq.html

TS:   class User { name: string = ""; }
来源：http://hz.316326.xyz/gtvczynehs.html

Java: class User {}
来源：http://hz.zhengqikj.top/gttunbpkfm.html

Go:   type User struct { Name string }
来源：http://hz.sweek.top/gtqfwxoxxz.html

Ruby: class User; end
来源：http://hz.hammf.cn/gtyqrvssev.html

C#:   class User {}
来源：http://hz.pengpengdd.cyou/gtzptptnav.html

[G02] 构造函数
来源：http://hz.wangdashe.top/gthqfxdqyf.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.vqdsnc.cn/gtvxmcchnn.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.jlsjyb.cn/gtcowgdwdo.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.smart0.xyz/gtmmhbbflq.html

TS:   constructor(public name: string) {}
来源：http://hz.jinyuanbaomall.cn/gtkizfhixx.html

Java: User(String name) { this.name = name; }
来源：http://hz.gotoacloud.top/gttvxzzxqw.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.hysaishi.cn/gtkeitomga.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.jqgufenzy.top/gtfcphtuwn.html

C#:   public User(string name) { Name = name; }
来源：http://hz.hysaishi.cn/gtipvcheev.html

[G03] 实例属性
来源：http://hz.xziqi.cn/gtyqlcidfs.html

Py:   self.name = "x"
来源：http://hz.gaohongyu789.top/gttfjdgtou.html

PHP:  public string $name = "x";
来源：http://hz.kuanghao11.cn/gtgkihrswx.html

JS:   this.name = "x";
来源：http://hz.smart0.xyz/gtlyvzbavg.html

TS:   name: string = "x";
来源：http://hz.haohaochexian.top/gtbfjgvsfl.html

Java: private String name;
来源：http://hz.shangyingyoupin.top/gtlfufohap.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.c1oappe.top/gtolawpmfh.html

Ruby: @name = "x"
来源：http://hz.chenjidiqi.icu/gtpbbxsbmn.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.bjfxy.top/gtjixotkhx.html

[G04] 定义方法
来源：http://hz.ybcxt.top/gtxjjaiqzi.html

Py:   def greet(self): return self.name
来源：http://hz.aibaodan.cn/gtsarffzzz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.52xcode.cn/gtjmtvvzcd.html

JS:   greet() { return this.name; }
来源：http://hz.havefunace.top/gtbriehtrr.html

TS:   greet(): string { return this.name; }
来源：http://hz.ehwqpu.com/gtbhziogbb.html

Java: String greet() { return name; }
来源：http://hz.jqgufenzy.top/gtejauwwtn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.guowangkeji.top/gtzxkiuhwq.html

Ruby: def greet; @name; end
来源：http://hz.jinyuanbaomall.cn/gtdvmeepmh.html

C#:   public string Greet() => Name;
来源：http://hz.yueranfly.top/gtfdlpjhav.html

[G05] 继承
来源：http://hz.jinghuilouyu.cn/gtgglukuvi.html

Py:   class Admin(User): pass
来源：http://hz.daxiang520.top/gtbejcmuci.html

PHP:  class Admin extends User {}
来源：http://hz.yangfankeji.com/gtlfpyoznk.html

JS:   class Admin extends User {}
来源：http://hz.zhaomingkeji.xyz/gtijkjyszd.html

TS:   class Admin extends User {}
来源：http://hz.svipenyu.cn/gtnpcivhao.html

Java: class Admin extends User {}
来源：http://hz.yj20258.top/gterhpcaxi.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.guowangkeji.top/gtyngswapl.html

Ruby: class Admin < User; end
来源：http://hz.guowangkeji.top/gthowuhgwg.html

C#:   class Admin : User {}
来源：http://hz.fzhhl.top/gtspistsmh.html

[G06] 重写方法
来源：http://hz.birdmap.top/gtgywiyzuh.html

Py:   def greet(self): return "admin"
来源：http://hz.yueranfly.top/gtxqaegzgg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jyoumei.cn/gtzmtiekol.html

JS:   greet() { return "admin"; }
来源：http://hz.xinyue.icu/gtcuxrkmes.html

TS:   greet(): string { return "admin"; }
来源：http://hz.yj202588.top/gtdcquhshn.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.sufxvd.cn/gtnwqkuwbv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.yvedp.cn/gtsfoqrggs.html

Ruby: def greet; "admin"; end
来源：http://hz.zhoulong.xyz/gtxesnqzkh.html

C#:   public override string Greet() => "admin";
来源：http://hz.quarkkingdee.top/gtonmzmzec.html

[G07] 调用父类方法
来源：http://hz.jinqigufen.top/gtdnvoptha.html

Py:   super().greet()
来源：http://hz.tian-w.cn/gtctypjbyr.html

PHP:  parent::greet();
来源：http://hz.redwolf501.top/gtkgvdslof.html

JS:   super.greet();
来源：http://hz.jiagoushi.top/gtbuezpadi.html

TS:   super.greet();
来源：http://hz.daxiang520.top/gttcmmvepq.html

Java: super.greet();
来源：http://hz.yvedp.cn/gtscszohhd.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.316326.xyz/gtxbubqgvi.html

Ruby: super
来源：http://hz.birdmap.top/gtppzhgned.html

C#:   base.Greet();
来源：http://hz.sufxvd.cn/gtfzkdsjpd.html

[G08] 静态方法与属性
来源：http://hz.birdmap.top/gtxklellua.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.smart0.xyz/gtxlasfcwr.html

PHP:  public static function f() {}
来源：http://hz.jinqigfzy.top/gtsyzwylxc.html

JS:   static f() {}
来源：http://hz.yanxiufei.cn/gtlswfwkfl.html

TS:   static f(): void {}
来源：http://hz.dianchejie.cn/gtgllkvimv.html

Java: static void f() {}
来源：http://hz.shanyushiyangtech.top/gtyjatycin.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yueranfly.top/gtpdqtsfgy.html

Ruby: def self.f; end
来源：http://hz.shangyingyoupin.top/gtyecawasl.html

C#:   public static void F() {}
来源：http://hz.wangshuangyany.cn/gtcmsllonb.html

[G09] 接口 / 抽象类
来源：http://hz.shuidangran.top/gteywmbjvv.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.ywan-chungtsiang.top/gtdsapiwri.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.chenzaomai.com/gteschiftr.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.andypj.xyz/gtcrfppdrj.html

TS:   interface Shape { area(): number; }
来源：http://hz.jinqigufen.top/gtylcyqbid.html

Java: interface Shape { double area(); }
来源：http://hz.cucudq.cn/gtmnplpjhk.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yangfankeji.com/gteloafxdb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yuanzhike.top/gtsmnczwti.html

C#:   interface IShape { double Area(); }
来源：http://hz.gotoacloud.top/gtbtosaopj.html

[G10] 访问控制
来源：http://hz.yuxming.cn/gtrquvlpas.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.sxryk.cn/gtxbgbgqas.html

PHP:  public / protected / private
来源：http://hz.ybcxt.top/gthmpoitij.html

JS:   #private 字段；其余公开
来源：http://hz.yvedp.cn/gttpfgjznl.html

TS:   public / protected / private
来源：http://hz.hysaishi.cn/gtzspkpmew.html

Java: public / protected / private / 默认包级
来源：http://hz.snrcjt.cn/gtajyybbal.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.xuetiantiany.cn/gtdkwunokq.html

Ruby: public / protected / private
来源：http://hz.jyoumei.cn/gtiaezkedf.html

C#:   public / protected / private / internal
来源：http://hz.vqdsnc.cn/gtextnjkhr.html

[G11] getter / setter
来源：http://hz.c1oappe.top/gtsvrbzipk.html

Py:   @property 与 @x.setter
来源：http://hz.pycfn.com/gtwjkeberr.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.wangshuangyany.cn/gtlwdynvsp.html

JS:   get name() { return this._name; }
来源：http://hz.jianghu66.top/gtgtvravaj.html

TS:   get name(): string { return this._name; }
来源：http://hz.tianlin.xyz/gtzkwybfyu.html

Java: public String getName() { return name; }
来源：http://hz.zhoulong.xyz/gtafswqjqc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.tian-w.cn/gteypdgvcz.html

Ruby: attr_accessor :name
来源：http://hz.yuxming.cn/gtpgrqfoez.html

C#:   public string Name { get; set; }
来源：http://hz.hnxiangtu.top/gthczchxze.html

[G12] 对象转字符串
来源：http://hz.yj20258888.top/gtuwmvknjv.html

Py:   def __str__(self): return self.name
来源：http://hz.nwbrower.top/gtwzmbcwvo.html


<!-- 参考信息 -->