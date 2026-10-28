代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.snrcjt.cn/gtdancwtdu.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.fengsongda.top/gtvxghlbfb.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.yuxming.cn/gtuenkojoi.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.hnxiangtu.top/gtpbxnlpbt.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.zhoulong.xyz/gtxzeltues.html

[E15] HTML 转义 / 反转义
来源：http://hz.jyoumei.cn/gtinchflny.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.52xcode.cn/gtnoeyblzf.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.xinyue.icu/gtcdnzryvr.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.zhoulong.xyz/gtcygyubrd.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.shuidangran.top/gtpwxeokoz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.ydzc1.top/gtsaahmbgu.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.yj20258888.top/gtnyqcikwo.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.xinyue.icu/gttnykeavj.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.snrcjt.cn/gtobqfxudc.html

[E16] 数字千分位
来源：http://hz.zhiwuduotai.top/gtvyuelnne.html

Py:   f"{1234567:,}"
来源：http://hz.cdnleiting.top/gtuinorqzh.html

PHP:  number_format(1234567);
来源：http://hz.havefunace.top/gtsswzxvpe.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.quarkkingdee.top/gtuokcckkr.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.sysykeji.top/gtekuvxcvu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.zdqjudy.top/gtarjozurb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.jinghuilouyu.cn/gtvqlwsvlw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.jianghu66.top/gtsxvediiw.html

C#:   1234567.ToString("N0")
来源：http://hz.fengsongda.top/gtshcyrhlq.html

[E17] 首字母大写
来源：http://hz.0kj1m.cn/gtvppdmjpv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.shanyushiyangtech.top/gtuaxszsdm.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.xinyue.icu/gtdzynkxld.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.nwbrower.top/gtxisdgsdl.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jinqigufen.top/gtdnnnwvur.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.ivvv.top/gtxnfreejo.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.hywenlv.cn/gtiokzkruz.html

Ruby: s.capitalize
来源：http://hz.ppjwa.cn/gttkanyjdv.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.gotoacloud.top/gtkklxsduc.html

[E18] 模板占位符替换
来源：http://hz.9152youxi.cn/gtlzanwtvu.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.shangyingyoupin.top/gtkwcpsmsp.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.aizwys.cn/gtcvzgradu.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.hnxiangtu.top/gtvoxkpltg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.sweek.top/gtbusdbzli.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.yuxming.cn/gtqclkccup.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.xuanzx.com/gtfifhyayn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.jinghuilouyu.cn/gtzveftpkq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.jinyuanbaomall.cn/gttwouoits.html

[E19] 多行文本按行拆分
来源：http://hz.0kj1m.cn/gtlmqxoytk.html

Py:   s.splitlines()
来源：http://hz.jlsjyb.cn/gtvonhyplp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.cucudq.cn/gtvsgelphl.html

JS:   s.split(/\r?\n/)
来源：http://hz.ehwqpu.com/gtddxnvapo.html

TS:   s.split(/\r?\n/)
来源：http://hz.zhijiandao.cn/gtutyipvws.html

Java: s.lines().toList()
来源：http://hz.xinyue.icu/gtwqvzotcm.html

Go:   strings.Split(s, "\n")
来源：http://hz.iojbl.cn/gtdjbnxhpl.html

Ruby: s.lines
来源：http://hz.snrcjt.cn/gtlabmqkwl.html

C#:   s.Split('\n')
来源：http://hz.yj202588.top/gtjctyxzkl.html

[E20] 判断字符串是否为空
来源：http://hz.hongshengwenyu.top/gtqxgzaplz.html

Py:   if not s:
来源：http://hz.hammf.cn/gtdktmmlpl.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.fengsongda.top/gtktokwbbb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.gaohongyu789.top/gtuqrrqttn.html

TS:   if (s === "") {}
来源：http://hz.jinghuilouyu.cn/gteafcywvt.html

