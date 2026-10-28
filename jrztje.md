代发 wailian999

[E14] URL 编码与 Base64
来源：http://hz.dashuyun.cn/gtrqyxpctg.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.ivvv.top/gtylvgepvj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.svipenyu.cn/gtgtcwxejy.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.shanyushiyangkeji.top/gtymzmjoyo.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.jinyuanbaomall.cn/gtanxkxlqk.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.zhoulong.xyz/gtmkaqofqp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.aizwys.cn/gttlgqfsuh.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.hnxiangtu.top/gtojhtrjsi.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.cucudq.cn/gtpugrowkb.html

[E15] HTML 转义 / 反转义
来源：http://hz.pengpengdd.cyou/gtbjxhdbpy.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.zhijiandao.cn/gtwbjlooqb.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.haohaochexian.top/gtleqpqtoa.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.tanke756.top/gtnixuowue.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.gzhubu.top/gtipiqdtrh.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.daxiang520.top/gtgawiywtj.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.chenzaomai.com/gtdmihguea.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.sysykeji.top/gtwydcqgrg.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.cheryme.top/gtrlbdijck.html

[E16] 数字千分位
来源：http://hz.guannengcc.top/gtsdghpfap.html

Py:   f"{1234567:,}"
来源：http://hz.yangfankeji.com/gtatsgyxcw.html

PHP:  number_format(1234567);
来源：http://hz.hywenlv.cn/gttuwnmzdw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.ydjk.org.cn/gtmuxmgwdu.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.yj20258888.top/gtxpcvvist.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.gaohongyu789.top/gtirsltryl.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.ybcxt.top/gtsrtmnauq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.cdnleiting.top/gtdsyyzmff.html

C#:   1234567.ToString("N0")
来源：http://hz.zhengqikj.top/gtghpelyhh.html

[E17] 首字母大写
来源：http://hz.vqdsnc.cn/gtffqjqhqc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.jyoumei.cn/gtdamnaald.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.feifeiyinyue.top/gtbddcbrlp.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhongyouzk.top/gtjvwlikuy.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.shangyingyoupin.top/gtfkbjwtjz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.fengsongda.top/gtopjkzpxf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.gaohongyu789.top/gtrqfmgfew.html

Ruby: s.capitalize
来源：http://hz.yj202588.top/gtwdfaoqho.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.jinghuilouyu.cn/gtejlrxdmb.html

[E18] 模板占位符替换
来源：http://hz.wangshuangyany.cn/gtzvwaievx.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.dashuyun.cn/gtjnythvoe.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.zhijiandao.cn/gtsdbryuzt.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.fzhhl.top/gtooiwppaq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.redwolf501.top/gttvytkfxn.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.chenlongwang.top/gthmqzddlb.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.yvedp.cn/gtfdsazhug.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.iojbl.cn/gtmyblptny.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.yuanzhike.top/gtxblvmtpu.html

[E19] 多行文本按行拆分
来源：http://hz.birdmap.top/gtkplcrpvo.html

Py:   s.splitlines()
来源：http://hz.zhongyouzk.top/gtprjnerle.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jinyuanbaomall.cn/gtmufcxxyx.html

JS:   s.split(/\r?\n/)
来源：http://hz.zhiwuduotai.top/gtxzftkbpa.html

TS:   s.split(/\r?\n/)
来源：http://hz.wangshuangyany.cn/gtbhzdfyls.html

Java: s.lines().toList()
来源：http://hz.fzhhl.top/gthmwweexe.html

Go:   strings.Split(s, "\n")
来源：http://hz.daxiang520.top/gtjqwysllx.html

Ruby: s.lines
来源：http://hz.feifeiyinyue.top/gtneqdejuq.html

C#:   s.Split('\n')
来源：http://hz.wangdashe.top/gtcnjxvunx.html

[E20] 判断字符串是否为空
来源：http://hz.tian-w.cn/gtxkfvmsic.html

Py:   if not s:
来源：http://hz.jinghuilouyu.cn/gtdulteqib.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.vqdsnc.cn/gtjfyxbext.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.redwolf501.top/gtmjflonxj.html

TS:   if (s === "") {}
来源：http://hz.cqqwz.cn/gtpogvkyby.html

Java: if (s.isEmpty()) {}
来源：http://hz.jinqigfzy.top/gtnmeeprgb.html

Go:   if s == "" {}
来源：http://hz.ivvv.top/gtkmnynphk.html

Ruby: if s.empty?
来源：http://hz.guannengcc.top/gtntgrprlw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.xylfe.cn/gtkhfnmimd.html

