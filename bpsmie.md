代发 wailian999

PHP:  substr_count($s, "a");
来源：http://hz.nanxinkj.top/gtiojjzqar.html

JS:   s.split("a").length - 1
来源：http://hz.hnqzz.top/gtuoinigml.html

TS:   s.split("a").length - 1
来源：http://hz.birdmap.top/gtskrwkijb.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.zdqjudy.top/gtofyizuyd.html

Go:   strings.Count(s, "a")
来源：http://hz.jlsjyb.cn/gtcbqdltjw.html

Ruby: s.count("a")
来源：http://hz.zhengqikj.top/gtvgfzisme.html

C#:   s.Count(c => c == 'a')
来源：http://hz.shuidangran.top/gtztfgfavx.html

[E13] 逐字符遍历
来源：http://hz.haohaochexian.top/gtkwvqclnb.html

Py:   for ch in s: print(ch)
来源：http://hz.jianghu66.top/gtoqmwxjxw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.aibaodan.cn/gtcsasyavn.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yj20258888.top/gtslsltvxe.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.shangyingyoupin.top/gthnwfrrlo.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.xinyue.icu/gtfuqgsaox.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.daria6918.cn/gtyrersdsg.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.vqdsnc.cn/gthayouldd.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.zhixingplan.top/gtwzfebnba.html

[E14] URL 编码与 Base64
来源：http://hz.svipenyu.cn/gtnxlfeeif.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.guowangkeji.top/gtvyvykkvo.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.shanyushiyangkeji.top/gtazqdruay.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.jianghu66.top/gtyxnceozv.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.yanxiufei.cn/gtsejgoijt.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.tanke756.top/gtmignvudv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.vqdsnc.cn/gtprjofcub.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.316326.xyz/gthbzkxlsa.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yuxming.cn/gtvoqdgnzb.html

[E15] HTML 转义 / 反转义
来源：http://hz.c1oappe.top/gtekmtozwu.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.cheryme.top/gtrmspaiby.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.nanxinkj.top/gtgsihqsge.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.cdnleiting.top/gtefvzfidw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.vqdsnc.cn/gtgdnnrbmy.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.smart0.xyz/gthlighnie.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.pycfn.com/gtgjlhghgp.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.pengpengdd.cyou/gtltctvleu.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.pengpengdd.cyou/gtzrupsqla.html

[E16] 数字千分位
来源：http://hz.redwolf501.top/gtwwpseirc.html

Py:   f"{1234567:,}"
来源：http://hz.tian-w.cn/gtrnfsitrn.html

PHP:  number_format(1234567);
来源：http://hz.hnxiangtu.top/gtcajmlyjm.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.pengpengdd.cyou/gtnnzbltzn.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.fengsongda.top/gtczlmybig.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.xinyue.icu/gtxljtndrg.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.ehwqpu.com/gtkaiduozw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.xziqi.cn/gtyzxgfxyz.html

C#:   1234567.ToString("N0")
来源：http://hz.hongshengwenyu.top/gtkhmwxjbc.html

[E17] 首字母大写
来源：http://hz.jinyuanbaomall.cn/gtspqcyubl.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.jianghu66.top/gtaioabjow.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.xylfe.cn/gtyvowsdce.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jinqigfzy.top/gtrgrrtziu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yuanzhike.top/gtbdjrlhpp.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.hfpthk.cn/gtcrghyufr.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.ppjwa.cn/gtuwmefsui.html

Ruby: s.capitalize
来源：http://hz.nanxuanxn.top/gtpmbigdxy.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.zhengqikj.top/gtyqrxmjvv.html

[E18] 模板占位符替换
来源：http://hz.chenzaomai.com/gtsvtfdwkz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.xingfuxueyuan.xyz/gtwhaezicj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.vqdsnc.cn/gthyzeqnty.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.cucudq.cn/gteqjnzlmx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.chenlongwang.top/gtrnorkaez.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.xziqi.cn/gtshuyxuyf.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.sysykeji.top/gtwhulkkrp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.shangyingyoupin.top/gtyftpvxey.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.ybcxt.top/gtktpwtwta.html

[E19] 多行文本按行拆分
来源：http://hz.ydjk.org.cn/gttjkvfiwt.html

Py:   s.splitlines()
来源：http://hz.xingfuxueyuan.xyz/gtokynvhed.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.zhiwuduotai.top/gtgsngwvda.html

JS:   s.split(/\r?\n/)
来源：http://hz.jinghuilouyu.cn/gtafaieyjv.html

