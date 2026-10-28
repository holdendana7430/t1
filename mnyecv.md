代发 wailian999

Ruby: s.reverse
来源：http://hz.jlsjyb.cn/gtoswordkt.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.wangdashe.top/gteohqmtgd.html

[E12] 统计某字符出现次数
来源：http://hz.dianchejie.cn/gtxhtbixni.html

Py:   s.count("a")
来源：http://hz.wangshuangyany.cn/gtupzktppz.html

PHP:  substr_count($s, "a");
来源：http://hz.cdnleiting.top/gtkhuyvojd.html

JS:   s.split("a").length - 1
来源：http://hz.yuanzhike.top/gtenqszwdv.html

TS:   s.split("a").length - 1
来源：http://hz.chenzaomai.com/gtcjbgcapz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.sufxvd.cn/gthziqzqah.html

Go:   strings.Count(s, "a")
来源：http://hz.guannengcc.top/gtzupgklvd.html

Ruby: s.count("a")
来源：http://hz.yonumen.top/gthwjamseb.html

C#:   s.Count(c => c == 'a')
来源：http://hz.guowangkeji.top/gtcptpxyez.html

[E13] 逐字符遍历
来源：http://hz.svipenyu.cn/gtjiacoblt.html

Py:   for ch in s: print(ch)
来源：http://hz.ehwqpu.com/gtoulvdlre.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.316326.xyz/gtinqujnxi.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xuetiantiany.cn/gtwvlimmja.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yj20258888.top/gtdqgrtbrr.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.cucudq.cn/gtcxpsrkkh.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.jiagoushi.top/gttcwqujho.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.sufxvd.cn/gteyyupbdu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.hongshengwenyu.top/gtuvpwhkmj.html

[E14] URL 编码与 Base64
来源：http://hz.xylfe.cn/gtvihltpgm.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.fengsongda.top/gtgbivcate.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.sweek.top/gtjjdqubxk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.nanxinkj.top/gtcvukfjln.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.havefunace.top/gtxauvuhdg.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.yonumen.top/gthonkakan.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.sysykeji.top/gtixinwzek.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.redwolf501.top/gttvceshpr.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.sxryk.cn/gthwylxcra.html

[E15] HTML 转义 / 反转义
来源：http://hz.nanxinkj.top/gtyaqwvzje.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.yangfankeji.com/gtjphvdlte.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.birdmap.top/gttxguuwjo.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.gotoacloud.top/gtdlwofqfg.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.wangdashe.top/gtvfrbnrnw.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.dashuyun.cn/gtxvdhcpxu.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.ivvv.top/gtuzcmxkpo.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.wangshuangyany.cn/gtmkjvumsz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.ybcxt.top/gtaurcgfxy.html

[E16] 数字千分位
来源：http://hz.zycfv.cn/gtfknqltxm.html

Py:   f"{1234567:,}"
来源：http://hz.zhijiandao.cn/gtcvodfaub.html

PHP:  number_format(1234567);
来源：http://hz.pengpengdd.cyou/gtbpmbkpow.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.sxryk.cn/gtsgngktlc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.gotoacloud.top/gtknimcgex.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.daxiang520.top/gtxxuapzbp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.dianchejie.cn/gtqratvqtg.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.52xcode.cn/gtqounsokd.html

C#:   1234567.ToString("N0")
来源：http://hz.chenjidiqi.icu/gtbeedoots.html

[E17] 首字母大写
来源：http://hz.zhengqikj.top/gtlcqywapk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.guannengcc.top/gtovijrbiv.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.cucudq.cn/gtiyrdeqni.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.chenjidiqi.icu/gtachiiufo.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.cashguo.top/gtzgacmzsn.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.jinyuanbaomall.cn/gtcohdzzfl.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.xuetiantiany.cn/gtqxvnppbu.html

Ruby: s.capitalize
来源：http://hz.wangdashe.top/gtnlxqodfj.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.aibaodan.cn/gtdiqvqpoy.html

[E18] 模板占位符替换
来源：http://hz.cucudq.cn/gtjcwntcyq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.havefunace.top/gtearmhzyp.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.meibo888.top/gtmkmztyad.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.yangfankeji.com/gtpsddhyji.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.zhiwuduotai.top/gtuamsykmz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.yonumen.top/gtvlounikv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.ehwqpu.com/gtquypskue.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.gotoacloud.top/gthgvxisug.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.hongshengwenyu.top/gtntefvcyz.html

[E19] 多行文本按行拆分
来源：http://hz.tanke756.top/gtbeuytolb.html