[E21] 超长截断加省略号
来源：http://hz.zhongyouzk.top/gtrvncajcq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.hywenlv.cn/gtkpxtucxb.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.meibo888.top/gtxycruwmm.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.sweek.top/gtazzeapin.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.nanxuanxn.top/gtxtqniwou.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.pycfn.com/gtujdkzlda.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.gogol.net.cn/gtbjjvdint.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.cashguo.top/gtniyjuzgz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.nanxinkj.top/gtawcdydyz.html

[E22] 字节长度与字符长度
来源：http://hz.guowangkeji.top/gtdgvnuymw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.pycfn.com/gtnasxetts.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ywan-chungtsiang.top/gthqrczotn.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zdqjudy.top/gtqczaptyv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.wangshuangyany.cn/gthieddobh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.snrcjt.cn/gtdnipvnie.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.cheryme.top/gtmmcdtseb.html

Ruby: s.bytesize;  s.length
来源：http://hz.xuetiantiany.cn/gtmbystbjp.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.hywenlv.cn/gtbcpgwrfh.html

================================================================================
来源：http://hz.jqgfzy.top/gtivyzydhx.html

F. 文件与目录
来源：http://hz.yonumen.top/gtuqvncgfo.html

================================================================================
来源：http://hz.9152youxi.cn/gtvbrgxdik.html

[F01] 读取整个文件
来源：http://hz.hywenlv.cn/gtveakntca.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.chenjidiqi.icu/gtlmnxtbmu.html

PHP:  file_get_contents("a.txt");
来源：http://hz.fengsongda.top/gtddeenjte.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.quarkkingdee.top/gtayycipxm.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.shuidangran.top/gtavwwxgwy.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.jinqigfzy.top/gtoljjuoaj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.shuidangran.top/gtigueithh.html

Ruby: File.read("a.txt")
来源：http://hz.zhengqikj.top/gteqevkgen.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.wangshuangyany.cn/gtnkzrnkkp.html

[F02] 逐行读取文件
来源：http://hz.hywenlv.cn/gtbicajvot.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.aibaodan.cn/gtavfhycxf.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.zycfv.cn/gtsaojdcqh.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yueranfly.top/gthgfvcbmh.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ppjwa.cn/gthohergpv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.zhongyouzk.top/gtcafzmprz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.xingfuxueyuan.xyz/gtbmxqfyik.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.hfpthk.cn/gtejwdmwjy.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.cashguo.top/gttfnugisp.html

[F03] 写入文件（覆盖）
来源：http://hz.zhiwuduotai.top/gttpbsrmja.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.hywenlv.cn/gthgrprode.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.shuidangran.top/gtmloqesql.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhixingplan.top/gtlikidzuq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ydjk.org.cn/gtpwlvhvkx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.ywan-chungtsiang.top/gtqpakehln.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.meibo888.top/gtfdefwtbv.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.zhaomingkeji.xyz/gtmlyaqgst.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.xylfe.cn/gtchsekanl.html

[F04] 追加写入文件
来源：http://hz.guannengcc.top/gtaqorruxp.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.cashguo.top/gtiuhofwfx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.sxryk.cn/gtjdinzhxe.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.haohaochexian.top/gtutgthlkr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.kuanghao11.cn/gtadlhgduz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.pengpengdd.cyou/gtqjtiewwb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.tanke756.top/gtauqncmfk.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.snrcjt.cn/gteeyugqjc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.hammf.cn/gtscjjeqqf.html

[F05] 判断文件或目录是否存在
来源：http://hz.0kj1m.cn/gthjhszlet.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.quarkkingdee.top/gtrvpgdvud.html

PHP:  file_exists("a.txt");
来源：http://hz.jqgufenzy.top/gtlpcamrks.html

JS:   fs.existsSync("a.txt")
来源：http://hz.ppjwa.cn/gtrphtobqs.html

TS:   fs.existsSync("a.txt")
来源：http://hz.ydjk.org.cn/gtiaejmtak.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.xuetiantiany.cn/gtzqecwqaw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.yj20258.top/gtizfyfbqt.html

Ruby: File.exist?("a.txt")
来源：http://hz.nanxinkj.top/gtwxmwwuic.html

C#:   File.Exists("a.txt")
来源：http://hz.chenlongwang.top/gteinfrrrd.html

[F06] 删除文件
来源：http://hz.yuxming.cn/gttwezbujz.html

Py:   os.remove("a.txt")
来源：http://hz.hammf.cn/gteqdvxnbq.html

PHP:  unlink("a.txt");
来源：http://hz.nwbrower.top/gtjxwleytm.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.aizwys.cn/gtsnlozwni.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.yangfankeji.com/gtnlevnzdh.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.yvedp.cn/gtnqkuhmuw.html

