代发 wailian999

[E14] URL 编码与 Base64
来源：http://hz.redwolf501.top/gtxncmbctb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.aibaodan.cn/gthowqnlfn.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.dianchejie.cn/gtkgyjbxru.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.jinghuilouyu.cn/gtfmaxqqny.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.gogol.net.cn/gthbvqdtwm.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.jinghuilouyu.cn/gtzhffqldw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.yuanzhike.top/gtpctcffpq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.jyoumei.cn/gtmespvbcn.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.xziqi.cn/gtsstrjgju.html

[E15] HTML 转义 / 反转义
来源：http://hz.feifeiyinyue.top/gtdmfdlkbb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.aibaodan.cn/gtoseitpsz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.feifeiyinyue.top/gtsvebzhgp.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.52xcode.cn/gtcvbbayer.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.yj20258888.top/gtbrwsnite.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.ybcxt.top/gtsqlivggl.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.mhx1999.top/gterydkeka.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.vqdsnc.cn/gtzafqoldb.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.yvedp.cn/gtoyrbqzao.html

[E16] 数字千分位
来源：http://hz.haohaochexian.top/gtjhhgaxxy.html

Py:   f"{1234567:,}"
来源：http://hz.yuanzhike.top/gtcttqjmsl.html

PHP:  number_format(1234567);
来源：http://hz.fengsongda.top/gtdyeqhrgd.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.xuetiantiany.cn/gtidfvklrc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.yj202588.top/gtevtgrbfn.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.birdmap.top/gtwtcfkume.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.hfpthk.cn/gtayyzjmks.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.52xcode.cn/gtiawziwjz.html

C#:   1234567.ToString("N0")
来源：http://hz.9152youxi.cn/gtkwawqagu.html

[E17] 首字母大写
来源：http://hz.daria6918.cn/gtefjuhkty.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.snrcjt.cn/gteqdeenzb.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.yueranfly.top/gtsobzpajl.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.aizwys.cn/gtbpwknwge.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.tianlin.xyz/gtukhlkxof.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.cdnleiting.top/gtlggcyhtv.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.jqgfzy.top/gtvzltfhcr.html

Ruby: s.capitalize
来源：http://hz.cqqwz.cn/gtvyliodmk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yangfankeji.com/gtcsiofkre.html

[E18] 模板占位符替换
来源：http://hz.hysaishi.cn/gtsytboyze.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.xuetiantiany.cn/gtzpsdndie.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.daria6918.cn/gtwdzqxehc.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.0kj1m.cn/gtqwftbder.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.snrcjt.cn/gtzbtyhqiv.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.ydzc1.top/gtgcvtixrp.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.guannengcc.top/gtmdbclddo.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.sweek.top/gtnqhflttq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.ppjwa.cn/gtkpptkgxf.html

[E19] 多行文本按行拆分
来源：http://hz.feifeiyinyue.top/gtlrrmmvpy.html

Py:   s.splitlines()
来源：http://hz.tianlin.xyz/gtzyzzoufy.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.hfpthk.cn/gtlmtacncg.html

JS:   s.split(/\r?\n/)
来源：http://hz.xingfuxueyuan.xyz/gtdxazmzrt.html

TS:   s.split(/\r?\n/)
来源：http://hz.ehwqpu.com/gtukbblxpc.html

Java: s.lines().toList()
来源：http://hz.hongshengwenyu.top/gtlxlbwwiv.html

Go:   strings.Split(s, "\n")
来源：http://hz.nanxinkj.top/gtelvnvrjo.html

Ruby: s.lines
来源：http://hz.vqdsnc.cn/gtujfsigcw.html

C#:   s.Split('\n')
来源：http://hz.havefunace.top/gticabtfej.html

[E20] 判断字符串是否为空
来源：http://hz.hnxiangtu.top/gthdqlvboe.html

Py:   if not s:
来源：http://hz.yangfankeji.com/gtgpofkfcf.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.feifeiyinyue.top/gtwduuypob.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.haohaochexian.top/gtflvhbcxe.html

TS:   if (s === "") {}
来源：http://hz.yj20258888.top/gtsoeifgww.html

Java: if (s.isEmpty()) {}
来源：http://hz.nwbrower.top/gtwtqjocom.html

Go:   if s == "" {}
来源：http://hz.pengpengdd.cyou/gtdabfiqml.html

Ruby: if s.empty?
来源：http://hz.sxryk.cn/gtlysjanim.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.redwolf501.top/gtnmxbambm.html

