代发 wailian999

[E14] URL 编码与 Base64
来源：http://hz.zhoulong.xyz/gtqptemead.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.haohaochexian.top/gtkcljxhyl.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.fzhhl.top/gteddflxij.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.birdmap.top/gtoaogcqbi.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.aibaodan.cn/gtgnshaekd.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.aibaodan.cn/gtshxephjk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.kuanghao11.cn/gtbtxdstcm.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.cashguo.top/gtnjnnpjtn.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yangfankeji.com/gtlmpzhsxc.html

[E15] HTML 转义 / 反转义
来源：http://hz.cashguo.top/gtprzexdnm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.nanxuanxn.top/gtkjmatdud.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.birdmap.top/gtqkmwzohz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.bjfxy.top/gtauknavrj.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.gaohongyu789.top/gtdizmsvod.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.shuidangran.top/gtiqtrgdck.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.fengsongda.top/gtpqkjxvkb.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.tian-w.cn/gtopuenmrw.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.ydjk.org.cn/gteydtyiac.html

[E16] 数字千分位
来源：http://hz.zhongyouzk.top/gtdfbcggvt.html

Py:   f"{1234567:,}"
来源：http://hz.jlsjyb.cn/gtzrsdhdln.html

PHP:  number_format(1234567);
来源：http://hz.jqgfzy.top/gtlywekqeu.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.jinqigfzy.top/gtanhlkuot.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.redwolf501.top/gtwodpfmeg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.dashuyun.cn/gtldmbzngp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.vqdsnc.cn/gtssxhfvxt.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.0kj1m.cn/gtbgmrenoq.html

C#:   1234567.ToString("N0")
来源：http://hz.gogol.net.cn/gtxsquwple.html

[E17] 首字母大写
来源：http://hz.yj20258.top/gtabbifisi.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.redwolf501.top/gtgkdpkfvj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.jlsjyb.cn/gtndvrkblx.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.gotoacloud.top/gtfavyohek.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.gaohongyu789.top/gtbtrufxxe.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.guowangkeji.top/gtjcjsucgh.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.zdqjudy.top/gtarabjcte.html

Ruby: s.capitalize
来源：http://hz.jlsjyb.cn/gtxmbtlfda.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.dashuyun.cn/gtwsiebsda.html

[E18] 模板占位符替换
来源：http://hz.yuxming.cn/gtjujogjgc.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.redwolf501.top/gtpucxxuqa.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.0kj1m.cn/gtfaofangg.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.hfpthk.cn/gtwdashqxc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.cqqwz.cn/gtlpifyddt.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.haohaochexian.top/gtdwyaujqm.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.dashuyun.cn/gtpskorhem.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.chenlongwang.top/gtenfixqer.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.daxiang520.top/gtpfxrkxfs.html

[E19] 多行文本按行拆分
来源：http://hz.jianghu66.top/gtorfvnmik.html

Py:   s.splitlines()
来源：http://hz.hongshengwenyu.top/gtziaoelpu.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.chenjidiqi.icu/gtakqdsnsw.html

JS:   s.split(/\r?\n/)
来源：http://hz.nanxuanxn.top/gtjtilmnyu.html

TS:   s.split(/\r?\n/)
来源：http://hz.xylfe.cn/gtihfsjfya.html

Java: s.lines().toList()
来源：http://hz.sxryk.cn/gtjvqjlzvx.html

Go:   strings.Split(s, "\n")
来源：http://hz.yj202588.top/gtahosozyq.html

Ruby: s.lines
来源：http://hz.feifeiyinyue.top/gtqwqsmxyt.html

C#:   s.Split('\n')
来源：http://hz.nanxuanxn.top/gtyavxogrd.html

[E20] 判断字符串是否为空
来源：http://hz.chenjidiqi.icu/gtwhqqcxyf.html

Py:   if not s:
来源：http://hz.ywan-chungtsiang.top/gtvuyelcxx.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.52xcode.cn/gtpisrache.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.jyoumei.cn/gtjuncttlu.html

TS:   if (s === "") {}
来源：http://hz.hnqzz.top/gtojsuggks.html

Java: if (s.isEmpty()) {}
来源：http://hz.haohaochexian.top/gtfzhoilgm.html

Go:   if s == "" {}
来源：http://hz.ppjwa.cn/gttkqhuxvu.html

Ruby: if s.empty?
来源：http://hz.yuanzhike.top/gtnoysrcnv.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.cashguo.top/gtdlmtuyar.html