Go:   os.Remove("a.txt")
来源：http://hz.mhx1999.top/gtwsfpcgye.html

Ruby: File.delete("a.txt")
来源：http://hz.cashguo.top/gtvhwndern.html

C#:   File.Delete("a.txt");
来源：http://hz.yuanzhike.top/gtaefpikij.html

[F07] 创建目录（含多级）
来源：http://hz.yj202588.top/gtzztshgum.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.sweek.top/gtfywexesi.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.ydzc1.top/gtsaggiajj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.chenzaomai.com/gtgfiehutj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ivvv.top/gtjhzgzqst.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.aizwys.cn/gtoiadiyan.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.0kj1m.cn/gtmzorfbmp.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.jqgufenzy.top/gttqieatzj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.9152youxi.cn/gtcjacllqf.html

[F08] 遍历目录
来源：http://hz.iojbl.cn/gtmcdfnhrw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.pengpengdd.cyou/gtzdxzzlak.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.sysykeji.top/gtgsduhghq.html

JS:   fs.readdirSync("dir")
来源：http://hz.jlsjyb.cn/gtbpkrcfxb.html

TS:   fs.readdirSync("dir")
来源：http://hz.chenzaomai.com/gtonyghspk.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.xziqi.cn/gtqtzshlog.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.ywan-chungtsiang.top/gtrsgtnzht.html

Ruby: Dir.children("dir")
来源：http://hz.tianlin.xyz/gtelmpuygl.html

C#:   Directory.GetFiles("dir")
来源：http://hz.wangshuangyany.cn/gtjhsrqfun.html

[F09] 获取文件大小
来源：http://hz.andypj.xyz/gtcmugivzf.html

Py:   os.path.getsize("a.txt")
来源：http://hz.jlsjyb.cn/gtvjpnfljh.html

PHP:  filesize("a.txt");
来源：http://hz.316326.xyz/gtjfaiwrku.html

JS:   fs.statSync("a.txt").size
来源：http://hz.smart0.xyz/gtasdlemtu.html

TS:   fs.statSync("a.txt").size
来源：http://hz.gzhubu.top/gthhwcarzk.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jiagoushi.top/gtcymvlcrl.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.zycfv.cn/gtvdwgqviq.html

Ruby: File.size("a.txt")
来源：http://hz.nanxinkj.top/gtwuehvvjd.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.hammf.cn/gttuqdqrxf.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.ybcxt.top/gttxxkspld.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.hnqzz.top/gttrthvhyt.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.shanyushiyangtech.top/gtpnivtvve.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.hysaishi.cn/gtpmhszfoe.html

TS:   path.extname("a.txt")
来源：http://hz.sufxvd.cn/gtvtsgymdx.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.cdnleiting.top/gtjqiltmpw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.shanyushiyangkeji.top/gtsopwjccw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.quarkkingdee.top/gtmtngwzrb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.cashguo.top/gtxvqtbzlt.html

[F11] 复制与移动文件
来源：http://hz.52xcode.cn/gthzrgyppl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.xingfuxueyuan.xyz/gtnzijurwb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.svipenyu.cn/gtoyrczzsz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.quarkkingdee.top/gtnqpiqkxg.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.dianchejie.cn/gtazsysrrs.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.aizwys.cn/gtlxhespsz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jinqigfzy.top/gtoxzgvisq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.hfpthk.cn/gtqrktoprm.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.cdnleiting.top/gtqxudtfjf.html

[F12] CSV 读写
来源：http://hz.yonumen.top/gthpvaincu.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.tian-w.cn/gtewrgxjxw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.zhijiandao.cn/gtwfhtsyuu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.ydzc1.top/gtnoszliov.html

TS:   // 同上
来源：http://hz.yj20258888.top/gtpgehlpdc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.shanyushiyangtech.top/gtenfhtnlb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.snrcjt.cn/gtrommbtsf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.cdnleiting.top/gttxaxeoom.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.hongshengwenyu.top/gteqgbfxhn.html

================================================================================
来源：http://hz.ydzc1.top/gticpgrdns.html

G. 面向对象
来源：http://hz.shangyingyoupin.top/gtrozoiena.html

================================================================================
来源：http://hz.gotoacloud.top/gtjbqypixw.html

[G01] 定义类
来源：http://hz.xuetiantiany.cn/gtiyggfsbe.html

Py:   class User: pass
来源：http://hz.tian-w.cn/gtprshqvwv.html

PHP:  class User {}
来源：http://hz.guannengcc.top/gtqbqyeghu.html