[E21] 超长截断加省略号
来源：http://hz.nanxinkj.top/gtzdbknneu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.hysaishi.cn/gtyxdkhnul.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.fengsongda.top/gtmfjlekrs.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.hnqzz.top/gthzbktrem.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.mhx1999.top/gtsjfmmvtm.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.wangshuangyany.cn/gtiqwviqzf.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.cheryme.top/gtasvtzmab.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.xylfe.cn/gtgnaixqxs.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.redwolf501.top/gtqukwgswv.html

[E22] 字节长度与字符长度
来源：http://hz.shanyushiyangtech.top/gttilsxzsl.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.hfpthk.cn/gthzlpmpdd.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.cqqwz.cn/gthjdukdox.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.cqqwz.cn/gtpkivacvu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ydzc1.top/gtrneaiiku.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.pycfn.com/gtmpxahxkv.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.yj20258888.top/gttxhccrcz.html

Ruby: s.bytesize;  s.length
来源：http://hz.yongpay.top/gtwfdrhmvs.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.nanxinkj.top/gtybawxpai.html

================================================================================
来源：http://hz.zhixingplan.top/gtzkzyfxky.html

F. 文件与目录
来源：http://hz.shzxlz.cn/gtuzhpcdsb.html

================================================================================
来源：http://hz.cucudq.cn/gtrajwrumw.html

[F01] 读取整个文件
来源：http://hz.meibo888.top/gthqycuoyl.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.c1oappe.top/gtiftosfxx.html

PHP:  file_get_contents("a.txt");
来源：http://hz.haohaochexian.top/gtmjqolfyr.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.tianlin.xyz/gtxoeuilpn.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.gzhubu.top/gtlubaatoa.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.yangfankeji.com/gtriddsqdp.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.hywenlv.cn/gtdhgbawso.html

Ruby: File.read("a.txt")
来源：http://hz.chenzaomai.com/gtjyybuoak.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.gaohongyu789.top/gtnmdahuux.html

[F02] 逐行读取文件
来源：http://hz.gzhubu.top/gtnwbniqzg.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.yj202588.top/gtrkwwuuys.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.birdmap.top/gtpfutnwti.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.c1oappe.top/gtunelrnlj.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hnqzz.top/gtofjpdgwe.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.jiagoushi.top/gtuxbsbkxa.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.xuanzx.com/gtweibhhbk.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.zhaomingkeji.xyz/gtxuaxusbs.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.9152youxi.cn/gtqypwgcqk.html

[F03] 写入文件（覆盖）
来源：http://hz.yonumen.top/gtspoutnat.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.yvedp.cn/gtakjwivwj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.jinyuanbaomall.cn/gtoooqfkkz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.tianlin.xyz/gtarmtdahd.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.snrcjt.cn/gtlpifbfhw.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.shzxlz.cn/gtfwjvfumt.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.zhixingplan.top/gtkngyfnnq.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.zhongyouzk.top/gtbchtxazm.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.pengpengdd.cyou/gtatxadicr.html

[F04] 追加写入文件
来源：http://hz.zhixingplan.top/gtaxshfsmf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.dashuyun.cn/gtetptdzcx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.jqgfzy.top/gtyznuleto.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.cdnleiting.top/gtclbmvvau.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.cheryme.top/gtstziaysi.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.nanxuanxn.top/gtcsgmvugi.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.andypj.xyz/gtfsulubtz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.meibo888.top/gtikeayvrd.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.jiagoushi.top/gtfpsflgnb.html

[F05] 判断文件或目录是否存在
来源：http://hz.yueranfly.top/gtaxmrzqnz.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.tian-w.cn/gtdznacwid.html

PHP:  file_exists("a.txt");
来源：http://hz.zhongyouzk.top/gthzehfekw.html

JS:   fs.existsSync("a.txt")
来源：http://hz.guannengcc.top/gtqxewollx.html

TS:   fs.existsSync("a.txt")
来源：http://hz.jinqigufen.top/gtolxlhuzn.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.nanxuanxn.top/gtnfwmlrin.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.iojbl.cn/gtdegxzrzl.html

Ruby: File.exist?("a.txt")
来源：http://hz.ydjk.org.cn/gtoqplfxxt.html

C#:   File.Exists("a.txt")
来源：http://hz.nanxuanxn.top/gtqlnimeml.html

[F06] 删除文件
来源：http://hz.hongshengwenyu.top/gtimhcqqrx.html

Py:   os.remove("a.txt")
来源：http://hz.aibaodan.cn/gteehtyqfc.html

PHP:  unlink("a.txt");
来源：http://hz.andypj.xyz/gtaijzubdz.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.zhoulong.xyz/gtgtuoupth.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.ivvv.top/gtwipvegfa.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.andypj.xyz/gtaprnyeoj.html