Java: if (s.isEmpty()) {}
来源：http://hz.52xcode.cn/gtsmonjzlq.html

Go:   if s == "" {}
来源：http://hz.kuanghao11.cn/gtchcnqfmh.html

Ruby: if s.empty?
来源：http://hz.tian-w.cn/gtaxlpgesd.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.ywan-chungtsiang.top/gtthebuyxt.html

[E21] 超长截断加省略号
来源：http://hz.hywenlv.cn/gtrlhgbnxm.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.0kj1m.cn/gtqphafwmi.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.xylfe.cn/gtflrprfgz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.gzhubu.top/gtcpzgfqzf.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jinqigufen.top/gtdaeckwqd.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.iojbl.cn/gtvpgvopsa.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.birdmap.top/gtcgsurxqa.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.iojbl.cn/gtvumnouyj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.hywenlv.cn/gtkcdnotcb.html

[E22] 字节长度与字符长度
来源：http://hz.ywan-chungtsiang.top/gtwttidjrn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.yongpay.top/gtxaqsrsqz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yj202588.top/gtegpmcvae.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.vqdsnc.cn/gtatqebnnz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.sufxvd.cn/gthneksyhc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.yuxming.cn/gteqkcfxfq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.gotoacloud.top/gtsbapzfpf.html

Ruby: s.bytesize;  s.length
来源：http://hz.yvedp.cn/gtfjudmzwa.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.havefunace.top/gtdapnbhrj.html

================================================================================
来源：http://hz.snrcjt.cn/gtryiscrlr.html

F. 文件与目录
来源：http://hz.quarkkingdee.top/gthpihkxzc.html

================================================================================
来源：http://hz.cashguo.top/gtwtqfnmaf.html

[F01] 读取整个文件
来源：http://hz.nanxinkj.top/gtusbvsygu.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yj202588.top/gtlyrvkbfd.html

PHP:  file_get_contents("a.txt");
来源：http://hz.52xcode.cn/gtaftgrkdz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.0kj1m.cn/gtgxdhwqfx.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.birdmap.top/gtuzikbydp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.pengpengdd.cyou/gtzvfylfhi.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.hammf.cn/gtepcixcdd.html

Ruby: File.read("a.txt")
来源：http://hz.yj20258888.top/gtfwkqnzou.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.nanxuanxn.top/gtnnprpxhh.html

[F02] 逐行读取文件
来源：http://hz.xziqi.cn/gtyfhhqnwp.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.hammf.cn/gtoovtqfrw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.ydjk.org.cn/gtnsjqmuqc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zycfv.cn/gtemflmwib.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.cheryme.top/gtmgrxfvcl.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.sxryk.cn/gtlrdvvaaq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.cucudq.cn/gtvctnmjcv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.chenlongwang.top/gtktgezuzo.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.316326.xyz/gtxduhvnmb.html

[F03] 写入文件（覆盖）
来源：http://hz.hammf.cn/gtbuljfrbx.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.daria6918.cn/gtjroheukj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.zycfv.cn/gtvklkxcfc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.iojbl.cn/gttzxourja.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.shuidangran.top/gtonukicix.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.chenjidiqi.icu/gtogyzjrsc.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.gogol.net.cn/gtlmnvcygl.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.xinyue.icu/gtndljlpns.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.zycfv.cn/gtukqbwqgz.html

[F04] 追加写入文件
来源：http://hz.shanyushiyangtech.top/gtqlzwexvq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yangfankeji.com/gtgccqnbtg.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.chenzaomai.com/gtnqpzxzyj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zycfv.cn/gtzforjzgn.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.snrcjt.cn/gtcdgjxapz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.sufxvd.cn/gtltssdygc.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.xingfuxueyuan.xyz/gtxwznatmd.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.wangdashe.top/gtgvlnuvqi.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.yonumen.top/gtjpithinu.html