Py:   s.splitlines()
来源：http://hz.mhx1999.top/gtsfbrcixp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jinghuilouyu.cn/gtrdzqfwcl.html

JS:   s.split(/\r?\n/)
来源：http://hz.havefunace.top/gtciocloex.html

TS:   s.split(/\r?\n/)
来源：http://hz.haohaochexian.top/gtxytshqri.html

Java: s.lines().toList()
来源：http://hz.jinyuanbaomall.cn/gtijadvmou.html

Go:   strings.Split(s, "\n")
来源：http://hz.xuanzx.com/gtimnaadpq.html

Ruby: s.lines
来源：http://hz.guowangkeji.top/gtdtpscjyv.html

C#:   s.Split('\n')
来源：http://hz.shuidangran.top/gtpzvjcjeu.html

[E20] 判断字符串是否为空
来源：http://hz.andypj.xyz/gtzcmwurpf.html

Py:   if not s:
来源：http://hz.52xcode.cn/gtysitfwvf.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.aizwys.cn/gtfxjfinet.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.chenlongwang.top/gtmnmioklx.html

TS:   if (s === "") {}
来源：http://hz.xinyue.icu/gttsyxgmkc.html

Java: if (s.isEmpty()) {}
来源：http://hz.cheryme.top/gtuyptwcyv.html

Go:   if s == "" {}
来源：http://hz.yuanzhike.top/gtbijoeapu.html

Ruby: if s.empty?
来源：http://hz.pycfn.com/gtrrrfjwoy.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.jyoumei.cn/gtgytrqoky.html

[E21] 超长截断加省略号
来源：http://hz.yuxming.cn/gttyvlpdly.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.xinyue.icu/gteeiilixt.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.sxryk.cn/gtiwxrtfjt.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.havefunace.top/gtpwahndpm.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.xinyue.icu/gtgijwxbmj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.hnxiangtu.top/gtqbrlucjo.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.hfpthk.cn/gtpudqsuuq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.dashuyun.cn/gtdyyyjwki.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.jinghuilouyu.cn/gtiiedvntw.html

[E22] 字节长度与字符长度
来源：http://hz.yueranfly.top/gtromvguyz.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.daxiang520.top/gtayvomhke.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.gogol.net.cn/gtabkdalti.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hnxiangtu.top/gtjmekopzw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.shanyushiyangkeji.top/gtiakyufrv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.yangfankeji.com/gtmjqoptfx.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.daria6918.cn/gtscegigij.html

Ruby: s.bytesize;  s.length
来源：http://hz.chenjidiqi.icu/gtnxbbfmxx.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.yonumen.top/gtuxgydgku.html

================================================================================
来源：http://hz.zhixingplan.top/gtsxcqdgal.html

F. 文件与目录
来源：http://hz.ivvv.top/gtbdqaqdvl.html

================================================================================
来源：http://hz.xinyue.icu/gtrmcfqriz.html

[F01] 读取整个文件
来源：http://hz.wangshuangyany.cn/gtwaltjbjr.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.xinyue.icu/gtoukiapbm.html

PHP:  file_get_contents("a.txt");
来源：http://hz.jinqigufen.top/gtnfdlxcxd.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.redwolf501.top/gtytvyieuo.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.xziqi.cn/gtaonfvswf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.fzhhl.top/gtghnqayqt.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.jinqigufen.top/gtbzpdwjzz.html

Ruby: File.read("a.txt")
来源：http://hz.tian-w.cn/gtwtemguhw.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.hongshengwenyu.top/gtzmwwfpmz.html

[F02] 逐行读取文件
来源：http://hz.iojbl.cn/gtimmavdyw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.gotoacloud.top/gtbaavvbil.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.tanke756.top/gtzvzshnlb.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jinyuanbaomall.cn/gtdmegxxsy.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.haohaochexian.top/gtzmzskohd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.nwbrower.top/gtjpctifql.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.xinyue.icu/gtjgmtldpj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yuxming.cn/gtzdketucw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.xuanzx.com/gthbbkmbnq.html

[F03] 写入文件（覆盖）
来源：http://hz.andypj.xyz/gtawelkwbd.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.0kj1m.cn/gtwqevyayx.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.smart0.xyz/gtkpmyawqy.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.guannengcc.top/gtgdonowqt.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.sysykeji.top/gtpvrezplx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.ybcxt.top/gtyvvywdyf.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.ybcxt.top/gtyiqrgfvt.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.gaohongyu789.top/gthnzmjhzj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.gzhubu.top/gtgzkowmya.html