[E21] 超长截断加省略号
来源：http://hz.yanxiufei.cn/gtsbvhpuob.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.cashguo.top/gtvtglikaq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.yuxming.cn/gtoiesasbq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.havefunace.top/gtusmtbxhv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.redwolf501.top/gtraqxpzxj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yanxiufei.cn/gtnrzfydjk.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.cqqwz.cn/gtygwcamhy.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.gaohongyu789.top/gtldmwbify.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.sweek.top/gthaquutsh.html

[E22] 字节长度与字符长度
来源：http://hz.fengsongda.top/gtphulkpvu.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.shuidangran.top/gttrmwsuwq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.cashguo.top/gthoocmuie.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.daria6918.cn/gtiwactxfk.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.meibo888.top/gtnvvgbtpe.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.mhx1999.top/gtbhihkaws.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.aibaodan.cn/gtgccepjed.html

Ruby: s.bytesize;  s.length
来源：http://hz.zhaomingkeji.xyz/gtkbeltxmb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.yueranfly.top/gtidasswsa.html

================================================================================
来源：http://hz.tanke756.top/gtoxcncxmw.html

F. 文件与目录
来源：http://hz.jiagoushi.top/gtqgcxvgrw.html

================================================================================
来源：http://hz.hfpthk.cn/gtrzgcmttl.html

[F01] 读取整个文件
来源：http://hz.yj202588.top/gtwvajwffq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.sxryk.cn/gtejkefiac.html

PHP:  file_get_contents("a.txt");
来源：http://hz.tanke756.top/gtaprikurh.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.chenzaomai.com/gtvrqobfwr.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.dianchejie.cn/gtywcdywmj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.dashuyun.cn/gtwrnrnocv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.tianlin.xyz/gtgnmhdtuj.html

Ruby: File.read("a.txt")
来源：http://hz.zhijiandao.cn/gtearxoqot.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.zhixingplan.top/gtugqffujv.html

[F02] 逐行读取文件
来源：http://hz.ydzc1.top/gtkyvifzyd.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.jqgfzy.top/gtnyohspxv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.pengpengdd.cyou/gtfvgkklhx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.shanyushiyangkeji.top/gtcxznapkh.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhijiandao.cn/gtxppliegu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.kuanghao11.cn/gtbmodlxqx.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.iojbl.cn/gtaglcfyon.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.jlsjyb.cn/gtezxcsqcg.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.nanxuanxn.top/gtthjawxnm.html

[F03] 写入文件（覆盖）
来源：http://hz.guannengcc.top/gtziialjkq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.xuetiantiany.cn/gtfpqnmzwg.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.yj20258888.top/gtlfvkknvx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.mhx1999.top/gtkdlkvryj.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jqgufenzy.top/gthffqemtc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.shanyushiyangtech.top/gtsnldnhdn.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.yanxiufei.cn/gtkkzwjsto.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.jianghu66.top/gtnjskmtlk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.gaohongyu789.top/gtnyobsrbd.html

[F04] 追加写入文件
来源：http://hz.snrcjt.cn/gtacxugzko.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.gogol.net.cn/gtxjjgtuxp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.hnxiangtu.top/gttkrjucbc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.c1oappe.top/gtdrneyhea.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.haohaochexian.top/gtsywsyptn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.tian-w.cn/gtrdyfgfaw.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.yuanzhike.top/gtlevkhxvw.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.316326.xyz/gtllgckdfb.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.pycfn.com/gtfjiontnn.html

[F05] 判断文件或目录是否存在
来源：http://hz.hammf.cn/gtjbndxgfp.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.hongshengwenyu.top/gtwfveqmpl.html

PHP:  file_exists("a.txt");
来源：http://hz.yanxiufei.cn/gtdzwppedf.html

JS:   fs.existsSync("a.txt")
来源：http://hz.pycfn.com/gtodnaxjoc.html

TS:   fs.existsSync("a.txt")
来源：http://hz.hysaishi.cn/gtbrexcryc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.yonumen.top/gtafwuiwox.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.xuetiantiany.cn/gtibtlcymu.html

Ruby: File.exist?("a.txt")
来源：http://hz.chenlongwang.top/gtbxxfdnjb.html

C#:   File.Exists("a.txt")
来源：http://hz.tianlin.xyz/gtcaseatwg.html

[F06] 删除文件
来源：http://hz.c1oappe.top/gtlklkxoju.html

Py:   os.remove("a.txt")
来源：http://hz.sweek.top/gtpzbddufy.html

PHP:  unlink("a.txt");
来源：http://hz.shanyushiyangkeji.top/gtbcglrdaw.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.dianchejie.cn/gtbhpqvhug.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.sweek.top/gtjpnbhvop.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.daxiang520.top/gtewvtlbmg.html

