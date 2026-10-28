代发 wailian999

Py:   for ch in s: print(ch)
来源：http://hz.hongshengwenyu.top/gtplzlzgma.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.zhaomingkeji.xyz/gtqqjzkrkv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.gogol.net.cn/gttrdndtjn.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zhiwuduotai.top/gtjbcndwav.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.mhx1999.top/gtepvaldtl.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.pengpengdd.cyou/gtpqoiiuvr.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.zhongyouzk.top/gtxamggoyy.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.hongshengwenyu.top/gtkjeswjlp.html

[E14] URL 编码与 Base64
来源：http://hz.52xcode.cn/gtqphobgxi.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.yj202588.top/gtccgzzlev.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.cucudq.cn/gttprowyor.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.yj20258888.top/gtrmzvrwba.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.hysaishi.cn/gtyxsrudre.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.shanyushiyangtech.top/gtpdtatcjn.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.snrcjt.cn/gtnygdjvdr.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.gogol.net.cn/gtmvkkpald.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.hnqzz.top/gtmjvkfhra.html

[E15] HTML 转义 / 反转义
来源：http://hz.redwolf501.top/gtnihsumak.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.xylfe.cn/gtgsufijjr.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.xziqi.cn/gtjvrairmg.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yongpay.top/gtcrjmlirl.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.gaohongyu789.top/gtgoawdnbu.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.guowangkeji.top/gtlmncygfi.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.iojbl.cn/gtzewwumhz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.gotoacloud.top/gtzlaxkgpe.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.jyoumei.cn/gtuomtkzgp.html

[E16] 数字千分位
来源：http://hz.daxiang520.top/gttpargfay.html

Py:   f"{1234567:,}"
来源：http://hz.daria6918.cn/gtzzpffjdx.html

PHP:  number_format(1234567);
来源：http://hz.jlsjyb.cn/gtiyopfbgh.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.yvedp.cn/gtafzoaywz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.chenzaomai.com/gtwoylutbw.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.meibo888.top/gtrbvbxpwc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.daxiang520.top/gtbfbydqbx.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.ivvv.top/gtpsfqjpxg.html

C#:   1234567.ToString("N0")
来源：http://hz.zhengqikj.top/gtjcopfwbi.html

[E17] 首字母大写
来源：http://hz.ydjk.org.cn/gtsopmtwvh.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.zhixingplan.top/gtdodlkrjk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.ydzc1.top/gtmhydgmyf.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.shuidangran.top/gtjjnwuirb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.hnxiangtu.top/gtipyjtlsx.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.sxryk.cn/gtalcismxw.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.nwbrower.top/gtfcsabiry.html

Ruby: s.capitalize
来源：http://hz.0kj1m.cn/gtsdaapgrt.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.kuanghao11.cn/gtaywvrylu.html

[E18] 模板占位符替换
来源：http://hz.xuanzx.com/gtbuhyxtji.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.c1oappe.top/gtpcijtjtw.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.zhoulong.xyz/gtgjytalye.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.shuidangran.top/gttjocgbdq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.mhx1999.top/gtdawcenjn.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.hammf.cn/gtqrqhfdew.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.gzhubu.top/gthwuoiivk.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.xingfuxueyuan.xyz/gtngfiuwsa.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.pycfn.com/gthbslauei.html

[E19] 多行文本按行拆分
来源：http://hz.snrcjt.cn/gtgorrvlpb.html

Py:   s.splitlines()
来源：http://hz.gotoacloud.top/gtkabrbzah.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.yj20258888.top/gtfaaqokty.html

JS:   s.split(/\r?\n/)
来源：http://hz.pycfn.com/gtmxyinjlp.html

TS:   s.split(/\r?\n/)
来源：http://hz.guowangkeji.top/gthaviaune.html

Java: s.lines().toList()
来源：http://hz.yangfankeji.com/gtjxjfkbid.html

Go:   strings.Split(s, "\n")
来源：http://hz.xylfe.cn/gtktejpisq.html

Ruby: s.lines
来源：http://hz.sweek.top/gtajtfebim.html

C#:   s.Split('\n')
来源：http://hz.redwolf501.top/gtphjqapzt.html

[E20] 判断字符串是否为空
来源：http://hz.ydzc1.top/gtglfzffub.html

Py:   if not s:
来源：http://hz.cqqwz.cn/gtghvxpsca.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.tanke756.top/gtqlxnwrap.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.hfpthk.cn/gtktqhpfnt.html

TS:   if (s === "") {}
来源：http://hz.chenlongwang.top/gtdwsnpzjn.html