[F05] 判断文件或目录是否存在
来源：http://hz.shanyushiyangkeji.top/gtkgncizix.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.jiagoushi.top/gtdsuplgsp.html

PHP:  file_exists("a.txt");
来源：http://hz.sweek.top/gtccbblbvl.html

JS:   fs.existsSync("a.txt")
来源：http://hz.jianghu66.top/gtejyyjdvi.html

TS:   fs.existsSync("a.txt")
来源：http://hz.ehwqpu.com/gtohhqdaeq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.cdnleiting.top/gtorribcjp.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.yuxming.cn/gtuahggdhw.html

Ruby: File.exist?("a.txt")
来源：http://hz.bjfxy.top/gtgjacwmta.html

C#:   File.Exists("a.txt")
来源：http://hz.ydzc1.top/gthbqbzqdk.html

[F06] 删除文件
来源：http://hz.cashguo.top/gtztnfebin.html

Py:   os.remove("a.txt")
来源：http://hz.aizwys.cn/gthzlqeryo.html

PHP:  unlink("a.txt");
来源：http://hz.wangdashe.top/gtqsyenyjy.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yj20258888.top/gtlbgwbugr.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.zhijiandao.cn/gtmudkktix.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.yvedp.cn/gtlalkpdsp.html

Go:   os.Remove("a.txt")
来源：http://hz.chenzaomai.com/gtqwwrefup.html

Ruby: File.delete("a.txt")
来源：http://hz.yj20258.top/gttwtscobp.html

C#:   File.Delete("a.txt");
来源：http://hz.jiagoushi.top/gthhlixkdr.html

[F07] 创建目录（含多级）
来源：http://hz.jlsjyb.cn/gtjifkhenk.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yj20258888.top/gtekpkwhad.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.yvedp.cn/gtnrfjltqm.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.pycfn.com/gtkwzgyvss.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hysaishi.cn/gtshthfuyi.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.sweek.top/gtxeobwbpi.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.tianlin.xyz/gtzonyewal.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.havefunace.top/gtnfdsnchd.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.vqdsnc.cn/gtpzihuqtx.html

[F08] 遍历目录
来源：http://hz.hfpthk.cn/gtyfcgrwyt.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.ivvv.top/gtuityvnpj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.yvedp.cn/gtmktqmyvl.html

JS:   fs.readdirSync("dir")
来源：http://hz.birdmap.top/gtzzeouxri.html

TS:   fs.readdirSync("dir")
来源：http://hz.gaohongyu789.top/gtxzyklwqn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.xingfuxueyuan.xyz/gtyzfmctoj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.ppjwa.cn/gtyxcrizot.html

Ruby: Dir.children("dir")
来源：http://hz.ehwqpu.com/gtljazanzi.html

C#:   Directory.GetFiles("dir")
来源：http://hz.dashuyun.cn/gtsanbgjdx.html

[F09] 获取文件大小
来源：http://hz.yangfankeji.com/gtilncbweu.html

Py:   os.path.getsize("a.txt")
来源：http://hz.0kj1m.cn/gtpadrbjqe.html

PHP:  filesize("a.txt");
来源：http://hz.hammf.cn/gtumbhpbjv.html

JS:   fs.statSync("a.txt").size
来源：http://hz.cheryme.top/gttzequzpg.html

TS:   fs.statSync("a.txt").size
来源：http://hz.hfpthk.cn/gtozwvnqtg.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.ehwqpu.com/gtmdgssalx.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.sweek.top/gtyhorrnbf.html

Ruby: File.size("a.txt")
来源：http://hz.havefunace.top/gtgttdmolw.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.mhx1999.top/gtwblcnybz.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.ydjk.org.cn/gtncgqxyco.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.c1oappe.top/gtxryhfqrj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.jqgufenzy.top/gtnlxzhgah.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.yvedp.cn/gthjnbdtyc.html