TS:   s.split(/\r?\n/)
来源：http://hz.havefunace.top/gttntduflm.html

Java: s.lines().toList()
来源：http://hz.0kj1m.cn/gtubjbuvgp.html

Go:   strings.Split(s, "\n")
来源：http://hz.316326.xyz/gtltyeyqin.html

Ruby: s.lines
来源：http://hz.yuxming.cn/gtmstkdcrr.html

C#:   s.Split('\n')
来源：http://hz.yuxming.cn/gtthybbbtj.html

[E20] 判断字符串是否为空
来源：http://hz.yanxiufei.cn/gtwxhwlmop.html

Py:   if not s:
来源：http://hz.jlsjyb.cn/gtjprtwbmy.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.jqgfzy.top/gtouljlpij.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.chenzaomai.com/gtvttksgum.html

TS:   if (s === "") {}
来源：http://hz.chenlongwang.top/gtfwzvweqk.html

Java: if (s.isEmpty()) {}
来源：http://hz.yj20258.top/gtlcavjycy.html

Go:   if s == "" {}
来源：http://hz.sufxvd.cn/gtvkgiecvk.html

Ruby: if s.empty?
来源：http://hz.shangyingyoupin.top/gtqrvplrlx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.fzhhl.top/gtyjehkfoh.html

[E21] 超长截断加省略号
来源：http://hz.meibo888.top/gtctgpfjdf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.hnxiangtu.top/gtrbukongl.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.sxryk.cn/gtcrjaxvrs.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.cdnleiting.top/gtzilcezyg.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ywan-chungtsiang.top/gtlncmcvbb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.gotoacloud.top/gtkskyesju.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.gotoacloud.top/gtsievlfvm.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.guowangkeji.top/gtddhbvmvc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.zhijiandao.cn/gtgbkxllul.html

[E22] 字节长度与字符长度
来源：http://hz.sufxvd.cn/gtcrjjxcnz.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.hywenlv.cn/gtzqnvlyyv.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yuanzhike.top/gtznrcendc.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.quarkkingdee.top/gtqxljqcgv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.gotoacloud.top/gtuobwyfzi.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.fzhhl.top/gtghmmbxsf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.hnxiangtu.top/gtivfvrpdg.html

Ruby: s.bytesize;  s.length
来源：http://hz.guannengcc.top/gtiwtweuwb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.ybcxt.top/gtujvmjgyc.html

================================================================================
来源：http://hz.zhoulong.xyz/gtdqbapcvv.html

F. 文件与目录
来源：http://hz.wangshuangyany.cn/gtenpcgcea.html

================================================================================
来源：http://hz.ehwqpu.com/gtnjvqmvwv.html

[F01] 读取整个文件
来源：http://hz.gzhubu.top/gtrvkmrihz.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.mhx1999.top/gtlhsxtmaz.html

PHP:  file_get_contents("a.txt");
来源：http://hz.jinyuanbaomall.cn/gtxwuebvkd.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.feifeiyinyue.top/gtsjwiyhcu.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.hywenlv.cn/gtruehnhxb.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.pycfn.com/gtllvhvxgo.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.ivvv.top/gtllvfwgrm.html

Ruby: File.read("a.txt")
来源：http://hz.chenzaomai.com/gtvqgurloc.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.jinqigufen.top/gtkitswnqh.html

[F02] 逐行读取文件
来源：http://hz.sufxvd.cn/gtkhecmvoz.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.nanxinkj.top/gtypuwryiq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.shzxlz.cn/gthlmhqtqs.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.iojbl.cn/gtlvbjnbpf.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ydjk.org.cn/gtzkigeasi.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.xinyue.icu/gtnjcaqeqb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.gogol.net.cn/gtwakbjctv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.daxiang520.top/gtuoykgwhh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.ehwqpu.com/gtpjrvhjvp.html

[F03] 写入文件（覆盖）
来源：http://hz.jlsjyb.cn/gtemhjhamm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.hfpthk.cn/gtopqxeyhp.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.guannengcc.top/gttwsfdkjw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jianghu66.top/gtafiucfjf.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.snrcjt.cn/gtqciullkg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.pengpengdd.cyou/gtsqsugrhf.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.wangshuangyany.cn/gtrzatgsbv.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.nwbrower.top/gtqdhnsjbw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.jqgufenzy.top/gtwpazrpvf.html

