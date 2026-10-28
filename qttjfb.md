代发 wailian999

Py:   for ch in s: print(ch)
来源：http://hz.zhoulong.xyz/gtotelqcfz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.andypj.xyz/gticuyabvl.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.havefunace.top/gthulurlwm.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.pycfn.com/gtxxclytgy.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.daria6918.cn/gtjpnyodjt.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.hammf.cn/gtcmkqrvyp.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.kuanghao11.cn/gtchhuecar.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.daria6918.cn/gtxkiqhxjn.html

[E14] URL 编码与 Base64
来源：http://hz.yj20258.top/gtiiwcwiyh.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.zhengqikj.top/gtpnhaamcg.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.hnqzz.top/gtkpmbsifl.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.cdnleiting.top/gtjamtsgqi.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.birdmap.top/gtksgyvqce.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.52xcode.cn/gtpcuqlnxh.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.yangfankeji.com/gtrndnnuxd.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.xingfuxueyuan.xyz/gtngskvhdi.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.xuanzx.com/gtrgjttryf.html

[E15] HTML 转义 / 反转义
来源：http://hz.nwbrower.top/gthddohlks.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.nanxuanxn.top/gtrawbtois.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.bjfxy.top/gtcxvkkisw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.c1oappe.top/gtmdknnvnw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.hywenlv.cn/gtjtzaxswj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.shzxlz.cn/gtjekfnhtb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.c1oappe.top/gtvnrcvssq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.tian-w.cn/gtrlwyhmnq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.wangshuangyany.cn/gtknhfsbsd.html

[E16] 数字千分位
来源：http://hz.pycfn.com/gtmgdmobbb.html

Py:   f"{1234567:,}"
来源：http://hz.xziqi.cn/gtypyojygp.html

PHP:  number_format(1234567);
来源：http://hz.316326.xyz/gtnigpfdzf.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.yuxming.cn/gtgvdztryf.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.tianlin.xyz/gtowlccdlu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.jiagoushi.top/gtqeztfhbt.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.yuanzhike.top/gtupzmawqs.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.yangfankeji.com/gtuerjkeio.html

C#:   1234567.ToString("N0")
来源：http://hz.bjfxy.top/gtczyhxbfd.html

[E17] 首字母大写
来源：http://hz.yuanzhike.top/gtpqpmhmnc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.sysykeji.top/gtyaoihmhf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.tanke756.top/gteubhxljn.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jqgfzy.top/gtncjlkfmx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.quarkkingdee.top/gtukpislde.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.shanyushiyangkeji.top/gtwlfiwmur.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.cqqwz.cn/gtujzizreb.html

Ruby: s.capitalize
来源：http://hz.zhoulong.xyz/gtxasowkdv.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.wangdashe.top/gtnkotalaw.html

[E18] 模板占位符替换
来源：http://hz.chenjidiqi.icu/gtjujcpsuv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.yuanzhike.top/gtimirfutc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.yj20258888.top/gtdavrfapg.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.kuanghao11.cn/gtyyeqzsqq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.kuanghao11.cn/gtbfmqpuoy.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.cdnleiting.top/gtpoeuzzik.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.shuidangran.top/gtkluhanxe.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.hnxiangtu.top/gtsqthdhtu.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.zhijiandao.cn/gtylxbrugj.html

[E19] 多行文本按行拆分
来源：http://hz.cashguo.top/gtwzkctzoa.html

Py:   s.splitlines()
来源：http://hz.0kj1m.cn/gtmxzlhbjh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.cucudq.cn/gttabioeqa.html

JS:   s.split(/\r?\n/)
来源：http://hz.meibo888.top/gtxpiipngm.html

TS:   s.split(/\r?\n/)
来源：http://hz.hammf.cn/gtlzvdssck.html

Java: s.lines().toList()
来源：http://hz.52xcode.cn/gtcizdngox.html

Go:   strings.Split(s, "\n")
来源：http://hz.dianchejie.cn/gtqbiqesad.html

Ruby: s.lines
来源：http://hz.ydjk.org.cn/gtpjxhmbgs.html

C#:   s.Split('\n')
来源：http://hz.zhoulong.xyz/gtddumipni.html

[E20] 判断字符串是否为空
来源：http://hz.andypj.xyz/gtppgoigts.html

Py:   if not s:
来源：http://hz.yuanzhike.top/gtviuypqvb.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.jinqigfzy.top/gtcmgpnqbc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.52xcode.cn/gthrozllqp.html