Java: if (s.isEmpty()) {}
来源：http://hz.ppjwa.cn/gtlmgyvqpc.html

Go:   if s == "" {}
来源：http://hz.ywan-chungtsiang.top/gtbkdvejeh.html

Ruby: if s.empty?
来源：http://hz.hfpthk.cn/gthiiwhvnk.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.hywenlv.cn/gtcfolsjep.html

[E21] 超长截断加省略号
来源：http://hz.haohaochexian.top/gtwspgahqi.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.sysykeji.top/gtxkjurchm.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.nanxuanxn.top/gtkehrsnvs.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jinyuanbaomall.cn/gtxbkxqcns.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.redwolf501.top/gtzgczexie.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.gaohongyu789.top/gtphzmdbod.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.yuanzhike.top/gtvgotcety.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.shangyingyoupin.top/gtlbcrygqn.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.zhoulong.xyz/gtsubktiwq.html

[E22] 字节长度与字符长度
来源：http://hz.xinyue.icu/gtrikgzagm.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.smart0.xyz/gtvylcorsy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.vqdsnc.cn/gtcgcxvhvt.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.smart0.xyz/gtihbgxmek.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.guowangkeji.top/gtscgczuuc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.gogol.net.cn/gtlrxnjpdv.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.cheryme.top/gtwnqtandi.html

Ruby: s.bytesize;  s.length
来源：http://hz.xingfuxueyuan.xyz/gtmjcyiygs.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.xingfuxueyuan.xyz/gtenzbgkru.html

================================================================================
来源：http://hz.yvedp.cn/gtwqfkhjto.html

F. 文件与目录
来源：http://hz.wangdashe.top/gtqmudylsq.html

================================================================================
来源：http://hz.xziqi.cn/gtvwlzkonn.html

[F01] 读取整个文件
来源：http://hz.zhongyouzk.top/gtmvudeekn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.52xcode.cn/gtepwlxbwr.html

PHP:  file_get_contents("a.txt");
来源：http://hz.iojbl.cn/gtxglnwtcv.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.jlsjyb.cn/gtwwhtlzvx.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.sufxvd.cn/gtfmlpyqxe.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.snrcjt.cn/gtanngcflo.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.birdmap.top/gtqhhsapzt.html

Ruby: File.read("a.txt")
来源：http://hz.guowangkeji.top/gtoelfkqry.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.gaohongyu789.top/gtpjhxmkbh.html

[F02] 逐行读取文件
来源：http://hz.gaohongyu789.top/gtoioxzqbq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.sxryk.cn/gtdlcttgob.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.52xcode.cn/gtttgmlzql.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.shzxlz.cn/gtbspjegtv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ydjk.org.cn/gtyylpymsz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.316326.xyz/gttcvtfbxx.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.yongpay.top/gtokbmgykw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.tian-w.cn/gtdqgfcvqx.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.ydjk.org.cn/gtdxdenhax.html

[F03] 写入文件（覆盖）
来源：http://hz.ydzc1.top/gtqvdioogn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.chenlongwang.top/gtooschsat.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.gaohongyu789.top/gtdjaswzpr.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.guannengcc.top/gtibxnmfsr.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zycfv.cn/gtbzrlzwda.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.yuanzhike.top/gtelvmxqsz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.0kj1m.cn/gtacvnonyo.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.ywan-chungtsiang.top/gtdcsnbysu.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.ywan-chungtsiang.top/gtuycliomo.html

[F04] 追加写入文件
来源：http://hz.0kj1m.cn/gtrwnmgiin.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.xziqi.cn/gtirgsizta.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.shangyingyoupin.top/gtlsjfszgg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.guannengcc.top/gtffqppwro.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.gogol.net.cn/gtqtecnmeo.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.yj20258888.top/gtyydjswlq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.zhoulong.xyz/gtkoyplulb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.hysaishi.cn/gtzfpkmspt.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.xziqi.cn/gtegutwvbs.html

[F05] 判断文件或目录是否存在
来源：http://hz.hywenlv.cn/gtppfvytfi.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.sxryk.cn/gtppoxvltt.html

PHP:  file_exists("a.txt");
来源：http://hz.aibaodan.cn/gtcwywrlqw.html

JS:   fs.existsSync("a.txt")
来源：http://hz.cqqwz.cn/gtaehxjrjv.html

TS:   fs.existsSync("a.txt")
来源：http://hz.cashguo.top/gtrouzqwst.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.zhaomingkeji.xyz/gtxjszfrbf.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.gogol.net.cn/gtaoyjsvyh.html