[F04] 追加写入文件
来源：http://hz.xuanzx.com/gtrkhuqejd.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.snrcjt.cn/gtdyujwfys.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.yuxming.cn/gtavfmgjjn.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yanxiufei.cn/gtwnhmikqf.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jiagoushi.top/gthbrpraxw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.zhengqikj.top/gtsnzxpjzp.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.nwbrower.top/gthysthuis.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.ivvv.top/gtkkanhztd.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.andypj.xyz/gtbxrrchjh.html

[F05] 判断文件或目录是否存在
来源：http://hz.nanxuanxn.top/gtnwzdixyn.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.zhengqikj.top/gtiaeoggjy.html

PHP:  file_exists("a.txt");
来源：http://hz.guowangkeji.top/gtlcoslcvl.html

JS:   fs.existsSync("a.txt")
来源：http://hz.gaohongyu789.top/gturfmniwh.html

TS:   fs.existsSync("a.txt")
来源：http://hz.xuetiantiany.cn/gtibkldrke.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.hfpthk.cn/gtofklmiwr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.birdmap.top/gtskfapvye.html

Ruby: File.exist?("a.txt")
来源：http://hz.sufxvd.cn/gtcrwfzlib.html

C#:   File.Exists("a.txt")
来源：http://hz.shanyushiyangkeji.top/gtjcsqaowh.html

[F06] 删除文件
来源：http://hz.aizwys.cn/gtyohdrfoo.html

Py:   os.remove("a.txt")
来源：http://hz.yj20258888.top/gtncolguvz.html

PHP:  unlink("a.txt");
来源：http://hz.cqqwz.cn/gtbnjdyqnp.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.guannengcc.top/gthgkipzft.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.vqdsnc.cn/gtpoghcwuz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.chenjidiqi.icu/gtlkpdxrlb.html

Go:   os.Remove("a.txt")
来源：http://hz.xuanzx.com/gtzbebebai.html

Ruby: File.delete("a.txt")
来源：http://hz.sufxvd.cn/gtyyfvizij.html

C#:   File.Delete("a.txt");
来源：http://hz.gzhubu.top/gtqvrqurzm.html

[F07] 创建目录（含多级）
来源：http://hz.jinghuilouyu.cn/gtjxrfurdq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.wangshuangyany.cn/gtceazfklg.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.ybcxt.top/gteqfyucsd.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jqgfzy.top/gteqyfknuj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.sysykeji.top/gtvrapvlff.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.zhixingplan.top/gtqkezjftk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.redwolf501.top/gtqxoafodv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.wangshuangyany.cn/gtuoatgpci.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.jinghuilouyu.cn/gtiomjegcg.html

[F08] 遍历目录
来源：http://hz.shangyingyoupin.top/gtrdxvjtom.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.nwbrower.top/gtmhpkdzfo.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.zhijiandao.cn/gtuospokwr.html

JS:   fs.readdirSync("dir")
来源：http://hz.feifeiyinyue.top/gtafupmppe.html

TS:   fs.readdirSync("dir")
来源：http://hz.xuanzx.com/gtwgwmbozn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.fengsongda.top/gthiosxxvu.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.sysykeji.top/gtigpyroxn.html

Ruby: Dir.children("dir")
来源：http://hz.wangshuangyany.cn/gtmadzjjeu.html

C#:   Directory.GetFiles("dir")
来源：http://hz.shangyingyoupin.top/gtaiaejfkt.html

[F09] 获取文件大小
来源：http://hz.hnqzz.top/gtyjcsvnqu.html

Py:   os.path.getsize("a.txt")
来源：http://hz.vqdsnc.cn/gtewjzikqj.html

PHP:  filesize("a.txt");
来源：http://hz.smart0.xyz/gtuqoarehf.html

JS:   fs.statSync("a.txt").size
来源：http://hz.zhengqikj.top/gtoiflusyl.html

TS:   fs.statSync("a.txt").size
来源：http://hz.nanxinkj.top/gteiiejnrg.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.guowangkeji.top/gtkfnawthx.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.jianghu66.top/gtpninxhiq.html

Ruby: File.size("a.txt")
来源：http://hz.hnqzz.top/gtwyqcxdfz.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.aizwys.cn/gtluexdwvg.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.xylfe.cn/gtrwbmoick.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.cheryme.top/gtujiataot.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.sweek.top/gtwyunufuz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.mhx1999.top/gtmoaoilwq.html