[F04] 追加写入文件
来源：http://hz.ehwqpu.com/gtuuszkhdh.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.52xcode.cn/gtbwremuqd.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.jqgufenzy.top/gtfgllkzzh.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.smart0.xyz/gtbphbrfim.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jlsjyb.cn/gtkgilatol.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.shanyushiyangkeji.top/gtnqxcagua.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.iojbl.cn/gtpgvhtouj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.pengpengdd.cyou/gtjqrfveat.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.feifeiyinyue.top/gtskuaejua.html

[F05] 判断文件或目录是否存在
来源：http://hz.xuanzx.com/gtvfzzbgaw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.guowangkeji.top/gtpwwpcgct.html

PHP:  file_exists("a.txt");
来源：http://hz.tanke756.top/gtyvmjxhqj.html

JS:   fs.existsSync("a.txt")
来源：http://hz.dashuyun.cn/gtsjucsjfm.html

TS:   fs.existsSync("a.txt")
来源：http://hz.jqgufenzy.top/gtcglqnsmz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.zhijiandao.cn/gtimvckboo.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.yj20258888.top/gtjvvbrlic.html

Ruby: File.exist?("a.txt")
来源：http://hz.hnxiangtu.top/gtmybwaoaj.html

C#:   File.Exists("a.txt")
来源：http://hz.snrcjt.cn/gtbphjvzte.html

[F06] 删除文件
来源：http://hz.ppjwa.cn/gtzribkyxd.html

Py:   os.remove("a.txt")
来源：http://hz.sufxvd.cn/gtjzbwnxwn.html

PHP:  unlink("a.txt");
来源：http://hz.havefunace.top/gtecawkpst.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.birdmap.top/gtqibxfegj.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.yuanzhike.top/gtynyicare.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.pengpengdd.cyou/gtpllzvpyt.html

Go:   os.Remove("a.txt")
来源：http://hz.birdmap.top/gtlcqdjafs.html

Ruby: File.delete("a.txt")
来源：http://hz.shanyushiyangkeji.top/gtvcnopeih.html

C#:   File.Delete("a.txt");
来源：http://hz.jianghu66.top/gtdgwprwfk.html

[F07] 创建目录（含多级）
来源：http://hz.hnxiangtu.top/gtxpdsjgpf.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.hfpthk.cn/gtbkxamapz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.xziqi.cn/gtpsdtgpmj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.snrcjt.cn/gtrhuyogsv.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.shangyingyoupin.top/gthrbmfeld.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.0kj1m.cn/gtkmewdlft.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.zhengqikj.top/gtxdznozue.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.gzhubu.top/gtfjgmhonl.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.redwolf501.top/gtahkmonpl.html

[F08] 遍历目录
来源：http://hz.yonumen.top/gtwspqpwkc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.bjfxy.top/gthgdclmkr.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.iojbl.cn/gtryoxcqdx.html

JS:   fs.readdirSync("dir")
来源：http://hz.zhengqikj.top/gtgurxerzd.html

TS:   fs.readdirSync("dir")
来源：http://hz.hysaishi.cn/gtomwittvb.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.guowangkeji.top/gthbrhkkmc.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.mhx1999.top/gtvidfcbhh.html

Ruby: Dir.children("dir")
来源：http://hz.cashguo.top/gtwzvbhmrm.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yongpay.top/gtkxreaesh.html

[F09] 获取文件大小
来源：http://hz.sufxvd.cn/gtnpqiryvu.html

Py:   os.path.getsize("a.txt")
来源：http://hz.yonumen.top/gttbihxmlh.html

PHP:  filesize("a.txt");
来源：http://hz.gzhubu.top/gtmexchqud.html

JS:   fs.statSync("a.txt").size
来源：http://hz.ybcxt.top/gtkypjqtmi.html

TS:   fs.statSync("a.txt").size
来源：http://hz.jinghuilouyu.cn/gtgugobmvt.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.andypj.xyz/gtckatpypb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.9152youxi.cn/gtybilnobv.html

Ruby: File.size("a.txt")
来源：http://hz.yanxiufei.cn/gtsijjfchd.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.iojbl.cn/gtgrfpvvim.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.chenlongwang.top/gtwauykcjj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.gzhubu.top/gtxavbaddp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.hammf.cn/gthwwyomhp.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.bjfxy.top/gthfchyntj.html

TS:   path.extname("a.txt")
来源：http://hz.cashguo.top/gtkgegvvlu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.jinqigufen.top/gtzyunzpya.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.chenzaomai.com/gtyscvgjrd.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.gaohongyu789.top/gthhvbfmep.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.zycfv.cn/gtrtapcryg.html

