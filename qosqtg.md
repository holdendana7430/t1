代发 wailian999

Py:   for ch in s: print(ch)
来源：http://hz.smart0.xyz/gtnagitlrc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.sxryk.cn/gtjgewlboa.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jinyuanbaomall.cn/gtwowibfmb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.hfpthk.cn/gtwxciruaa.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.52xcode.cn/gtjnyudowo.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.yanxiufei.cn/gtsfarfukq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.52xcode.cn/gticljdzqd.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.shanyushiyangtech.top/gtuzizlddf.html

[E14] URL 编码与 Base64
来源：http://hz.zdqjudy.top/gtzqgwnhlj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.havefunace.top/gtiyghsnyb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.yuanzhike.top/gtbdelvqyn.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.guannengcc.top/gtkmkthbbp.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.shuidangran.top/gtkkedhikh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.yj202588.top/gtjzunqruw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.jiagoushi.top/gtobwrecfn.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.shangyingyoupin.top/gtorskehde.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.shanyushiyangtech.top/gtjojscrrz.html

[E15] HTML 转义 / 反转义
来源：http://hz.shanyushiyangtech.top/gtgtrbkeuq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.nanxinkj.top/gtbvwqjwji.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.cucudq.cn/gtgigplodz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.redwolf501.top/gtmzygsiuo.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.cashguo.top/gtxxuhzluu.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.hongshengwenyu.top/gtxlcbbgtv.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.0kj1m.cn/gtbqlbgebt.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.kuanghao11.cn/gteycjhxoa.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.ydzc1.top/gtaqmkjwua.html

[E16] 数字千分位
来源：http://hz.0kj1m.cn/gtmfcwipkq.html

Py:   f"{1234567:,}"
来源：http://hz.xinyue.icu/gtmxigkrtt.html

PHP:  number_format(1234567);
来源：http://hz.ehwqpu.com/gtxyzeglvm.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhongyouzk.top/gtfqvetccz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.chenlongwang.top/gtfdnhujri.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.smart0.xyz/gtovlietib.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.hfpthk.cn/gtzaatbtlq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.hfpthk.cn/gtzssuneqq.html

C#:   1234567.ToString("N0")
来源：http://hz.kuanghao11.cn/gtjkaccrac.html

[E17] 首字母大写
来源：http://hz.mhx1999.top/gtbbzmtjsy.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.hfpthk.cn/gtwdflcreb.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.cqqwz.cn/gtsxkypgrf.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.sweek.top/gtzbejtlwb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jqgfzy.top/gtciuvewkd.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.gogol.net.cn/gtusxahlql.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.9152youxi.cn/gtheuuioqr.html

Ruby: s.capitalize
来源：http://hz.0kj1m.cn/gtpogcirdf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.pycfn.com/gtfhuoxwxr.html

[E18] 模板占位符替换
来源：http://hz.zhongyouzk.top/gtvgvzyzwn.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.shangyingyoupin.top/gtilpnncuw.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.yj20258888.top/gtqieqblkm.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.sysykeji.top/gtxtoxflit.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.hywenlv.cn/gtrqogcczv.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.yangfankeji.com/gtlsgrgwth.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.yueranfly.top/gtynqfguvd.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.zhaomingkeji.xyz/gtohksjimb.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.zdqjudy.top/gtxpoeqnoq.html

[E19] 多行文本按行拆分
来源：http://hz.zhaomingkeji.xyz/gtzinovqnp.html

Py:   s.splitlines()
来源：http://hz.yueranfly.top/gtghqolvjh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.aibaodan.cn/gtsairfxth.html

JS:   s.split(/\r?\n/)
来源：http://hz.jinyuanbaomall.cn/gtrenklmvl.html

TS:   s.split(/\r?\n/)
来源：http://hz.yuanzhike.top/gtafeulcxl.html

Java: s.lines().toList()
来源：http://hz.jinghuilouyu.cn/gtuvkvvetd.html

Go:   strings.Split(s, "\n")
来源：http://hz.pengpengdd.cyou/gtrpdrwuuz.html

Ruby: s.lines
来源：http://hz.0kj1m.cn/gtfemchtux.html

C#:   s.Split('\n')
来源：http://hz.ehwqpu.com/gtwipktkid.html

[E20] 判断字符串是否为空
来源：http://hz.jinghuilouyu.cn/gtxrdndpnr.html

Py:   if not s:
来源：http://hz.zhengqikj.top/gtxvqryuug.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.zhijiandao.cn/gtsfnhfawo.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.cheryme.top/gtcpjlqnko.html