JS:   class User {}
来源：http://hz.nwbrower.top/gtxugeqibb.html

TS:   class User { name: string = ""; }
来源：http://hz.zdqjudy.top/gtulmrikek.html

Java: class User {}
来源：http://hz.ydzc1.top/gtuhlgwgnx.html

Go:   type User struct { Name string }
来源：http://hz.jiagoushi.top/gtlyunwlua.html

Ruby: class User; end
来源：http://hz.guowangkeji.top/gtyjgvsruo.html

C#:   class User {}
来源：http://hz.dashuyun.cn/gtigeyyklv.html

[G02] 构造函数
来源：http://hz.mhx1999.top/gtckjokpyn.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zdqjudy.top/gtfgurants.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.xziqi.cn/gtbjlzmsbe.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.hongshengwenyu.top/gthypgusbl.html

TS:   constructor(public name: string) {}
来源：http://hz.sxryk.cn/gttqoclcqz.html

Java: User(String name) { this.name = name; }
来源：http://hz.jqgufenzy.top/gteqrtzndl.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yueranfly.top/gtdpdbtckj.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.gotoacloud.top/gtdilxdobp.html

C#:   public User(string name) { Name = name; }
来源：http://hz.xylfe.cn/gtzugahwrb.html

[G03] 实例属性
来源：http://hz.chenzaomai.com/gtahhywgpu.html

Py:   self.name = "x"
来源：http://hz.52xcode.cn/gtmdorpgij.html

PHP:  public string $name = "x";
来源：http://hz.shanyushiyangtech.top/gtxkvtmtom.html

JS:   this.name = "x";
来源：http://hz.dianchejie.cn/gtijbodnqn.html

TS:   name: string = "x";
来源：http://hz.redwolf501.top/gtgqipgdbs.html

Java: private String name;
来源：http://hz.tanke756.top/gtvuwxdzgs.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.tian-w.cn/gtyhvnhdfq.html

Ruby: @name = "x"
来源：http://hz.chenjidiqi.icu/gtcwwgppsa.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.zycfv.cn/gtvtqinnqe.html

[G04] 定义方法
来源：http://hz.jinqigufen.top/gtaarncjyk.html

Py:   def greet(self): return self.name
来源：http://hz.cucudq.cn/gtxkghxpmu.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.hywenlv.cn/gtqlghhiby.html

JS:   greet() { return this.name; }
来源：http://hz.ydjk.org.cn/gtgdkxdkvm.html

TS:   greet(): string { return this.name; }
来源：http://hz.yuxming.cn/gtrbpybwcg.html

Java: String greet() { return name; }
来源：http://hz.cashguo.top/gthirznykg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.zhengqikj.top/gtforfxgct.html

Ruby: def greet; @name; end
来源：http://hz.gogol.net.cn/gtembgacsx.html

C#:   public string Greet() => Name;
来源：http://hz.shanyushiyangtech.top/gthxvxgtjs.html

[G05] 继承
来源：http://hz.zhijiandao.cn/gtxdnlltmf.html

Py:   class Admin(User): pass
来源：http://hz.jiagoushi.top/gtmrxdzkxl.html

PHP:  class Admin extends User {}
来源：http://hz.jianghu66.top/gtgnvsfnks.html

JS:   class Admin extends User {}
来源：http://hz.yanxiufei.cn/gtcepeyunx.html

TS:   class Admin extends User {}
来源：http://hz.shzxlz.cn/gtcrunisxb.html

Java: class Admin extends User {}
来源：http://hz.aizwys.cn/gtpuvbehcm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.chenjidiqi.icu/gtmnylwbzg.html

Ruby: class Admin < User; end
来源：http://hz.dashuyun.cn/gtycfxxzbe.html

C#:   class Admin : User {}
来源：http://hz.zycfv.cn/gtcyjazmsh.html

[G06] 重写方法
来源：http://hz.wangshuangyany.cn/gtzpcnwtdq.html

Py:   def greet(self): return "admin"
来源：http://hz.yj20258888.top/gtibibfusk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jiagoushi.top/gtoyambdhi.html

JS:   greet() { return "admin"; }
来源：http://hz.316326.xyz/gtlrcygfss.html

TS:   greet(): string { return "admin"; }
来源：http://hz.jqgfzy.top/gtqceogkto.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.dashuyun.cn/gtrenemhij.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.shanyushiyangtech.top/gtvqdqbhdd.html

Ruby: def greet; "admin"; end
来源：http://hz.zhixingplan.top/gtshkwxttz.html

C#:   public override string Greet() => "admin";
来源：http://hz.sxryk.cn/gtgiadlbmd.html