TS:   path.extname("a.txt")
来源：http://hz.yj20258.top/gtvgyvpxag.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.c1oappe.top/gtfexhqlsk.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yj202588.top/gtixhkxlyi.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.redwolf501.top/gtazimrclx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.52xcode.cn/gtpscxhqga.html

[F11] 复制与移动文件
来源：http://hz.chenzaomai.com/gtfhkcbmdj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.birdmap.top/gtnlcdjtbh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.ywan-chungtsiang.top/gtoudjpobf.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.cucudq.cn/gtwkciqjsa.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jianghu66.top/gtoqrqofoo.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.yangfankeji.com/gtqpwfoaoc.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.havefunace.top/gttocrdthg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.vqdsnc.cn/gtiyujafzq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.hnqzz.top/gtolbrhhaf.html

[F12] CSV 读写
来源：http://hz.sufxvd.cn/gtaxjytvkl.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.cheryme.top/gtrxdjpilj.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.0kj1m.cn/gtbjsntzjg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.zhaomingkeji.xyz/gtyxrwzblu.html

TS:   // 同上
来源：http://hz.redwolf501.top/gtgrfblaxf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.tanke756.top/gtnyqwzzva.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.sysykeji.top/gtmyjpxjgm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.xuetiantiany.cn/gtkhwzetnm.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.zhaomingkeji.xyz/gtjsjsnaqc.html

================================================================================
来源：http://hz.quarkkingdee.top/gtfxkfpxax.html

G. 面向对象
来源：http://hz.shanyushiyangtech.top/gtgzfsurjw.html

================================================================================
来源：http://hz.fengsongda.top/gtymhwnuhr.html

[G01] 定义类
来源：http://hz.zhengqikj.top/gtndlikmbt.html

Py:   class User: pass
来源：http://hz.shangyingyoupin.top/gtqepoefgl.html

PHP:  class User {}
来源：http://hz.wangshuangyany.cn/gtazpijmvf.html

JS:   class User {}
来源：http://hz.guowangkeji.top/gtszwdksdq.html

TS:   class User { name: string = ""; }
来源：http://hz.xingfuxueyuan.xyz/gtcmgqyvtj.html

Java: class User {}
来源：http://hz.xziqi.cn/gtkjvgiwii.html

Go:   type User struct { Name string }
来源：http://hz.aibaodan.cn/gtymuhsqtl.html

Ruby: class User; end
来源：http://hz.jinqigufen.top/gtgnnvnelb.html

C#:   class User {}
来源：http://hz.shzxlz.cn/gttcotgxit.html

[G02] 构造函数
来源：http://hz.havefunace.top/gtremwnibq.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.jinghuilouyu.cn/gtcivdbakc.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.hnqzz.top/gtdidovozp.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.xuetiantiany.cn/gtbfbqgmzt.html

TS:   constructor(public name: string) {}
来源：http://hz.ydjk.org.cn/gtuqhqracu.html

Java: User(String name) { this.name = name; }
来源：http://hz.daxiang520.top/gtngbrniiv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.xziqi.cn/gtpwgeclyu.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.jlsjyb.cn/gtsqsdmluw.html

C#:   public User(string name) { Name = name; }
来源：http://hz.hnqzz.top/gtfcrgbwbu.html

[G03] 实例属性
来源：http://hz.birdmap.top/gtdalolasw.html

Py:   self.name = "x"
来源：http://hz.xziqi.cn/gtyfkqnkmg.html

PHP:  public string $name = "x";
来源：http://hz.xylfe.cn/gtkquunobr.html

JS:   this.name = "x";
来源：http://hz.shangyingyoupin.top/gtcupggvgq.html

TS:   name: string = "x";
来源：http://hz.fengsongda.top/gtcoqlalxi.html

Java: private String name;
来源：http://hz.shanyushiyangkeji.top/gtennqpnez.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.cdnleiting.top/gtnzsfqdph.html