Ruby: File.exist?("a.txt")
来源：http://hz.iojbl.cn/gtkprnolye.html

C#:   File.Exists("a.txt")
来源：http://hz.cashguo.top/gtgnqyrliv.html

[F06] 删除文件
来源：http://hz.yanxiufei.cn/gtmxgyijhu.html

Py:   os.remove("a.txt")
来源：http://hz.cheryme.top/gtpxxldzqu.html

PHP:  unlink("a.txt");
来源：http://hz.xinyue.icu/gtbhfwnggv.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.meibo888.top/gtntqnqynr.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.guowangkeji.top/gtegsawqzz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.nanxinkj.top/gtcvxbkymu.html

Go:   os.Remove("a.txt")
来源：http://hz.xylfe.cn/gtlizlefrp.html

Ruby: File.delete("a.txt")
来源：http://hz.yj202588.top/gtsxxsrcja.html

C#:   File.Delete("a.txt");
来源：http://hz.ehwqpu.com/gtobnjyjug.html

[F07] 创建目录（含多级）
来源：http://hz.ydjk.org.cn/gtaopntmxr.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.cheryme.top/gtolwyztyw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.tanke756.top/gtxplcmled.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.chenlongwang.top/gtbkukdcgy.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ppjwa.cn/gtiuectirh.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.0kj1m.cn/gteospznms.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.daria6918.cn/gtvzbvqnam.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.gzhubu.top/gtkroxqahj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.aibaodan.cn/gtikkdbtug.html

[F08] 遍历目录
来源：http://hz.shzxlz.cn/gtzlutxadt.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.iojbl.cn/gtbakltagc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.tanke756.top/gtrvhmsslc.html

JS:   fs.readdirSync("dir")
来源：http://hz.mhx1999.top/gtpbhcodge.html

TS:   fs.readdirSync("dir")
来源：http://hz.9152youxi.cn/gtfmcwaxuv.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.bjfxy.top/gtmqejukzv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.shanyushiyangkeji.top/gtvprmmivi.html

Ruby: Dir.children("dir")
来源：http://hz.zdqjudy.top/gtxnkzeuwu.html

C#:   Directory.GetFiles("dir")
来源：http://hz.chenzaomai.com/gtcjyriisq.html

[F09] 获取文件大小
来源：http://hz.zycfv.cn/gtwfbmlmrn.html

Py:   os.path.getsize("a.txt")
来源：http://hz.zhongyouzk.top/gtnfbabtxu.html

PHP:  filesize("a.txt");
来源：http://hz.xingfuxueyuan.xyz/gtihwiwbqz.html

JS:   fs.statSync("a.txt").size
来源：http://hz.sxryk.cn/gtzksldvwc.html

TS:   fs.statSync("a.txt").size
来源：http://hz.xziqi.cn/gtzwqozhoe.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.xuanzx.com/gtvntotooh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.zhiwuduotai.top/gtzndcxosf.html

Ruby: File.size("a.txt")
来源：http://hz.xuanzx.com/gtkrthqfye.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.316326.xyz/gtbtquvxyk.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.nwbrower.top/gtyvpokcmp.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jinqigufen.top/gtbwvwrqct.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.hnxiangtu.top/gtnnnpnamh.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.ydzc1.top/gtbqrvvohu.html

TS:   path.extname("a.txt")
来源：http://hz.smart0.xyz/gtpcriirgr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.nanxuanxn.top/gtkcldcawq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.ybcxt.top/gtduxbmgdg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.fengsongda.top/gtnrotlqbe.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.sufxvd.cn/gtzzplthkh.html

[F11] 复制与移动文件
来源：http://hz.zycfv.cn/gtunxvaztf.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.hysaishi.cn/gttijuebap.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yj20258.top/gtxwuqfmue.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.daxiang520.top/gtvyuhftdy.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.feifeiyinyue.top/gttqrxmiej.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.jinqigfzy.top/gteeqhluvj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.shanyushiyangtech.top/gtbxmsywrk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.dianchejie.cn/gtawbbxkdw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.ydzc1.top/gtypbwgerp.html

[F12] CSV 读写
来源：http://hz.hnqzz.top/gtvajtsqqa.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.xuanzx.com/gtdgvwkfbp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.shanyushiyangkeji.top/gtyaoxpuun.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.shanyushiyangtech.top/gtkshwzfyu.html

TS:   // 同上
来源：http://hz.svipenyu.cn/gtkhutnnfn.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.zdqjudy.top/gttshqcvkw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.mhx1999.top/gtjuilxdbg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.c1oappe.top/gtkkxmhacd.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.ydjk.org.cn/gtorvwylbt.html