[G07] 调用父类方法
来源：http://hz.havefunace.top/gttsyuvhsc.html

Py:   super().greet()
来源：http://hz.zhijiandao.cn/gtzashpdqo.html

PHP:  parent::greet();
来源：http://hz.xylfe.cn/gtlipoykbm.html

JS:   super.greet();
来源：http://hz.chenlongwang.top/gtkwggqrue.html

TS:   super.greet();
来源：http://hz.kuanghao11.cn/gtawrjglku.html

Java: super.greet();
来源：http://hz.dianchejie.cn/gtxxskoxju.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.aibaodan.cn/gtqyrlxkjs.html

Ruby: super
来源：http://hz.aibaodan.cn/gtmopbyzkf.html

C#:   base.Greet();
来源：http://hz.guowangkeji.top/gtjyjhhssq.html

[G08] 静态方法与属性
来源：http://hz.andypj.xyz/gthxtiouju.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.guannengcc.top/gtykksvooj.html

PHP:  public static function f() {}
来源：http://hz.xuanzx.com/gtrrazqsen.html

JS:   static f() {}
来源：http://hz.cqqwz.cn/gttqjdddzw.html

TS:   static f(): void {}
来源：http://hz.52xcode.cn/gtwiubswyp.html

Java: static void f() {}
来源：http://hz.0kj1m.cn/gtibniocpq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.quarkkingdee.top/gtuaxaanww.html

Ruby: def self.f; end
来源：http://hz.daxiang520.top/gtcrnahdie.html

C#:   public static void F() {}
来源：http://hz.cashguo.top/gtkylbneys.html

[G09] 接口 / 抽象类
来源：http://hz.daria6918.cn/gtezmpikgc.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.jinghuilouyu.cn/gtqejlrkvm.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.cheryme.top/gtcnpywmhf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.ybcxt.top/gtpforbrzj.html

TS:   interface Shape { area(): number; }
来源：http://hz.cdnleiting.top/gtruadkowf.html

Java: interface Shape { double area(); }
来源：http://hz.daxiang520.top/gtpniurgeg.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.jinqigfzy.top/gtxtoqecno.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.nanxinkj.top/gtkxyerftm.html

C#:   interface IShape { double Area(); }
来源：http://hz.zycfv.cn/gtsddzcfsk.html

[G10] 访问控制
来源：http://hz.bjfxy.top/gtwdkjycyo.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yangfankeji.com/gtacwvarax.html

PHP:  public / protected / private
来源：http://hz.snrcjt.cn/gtyyeynfyn.html

JS:   #private 字段；其余公开
来源：http://hz.yj202588.top/gtcakumwgx.html

TS:   public / protected / private
来源：http://hz.sysykeji.top/gtnmjprdbd.html

Java: public / protected / private / 默认包级
来源：http://hz.iojbl.cn/gtwodewhxi.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.guowangkeji.top/gtpxpyvnlo.html

Ruby: public / protected / private
来源：http://hz.shzxlz.cn/gtxzhaszth.html

C#:   public / protected / private / internal
来源：http://hz.shanyushiyangtech.top/gtkeruvzxv.html

[G11] getter / setter
来源：http://hz.birdmap.top/gtqlyvnehz.html

Py:   @property 与 @x.setter
来源：http://hz.yj20258.top/gtmdrwcuhe.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.aizwys.cn/gtlpmqzjzh.html

JS:   get name() { return this._name; }
来源：http://hz.jqgufenzy.top/gtcnjeudzl.html

TS:   get name(): string { return this._name; }
来源：http://hz.zhoulong.xyz/gtfmixzfox.html

Java: public String getName() { return name; }
来源：http://hz.svipenyu.cn/gthrtoqosn.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.jyoumei.cn/gtybrktjpb.html

Ruby: attr_accessor :name
来源：http://hz.fzhhl.top/gtvcjeelro.html

C#:   public string Name { get; set; }
来源：http://hz.ydjk.org.cn/gtvxudayit.html

[G12] 对象转字符串
来源：http://hz.pengpengdd.cyou/gtkzforlbc.html

Py:   def __str__(self): return self.name
来源：http://hz.yangfankeji.com/gttabgaxth.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jinghuilouyu.cn/gtbnmtigqb.html

JS:   toString() { return this.name; }
来源：http://hz.nwbrower.top/gtgwsjrmkt.html

TS:   toString(): string { return this.name; }
来源：http://hz.316326.xyz/gttdulzwgk.html

Java: @Override public String toString() { return name; }
来源：http://hz.zhixingplan.top/gtlltvzhai.html


<!-- 参考信息 -->