Go:   os.Remove("a.txt")
来源：http://hz.zhaomingkeji.xyz/gtjggwqvov.html

Ruby: File.delete("a.txt")
来源：http://hz.yonumen.top/gtobclzoyf.html

C#:   File.Delete("a.txt");
来源：http://hz.andypj.xyz/gtgobacxaf.html

[F07] 创建目录（含多级）
来源：http://hz.cashguo.top/gtdrsbavox.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.jinghuilouyu.cn/gtdmdrjszs.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.tian-w.cn/gtvkipspof.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhijiandao.cn/gtizmdgxgm.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.52xcode.cn/gtulexjvxz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.hnxiangtu.top/gtkxdxslxy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.zhijiandao.cn/gtjxdftjgb.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.svipenyu.cn/gtoohzvghq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.xuetiantiany.cn/gtozxgxmas.html

[F08] 遍历目录
来源：http://hz.jinqigufen.top/gtqbyyhywu.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.zhengqikj.top/gtjtolshcn.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.daria6918.cn/gtaeypfozi.html

JS:   fs.readdirSync("dir")
来源：http://hz.fzhhl.top/gtguyagcca.html

TS:   fs.readdirSync("dir")
来源：http://hz.jinqigufen.top/gtozhfrqlf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.hongshengwenyu.top/gtqjtugank.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.cqqwz.cn/gtonpggvjc.html

Ruby: Dir.children("dir")
来源：http://hz.shangyingyoupin.top/gtxsmsjzkc.html

C#:   Directory.GetFiles("dir")
来源：http://hz.nanxuanxn.top/gtdmdaielz.html

[F09] 获取文件大小
来源：http://hz.hnqzz.top/gtsfqiunkb.html

Py:   os.path.getsize("a.txt")
来源：http://hz.cashguo.top/gtnoupgvmu.html

PHP:  filesize("a.txt");
来源：http://hz.zhiwuduotai.top/gtywqmftzm.html

JS:   fs.statSync("a.txt").size
来源：http://hz.redwolf501.top/gttwkaefwv.html

TS:   fs.statSync("a.txt").size
来源：http://hz.gaohongyu789.top/gtjajjsmtd.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.sufxvd.cn/gtjhxcpxpl.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.daxiang520.top/gtvqeppbbj.html

Ruby: File.size("a.txt")
来源：http://hz.0kj1m.cn/gtluvpjfgk.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.zhiwuduotai.top/gttyhqnwaw.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.vqdsnc.cn/gthrcgqukd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.chenjidiqi.icu/gtvqiijbyz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.dianchejie.cn/gthlnimgxw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.ywan-chungtsiang.top/gthyvrlztz.html

TS:   path.extname("a.txt")
来源：http://hz.svipenyu.cn/gtujfdzbwx.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.ehwqpu.com/gtrxpplzkb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.9152youxi.cn/gtyywrgffh.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.nwbrower.top/gtzftnscbf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.ydjk.org.cn/gtdjyygokd.html

[F11] 复制与移动文件
来源：http://hz.chenzaomai.com/gtarqwxyob.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.hywenlv.cn/gtrerlrrgv.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.cdnleiting.top/gtxepjzrdv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yongpay.top/gtqyszvmpp.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.pycfn.com/gtyeetmzdd.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.tian-w.cn/gtnpusjnfl.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.hnqzz.top/gtijxmygmv.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.zycfv.cn/gtdpqukdke.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.jiagoushi.top/gtoxdduued.html

[F12] CSV 读写
来源：http://hz.shuidangran.top/gtungqxxqp.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.0kj1m.cn/gtkaybxnds.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.tianlin.xyz/gteifxsytm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.vqdsnc.cn/gtanmmogkx.html

TS:   // 同上
来源：http://hz.tianlin.xyz/gtdfuhxcjv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.dashuyun.cn/gtnabwyzdp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yangfankeji.com/gtlocxpsjp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.wangdashe.top/gtbuuzmlbj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.xylfe.cn/gtxhliomsy.html

================================================================================
来源：http://hz.zhijiandao.cn/gtiufnkqpz.html

G. 面向对象
来源：http://hz.jinqigfzy.top/gtbotjeinp.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtktxwhszm.html

[G01] 定义类
来源：http://hz.wangshuangyany.cn/gthxedvazt.html

Py:   class User: pass
来源：http://hz.ydzc1.top/gtaxfuydif.html

PHP:  class User {}
来源：http://hz.zhixingplan.top/gtlfexkfcd.html