================================================================================
来源：http://hz.vqdsnc.cn/gtsyjjcjfn.html

G. 面向对象
来源：http://hz.pycfn.com/gtndzitcjl.html

================================================================================
来源：http://hz.yanxiufei.cn/gtiqtqjmcj.html

[G01] 定义类
来源：http://hz.xziqi.cn/gtfofvsekd.html

Py:   class User: pass
来源：http://hz.guowangkeji.top/gtkfydzpgy.html

PHP:  class User {}
来源：http://hz.yvedp.cn/gtmwrusaia.html

JS:   class User {}
来源：http://hz.redwolf501.top/gtywudalwx.html

TS:   class User { name: string = ""; }
来源：http://hz.hammf.cn/gtwqxpfyim.html

Java: class User {}
来源：http://hz.jqgufenzy.top/gtwefwdnvi.html

Go:   type User struct { Name string }
来源：http://hz.nwbrower.top/gttathughr.html

Ruby: class User; end
来源：http://hz.yj202588.top/gtvtohojwe.html

C#:   class User {}
来源：http://hz.zhixingplan.top/gtiyqsqart.html

[G02] 构造函数
来源：http://hz.yonumen.top/gthozkapfa.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yueranfly.top/gtdackknxh.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.dianchejie.cn/gtnszgcvmk.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.jqgfzy.top/gtdlsvpifv.html

TS:   constructor(public name: string) {}
来源：http://hz.ivvv.top/gtrjeyqgpe.html

Java: User(String name) { this.name = name; }
来源：http://hz.fzhhl.top/gtxlyxkvhd.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.316326.xyz/gtcmoejbsp.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.aibaodan.cn/gtaizmnwsp.html

C#:   public User(string name) { Name = name; }
来源：http://hz.tanke756.top/gtorlmtijl.html

[G03] 实例属性
来源：http://hz.sxryk.cn/gtackmrlfr.html

Py:   self.name = "x"
来源：http://hz.pycfn.com/gtjsqlzraw.html

PHP:  public string $name = "x";
来源：http://hz.pycfn.com/gtcpqurjqc.html

JS:   this.name = "x";
来源：http://hz.tianlin.xyz/gtybiqlpkk.html

TS:   name: string = "x";
来源：http://hz.gogol.net.cn/gtlvnbruwy.html

Java: private String name;
来源：http://hz.tianlin.xyz/gtwstrhpkq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.cashguo.top/gtifnhojoj.html

Ruby: @name = "x"
来源：http://hz.chenlongwang.top/gttexwbbsk.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.sysykeji.top/gtehdcudyk.html

[G04] 定义方法
来源：http://hz.smart0.xyz/gtmmvvxbrz.html

Py:   def greet(self): return self.name
来源：http://hz.yj20258.top/gthskdzvgx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.guowangkeji.top/gtovcehacd.html

JS:   greet() { return this.name; }
来源：http://hz.shanyushiyangkeji.top/gtnqwjcves.html

TS:   greet(): string { return this.name; }
来源：http://hz.zhijiandao.cn/gtnhlmqqor.html

Java: String greet() { return name; }
来源：http://hz.daxiang520.top/gtbosztyfd.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.nanxinkj.top/gtfqxttabs.html

Ruby: def greet; @name; end
来源：http://hz.0kj1m.cn/gtdccrsajp.html

C#:   public string Greet() => Name;
来源：http://hz.jinqigufen.top/gtbabaovoi.html

[G05] 继承
来源：http://hz.jianghu66.top/gtfdsvjkjp.html

Py:   class Admin(User): pass
来源：http://hz.yuxming.cn/gtdywjytez.html

PHP:  class Admin extends User {}
来源：http://hz.jyoumei.cn/gtrzindjdi.html

JS:   class Admin extends User {}
来源：http://hz.nanxinkj.top/gtghypowdq.html

TS:   class Admin extends User {}
来源：http://hz.cheryme.top/gtvotwtvqb.html

Java: class Admin extends User {}
来源：http://hz.zhiwuduotai.top/gtbjsetegj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.xziqi.cn/gtwoqbwubx.html

Ruby: class Admin < User; end
来源：http://hz.jyoumei.cn/gtapqpurdn.html

C#:   class Admin : User {}
来源：http://hz.ehwqpu.com/gtgejrbicf.html

[G06] 重写方法
来源：http://hz.jinyuanbaomall.cn/gttbmqqqiz.html