TS:   if (s === "") {}
来源：http://hz.cqqwz.cn/gtzpppjntm.html

Java: if (s.isEmpty()) {}
来源：http://hz.haohaochexian.top/gtqfofhlmp.html

Go:   if s == "" {}
来源：http://hz.birdmap.top/gtogvhzbgc.html

Ruby: if s.empty?
来源：http://hz.yanxiufei.cn/gtjrqdxabd.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.jlsjyb.cn/gtdamuzjmj.html

[E21] 超长截断加省略号
来源：http://hz.bjfxy.top/gtsyqyemae.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.svipenyu.cn/gtuuscykcf.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.gotoacloud.top/gtatrwtiyf.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.sxryk.cn/gtdwlbhryj.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhijiandao.cn/gtbqydtixq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.haohaochexian.top/gtauvrzzvh.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.yonumen.top/gtpqnozefb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.hongshengwenyu.top/gtfigzkuls.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.feifeiyinyue.top/gtrfrcrfix.html

[E22] 字节长度与字符长度
来源：http://hz.hongshengwenyu.top/gttliklfbu.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.guannengcc.top/gthefkmimo.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ydjk.org.cn/gtupfsuetw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yuxming.cn/gtvvyudfyi.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.haohaochexian.top/gtwqumogif.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jinqigfzy.top/gtgrmndecd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.ywan-chungtsiang.top/gtgmxfuvbo.html

Ruby: s.bytesize;  s.length
来源：http://hz.dashuyun.cn/gtnyodhahn.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.guannengcc.top/gtedhuqcyr.html

================================================================================
来源：http://hz.hywenlv.cn/gtwvfbjtkb.html

F. 文件与目录
来源：http://hz.zhaomingkeji.xyz/gtwdsjraql.html

================================================================================
来源：http://hz.aibaodan.cn/gtszkdhwrv.html

[F01] 读取整个文件
来源：http://hz.cucudq.cn/gtvhvzaazx.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.shangyingyoupin.top/gtyrmfwbdv.html

PHP:  file_get_contents("a.txt");
来源：http://hz.cheryme.top/gttngpqgrw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.0kj1m.cn/gtplgklvaw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.shzxlz.cn/gtdqtndvqq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.jinqigfzy.top/gtwctoazzx.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.nanxinkj.top/gtthcsgerz.html

Ruby: File.read("a.txt")
来源：http://hz.gaohongyu789.top/gtadcxfaye.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yvedp.cn/gtrpcoxcad.html

[F02] 逐行读取文件
来源：http://hz.gogol.net.cn/gtqcediuem.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.daria6918.cn/gthqtbaayt.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.jqgufenzy.top/gtxuyfxaih.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.shanyushiyangkeji.top/gtgnwkgskl.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yuanzhike.top/gtvpljcoiv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.redwolf501.top/gttfgeurqg.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.guowangkeji.top/gtrkirqcmb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yanxiufei.cn/gtrnrdkeve.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.snrcjt.cn/gtvwlfkdua.html

[F03] 写入文件（覆盖）
来源：http://hz.hywenlv.cn/gtuzpazwxx.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.hfpthk.cn/gtqwrdcshd.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.nwbrower.top/gtvmtewrkv.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.kuanghao11.cn/gticcjugud.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.chenlongwang.top/gtjaeespnt.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.0kj1m.cn/gtwycexxku.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.zhoulong.xyz/gtqfxxdjom.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.wangshuangyany.cn/gtjyeljfqv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.tian-w.cn/gtblvudueb.html

[F04] 追加写入文件
来源：http://hz.tanke756.top/gtuxdvvlqi.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.wangshuangyany.cn/gtcvbsulsb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.vqdsnc.cn/gtvnpagrdo.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.hysaishi.cn/gtooilthxu.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yonumen.top/gthvlrcgvv.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.hysaishi.cn/gtuffrjueh.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.sweek.top/gtnkyjcnpk.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.svipenyu.cn/gtnlbrawbx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.haohaochexian.top/gtvjoudamj.html

[F05] 判断文件或目录是否存在
来源：http://hz.0kj1m.cn/gtdhbvhywd.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.chenlongwang.top/gtptsiuttq.html

PHP:  file_exists("a.txt");
来源：http://hz.yueranfly.top/gtziabwket.html

JS:   fs.existsSync("a.txt")
来源：http://hz.nanxinkj.top/gtwbrlkyvi.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yongpay.top/gtqxjelwcg.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.gotoacloud.top/gtgqqzplve.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.cashguo.top/gtfkcldvhx.html