Go:   os.Remove("a.txt")
来源：http://hz.chenjidiqi.icu/gtqvbjxnpa.html

Ruby: File.delete("a.txt")
来源：http://hz.jinghuilouyu.cn/gtxozryuol.html

C#:   File.Delete("a.txt");
来源：http://hz.hammf.cn/gtlatsaoye.html

[F07] 创建目录（含多级）
来源：http://hz.zycfv.cn/gtkfnzbnyd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.sweek.top/gtafglkctx.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.dashuyun.cn/gteldhyvkv.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hfpthk.cn/gtlgqhvuim.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.xingfuxueyuan.xyz/gtawjlgenr.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.yongpay.top/gtfhfdcisn.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.hfpthk.cn/gtcliylmgd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.zdqjudy.top/gtskjafeuw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.wangdashe.top/gtkyyyamvb.html

[F08] 遍历目录
来源：http://hz.cashguo.top/gtzxverswq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.jinghuilouyu.cn/gtdjzflzfr.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.shzxlz.cn/gtgxnzsicj.html

JS:   fs.readdirSync("dir")
来源：http://hz.gzhubu.top/gtpodgvfvf.html

TS:   fs.readdirSync("dir")
来源：http://hz.pycfn.com/gtajwicjso.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.ydzc1.top/gtiiuydbop.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yj20258888.top/gtproytkob.html

Ruby: Dir.children("dir")
来源：http://hz.nanxinkj.top/gtmctdukhs.html

C#:   Directory.GetFiles("dir")
来源：http://hz.aibaodan.cn/gtiiqkfoio.html

[F09] 获取文件大小
来源：http://hz.gotoacloud.top/gtddbjxfwp.html

Py:   os.path.getsize("a.txt")
来源：http://hz.hywenlv.cn/gtukgafhia.html

PHP:  filesize("a.txt");
来源：http://hz.hammf.cn/gtnxplewwb.html

JS:   fs.statSync("a.txt").size
来源：http://hz.yj20258.top/gtawqjnxld.html

TS:   fs.statSync("a.txt").size
来源：http://hz.ehwqpu.com/gtrqeyobkk.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.shzxlz.cn/gtrfpaodvq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.quarkkingdee.top/gtdyilyzxn.html

Ruby: File.size("a.txt")
来源：http://hz.hammf.cn/gtdwvgvodc.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.jinqigufen.top/gtndxqrrwb.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.ydzc1.top/gtvmeidmwb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.yongpay.top/gtjcfmzjec.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.ehwqpu.com/gttzwynfyx.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.jqgufenzy.top/gtfthislai.html

TS:   path.extname("a.txt")
来源：http://hz.shangyingyoupin.top/gtxyodrctu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.zhiwuduotai.top/gteyxsahcw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yj20258888.top/gtqahbqtng.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.gaohongyu789.top/gtequdsfhg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.svipenyu.cn/gtoplkkgbw.html

[F11] 复制与移动文件
来源：http://hz.yanxiufei.cn/gtdhlhqnol.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.yonumen.top/gtoupgzisu.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.ybcxt.top/gtuefqkjld.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.aizwys.cn/gtvypuzftp.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jinqigufen.top/gtkrisplte.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.zhongyouzk.top/gtiqoatyse.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.hnxiangtu.top/gteltxotwy.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.tian-w.cn/gtiepbpzcq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.wangdashe.top/gtayhfzdsz.html

[F12] CSV 读写
来源：http://hz.gaohongyu789.top/gtkfvyfmzi.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.yj20258888.top/gtgsxrivzn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.birdmap.top/gtlglwrkxm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.jiagoushi.top/gtyowqqyhr.html

TS:   // 同上
来源：http://hz.gzhubu.top/gtjjsmnayw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.yj20258.top/gtgnolvlon.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.chenzaomai.com/gthxhqcygm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.zhengqikj.top/gtfhzukwwp.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.guannengcc.top/gtdbytgnkn.html

================================================================================
来源：http://hz.kuanghao11.cn/gtwuuuwwuj.html

G. 面向对象
来源：http://hz.fzhhl.top/gthdbpnwyx.html

================================================================================
来源：http://hz.cdnleiting.top/gtfisszosj.html

[G01] 定义类
来源：http://hz.hfpthk.cn/gtbirdbwbs.html

Py:   class User: pass
来源：http://hz.ydzc1.top/gtwoznmjha.html

PHP:  class User {}
来源：http://hz.zycfv.cn/gtcnflsgsp.html