Ruby: @name = "x"
来源：http://hz.hysaishi.cn/gtkynmwyho.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.shanyushiyangkeji.top/gtbpqyrxlh.html

[G04] 定义方法
来源：http://hz.cashguo.top/gtwzkkluie.html

Py:   def greet(self): return self.name
来源：http://hz.snrcjt.cn/gtogvrgika.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.zycfv.cn/gtkgbufqfe.html

JS:   greet() { return this.name; }
来源：http://hz.hnxiangtu.top/gticexamwo.html

TS:   greet(): string { return this.name; }
来源：http://hz.shanyushiyangtech.top/gtkakziavl.html

Java: String greet() { return name; }
来源：http://hz.gzhubu.top/gtzzxeofur.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.ehwqpu.com/gtupgxypba.html

Ruby: def greet; @name; end
来源：http://hz.ppjwa.cn/gtzrtfcagi.html

C#:   public string Greet() => Name;
来源：http://hz.shanyushiyangtech.top/gthfeixvyn.html

[G05] 继承
来源：http://hz.cheryme.top/gtbrmalxrc.html

Py:   class Admin(User): pass
来源：http://hz.jinyuanbaomall.cn/gtzcyhvezg.html

PHP:  class Admin extends User {}
来源：http://hz.nwbrower.top/gtfzopsnxe.html

JS:   class Admin extends User {}
来源：http://hz.aizwys.cn/gttjyywglg.html

TS:   class Admin extends User {}
来源：http://hz.9152youxi.cn/gtznqsmesa.html

Java: class Admin extends User {}
来源：http://hz.feifeiyinyue.top/gtlcgjkjyu.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.jyoumei.cn/gtnxkxjvze.html

Ruby: class Admin < User; end
来源：http://hz.fengsongda.top/gtqfhqihln.html

C#:   class Admin : User {}
来源：http://hz.316326.xyz/gtkwqalpmb.html

[G06] 重写方法
来源：http://hz.tianlin.xyz/gtmjytehwk.html

Py:   def greet(self): return "admin"
来源：http://hz.zycfv.cn/gtdmwemhta.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.yanxiufei.cn/gtrrrrqynp.html

JS:   greet() { return "admin"; }
来源：http://hz.shanyushiyangtech.top/gtfqccsmgh.html

TS:   greet(): string { return "admin"; }
来源：http://hz.yvedp.cn/gtlmgnxner.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.gogol.net.cn/gtaheutlzl.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zdqjudy.top/gtkhdhfniz.html

Ruby: def greet; "admin"; end
来源：http://hz.jlsjyb.cn/gtirmjcdox.html

C#:   public override string Greet() => "admin";
来源：http://hz.pengpengdd.cyou/gtbjrkdpaq.html

[G07] 调用父类方法
来源：http://hz.fengsongda.top/gtykkubnbs.html

Py:   super().greet()
来源：http://hz.jinqigfzy.top/gtswvwtbwl.html

PHP:  parent::greet();
来源：http://hz.ppjwa.cn/gtjcbibcsp.html

JS:   super.greet();
来源：http://hz.zhoulong.xyz/gtnvaealkx.html

TS:   super.greet();
来源：http://hz.zhongyouzk.top/gtacxuwrnm.html

Java: super.greet();
来源：http://hz.hnqzz.top/gtspwkkpha.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.zhiwuduotai.top/gtmaqgozdu.html

Ruby: super
来源：http://hz.yangfankeji.com/gttchnbxhr.html

C#:   base.Greet();
来源：http://hz.iojbl.cn/gtlrvwtuef.html

[G08] 静态方法与属性
来源：http://hz.xuetiantiany.cn/gtujkrdbim.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jinghuilouyu.cn/gtolbdpkig.html

PHP:  public static function f() {}
来源：http://hz.xziqi.cn/gtoacvqvcr.html

JS:   static f() {}
来源：http://hz.smart0.xyz/gtfbcjevxw.html