Ruby: File.exist?("a.txt")
来源：http://hz.ivvv.top/gtepkofixx.html

C#:   File.Exists("a.txt")
来源：http://hz.feifeiyinyue.top/gtxwnlpluw.html

[F06] 删除文件
来源：http://hz.bjfxy.top/gtsvffzogm.html

Py:   os.remove("a.txt")
来源：http://hz.jiagoushi.top/gtoywvntce.html

PHP:  unlink("a.txt");
来源：http://hz.cqqwz.cn/gtrocssjaz.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.ydjk.org.cn/gtdonsqtnl.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.daria6918.cn/gtoaryrjej.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.shanyushiyangtech.top/gtpkmezhyc.html

Go:   os.Remove("a.txt")
来源：http://hz.jinqigfzy.top/gthcuquqbk.html

Ruby: File.delete("a.txt")
来源：http://hz.zhijiandao.cn/gtdkacixek.html

C#:   File.Delete("a.txt");
来源：http://hz.guannengcc.top/gtksxqjydk.html

[F07] 创建目录（含多级）
来源：http://hz.smart0.xyz/gtuvrxgobq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yongpay.top/gttureszqh.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.meibo888.top/gtkdkqmwpf.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.sysykeji.top/gtmaqvbkrn.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.cashguo.top/gtdoaxpqrr.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.hysaishi.cn/gtofdxewnk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.kuanghao11.cn/gttrncpavy.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.kuanghao11.cn/gtzssmvrrm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.gotoacloud.top/gtmrxhvtnk.html

[F08] 遍历目录
来源：http://hz.iojbl.cn/gtlryzvpfb.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.birdmap.top/gteubkkiet.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.nanxuanxn.top/gtkspcauyy.html

JS:   fs.readdirSync("dir")
来源：http://hz.xuetiantiany.cn/gttwlmlmwj.html

TS:   fs.readdirSync("dir")
来源：http://hz.birdmap.top/gtgovpxdhx.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.xuanzx.com/gtqhhhhayy.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yonumen.top/gtgtpaxmra.html

Ruby: Dir.children("dir")
来源：http://hz.jinqigfzy.top/gtwrscpscv.html

C#:   Directory.GetFiles("dir")
来源：http://hz.nanxinkj.top/gtzlqtnhib.html

[F09] 获取文件大小
来源：http://hz.tian-w.cn/gtfnmlsiug.html

Py:   os.path.getsize("a.txt")
来源：http://hz.ivvv.top/gtizveriow.html

PHP:  filesize("a.txt");
来源：http://hz.shuidangran.top/gtjmnoywaz.html

JS:   fs.statSync("a.txt").size
来源：http://hz.kuanghao11.cn/gtquszuvbt.html

TS:   fs.statSync("a.txt").size
来源：http://hz.cdnleiting.top/gtxudibqcq.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.dianchejie.cn/gtjxaeuxxq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.hysaishi.cn/gtanjpllzb.html

Ruby: File.size("a.txt")
来源：http://hz.yanxiufei.cn/gtojbamrnx.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yangfankeji.com/gtuigidklo.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yvedp.cn/gtrzfpnvdi.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.52xcode.cn/gtsghwkbci.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.zhijiandao.cn/gtimmvldmu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.shangyingyoupin.top/gtovzysimp.html

TS:   path.extname("a.txt")
来源：http://hz.iojbl.cn/gtvjdutimn.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.zhiwuduotai.top/gtdkpsifzg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.hywenlv.cn/gtcfyqlslr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.c1oappe.top/gtlqhbimfm.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.xziqi.cn/gtvdvzbupk.html

[F11] 复制与移动文件
来源：http://hz.nanxuanxn.top/gtyrmlbfan.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.yongpay.top/gtqzduihiy.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.sysykeji.top/gtjtnfjfwk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.guannengcc.top/gtlqubpqdh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.chenjidiqi.icu/gtzwolivkr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.0kj1m.cn/gtmmyewifp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.pengpengdd.cyou/gtdrzlksid.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.jinqigfzy.top/gtgrxxayvt.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.xinyue.icu/gtuzpquozj.html

[F12] CSV 读写
来源：http://hz.jiagoushi.top/gtifcpkstd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.quarkkingdee.top/gtczdcsytw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.nanxinkj.top/gtzkpqmbqk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yvedp.cn/gtuwsvsbri.html

TS:   // 同上
来源：http://hz.wangdashe.top/gtclrbnauw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.daxiang520.top/gtfknyyqil.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.shuidangran.top/gtbjpasbnb.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jianghu66.top/gtmcxglfsu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jqgfzy.top/gtrorwhtco.html