TS:   if (s === "") {}
来源：http://hz.pengpengdd.cyou/gtkxdbzszt.html

Java: if (s.isEmpty()) {}
来源：http://hz.dashuyun.cn/gtdsdunbih.html

Go:   if s == "" {}
来源：http://hz.yueranfly.top/gtryrfmrri.html

Ruby: if s.empty?
来源：http://hz.feifeiyinyue.top/gtooetvzmg.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.xylfe.cn/gtrdcrvvbe.html

[E21] 超长截断加省略号
来源：http://hz.shanyushiyangtech.top/gtzxphzwvy.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.gzhubu.top/gtfoizjmyy.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.bjfxy.top/gtukuqxvsx.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.hammf.cn/gthdxswdol.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.gotoacloud.top/gtbbgpwyyg.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.pengpengdd.cyou/gtewfmfgre.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.wangdashe.top/gtfxktrjiv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.pengpengdd.cyou/gtrzgunayf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.yvedp.cn/gtvokyilxq.html

[E22] 字节长度与字符长度
来源：http://hz.daria6918.cn/gtsdlppajf.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.jinyuanbaomall.cn/gtfjtwryka.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhongyouzk.top/gtvtzfeffh.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.cqqwz.cn/gtkcopetnd.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jlsjyb.cn/gtqaugrgyf.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.dashuyun.cn/gteegkljtg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.zhengqikj.top/gtfihpmjev.html

Ruby: s.bytesize;  s.length
来源：http://hz.yuanzhike.top/gtuxfhjelb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.cqqwz.cn/gtgkrnmqwx.html

================================================================================
来源：http://hz.fzhhl.top/gttomsqwna.html

F. 文件与目录
来源：http://hz.yvedp.cn/gtllxeywdz.html

================================================================================
来源：http://hz.dianchejie.cn/gtdqbzeasx.html

[F01] 读取整个文件
来源：http://hz.shanyushiyangkeji.top/gtsuvzbdcx.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.xziqi.cn/gtvxxudquj.html

PHP:  file_get_contents("a.txt");
来源：http://hz.c1oappe.top/gteldythav.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.gogol.net.cn/gtbcxvdruj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.nanxinkj.top/gtwwzlkkwg.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.redwolf501.top/gtibjjnujv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.xylfe.cn/gtpcqawtbd.html

Ruby: File.read("a.txt")
来源：http://hz.bjfxy.top/gthiypdaub.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yj202588.top/gtuldmwhoe.html

[F02] 逐行读取文件
来源：http://hz.haohaochexian.top/gtqwbdgmyy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.nanxuanxn.top/gtlnujgbgo.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.fengsongda.top/gtovjsgxig.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.sxryk.cn/gtiwkghhkc.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jianghu66.top/gtpqsynhti.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.svipenyu.cn/gtdygevvby.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.snrcjt.cn/gtxjiwmmmj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.jqgfzy.top/gtywsegkut.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.jqgfzy.top/gtskdcindg.html

[F03] 写入文件（覆盖）
来源：http://hz.gzhubu.top/gtclmtcixu.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.gogol.net.cn/gtgdtgatok.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.nanxuanxn.top/gtdsfpvtam.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hywenlv.cn/gtvouyzvny.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.pycfn.com/gtsatrdjmr.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.tianlin.xyz/gtftpyiilq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.0kj1m.cn/gtiqpzxczg.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.yj20258888.top/gtvccvilqk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.yuanzhike.top/gtgbdgkvhf.html

[F04] 追加写入文件
来源：http://hz.gzhubu.top/gtkrenifxh.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.zhixingplan.top/gtugyrecoi.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.zhijiandao.cn/gtejlzwkdo.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhengqikj.top/gtyyjjqvhc.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.xingfuxueyuan.xyz/gtiwmpipmn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.xinyue.icu/gttzikswfq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.xuanzx.com/gtpjevpfdh.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.snrcjt.cn/gteqwienfn.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.shangyingyoupin.top/gtyvsdpbym.html

[F05] 判断文件或目录是否存在
来源：http://hz.hywenlv.cn/gtmyidinhj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.shuidangran.top/gtjdctbloc.html

PHP:  file_exists("a.txt");
来源：http://hz.smart0.xyz/gtztzmzqvs.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yueranfly.top/gtoncjpkwr.html

TS:   fs.existsSync("a.txt")
来源：http://hz.jinyuanbaomall.cn/gttumgzqhi.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.nwbrower.top/gtmkwqftsx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.tianlin.xyz/gtzeexjjnv.html