JS:   class User {}
来源：http://hz.xinyue.icu/gtbdnhzmhu.html

TS:   class User { name: string = ""; }
来源：http://hz.yuanzhike.top/gtlvnikzdc.html

Java: class User {}
来源：http://hz.9152youxi.cn/gtrlnxftoe.html

Go:   type User struct { Name string }
来源：http://hz.zhengqikj.top/gtjmvzhvfl.html

Ruby: class User; end
来源：http://hz.tian-w.cn/gtomvsaled.html

C#:   class User {}
来源：http://hz.haohaochexian.top/gtxvigtqbq.html

[G02] 构造函数
来源：http://hz.shanyushiyangkeji.top/gtkuzfaenk.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.fzhhl.top/gtckxtugnc.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.nanxuanxn.top/gtzdhbvkml.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.smart0.xyz/gtjdidpfoe.html

TS:   constructor(public name: string) {}
来源：http://hz.chenzaomai.com/gtdysbjaee.html

Java: User(String name) { this.name = name; }
来源：http://hz.meibo888.top/gtdwostdbk.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yj20258888.top/gtvnzxefwp.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.daxiang520.top/gtpwahlync.html

C#:   public User(string name) { Name = name; }
来源：http://hz.chenjidiqi.icu/gtggkdqbea.html

[G03] 实例属性
来源：http://hz.xylfe.cn/gtxiznjvbe.html

Py:   self.name = "x"
来源：http://hz.redwolf501.top/gtpspnxoij.html

PHP:  public string $name = "x";
来源：http://hz.hammf.cn/gtzjaooheh.html

JS:   this.name = "x";
来源：http://hz.yj20258.top/gtldefxpol.html

TS:   name: string = "x";
来源：http://hz.nanxuanxn.top/gtnlbmusuk.html

Java: private String name;
来源：http://hz.jinyuanbaomall.cn/gtvwnipnsq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.fzhhl.top/gtltzvsces.html

Ruby: @name = "x"
来源：http://hz.pengpengdd.cyou/gtcfuyhmaa.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.pycfn.com/gtxocdixhr.html

[G04] 定义方法
来源：http://hz.birdmap.top/gtljodhlso.html

Py:   def greet(self): return self.name
来源：http://hz.hnqzz.top/gtuhfmwaas.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.hammf.cn/gtenxsaqwf.html

JS:   greet() { return this.name; }
来源：http://hz.smart0.xyz/gtsuktbiwg.html

TS:   greet(): string { return this.name; }
来源：http://hz.pengpengdd.cyou/gtujsjcqob.html

Java: String greet() { return name; }
来源：http://hz.quarkkingdee.top/gtajquuuqy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.shuidangran.top/gtinhhkwzn.html

Ruby: def greet; @name; end
来源：http://hz.fzhhl.top/gtmyxhvgkn.html

C#:   public string Greet() => Name;
来源：http://hz.iojbl.cn/gtklubsqxy.html

[G05] 继承
来源：http://hz.nanxuanxn.top/gtlivobdyr.html

Py:   class Admin(User): pass
来源：http://hz.guannengcc.top/gtprlkposf.html

PHP:  class Admin extends User {}
来源：http://hz.havefunace.top/gtushwlebx.html

JS:   class Admin extends User {}
来源：http://hz.cashguo.top/gtjanehevz.html

TS:   class Admin extends User {}
来源：http://hz.vqdsnc.cn/gtphrgvtjq.html

Java: class Admin extends User {}
来源：http://hz.sweek.top/gtyshwfvin.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.jinqigfzy.top/gtxqialffi.html

Ruby: class Admin < User; end
来源：http://hz.gotoacloud.top/gtqhfgbfxk.html

C#:   class Admin : User {}
来源：http://hz.zhengqikj.top/gtrwtxmmnw.html

[G06] 重写方法
来源：http://hz.xuetiantiany.cn/gthcgiisgf.html

Py:   def greet(self): return "admin"
来源：http://hz.sxryk.cn/gtnvgxpcjl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.hywenlv.cn/gtnizyvuru.html

JS:   greet() { return "admin"; }
来源：http://hz.yonumen.top/gtbdychujs.html

TS:   greet(): string { return "admin"; }
来源：http://hz.vqdsnc.cn/gturlupzhd.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.yj202588.top/gtyjdingwf.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.havefunace.top/gthfslzphj.html

Ruby: def greet; "admin"; end
来源：http://hz.aizwys.cn/gtrzydwqro.html

C#:   public override string Greet() => "admin";
来源：http://hz.hfpthk.cn/gtwnoytrtw.html