================================================================================
来源：http://hz.snrcjt.cn/gtpgzjwnym.html

G. 面向对象
来源：http://hz.guannengcc.top/gtoxzmyhob.html

================================================================================
来源：http://hz.shuidangran.top/gtkygydsrl.html

[G01] 定义类
来源：http://hz.nwbrower.top/gtztxyivtm.html

Py:   class User: pass
来源：http://hz.ywan-chungtsiang.top/gtyozacqqe.html

PHP:  class User {}
来源：http://hz.cucudq.cn/gtapuaxnjk.html

JS:   class User {}
来源：http://hz.smart0.xyz/gtngrwdsyf.html

TS:   class User { name: string = ""; }
来源：http://hz.hnqzz.top/gtizbeinbp.html

Java: class User {}
来源：http://hz.pengpengdd.cyou/gtinonneix.html

Go:   type User struct { Name string }
来源：http://hz.zhoulong.xyz/gtocelpwgq.html

Ruby: class User; end
来源：http://hz.yongpay.top/gtlaefwbmb.html

C#:   class User {}
来源：http://hz.aizwys.cn/gtvonjabll.html

[G02] 构造函数
来源：http://hz.redwolf501.top/gtxoxzdrsw.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.snrcjt.cn/gttptpkebv.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.ydjk.org.cn/gtzztrleox.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.jqgufenzy.top/gthemmnydv.html

TS:   constructor(public name: string) {}
来源：http://hz.jqgufenzy.top/gtksopigfy.html

Java: User(String name) { this.name = name; }
来源：http://hz.cheryme.top/gtqhijpozr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.hammf.cn/gtznnztqyt.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.tian-w.cn/gtscpqegvi.html

C#:   public User(string name) { Name = name; }
来源：http://hz.snrcjt.cn/gtwhpoxnuk.html

[G03] 实例属性
来源：http://hz.gaohongyu789.top/gtybhcxtra.html

Py:   self.name = "x"
来源：http://hz.aizwys.cn/gtiigultlp.html

PHP:  public string $name = "x";
来源：http://hz.cheryme.top/gtvwbyvcko.html

JS:   this.name = "x";
来源：http://hz.iojbl.cn/gtvlxibsga.html

TS:   name: string = "x";
来源：http://hz.jiagoushi.top/gthtjpuvtr.html

Java: private String name;
来源：http://hz.vqdsnc.cn/gtxizfvggq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.meibo888.top/gtumcfhvcy.html

Ruby: @name = "x"
来源：http://hz.snrcjt.cn/gttrgzvfld.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.ywan-chungtsiang.top/gtysipfhnw.html

[G04] 定义方法
来源：http://hz.hammf.cn/gtcivjlmxn.html

Py:   def greet(self): return self.name
来源：http://hz.mhx1999.top/gtdleoymwh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.tianlin.xyz/gtdxcjtovf.html

JS:   greet() { return this.name; }
来源：http://hz.xuanzx.com/gtnxcnjheg.html

TS:   greet(): string { return this.name; }
来源：http://hz.yj20258888.top/gtrtlhyana.html

Java: String greet() { return name; }
来源：http://hz.sufxvd.cn/gtzvrqblxe.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.smart0.xyz/gtmxwtbyzv.html

Ruby: def greet; @name; end
来源：http://hz.yangfankeji.com/gtumupybsb.html

C#:   public string Greet() => Name;
来源：http://hz.tanke756.top/gtqjvgdhpj.html

[G05] 继承
来源：http://hz.52xcode.cn/gtunruxezv.html

Py:   class Admin(User): pass
来源：http://hz.ppjwa.cn/gthrusofzs.html

PHP:  class Admin extends User {}
来源：http://hz.wangshuangyany.cn/gtydrqybfs.html

JS:   class Admin extends User {}
来源：http://hz.zdqjudy.top/gtcjunigkq.html

TS:   class Admin extends User {}
来源：http://hz.shanyushiyangkeji.top/gtfdlxszcn.html

Java: class Admin extends User {}
来源：http://hz.cashguo.top/gtpljvxjdn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.shanyushiyangkeji.top/gtybobkocq.html

Ruby: class Admin < User; end
来源：http://hz.hnqzz.top/gtyutouvyf.html

C#:   class Admin : User {}
来源：http://hz.hongshengwenyu.top/gtnzezdjdp.html

[G06] 重写方法
来源：http://hz.smart0.xyz/gtfapafcsc.html