Ruby: File.exist?("a.txt")
来源：http://hz.jinqigufen.top/gtuulufjsk.html

C#:   File.Exists("a.txt")
来源：http://hz.tanke756.top/gtzbaioyih.html

[F06] 删除文件
来源：http://hz.aibaodan.cn/gtxhijhtkg.html

Py:   os.remove("a.txt")
来源：http://hz.meibo888.top/gtaszycdzb.html

PHP:  unlink("a.txt");
来源：http://hz.xuetiantiany.cn/gtuwucvchf.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.ydjk.org.cn/gtezqaaita.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.cheryme.top/gtjoamilvb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.jiagoushi.top/gtxqncsfht.html

Go:   os.Remove("a.txt")
来源：http://hz.birdmap.top/gtskuxkwqz.html

Ruby: File.delete("a.txt")
来源：http://hz.c1oappe.top/gtvtzoygge.html

C#:   File.Delete("a.txt");
来源：http://hz.svipenyu.cn/gtmnpaqgfx.html

[F07] 创建目录（含多级）
来源：http://hz.jinqigufen.top/gtcvbpghzq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.cqqwz.cn/gtcnnvmewd.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.jinqigufen.top/gtivjvnzrs.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.xinyue.icu/gtwxckujak.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jqgfzy.top/gtkhimxhjd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.316326.xyz/gtazmjhopd.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.c1oappe.top/gttirauvmd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.wangshuangyany.cn/gtxjfynczj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.hnqzz.top/gtybimxzhb.html

[F08] 遍历目录
来源：http://hz.0kj1m.cn/gtzwearrxk.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yj20258888.top/gtimrbhake.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.chenjidiqi.icu/gtpvrqvarm.html

JS:   fs.readdirSync("dir")
来源：http://hz.gzhubu.top/gtmdgxetco.html

TS:   fs.readdirSync("dir")
来源：http://hz.mhx1999.top/gtuuazomlg.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.snrcjt.cn/gtnemzoepf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.wangdashe.top/gthuresayo.html

Ruby: Dir.children("dir")
来源：http://hz.xylfe.cn/gtilxzxvpu.html

C#:   Directory.GetFiles("dir")
来源：http://hz.sweek.top/gtucppmgfq.html

[F09] 获取文件大小
来源：http://hz.shanyushiyangtech.top/gtxhckssop.html

Py:   os.path.getsize("a.txt")
来源：http://hz.tanke756.top/gtvxxzbarb.html

PHP:  filesize("a.txt");
来源：http://hz.aizwys.cn/gtupovsrxc.html

JS:   fs.statSync("a.txt").size
来源：http://hz.hammf.cn/gtvmqposta.html

TS:   fs.statSync("a.txt").size
来源：http://hz.ppjwa.cn/gtjirutdtb.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.daria6918.cn/gttvxjczfh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.gaohongyu789.top/gtcaxnqbko.html

Ruby: File.size("a.txt")
来源：http://hz.daria6918.cn/gtrfmtoxnc.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.dashuyun.cn/gtldovknhi.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.zhaomingkeji.xyz/gtrbmpilfk.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.cdnleiting.top/gtzjirqwcb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.ehwqpu.com/gtpzdonbes.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.zhongyouzk.top/gtkiczpivk.html

TS:   path.extname("a.txt")
来源：http://hz.dashuyun.cn/gtuowwsvtg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.hnqzz.top/gtibxrvnok.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yongpay.top/gtarxsgwew.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jinghuilouyu.cn/gtgporntdm.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.ivvv.top/gtjunpzqmi.html

[F11] 复制与移动文件
来源：http://hz.yvedp.cn/gtzemqscnh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.ehwqpu.com/gtczsufxct.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.shangyingyoupin.top/gtlwgmbavj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.nwbrower.top/gtgczcccvb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.sysykeji.top/gtisyjdzsr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.xingfuxueyuan.xyz/gtcbkzuelm.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.pycfn.com/gtyiegklrr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.hammf.cn/gtsqrrwaub.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.ywan-chungtsiang.top/gtbjkqxcka.html

[F12] CSV 读写
来源：http://hz.redwolf501.top/gtbwzyfufn.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.quarkkingdee.top/gtkxehkxwp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.feifeiyinyue.top/gtcfqmwyoj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.jinqigufen.top/gtlzaahjja.html

TS:   // 同上
来源：http://hz.zhengqikj.top/gtggzqdstw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.ppjwa.cn/gthvsdwfyq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.sysykeji.top/gtrhwryubn.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jinqigufen.top/gtgsbaehin.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.svipenyu.cn/gthfkgxhqt.html