[F11] 复制与移动文件
来源：http://hz.c1oappe.top/gtnibiumnn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.zdqjudy.top/gtswodybnw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.nwbrower.top/gtryyaspaf.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xinyue.icu/gthbfwminu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yanxiufei.cn/gtoqbrrgwg.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.hywenlv.cn/gtklmhxawi.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.tian-w.cn/gttpkqwwrk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.shzxlz.cn/gtxoedpoxa.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.pycfn.com/gtkjeyuxpt.html

[F12] CSV 读写
来源：http://hz.yj20258888.top/gtbzxlelvj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.zhoulong.xyz/gttmapijuv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.jqgfzy.top/gtsfccorec.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.xuetiantiany.cn/gtwrjfuyub.html

TS:   // 同上
来源：http://hz.cdnleiting.top/gtftkkvegf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.hammf.cn/gtthoopztq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.zycfv.cn/gtaqdpphuw.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.xziqi.cn/gteoqirmmn.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jinyuanbaomall.cn/gtpmmtrsqr.html

================================================================================
来源：http://hz.jqgfzy.top/gtgkapupxt.html

G. 面向对象
来源：http://hz.sysykeji.top/gteiorhhyx.html

================================================================================
来源：http://hz.316326.xyz/gthhpcaqvb.html

[G01] 定义类
来源：http://hz.meibo888.top/gtkxumnrpm.html

Py:   class User: pass
来源：http://hz.smart0.xyz/gtegzeqwot.html

PHP:  class User {}
来源：http://hz.hongshengwenyu.top/gtpoicemhy.html

JS:   class User {}
来源：http://hz.cashguo.top/gtvqtcaeis.html

TS:   class User { name: string = ""; }
来源：http://hz.0kj1m.cn/gtobbtoprp.html

Java: class User {}
来源：http://hz.jinqigufen.top/gtycgjzxlj.html

Go:   type User struct { Name string }
来源：http://hz.ybcxt.top/gtagvxigta.html

Ruby: class User; end
来源：http://hz.hysaishi.cn/gtsgkplsmj.html

C#:   class User {}
来源：http://hz.yanxiufei.cn/gtarmxxylc.html

[G02] 构造函数
来源：http://hz.jinqigfzy.top/gtljxmpqxs.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.nanxuanxn.top/gtvcwkiclr.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.jinqigfzy.top/gtftqzgfei.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.ydjk.org.cn/gtgdlguqej.html

TS:   constructor(public name: string) {}
来源：http://hz.yonumen.top/gthoeyoqru.html

Java: User(String name) { this.name = name; }
来源：http://hz.shanyushiyangkeji.top/gtudeiooyl.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.ydzc1.top/gtrglhmjyu.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.cheryme.top/gtfjivcfdm.html

C#:   public User(string name) { Name = name; }
来源：http://hz.xuetiantiany.cn/gtygfmipsz.html

[G03] 实例属性
来源：http://hz.wangshuangyany.cn/gtjohgavxa.html

Py:   self.name = "x"
来源：http://hz.aibaodan.cn/gtienuzccu.html

PHP:  public string $name = "x";
来源：http://hz.jinqigufen.top/gtvqnjvroe.html

JS:   this.name = "x";
来源：http://hz.jqgufenzy.top/gthiiixafx.html

TS:   name: string = "x";
来源：http://hz.yangfankeji.com/gtuamosrxg.html

Java: private String name;
来源：http://hz.dianchejie.cn/gtqsnzilsw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.cashguo.top/gtkoniprca.html

Ruby: @name = "x"
来源：http://hz.gogol.net.cn/gtqawxukza.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yanxiufei.cn/gtdyxbtysv.html

[G04] 定义方法
来源：http://hz.ywan-chungtsiang.top/gtckblqsen.html

Py:   def greet(self): return self.name
来源：http://hz.bjfxy.top/gtlgppprsi.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.jinqigufen.top/gtaabsjrur.html

JS:   greet() { return this.name; }
来源：http://hz.yangfankeji.com/gtpqgxsqic.html

TS:   greet(): string { return this.name; }
来源：http://hz.aibaodan.cn/gtomhbqmrz.html

Java: String greet() { return name; }
来源：http://hz.nanxinkj.top/gtdujmkdqb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.cucudq.cn/gtggcvnyek.html

Ruby: def greet; @name; end
来源：http://hz.vqdsnc.cn/gtdvcvsevs.html