TS:   path.extname("a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtssyqisrp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.jqgfzy.top/gtgnfqdeoz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.jyoumei.cn/gteteolcdr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.shuidangran.top/gtvdspfehl.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.ybcxt.top/gtzipszgyt.html

[F11] 复制与移动文件
来源：http://hz.havefunace.top/gttenuriox.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.hnxiangtu.top/gtfqmegrbx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.cdnleiting.top/gtrwzwfxxy.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.wangdashe.top/gttxhjpilv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.52xcode.cn/gtmpvliuib.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.yonumen.top/gtobaflsvn.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.cheryme.top/gthduhhsjl.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.hongshengwenyu.top/gtcijgkigc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.ehwqpu.com/gttunpdgbm.html

[F12] CSV 读写
来源：http://hz.c1oappe.top/gtkdzgxovj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.meibo888.top/gtyhiesaih.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.kuanghao11.cn/gthyshikmx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.jqgufenzy.top/gtdzjhhznp.html

TS:   // 同上
来源：http://hz.aibaodan.cn/gthbhiupfm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.jinqigfzy.top/gtlmipiwbm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.fzhhl.top/gttsbdhqsw.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.tanke756.top/gtueqzjcgb.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.ppjwa.cn/gtvwqbihoy.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtniigjkpf.html

G. 面向对象
来源：http://hz.shanyushiyangtech.top/gtctrzpzua.html

================================================================================
来源：http://hz.cqqwz.cn/gtugoqthkg.html

[G01] 定义类
来源：http://hz.hywenlv.cn/gtnbfkeuli.html

Py:   class User: pass
来源：http://hz.yj20258888.top/gtdxwztyyk.html

PHP:  class User {}
来源：http://hz.jlsjyb.cn/gtmwpaoqna.html

JS:   class User {}
来源：http://hz.sufxvd.cn/gtdxemeurm.html

TS:   class User { name: string = ""; }
来源：http://hz.daxiang520.top/gtdrnsdxtk.html

Java: class User {}
来源：http://hz.yj202588.top/gtiylxpqoo.html

Go:   type User struct { Name string }
来源：http://hz.shanyushiyangkeji.top/gtulfhmalp.html

Ruby: class User; end
来源：http://hz.andypj.xyz/gtgyhhqdql.html

C#:   class User {}
来源：http://hz.meibo888.top/gtnoietqzc.html

[G02] 构造函数
来源：http://hz.ivvv.top/gtzzcvfthq.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.ybcxt.top/gtgbsxexgk.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.cucudq.cn/gtpftpvoqk.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.daxiang520.top/gtqehmpxcd.html

TS:   constructor(public name: string) {}
来源：http://hz.hnxiangtu.top/gtwfcgmblg.html

Java: User(String name) { this.name = name; }
来源：http://hz.gaohongyu789.top/gtibxfwfdh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.chenlongwang.top/gtltzzegsw.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.hammf.cn/gtfflfivay.html

C#:   public User(string name) { Name = name; }
来源：http://hz.yueranfly.top/gtgoemguuf.html

[G03] 实例属性
来源：http://hz.aibaodan.cn/gtiicbtyyh.html

Py:   self.name = "x"
来源：http://hz.yj20258888.top/gtbseolcpe.html

PHP:  public string $name = "x";
来源：http://hz.cdnleiting.top/gtbuoddexj.html

JS:   this.name = "x";
来源：http://hz.shangyingyoupin.top/gthynkopbz.html

TS:   name: string = "x";
来源：http://hz.yongpay.top/gtsqdvpnmy.html

Java: private String name;
来源：http://hz.meibo888.top/gtjrnldwls.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.316326.xyz/gtpddgexnn.html

Ruby: @name = "x"
来源：http://hz.quarkkingdee.top/gtnjzpvsvg.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yangfankeji.com/gtbuptytdr.html

[G04] 定义方法
来源：http://hz.ydzc1.top/gtqvkkclhz.html

Py:   def greet(self): return self.name
来源：http://hz.daria6918.cn/gttkwkwsrt.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.smart0.xyz/gtmouptllo.html

JS:   greet() { return this.name; }
来源：http://hz.ppjwa.cn/gttsvalcam.html

TS:   greet(): string { return this.name; }
来源：http://hz.gzhubu.top/gtflyxgose.html

Java: String greet() { return name; }
来源：http://hz.jqgufenzy.top/gtzhjnwhcj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.haohaochexian.top/gtrbdhitia.html

Ruby: def greet; @name; end
来源：http://hz.havefunace.top/gteiljuxkx.html

C#:   public string Greet() => Name;
来源：http://hz.birdmap.top/gtqcnxducs.html

[G05] 继承
来源：http://hz.xylfe.cn/gtyzmmnqhx.html

Py:   class Admin(User): pass
来源：http://hz.hnxiangtu.top/gtmxpqbafz.html

PHP:  class Admin extends User {}
来源：http://hz.feifeiyinyue.top/gtdghhdlvr.html

JS:   class Admin extends User {}
来源：http://hz.yvedp.cn/gthutocguq.html

TS:   class Admin extends User {}
来源：http://hz.gotoacloud.top/gtpogwwimc.html

Java: class Admin extends User {}
来源：http://hz.yj202588.top/gtnckgsyth.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.daria6918.cn/gtjejgjmqs.html

Ruby: class Admin < User; end
来源：http://hz.hnxiangtu.top/gthknttmmk.html

C#:   class Admin : User {}
来源：http://hz.ydzc1.top/gtzkplctmd.html

[G06] 重写方法
来源：http://hz.yangfankeji.com/gtsutfnqei.html

Py:   def greet(self): return "admin"
来源：http://hz.jyoumei.cn/gtgmeumebw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.fzhhl.top/gtzdtgczmq.html

JS:   greet() { return "admin"; }
来源：http://hz.9152youxi.cn/gtkdamqwlg.html

TS:   greet(): string { return "admin"; }
来源：http://hz.cheryme.top/gtbijccsol.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.zhiwuduotai.top/gttjzcocbk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.shanyushiyangkeji.top/gtpldpkhux.html

Ruby: def greet; "admin"; end
来源：http://hz.tian-w.cn/gtyypavted.html

C#:   public override string Greet() => "admin";
来源：http://hz.shuidangran.top/gtczlhojvw.html

[G07] 调用父类方法
来源：http://hz.gogol.net.cn/gtipmzqgnv.html

Py:   super().greet()
来源：http://hz.jinqigfzy.top/gtrmjavvfb.html

PHP:  parent::greet();
来源：http://hz.fengsongda.top/gtlkdeneze.html

JS:   super.greet();
来源：http://hz.wangdashe.top/gtgnswfhpp.html

TS:   super.greet();
来源：http://hz.gaohongyu789.top/gtthbbtwjy.html

Java: super.greet();
来源：http://hz.bjfxy.top/gtzkzrbzaa.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jiagoushi.top/gtdbmkyumz.html

Ruby: super
来源：http://hz.aibaodan.cn/gtxgwgziub.html

C#:   base.Greet();
来源：http://hz.fzhhl.top/gtgalogzpo.html

[G08] 静态方法与属性
来源：http://hz.hfpthk.cn/gtsprtrcht.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.ydzc1.top/gtelygrrqd.html

PHP:  public static function f() {}
来源：http://hz.xuetiantiany.cn/gtxlvnfity.html

JS:   static f() {}
来源：http://hz.jinqigufen.top/gtsaqbtrqd.html

TS:   static f(): void {}
来源：http://hz.gzhubu.top/gtbqvkplcc.html

Java: static void f() {}
来源：http://hz.daria6918.cn/gtyfjffusw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.cucudq.cn/gtvozmrasn.html

Ruby: def self.f; end
来源：http://hz.jiagoushi.top/gtfynkvjsq.html

C#:   public static void F() {}
来源：http://hz.hnqzz.top/gtdnskkwqt.html

[G09] 接口 / 抽象类
来源：http://hz.jianghu66.top/gtjezwcham.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.cashguo.top/gtzcuapjcc.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yj202588.top/gttpyvdccj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.hnxiangtu.top/gtxgvcwhyh.html

TS:   interface Shape { area(): number; }
来源：http://hz.zdqjudy.top/gteucrjhig.html

Java: interface Shape { double area(); }
来源：http://hz.zhongyouzk.top/gtqalyleix.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.redwolf501.top/gthinojoyj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.sufxvd.cn/gtpsoazjoe.html

C#:   interface IShape { double Area(); }
来源：http://hz.52xcode.cn/gtfbnbmbjt.html

[G10] 访问控制
来源：http://hz.pengpengdd.cyou/gtxrnkrfxc.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.zhixingplan.top/gtezsgdham.html

PHP:  public / protected / private
来源：http://hz.aibaodan.cn/gtdfjncdew.html

JS:   #private 字段；其余公开
来源：http://hz.cucudq.cn/gtszempuxy.html

TS:   public / protected / private
来源：http://hz.hongshengwenyu.top/gtjliltofr.html

Java: public / protected / private / 默认包级
来源：http://hz.cashguo.top/gtuhlvkahd.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zycfv.cn/gtfeyrndpv.html

Ruby: public / protected / private
来源：http://hz.jqgfzy.top/gtjfjhdgia.html


<!-- 参考信息 -->