================================================================================
来源：http://hz.ehwqpu.com/gtntaitsvg.html

G. 面向对象
来源：http://hz.ppjwa.cn/gtbbvgsnew.html

================================================================================
来源：http://hz.guowangkeji.top/gtimynulig.html

[G01] 定义类
来源：http://hz.nwbrower.top/gtigsgqcam.html

Py:   class User: pass
来源：http://hz.yonumen.top/gtayzxmyoa.html

PHP:  class User {}
来源：http://hz.yuanzhike.top/gtfmlyhvyd.html

JS:   class User {}
来源：http://hz.xylfe.cn/gtvhygklle.html

TS:   class User { name: string = ""; }
来源：http://hz.yonumen.top/gtdryhvoyl.html

Java: class User {}
来源：http://hz.daxiang520.top/gtaekbtmqv.html

Go:   type User struct { Name string }
来源：http://hz.chenzaomai.com/gtosfdyton.html

Ruby: class User; end
来源：http://hz.wangdashe.top/gtfxmzjvsh.html

C#:   class User {}
来源：http://hz.yj20258.top/gtlmcfzntd.html

[G02] 构造函数
来源：http://hz.hongshengwenyu.top/gtlycffshr.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zhixingplan.top/gtdyufdfva.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.havefunace.top/gtjxitedkt.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.xuanzx.com/gtfjxnsolr.html

TS:   constructor(public name: string) {}
来源：http://hz.vqdsnc.cn/gtjbjpcbij.html

Java: User(String name) { this.name = name; }
来源：http://hz.pengpengdd.cyou/gtbvpxohck.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.gogol.net.cn/gtezdokgwd.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.ppjwa.cn/gttayugvfy.html

C#:   public User(string name) { Name = name; }
来源：http://hz.ivvv.top/gtixaeemky.html

[G03] 实例属性
来源：http://hz.hammf.cn/gtawqiehfp.html

Py:   self.name = "x"
来源：http://hz.fengsongda.top/gtiboucgeg.html

PHP:  public string $name = "x";
来源：http://hz.birdmap.top/gthbhgilru.html

JS:   this.name = "x";
来源：http://hz.jyoumei.cn/gtqtbttziq.html

TS:   name: string = "x";
来源：http://hz.shangyingyoupin.top/gtqinvuchs.html

Java: private String name;
来源：http://hz.zhaomingkeji.xyz/gthfauwdus.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yj20258888.top/gtivvfuatm.html

Ruby: @name = "x"
来源：http://hz.shzxlz.cn/gtnrtfixcc.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yueranfly.top/gtizwsvsdn.html

[G04] 定义方法
来源：http://hz.0kj1m.cn/gtbyfjwiwy.html

Py:   def greet(self): return self.name
来源：http://hz.mhx1999.top/gtnrjpnwjs.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.mhx1999.top/gtxxhvklxk.html

JS:   greet() { return this.name; }
来源：http://hz.jqgufenzy.top/gtetocwpnf.html

TS:   greet(): string { return this.name; }
来源：http://hz.yanxiufei.cn/gtsxvitnlm.html

Java: String greet() { return name; }
来源：http://hz.shangyingyoupin.top/gttemsfgbu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.shangyingyoupin.top/gtipoleenq.html

Ruby: def greet; @name; end
来源：http://hz.mhx1999.top/gtezjbswra.html

C#:   public string Greet() => Name;
来源：http://hz.yj20258888.top/gtutzlxoge.html

[G05] 继承
来源：http://hz.cheryme.top/gtjatckqji.html

Py:   class Admin(User): pass
来源：http://hz.chenzaomai.com/gtllwaoico.html

PHP:  class Admin extends User {}
来源：http://hz.jianghu66.top/gtdftqjytw.html

JS:   class Admin extends User {}
来源：http://hz.ehwqpu.com/gtvtvumrox.html

TS:   class Admin extends User {}
来源：http://hz.fzhhl.top/gtfzvgpzri.html

Java: class Admin extends User {}
来源：http://hz.yanxiufei.cn/gtyylafiqj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.fengsongda.top/gtjgktzfeg.html

Ruby: class Admin < User; end
来源：http://hz.nanxuanxn.top/gttzpjwdgd.html

C#:   class Admin : User {}
来源：http://hz.xuetiantiany.cn/gtwcpwzktq.html

[G06] 重写方法
来源：http://hz.zdqjudy.top/gtdbpusczz.html