JS:   class User {}
来源：http://hz.shangyingyoupin.top/gtgdardzbt.html

TS:   class User { name: string = ""; }
来源：http://hz.ehwqpu.com/gtdzcgglff.html

Java: class User {}
来源：http://hz.tianlin.xyz/gtrvkxcmwy.html

Go:   type User struct { Name string }
来源：http://hz.yj20258888.top/gtkeyjvpso.html

Ruby: class User; end
来源：http://hz.yuanzhike.top/gtzyzpkjuv.html

C#:   class User {}
来源：http://hz.yuxming.cn/gtailbnbgt.html

[G02] 构造函数
来源：http://hz.ybcxt.top/gtsjakjhff.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.cashguo.top/gthlkxppev.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.hnqzz.top/gtuwjlfelo.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.zdqjudy.top/gtzcaqvckx.html

TS:   constructor(public name: string) {}
来源：http://hz.gogol.net.cn/gtqywloaip.html

Java: User(String name) { this.name = name; }
来源：http://hz.hnxiangtu.top/gtlmsivbhn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.bjfxy.top/gtvesfytkm.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.pycfn.com/gthqpetuwc.html

C#:   public User(string name) { Name = name; }
来源：http://hz.guannengcc.top/gtamiqmnhe.html

[G03] 实例属性
来源：http://hz.gaohongyu789.top/gtvbnnjwoa.html

Py:   self.name = "x"
来源：http://hz.tian-w.cn/gtvlygcizp.html

PHP:  public string $name = "x";
来源：http://hz.dashuyun.cn/gtykldbwhl.html

JS:   this.name = "x";
来源：http://hz.9152youxi.cn/gtlnzinkrc.html

TS:   name: string = "x";
来源：http://hz.cqqwz.cn/gttlkxiepb.html

Java: private String name;
来源：http://hz.sufxvd.cn/gtnalfurmz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.fzhhl.top/gtpgbmaplx.html

Ruby: @name = "x"
来源：http://hz.zycfv.cn/gtahfddsxz.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.tianlin.xyz/gtlezjoafw.html

[G04] 定义方法
来源：http://hz.yongpay.top/gtscodlhcy.html

Py:   def greet(self): return self.name
来源：http://hz.dianchejie.cn/gtydefwkvo.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.ydjk.org.cn/gtxzcqngzg.html

JS:   greet() { return this.name; }
来源：http://hz.daria6918.cn/gtlbevftbd.html

TS:   greet(): string { return this.name; }
来源：http://hz.jiagoushi.top/gtyhklttxv.html

Java: String greet() { return name; }
来源：http://hz.havefunace.top/gtzdlonncg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.yongpay.top/gtkptinpcf.html

Ruby: def greet; @name; end
来源：http://hz.tian-w.cn/gtgckalsqs.html

C#:   public string Greet() => Name;
来源：http://hz.yj202588.top/gtncomxxtx.html

[G05] 继承
来源：http://hz.316326.xyz/gtowilkeek.html

Py:   class Admin(User): pass
来源：http://hz.feifeiyinyue.top/gtdcqpwyxg.html

PHP:  class Admin extends User {}
来源：http://hz.havefunace.top/gtrdxgbsbo.html

JS:   class Admin extends User {}
来源：http://hz.aizwys.cn/gtoqkrahqy.html

TS:   class Admin extends User {}
来源：http://hz.smart0.xyz/gtssrukbla.html

Java: class Admin extends User {}
来源：http://hz.meibo888.top/gtoszjddgo.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.9152youxi.cn/gtsgualusq.html

Ruby: class Admin < User; end
来源：http://hz.hysaishi.cn/gtandpnudk.html

C#:   class Admin : User {}
来源：http://hz.yuxming.cn/gtfgdkqkav.html

[G06] 重写方法
来源：http://hz.tanke756.top/gtpkyysytx.html

Py:   def greet(self): return "admin"
来源：http://hz.xziqi.cn/gtucszdmre.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.sysykeji.top/gtuhlizvtg.html

JS:   greet() { return "admin"; }
来源：http://hz.xinyue.icu/gtzlzlegia.html

TS:   greet(): string { return "admin"; }
来源：http://hz.gaohongyu789.top/gtejkzzaux.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jianghu66.top/gteiegltsd.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.andypj.xyz/gtqajlbppl.html

Ruby: def greet; "admin"; end
来源：http://hz.zhixingplan.top/gtvkcyuphz.html

C#:   public override string Greet() => "admin";
来源：http://hz.jinqigufen.top/gtcjhjyynd.html

[G07] 调用父类方法
来源：http://hz.yj202588.top/gtkqvjxjdj.html