C#:   public string Greet() => Name;
来源：http://hz.gogol.net.cn/gtetpthbnl.html

[G05] 继承
来源：http://hz.zhiwuduotai.top/gtfszoundt.html

Py:   class Admin(User): pass
来源：http://hz.xinyue.icu/gtfsuazxng.html

PHP:  class Admin extends User {}
来源：http://hz.yueranfly.top/gtpgmwmcnm.html

JS:   class Admin extends User {}
来源：http://hz.hongshengwenyu.top/gtjowopgok.html

TS:   class Admin extends User {}
来源：http://hz.yueranfly.top/gtgeaqrfwk.html

Java: class Admin extends User {}
来源：http://hz.aibaodan.cn/gtaklzkkfw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.dashuyun.cn/gtzfycneun.html

Ruby: class Admin < User; end
来源：http://hz.redwolf501.top/gtrlxdktre.html

C#:   class Admin : User {}
来源：http://hz.zhiwuduotai.top/gtssppljtf.html

[G06] 重写方法
来源：http://hz.xuetiantiany.cn/gtmsicrxkd.html

Py:   def greet(self): return "admin"
来源：http://hz.yuxming.cn/gtrymykopg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.wangdashe.top/gtifvgyfzt.html

JS:   greet() { return "admin"; }
来源：http://hz.xylfe.cn/gtuowquyuy.html

TS:   greet(): string { return "admin"; }
来源：http://hz.xziqi.cn/gtbtycpefz.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.hysaishi.cn/gtxflgmrsn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.0kj1m.cn/gtpvobxaqj.html

Ruby: def greet; "admin"; end
来源：http://hz.yvedp.cn/gtkjnpgged.html

C#:   public override string Greet() => "admin";
来源：http://hz.yvedp.cn/gtgonyjktq.html

[G07] 调用父类方法
来源：http://hz.cucudq.cn/gtonjamejm.html

Py:   super().greet()
来源：http://hz.gaohongyu789.top/gtugdvcpye.html

PHP:  parent::greet();
来源：http://hz.haohaochexian.top/gtnufqtlih.html

JS:   super.greet();
来源：http://hz.meibo888.top/gtdpsniilx.html

TS:   super.greet();
来源：http://hz.gotoacloud.top/gtzdgcxyrb.html

Java: super.greet();
来源：http://hz.daxiang520.top/gtxgjztcea.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.hnqzz.top/gtnyeempev.html

Ruby: super
来源：http://hz.cdnleiting.top/gtwdxhpxur.html

C#:   base.Greet();
来源：http://hz.feifeiyinyue.top/gtdugtchwn.html

[G08] 静态方法与属性
来源：http://hz.hnxiangtu.top/gtnqithqhk.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.gzhubu.top/gtdyuqqmhr.html

PHP:  public static function f() {}
来源：http://hz.yanxiufei.cn/gtvabbhuce.html

JS:   static f() {}
来源：http://hz.nwbrower.top/gtsjfkovjc.html

TS:   static f(): void {}
来源：http://hz.zhiwuduotai.top/gtwwrjhgms.html

Java: static void f() {}
来源：http://hz.zdqjudy.top/gtuctaklse.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.nanxinkj.top/gtvwdkrlem.html

Ruby: def self.f; end
来源：http://hz.jqgufenzy.top/gtigskdvcj.html

C#:   public static void F() {}
来源：http://hz.jyoumei.cn/gtjefhssze.html

[G09] 接口 / 抽象类
来源：http://hz.jqgfzy.top/gtjyddiwyi.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.shanyushiyangtech.top/gtckusprbf.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.gogol.net.cn/gtilosdpkn.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.guannengcc.top/gtuvsmvjhh.html

TS:   interface Shape { area(): number; }
来源：http://hz.hammf.cn/gtilehfjgo.html

Java: interface Shape { double area(); }
来源：http://hz.hnqzz.top/gtvkfjvcyn.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.zhiwuduotai.top/gtnyzzzliv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jinqigufen.top/gtnycrbhcx.html

C#:   interface IShape { double Area(); }
来源：http://hz.yj202588.top/gtqrylwkzr.html

[G10] 访问控制
来源：http://hz.jianghu66.top/gtefzraxrc.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.xziqi.cn/gtxtybzvkf.html

PHP:  public / protected / private
来源：http://hz.daria6918.cn/gtmvaszrhz.html

JS:   #private 字段；其余公开
来源：http://hz.chenlongwang.top/gtglaxlhoh.html


<!-- 参考信息 -->