[G07] 调用父类方法
来源：http://hz.cqqwz.cn/gtveziuxop.html

Py:   super().greet()
来源：http://hz.ydjk.org.cn/gttbugyimx.html

PHP:  parent::greet();
来源：http://hz.jinghuilouyu.cn/gtsiwcrbky.html

JS:   super.greet();
来源：http://hz.snrcjt.cn/gtirdbpfvr.html

TS:   super.greet();
来源：http://hz.aibaodan.cn/gtltodkyqy.html

Java: super.greet();
来源：http://hz.yonumen.top/gtznnpgmty.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.hfpthk.cn/gthaxaqkkz.html

Ruby: super
来源：http://hz.dianchejie.cn/gtixxexebi.html

C#:   base.Greet();
来源：http://hz.daxiang520.top/gtidbllhgd.html

[G08] 静态方法与属性
来源：http://hz.sufxvd.cn/gthqrlocre.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.c1oappe.top/gtwgrmwzvy.html

PHP:  public static function f() {}
来源：http://hz.jianghu66.top/gteqmszqqx.html

JS:   static f() {}
来源：http://hz.hysaishi.cn/gtsvfpacwy.html

TS:   static f(): void {}
来源：http://hz.yonumen.top/gtlrjwkilq.html

Java: static void f() {}
来源：http://hz.sufxvd.cn/gtkdqyuvhd.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yonumen.top/gthvywjtns.html

Ruby: def self.f; end
来源：http://hz.mhx1999.top/gtwksiyznx.html

C#:   public static void F() {}
来源：http://hz.chenlongwang.top/gtjrgkmxgj.html

[G09] 接口 / 抽象类
来源：http://hz.xziqi.cn/gtalcdixvi.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yangfankeji.com/gtrrnvemmb.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jinyuanbaomall.cn/gtqdqzywti.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.xinyue.icu/gtjvpyldct.html

TS:   interface Shape { area(): number; }
来源：http://hz.xziqi.cn/gtmwdqcpxl.html

Java: interface Shape { double area(); }
来源：http://hz.dashuyun.cn/gtijttxkev.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.birdmap.top/gtdyusrkle.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.pengpengdd.cyou/gtmuawkyvw.html

C#:   interface IShape { double Area(); }
来源：http://hz.wangshuangyany.cn/gtlzmznoot.html

[G10] 访问控制
来源：http://hz.hnqzz.top/gtawdphjbm.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.daxiang520.top/gthmntjmur.html

PHP:  public / protected / private
来源：http://hz.sweek.top/gtvrymuhti.html

JS:   #private 字段；其余公开
来源：http://hz.yuanzhike.top/gtyhfevpas.html

TS:   public / protected / private
来源：http://hz.feifeiyinyue.top/gtjafjcvds.html

Java: public / protected / private / 默认包级
来源：http://hz.vqdsnc.cn/gtvsoyidkf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.ybcxt.top/gtxuiseuyc.html

Ruby: public / protected / private
来源：http://hz.yonumen.top/gtfligqfvv.html

C#:   public / protected / private / internal
来源：http://hz.ehwqpu.com/gtcjpollzl.html

[G11] getter / setter
来源：http://hz.zhixingplan.top/gtiufvxonj.html

Py:   @property 与 @x.setter
来源：http://hz.guowangkeji.top/gtpnixyvjv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.ywan-chungtsiang.top/gtqgibpqib.html

JS:   get name() { return this._name; }
来源：http://hz.kuanghao11.cn/gtxixtgzry.html

TS:   get name(): string { return this._name; }
来源：http://hz.jqgfzy.top/gtbpkoshtf.html

Java: public String getName() { return name; }
来源：http://hz.jinyuanbaomall.cn/gtpfzblumq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.cucudq.cn/gtzqfmoqzp.html

Ruby: attr_accessor :name
来源：http://hz.snrcjt.cn/gttexcebgh.html

C#:   public string Name { get; set; }
来源：http://hz.vqdsnc.cn/gtynbaococ.html

[G12] 对象转字符串
来源：http://hz.snrcjt.cn/gttnhuzclz.html

Py:   def __str__(self): return self.name
来源：http://hz.yangfankeji.com/gtsjnfrhaa.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.xylfe.cn/gtvjcxjxtr.html

JS:   toString() { return this.name; }
来源：http://hz.jinghuilouyu.cn/gtuhgypxos.html

TS:   toString(): string { return this.name; }
来源：http://hz.pycfn.com/gtgyeziuci.html

Java: @Override public String toString() { return name; }
来源：http://hz.birdmap.top/gtamxhtnks.html


<!-- 参考信息 -->