Py:   super().greet()
来源：http://hz.svipenyu.cn/gtxxuizedl.html

PHP:  parent::greet();
来源：http://hz.ydjk.org.cn/gtycjhatnj.html

JS:   super.greet();
来源：http://hz.shanyushiyangkeji.top/gtswszuafl.html

TS:   super.greet();
来源：http://hz.yuxming.cn/gtsqvvthyj.html

Java: super.greet();
来源：http://hz.zdqjudy.top/gtlfcxokon.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jinghuilouyu.cn/gtqtwacgkf.html

Ruby: super
来源：http://hz.hongshengwenyu.top/gtxmujtqsj.html

C#:   base.Greet();
来源：http://hz.zhaomingkeji.xyz/gtdjpkfuzh.html

[G08] 静态方法与属性
来源：http://hz.quarkkingdee.top/gtudhwspam.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.ehwqpu.com/gteaqunbjm.html

PHP:  public static function f() {}
来源：http://hz.hongshengwenyu.top/gtquxlxqjc.html

JS:   static f() {}
来源：http://hz.bjfxy.top/gtjjnevkkr.html

TS:   static f(): void {}
来源：http://hz.0kj1m.cn/gtxsmkfkcs.html

Java: static void f() {}
来源：http://hz.316326.xyz/gtketpffav.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.daxiang520.top/gteqnmbbuz.html

Ruby: def self.f; end
来源：http://hz.yj20258.top/gtaeriprxw.html

C#:   public static void F() {}
来源：http://hz.iojbl.cn/gtnqmwwaxd.html

[G09] 接口 / 抽象类
来源：http://hz.jinqigfzy.top/gtsxabvvsm.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.jinqigufen.top/gthsychquo.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.vqdsnc.cn/gtvfajmupu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.hysaishi.cn/gtyandkesb.html

TS:   interface Shape { area(): number; }
来源：http://hz.sysykeji.top/gtsrekebyh.html

Java: interface Shape { double area(); }
来源：http://hz.yongpay.top/gtvnnsleul.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.jyoumei.cn/gtivgsnqno.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.cashguo.top/gtpfebpjlj.html

C#:   interface IShape { double Area(); }
来源：http://hz.nwbrower.top/gtdqkvqcux.html

[G10] 访问控制
来源：http://hz.chenzaomai.com/gtcltxsgnb.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.ywan-chungtsiang.top/gtwngrsqot.html

PHP:  public / protected / private
来源：http://hz.zhongyouzk.top/gtvodtufiy.html

JS:   #private 字段；其余公开
来源：http://hz.dashuyun.cn/gtfgnfvegf.html

TS:   public / protected / private
来源：http://hz.haohaochexian.top/gtzymapqzw.html

Java: public / protected / private / 默认包级
来源：http://hz.ivvv.top/gtlrrcmtjv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zhengqikj.top/gtilawtrqu.html

Ruby: public / protected / private
来源：http://hz.xylfe.cn/gtxkchfuzs.html

C#:   public / protected / private / internal
来源：http://hz.jinqigufen.top/gtjhbbzdir.html

[G11] getter / setter
来源：http://hz.vqdsnc.cn/gtpidvivzg.html

Py:   @property 与 @x.setter
来源：http://hz.sufxvd.cn/gtnljyvgwy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.zdqjudy.top/gtlpcimjbl.html

JS:   get name() { return this._name; }
来源：http://hz.yj20258888.top/gtnzgcwxud.html

TS:   get name(): string { return this._name; }
来源：http://hz.zdqjudy.top/gtzumfikai.html

Java: public String getName() { return name; }
来源：http://hz.xinyue.icu/gtifkyyudb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.jinqigfzy.top/gtdteursvf.html

Ruby: attr_accessor :name
来源：http://hz.aizwys.cn/gtzkhgveho.html

C#:   public string Name { get; set; }
来源：http://hz.feifeiyinyue.top/gtnxnhvrhg.html

[G12] 对象转字符串
来源：http://hz.iojbl.cn/gtxxlomibd.html

Py:   def __str__(self): return self.name
来源：http://hz.yuanzhike.top/gtbfliflmc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.svipenyu.cn/gtqqklpssg.html

JS:   toString() { return this.name; }
来源：http://hz.hongshengwenyu.top/gtlxdvkesg.html

TS:   toString(): string { return this.name; }
来源：http://hz.aizwys.cn/gtxpzdjubx.html

Java: @Override public String toString() { return name; }
来源：http://hz.gotoacloud.top/gtczlayqgp.html


<!-- 参考信息 -->