TS:   static f(): void {}
来源：http://hz.fengsongda.top/gtmesqpyjt.html

Java: static void f() {}
来源：http://hz.yj20258888.top/gtocdntlks.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.hnxiangtu.top/gtarnrezpz.html

Ruby: def self.f; end
来源：http://hz.jiagoushi.top/gtwxrhfcdn.html

C#:   public static void F() {}
来源：http://hz.dashuyun.cn/gttpcrifje.html

[G09] 接口 / 抽象类
来源：http://hz.zhongyouzk.top/gtzjqdyybi.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.dianchejie.cn/gtcaqhvexz.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.c1oappe.top/gtgzphkbzq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.jinyuanbaomall.cn/gtspexufre.html

TS:   interface Shape { area(): number; }
来源：http://hz.aizwys.cn/gtshttjeoh.html

Java: interface Shape { double area(); }
来源：http://hz.xziqi.cn/gthtwmrxwr.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.jianghu66.top/gtxdqqwqtp.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jinghuilouyu.cn/gtqrmgjpyl.html

C#:   interface IShape { double Area(); }
来源：http://hz.xylfe.cn/gttwyyinpl.html

[G10] 访问控制
来源：http://hz.ydjk.org.cn/gtxtzpqcws.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.guannengcc.top/gtbqzvxypy.html

PHP:  public / protected / private
来源：http://hz.wangdashe.top/gtpmtwpsof.html

JS:   #private 字段；其余公开
来源：http://hz.birdmap.top/gtksyrtgro.html

TS:   public / protected / private
来源：http://hz.wangdashe.top/gtivzhzers.html

Java: public / protected / private / 默认包级
来源：http://hz.snrcjt.cn/gtshxobbqt.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.sufxvd.cn/gtoexlrrbu.html

Ruby: public / protected / private
来源：http://hz.yuxming.cn/gtbtxwuatz.html

C#:   public / protected / private / internal
来源：http://hz.shangyingyoupin.top/gtdlwgkmcw.html

[G11] getter / setter
来源：http://hz.ydzc1.top/gtluwsmree.html

Py:   @property 与 @x.setter
来源：http://hz.gogol.net.cn/gttpuhqvlc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jinqigfzy.top/gtrsabpbqd.html

JS:   get name() { return this._name; }
来源：http://hz.yvedp.cn/gtnllljzst.html

TS:   get name(): string { return this._name; }
来源：http://hz.hnxiangtu.top/gtkpzconke.html

Java: public String getName() { return name; }
来源：http://hz.meibo888.top/gtgcnrxkpl.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.cucudq.cn/gtdiaqehkq.html

Ruby: attr_accessor :name
来源：http://hz.sweek.top/gtupspreel.html

C#:   public string Name { get; set; }
来源：http://hz.vqdsnc.cn/gtmdhgtpwb.html

[G12] 对象转字符串
来源：http://hz.hysaishi.cn/gtfjwylaxt.html

Py:   def __str__(self): return self.name
来源：http://hz.hnxiangtu.top/gtmgemtwyp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.andypj.xyz/gthzllmhlo.html

JS:   toString() { return this.name; }
来源：http://hz.shzxlz.cn/gtzwtlzwih.html

TS:   toString(): string { return this.name; }
来源：http://hz.0kj1m.cn/gtprhiwgnf.html

Java: @Override public String toString() { return name; }
来源：http://hz.jinqigfzy.top/gthxzaqlud.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.svipenyu.cn/gtnjpxjrga.html

Ruby: def to_s; @name; end
来源：http://hz.dianchejie.cn/gteljspxhz.html

C#:   public override string ToString() => Name;
来源：http://hz.jinghuilouyu.cn/gtvqsvzbrz.html

[G13] 判断对象类型
来源：http://hz.jinghuilouyu.cn/gtbhzuqbnl.html


<!-- 参考信息 -->