Py:   def greet(self): return "admin"
来源：http://hz.quarkkingdee.top/gtclutnkox.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.yuanzhike.top/gtnhwmjrlm.html

JS:   greet() { return "admin"; }
来源：http://hz.birdmap.top/gtksuhdvsm.html

TS:   greet(): string { return "admin"; }
来源：http://hz.tanke756.top/gtlwixmbqq.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.hfpthk.cn/gtowxshfqx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.jqgufenzy.top/gtnwjqfutd.html

Ruby: def greet; "admin"; end
来源：http://hz.xingfuxueyuan.xyz/gtvinlvjrs.html

C#:   public override string Greet() => "admin";
来源：http://hz.cashguo.top/gtkqqqcsvn.html

[G07] 调用父类方法
来源：http://hz.gzhubu.top/gtoopfopjq.html

Py:   super().greet()
来源：http://hz.hnqzz.top/gtkmolkhft.html

PHP:  parent::greet();
来源：http://hz.gzhubu.top/gtvljrgfjs.html

JS:   super.greet();
来源：http://hz.xylfe.cn/gthginxtra.html

TS:   super.greet();
来源：http://hz.havefunace.top/gtmsygwqkb.html

Java: super.greet();
来源：http://hz.jqgufenzy.top/gteadkurbv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.gaohongyu789.top/gtbneiepem.html

Ruby: super
来源：http://hz.jqgufenzy.top/gtxaykcfwm.html

C#:   base.Greet();
来源：http://hz.316326.xyz/gtuguibavi.html

[G08] 静态方法与属性
来源：http://hz.ydjk.org.cn/gtvxowjsda.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.ehwqpu.com/gtshqulmml.html

PHP:  public static function f() {}
来源：http://hz.ppjwa.cn/gtqneqnqwv.html

JS:   static f() {}
来源：http://hz.aizwys.cn/gtnkdkdufv.html

TS:   static f(): void {}
来源：http://hz.ybcxt.top/gtefwqvsln.html

Java: static void f() {}
来源：http://hz.yj20258888.top/gtwjgdzvoo.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.shanyushiyangtech.top/gtlsqnafli.html

Ruby: def self.f; end
来源：http://hz.xuanzx.com/gtjwyctdmg.html

C#:   public static void F() {}
来源：http://hz.316326.xyz/gtmldjufrf.html

[G09] 接口 / 抽象类
来源：http://hz.shangyingyoupin.top/gtwtatfheq.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.zhengqikj.top/gtngsghlhk.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.meibo888.top/gtrozoqcgn.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.chenlongwang.top/gtfdgtxvrm.html

TS:   interface Shape { area(): number; }
来源：http://hz.c1oappe.top/gtajtbuzfm.html

Java: interface Shape { double area(); }
来源：http://hz.yuanzhike.top/gthovzqsiv.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.ppjwa.cn/gteyhpuswu.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.gogol.net.cn/gtefnnlron.html

C#:   interface IShape { double Area(); }
来源：http://hz.wangshuangyany.cn/gtodnjssmb.html

[G10] 访问控制
来源：http://hz.xziqi.cn/gtryouosxk.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.kuanghao11.cn/gtwdzsrsvq.html

PHP:  public / protected / private
来源：http://hz.wangdashe.top/gtwthjfezh.html

JS:   #private 字段；其余公开
来源：http://hz.hnqzz.top/gttkzbbeen.html

TS:   public / protected / private
来源：http://hz.dianchejie.cn/gtjhuwkvba.html

Java: public / protected / private / 默认包级
来源：http://hz.yangfankeji.com/gtliovmkvf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.ybcxt.top/gtpcnogfla.html

Ruby: public / protected / private
来源：http://hz.jinqigfzy.top/gtmepzttci.html

C#:   public / protected / private / internal
来源：http://hz.hysaishi.cn/gtqfofwlvk.html

[G11] getter / setter
来源：http://hz.hysaishi.cn/gtxfrdxnib.html

Py:   @property 与 @x.setter
来源：http://hz.ehwqpu.com/gtabqtotpl.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.chenjidiqi.icu/gtadnxeyfw.html

JS:   get name() { return this._name; }
来源：http://hz.xingfuxueyuan.xyz/gtgrrrbksd.html

TS:   get name(): string { return this._name; }
来源：http://hz.xingfuxueyuan.xyz/gtfptzceey.html

Java: public String getName() { return name; }
来源：http://hz.yj20258888.top/gtfybddssb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.kuanghao11.cn/gtuxfneyze.html


<!-- 参考信息 -->