Py:   def greet(self): return "admin"
来源：http://hz.fzhhl.top/gtjsqubtyd.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.kuanghao11.cn/gtryfwpzej.html

JS:   greet() { return "admin"; }
来源：http://hz.dashuyun.cn/gtkbtklowt.html

TS:   greet(): string { return "admin"; }
来源：http://hz.xuanzx.com/gtuksdueki.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.shanyushiyangkeji.top/gtccemerux.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.shzxlz.cn/gthbrvligf.html

Ruby: def greet; "admin"; end
来源：http://hz.jyoumei.cn/gtwemgyaov.html

C#:   public override string Greet() => "admin";
来源：http://hz.mhx1999.top/gtnmjziyem.html

[G07] 调用父类方法
来源：http://hz.pengpengdd.cyou/gtofxuofey.html

Py:   super().greet()
来源：http://hz.xuetiantiany.cn/gtioopkpdm.html

PHP:  parent::greet();
来源：http://hz.xylfe.cn/gthuhdppzb.html

JS:   super.greet();
来源：http://hz.shzxlz.cn/gtmahraqvy.html

TS:   super.greet();
来源：http://hz.guannengcc.top/gtfjocaxhf.html

Java: super.greet();
来源：http://hz.hammf.cn/gtzmejurbc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jqgufenzy.top/gtdyhvrzob.html

Ruby: super
来源：http://hz.shuidangran.top/gtdzrasbss.html

C#:   base.Greet();
来源：http://hz.gaohongyu789.top/gtjraqhssl.html

[G08] 静态方法与属性
来源：http://hz.ydzc1.top/gtpwbadshq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.dashuyun.cn/gtgrknwwyl.html

PHP:  public static function f() {}
来源：http://hz.zycfv.cn/gtgejcroid.html

JS:   static f() {}
来源：http://hz.nwbrower.top/gtgxvwonje.html

TS:   static f(): void {}
来源：http://hz.316326.xyz/gticfbfgzp.html

Java: static void f() {}
来源：http://hz.zhongyouzk.top/gtjcdrskiz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.shanyushiyangkeji.top/gtqaxysjor.html

Ruby: def self.f; end
来源：http://hz.xylfe.cn/gtxjzuxxkv.html

C#:   public static void F() {}
来源：http://hz.yongpay.top/gtollahgic.html

[G09] 接口 / 抽象类
来源：http://hz.vqdsnc.cn/gtcolhxvft.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yj20258.top/gttjxqagdn.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.hywenlv.cn/gtcolnmapt.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.tianlin.xyz/gtipzbvmdh.html

TS:   interface Shape { area(): number; }
来源：http://hz.jqgfzy.top/gtbnxaedpy.html

Java: interface Shape { double area(); }
来源：http://hz.zhiwuduotai.top/gtexxkezkf.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.sxryk.cn/gtowgynagz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.zhaomingkeji.xyz/gtrfcsscrm.html

C#:   interface IShape { double Area(); }
来源：http://hz.snrcjt.cn/gtqmcrwcve.html

[G10] 访问控制
来源：http://hz.bjfxy.top/gtqqpurjkt.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.9152youxi.cn/gtfuzomjjt.html

PHP:  public / protected / private
来源：http://hz.nanxuanxn.top/gtqydghcgt.html

JS:   #private 字段；其余公开
来源：http://hz.guowangkeji.top/gtfoqvgfyd.html

TS:   public / protected / private
来源：http://hz.zhijiandao.cn/gtutfcqkjo.html

Java: public / protected / private / 默认包级
来源：http://hz.guannengcc.top/gtvbpdohli.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yj20258.top/gtjrvycwkt.html

Ruby: public / protected / private
来源：http://hz.jianghu66.top/gtxmbivwqi.html

C#:   public / protected / private / internal
来源：http://hz.hnxiangtu.top/gtfbldxrmg.html

[G11] getter / setter
来源：http://hz.yuxming.cn/gtezmfvfrz.html

Py:   @property 与 @x.setter
来源：http://hz.sxryk.cn/gtprdcqzpy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.wangdashe.top/gtmtkdfstt.html

JS:   get name() { return this._name; }
来源：http://hz.tanke756.top/gtaliplzpi.html

TS:   get name(): string { return this._name; }
来源：http://hz.birdmap.top/gtjzxjrrzl.html

Java: public String getName() { return name; }
来源：http://hz.vqdsnc.cn/gtsskyzaim.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.chenzaomai.com/gtmwbvuaul.html


<!-- 参考信息 -->