Py:   def greet(self): return "admin"
来源：http://hz.hnqzz.top/gtgrfzmchu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jqgufenzy.top/gthevfpvcl.html

JS:   greet() { return "admin"; }
来源：http://hz.ivvv.top/gtqwoafqnt.html

TS:   greet(): string { return "admin"; }
来源：http://hz.nwbrower.top/gtbxwyqrgk.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.gaohongyu789.top/gtzgaaffpy.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.xuanzx.com/gtywbsutpu.html

Ruby: def greet; "admin"; end
来源：http://hz.sufxvd.cn/gtfkfhwzij.html

C#:   public override string Greet() => "admin";
来源：http://hz.shanyushiyangkeji.top/gtggooxtpk.html

[G07] 调用父类方法
来源：http://hz.haohaochexian.top/gtfgivbipe.html

Py:   super().greet()
来源：http://hz.xylfe.cn/gtunzdhmmj.html

PHP:  parent::greet();
来源：http://hz.daria6918.cn/gtzbqbpyuy.html

JS:   super.greet();
来源：http://hz.gotoacloud.top/gtlluftlmg.html

TS:   super.greet();
来源：http://hz.shangyingyoupin.top/gthrxuhacf.html

Java: super.greet();
来源：http://hz.xylfe.cn/gtkfgbnjbz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.daxiang520.top/gtkovrfhyx.html

Ruby: super
来源：http://hz.pengpengdd.cyou/gtbrxxjbbl.html

C#:   base.Greet();
来源：http://hz.jqgfzy.top/gtjjummcgn.html

[G08] 静态方法与属性
来源：http://hz.yonumen.top/gtedvkrmnp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.sufxvd.cn/gtlzrkarxc.html

PHP:  public static function f() {}
来源：http://hz.yj20258.top/gtrjstfflg.html

JS:   static f() {}
来源：http://hz.xinyue.icu/gtdqxgfxbs.html

TS:   static f(): void {}
来源：http://hz.kuanghao11.cn/gtdtubgpqi.html

Java: static void f() {}
来源：http://hz.cheryme.top/gtlrbxnlig.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.snrcjt.cn/gtsuoxbgqf.html

Ruby: def self.f; end
来源：http://hz.ivvv.top/gtpcsdhnpo.html

C#:   public static void F() {}
来源：http://hz.wangshuangyany.cn/gtsjjgnrsr.html

[G09] 接口 / 抽象类
来源：http://hz.jinqigufen.top/gtyakunjit.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.hnxiangtu.top/gtbmeezasp.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.pycfn.com/gttetrsjgt.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.sweek.top/gtvedxqigi.html

TS:   interface Shape { area(): number; }
来源：http://hz.ydjk.org.cn/gtawicrcbd.html

Java: interface Shape { double area(); }
来源：http://hz.bjfxy.top/gtpjwmxepp.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.jinyuanbaomall.cn/gtxqqvwetr.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.meibo888.top/gtdpgskxoh.html

C#:   interface IShape { double Area(); }
来源：http://hz.zhixingplan.top/gtawsjwqwm.html

[G10] 访问控制
来源：http://hz.yongpay.top/gtnhzrhjla.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.pengpengdd.cyou/gttqappsbu.html

PHP:  public / protected / private
来源：http://hz.gogol.net.cn/gtipndiehi.html

JS:   #private 字段；其余公开
来源：http://hz.zdqjudy.top/gtwntpuiph.html

TS:   public / protected / private
来源：http://hz.redwolf501.top/gtbsukhahd.html

Java: public / protected / private / 默认包级
来源：http://hz.yonumen.top/gtppellgot.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.jqgufenzy.top/gtpfdevurr.html

Ruby: public / protected / private
来源：http://hz.tian-w.cn/gtjtrcpvct.html

C#:   public / protected / private / internal
来源：http://hz.daxiang520.top/gtjyptrevi.html

[G11] getter / setter
来源：http://hz.aizwys.cn/gtjaongrti.html

Py:   @property 与 @x.setter
来源：http://hz.jiagoushi.top/gtcywpbawc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.c1oappe.top/gtegbpevgd.html

JS:   get name() { return this._name; }
来源：http://hz.316326.xyz/gtatlwtixb.html

TS:   get name(): string { return this._name; }
来源：http://hz.yj202588.top/gtxpncxwha.html

Java: public String getName() { return name; }
来源：http://hz.quarkkingdee.top/gtnbqycqek.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.sysykeji.top/gtvwbckahy.html


<!-- 参考信息 -->