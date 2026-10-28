代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://hz.zhiwuduotai.top/gtqnhbqfaa.html

Java: String.format("%03d", 7)
来源：http://hz.tian-w.cn/gtimlansgs.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.chenzaomai.com/gtuuagmtzh.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.gaohongyu789.top/gticatgcva.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.meibo888.top/gtjdssgikk.html

[E11] 反转字符串
来源：http://hz.ppjwa.cn/gtpcllblbu.html

Py:   s[::-1]
来源：http://hz.vqdsnc.cn/gtzakrcomp.html

PHP:  strrev($s);
来源：http://hz.dashuyun.cn/gtchbngewv.html

JS:   [...s].reverse().join("")
来源：http://hz.daxiang520.top/gtewdvizpb.html

TS:   [...s].reverse().join("")
来源：http://hz.chenjidiqi.icu/gtoflxgnrt.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.jqgufenzy.top/gtailflryj.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.svipenyu.cn/gtftjsjnlm.html

Ruby: s.reverse
来源：http://hz.sxryk.cn/gtzfjzrnpk.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.chenzaomai.com/gtnkqsmvln.html

[E12] 统计某字符出现次数
来源：http://hz.9152youxi.cn/gtkcwiajlt.html

Py:   s.count("a")
来源：http://hz.haohaochexian.top/gtoglzlxog.html

PHP:  substr_count($s, "a");
来源：http://hz.hongshengwenyu.top/gtupxgtjkc.html

JS:   s.split("a").length - 1
来源：http://hz.gaohongyu789.top/gtsssocncx.html

TS:   s.split("a").length - 1
来源：http://hz.c1oappe.top/gtpdetvfci.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.ybcxt.top/gtczwxhymz.html

Go:   strings.Count(s, "a")
来源：http://hz.shuidangran.top/gtbmkiuwlt.html

Ruby: s.count("a")
来源：http://hz.jinyuanbaomall.cn/gthebpzprz.html

C#:   s.Count(c => c == 'a')
来源：http://hz.jinghuilouyu.cn/gtoscbhngq.html

[E13] 逐字符遍历
来源：http://hz.iojbl.cn/gtwstvvmqe.html

Py:   for ch in s: print(ch)
来源：http://hz.hfpthk.cn/gtscalleyn.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.cqqwz.cn/gtruevkkhd.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.aizwys.cn/gtirolubcw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.havefunace.top/gtuddkidfi.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.yj20258.top/gtoqziytlc.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.shanyushiyangkeji.top/gtayagkqti.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.chenjidiqi.icu/gtsmdopytg.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.cashguo.top/gtjtlowjsh.html

[E14] URL 编码与 Base64
来源：http://hz.dianchejie.cn/gtvwqbxpar.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.cucudq.cn/gtimflsxrd.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.zhoulong.xyz/gtdhokaafj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.jinqigfzy.top/gttgdfnkue.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.sxryk.cn/gtdryostvl.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.zhoulong.xyz/gtikxgvfxa.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.daria6918.cn/gtuxkfxpwl.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.cdnleiting.top/gtfvlldnxq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.zhengqikj.top/gtmjebnbzo.html

[E15] HTML 转义 / 反转义
来源：http://hz.birdmap.top/gtjhmvajud.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.0kj1m.cn/gtwpyzhoyn.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.zhongyouzk.top/gturswbssg.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.haohaochexian.top/gthakdnirm.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.sxryk.cn/gtydtuccor.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.jianghu66.top/gtveckjavz.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.tianlin.xyz/gtkzrcodvu.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.sysykeji.top/gtvufbiuzm.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.xylfe.cn/gtpqzamidd.html

[E16] 数字千分位
来源：http://hz.yongpay.top/gtrjfxpief.html

Py:   f"{1234567:,}"
来源：http://hz.guannengcc.top/gtrncfdtse.html

PHP:  number_format(1234567);
来源：http://hz.0kj1m.cn/gtnvxlkaam.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.hnqzz.top/gtzmpijimi.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhongyouzk.top/gtmfpbqwlr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.jinqigfzy.top/gtbrlvmqfj.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.hammf.cn/gtlwiyavbl.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.shanyushiyangtech.top/gtinhiqrur.html

C#:   1234567.ToString("N0")
来源：http://hz.jqgfzy.top/gtjrpqzztn.html

[E17] 首字母大写
来源：http://hz.nanxuanxn.top/gtlyhozspd.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.tanke756.top/gtksfrpdhk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.fzhhl.top/gtjtairgzb.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.hnqzz.top/gthvouclip.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.cucudq.cn/gtqjgqcryf.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.redwolf501.top/gtxpvlthcw.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.xuanzx.com/gtfmwipnvc.html

Ruby: s.capitalize
来源：http://hz.yj20258888.top/gtyyrqviyi.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.svipenyu.cn/gtuxslamia.html

[E18] 模板占位符替换
来源：http://hz.wangshuangyany.cn/gtdtxrdzgh.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.jqgufenzy.top/gtxrybuqrb.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.wangdashe.top/gtvyquuzwm.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.9152youxi.cn/gtbttzjyqe.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.wangdashe.top/gtidpmrqdi.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.cashguo.top/gtkjaoowly.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.yj20258888.top/gterjwaycr.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.hongshengwenyu.top/gtlepjfhjb.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.xuetiantiany.cn/gtmmmlrdnb.html

[E19] 多行文本按行拆分
来源：http://hz.redwolf501.top/gtycjghzka.html

Py:   s.splitlines()
来源：http://hz.zhiwuduotai.top/gtqjwffqfd.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.daxiang520.top/gteaqqhqvb.html

JS:   s.split(/\r?\n/)
来源：http://hz.zhijiandao.cn/gtzgxgybnc.html

TS:   s.split(/\r?\n/)
来源：http://hz.ivvv.top/gtnomrsyxa.html

Java: s.lines().toList()
来源：http://hz.yueranfly.top/gtjmnpydog.html

Go:   strings.Split(s, "\n")
来源：http://hz.jinyuanbaomall.cn/gtqvtklprz.html

Ruby: s.lines
来源：http://hz.52xcode.cn/gtahocydyw.html

C#:   s.Split('\n')
来源：http://hz.sweek.top/gtvhuqtbqb.html

[E20] 判断字符串是否为空
来源：http://hz.sysykeji.top/gtymwnlvbq.html

Py:   if not s:
来源：http://hz.yonumen.top/gtlejiarcg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.pycfn.com/gtcdygypro.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.yj202588.top/gtfcmwonvj.html

TS:   if (s === "") {}
来源：http://hz.feifeiyinyue.top/gtuwdamwzy.html

Java: if (s.isEmpty()) {}
来源：http://hz.smart0.xyz/gtbbnqigrf.html

Go:   if s == "" {}
来源：http://hz.xylfe.cn/gtwrtwouvc.html

Ruby: if s.empty?
来源：http://hz.cqqwz.cn/gtdqplcgvv.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.pengpengdd.cyou/gtkqkcdhjq.html

[E21] 超长截断加省略号
来源：http://hz.cucudq.cn/gtuwnhzkfr.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.guowangkeji.top/gtwcitfgxq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.meibo888.top/gtmybrlkvk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhixingplan.top/gtrovlhphd.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ywan-chungtsiang.top/gtltjflkav.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.vqdsnc.cn/gtlhrrunql.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.cqqwz.cn/gtjvxppnot.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.jlsjyb.cn/gtbgvvinjy.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.jinqigfzy.top/gtbjesywrj.html

[E22] 字节长度与字符长度
来源：http://hz.jlsjyb.cn/gtnqxbkntx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.shzxlz.cn/gteaysmovv.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.hongshengwenyu.top/gtfxayomhf.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jinqigufen.top/gtnvmuqjdq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.mhx1999.top/gtartujeal.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.nanxinkj.top/gtmrxkmliv.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.shzxlz.cn/gthwnqtjmj.html

Ruby: s.bytesize;  s.length
来源：http://hz.guowangkeji.top/gtdbolniuk.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.hfpthk.cn/gtrcunuecs.html

================================================================================
来源：http://hz.gogol.net.cn/gtcwotxpkh.html

F. 文件与目录
来源：http://hz.yonumen.top/gtcqzwyltn.html

================================================================================
来源：http://hz.jqgufenzy.top/gtjxtxcslf.html

[F01] 读取整个文件
来源：http://hz.wangdashe.top/gtesbzlhty.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.meibo888.top/gtprtotpyc.html

PHP:  file_get_contents("a.txt");
来源：http://hz.mhx1999.top/gtmnmvvvku.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.mhx1999.top/gtrmeelgyf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.yvedp.cn/gtxawcifyc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.jinghuilouyu.cn/gtbfpstuee.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.316326.xyz/gtkordrucq.html

Ruby: File.read("a.txt")
来源：http://hz.mhx1999.top/gtkwmbcmjp.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.ydzc1.top/gtcjrzgikk.html

[F02] 逐行读取文件
来源：http://hz.wangdashe.top/gtlfvtvieq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.jinyuanbaomall.cn/gtqrzomibd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.jyoumei.cn/gtruizhvpl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.svipenyu.cn/gtbhsjnzcu.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xziqi.cn/gtnrlzeyvl.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.jinghuilouyu.cn/gtvfmwrtdu.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.yj202588.top/gtcbmcqgcl.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yuanzhike.top/gtgnkpynob.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.sweek.top/gtoionfibh.html

[F03] 写入文件（覆盖）
来源：http://hz.svipenyu.cn/gtliqekgdq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.hysaishi.cn/gttmwhkwoa.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.tian-w.cn/gtxrlhrbeb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.aizwys.cn/gtqbrjbffy.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.52xcode.cn/gtynroqeix.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.zhoulong.xyz/gtcrmrgcud.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.nwbrower.top/gtcfggxewb.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.jqgfzy.top/gtcaphephz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.vqdsnc.cn/gtuhaqbnkd.html

[F04] 追加写入文件
来源：http://hz.xinyue.icu/gthmoiavna.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.smart0.xyz/gttozkfjuq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.ydzc1.top/gtbivcnwkl.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.sxryk.cn/gtaawolmkr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhongyouzk.top/gtkdbscotq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.snrcjt.cn/gttzzwwpdv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.sweek.top/gtjyogszjg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.jinyuanbaomall.cn/gtkmsemjfz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.xuanzx.com/gtnuftuqqy.html

[F05] 判断文件或目录是否存在
来源：http://hz.nanxuanxn.top/gtvxldqzbr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.hysaishi.cn/gtkabwghbb.html

PHP:  file_exists("a.txt");
来源：http://hz.gogol.net.cn/gtertzfhlb.html

JS:   fs.existsSync("a.txt")
来源：http://hz.chenzaomai.com/gtnokatukl.html

TS:   fs.existsSync("a.txt")
来源：http://hz.gogol.net.cn/gtyycrakks.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.pengpengdd.cyou/gtatplvhia.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.yuxming.cn/gtolinoyfc.html

Ruby: File.exist?("a.txt")
来源：http://hz.hywenlv.cn/gtnchsaecw.html

C#:   File.Exists("a.txt")
来源：http://hz.guowangkeji.top/gtalfobxwv.html

[F06] 删除文件
来源：http://hz.zhongyouzk.top/gtjxqzkhjo.html

Py:   os.remove("a.txt")
来源：http://hz.jyoumei.cn/gtgiqipzgi.html

PHP:  unlink("a.txt");
来源：http://hz.0kj1m.cn/gthnzeytpw.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yueranfly.top/gttvgsxdvk.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.ywan-chungtsiang.top/gtoiczrcmi.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.hfpthk.cn/gtposcwghw.html

Go:   os.Remove("a.txt")
来源：http://hz.nanxinkj.top/gtwznglnoj.html

Ruby: File.delete("a.txt")
来源：http://hz.jyoumei.cn/gtqmvonpkk.html

C#:   File.Delete("a.txt");
来源：http://hz.mhx1999.top/gtlmuxrjnc.html

[F07] 创建目录（含多级）
来源：http://hz.guannengcc.top/gttoooaidl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.snrcjt.cn/gtcdgjuxam.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.jianghu66.top/gttlhujjjo.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.dianchejie.cn/gtpjzdnocm.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yj20258888.top/gtlrcjutyc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.chenjidiqi.icu/gtirlhzslx.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jyoumei.cn/gtktrtbotv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.gotoacloud.top/gtiwqcjjmk.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.ywan-chungtsiang.top/gtkderhspn.html

[F08] 遍历目录
来源：http://hz.fzhhl.top/gtugsyxduv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yj20258888.top/gtwygcgrms.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.jlsjyb.cn/gtccewrkes.html

JS:   fs.readdirSync("dir")
来源：http://hz.mhx1999.top/gtkreivias.html

TS:   fs.readdirSync("dir")
来源：http://hz.tianlin.xyz/gtcnaoteel.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.nanxinkj.top/gtuadvzjya.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.jinyuanbaomall.cn/gtbuysfqbh.html

Ruby: Dir.children("dir")
来源：http://hz.yj202588.top/gtoxygnsoq.html

C#:   Directory.GetFiles("dir")
来源：http://hz.sufxvd.cn/gtaekaoltn.html

[F09] 获取文件大小
来源：http://hz.daxiang520.top/gtijbowzgt.html

Py:   os.path.getsize("a.txt")
来源：http://hz.wangshuangyany.cn/gtgtxgwnas.html

PHP:  filesize("a.txt");
来源：http://hz.ivvv.top/gtnlytknie.html

JS:   fs.statSync("a.txt").size
来源：http://hz.cdnleiting.top/gtorffbvax.html

TS:   fs.statSync("a.txt").size
来源：http://hz.yongpay.top/gtzaidihlo.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.sxryk.cn/gtlxbzyows.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.ydzc1.top/gtgkwfdqqm.html

Ruby: File.size("a.txt")
来源：http://hz.jinghuilouyu.cn/gtkudatvfk.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.quarkkingdee.top/gtagvtgkpf.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.ivvv.top/gteurrrgtx.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.zhijiandao.cn/gtdfqikrpp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.xuanzx.com/gtjupbkuxl.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.bjfxy.top/gthspsesyn.html

TS:   path.extname("a.txt")
来源：http://hz.zhiwuduotai.top/gtcompkssz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.daria6918.cn/gtzmeudmrm.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.hfpthk.cn/gtmwdzycnv.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.zhongyouzk.top/gtslbkardn.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.tian-w.cn/gthffwghsa.html

[F11] 复制与移动文件
来源：http://hz.zhaomingkeji.xyz/gtrfhytufw.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.cqqwz.cn/gtwqqevpbc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.shanyushiyangkeji.top/gtwoyoyfyg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.kuanghao11.cn/gtwvvlgykk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ppjwa.cn/gteufjurrn.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.yongpay.top/gtdhxjltpu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.snrcjt.cn/gtmhqudpkc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.jinqigufen.top/gtoehtwgpz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.zhengqikj.top/gtvwfewchf.html

[F12] CSV 读写
来源：http://hz.316326.xyz/gttvpgqmjz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.chenzaomai.com/gttfelcfim.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.chenjidiqi.icu/gtsunciatt.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.meibo888.top/gtohcrrlzr.html

TS:   // 同上
来源：http://hz.ppjwa.cn/gtaqczmiyv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.zdqjudy.top/gtoosgeumv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.daxiang520.top/gtdaaozbih.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.yangfankeji.com/gtgyqkkcvn.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.shuidangran.top/gtpnhsvkki.html

================================================================================
来源：http://hz.guannengcc.top/gtraalzkbt.html

G. 面向对象
来源：http://hz.yueranfly.top/gtockasugq.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtqgltuyzx.html

[G01] 定义类
来源：http://hz.jyoumei.cn/gtzkacwogo.html

Py:   class User: pass
来源：http://hz.hnqzz.top/gtufrlpbre.html

PHP:  class User {}
来源：http://hz.hnqzz.top/gtrsuooxal.html

JS:   class User {}
来源：http://hz.pengpengdd.cyou/gterfdsral.html

TS:   class User { name: string = ""; }
来源：http://hz.pengpengdd.cyou/gtymrvjygr.html

Java: class User {}
来源：http://hz.aibaodan.cn/gtxlsegyoi.html

Go:   type User struct { Name string }
来源：http://hz.yanxiufei.cn/gtixntmaia.html

Ruby: class User; end
来源：http://hz.jinghuilouyu.cn/gtjursuxgt.html

C#:   class User {}
来源：http://hz.9152youxi.cn/gtppqyehcz.html

[G02] 构造函数
来源：http://hz.cqqwz.cn/gtjmbxsqlz.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.ivvv.top/gthmxdiwix.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.cqqwz.cn/gtuyhsitbu.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.wangdashe.top/gtxoeaalmb.html

TS:   constructor(public name: string) {}
来源：http://hz.ywan-chungtsiang.top/gttysssqsg.html

Java: User(String name) { this.name = name; }
来源：http://hz.nwbrower.top/gtbxujasns.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.sxryk.cn/gtaukrouxm.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yuxming.cn/gtwrprhyuz.html

C#:   public User(string name) { Name = name; }
来源：http://hz.xuanzx.com/gthuahjznr.html

[G03] 实例属性
来源：http://hz.hongshengwenyu.top/gtqgkfxxlb.html

Py:   self.name = "x"
来源：http://hz.chenzaomai.com/gtayrwrruq.html

PHP:  public string $name = "x";
来源：http://hz.zycfv.cn/gtrlkmnxxt.html

JS:   this.name = "x";
来源：http://hz.sxryk.cn/gtqxozzsdy.html

TS:   name: string = "x";
来源：http://hz.feifeiyinyue.top/gtqfciqzwj.html

Java: private String name;
来源：http://hz.cqqwz.cn/gtlhbzmtto.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.zhiwuduotai.top/gtegtqbxnl.html

Ruby: @name = "x"
来源：http://hz.cucudq.cn/gtppxklbcs.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.hfpthk.cn/gtcnbrkcqs.html

[G04] 定义方法
来源：http://hz.jyoumei.cn/gthgtxsuxn.html

Py:   def greet(self): return self.name
来源：http://hz.yj202588.top/gtghzqsbkb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yj20258.top/gtxakwdreh.html

JS:   greet() { return this.name; }
来源：http://hz.52xcode.cn/gtlqlhpnbx.html

TS:   greet(): string { return this.name; }
来源：http://hz.hfpthk.cn/gtuehexrsn.html

Java: String greet() { return name; }
来源：http://hz.gogol.net.cn/gtybjveshy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.ydzc1.top/gttfpkymrd.html

Ruby: def greet; @name; end
来源：http://hz.gogol.net.cn/gttxfaoqmn.html

C#:   public string Greet() => Name;
来源：http://hz.aizwys.cn/gttzwuqutt.html

[G05] 继承
来源：http://hz.havefunace.top/gtnbfcszqu.html

Py:   class Admin(User): pass
来源：http://hz.smart0.xyz/gthqmmhnlu.html

PHP:  class Admin extends User {}
来源：http://hz.haohaochexian.top/gtmmrejptf.html

JS:   class Admin extends User {}
来源：http://hz.hnxiangtu.top/gtwyfescyn.html

TS:   class Admin extends User {}
来源：http://hz.kuanghao11.cn/gtkzwoxsry.html

Java: class Admin extends User {}
来源：http://hz.smart0.xyz/gtteiktrdn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.sweek.top/gtzjlupkrd.html

Ruby: class Admin < User; end
来源：http://hz.gotoacloud.top/gtycntscoa.html

C#:   class Admin : User {}
来源：http://hz.fzhhl.top/gtobagpytx.html

[G06] 重写方法
来源：http://hz.cqqwz.cn/gtelzxkecs.html

Py:   def greet(self): return "admin"
来源：http://hz.shuidangran.top/gtkvhtvija.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.zhiwuduotai.top/gtbinenjyc.html

JS:   greet() { return "admin"; }
来源：http://hz.vqdsnc.cn/gtzitbqnax.html

TS:   greet(): string { return "admin"; }
来源：http://hz.chenlongwang.top/gtilmhzvok.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jqgfzy.top/gtaofqmafh.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zhengqikj.top/gtnlwpnabe.html

Ruby: def greet; "admin"; end
来源：http://hz.dashuyun.cn/gtxmdlfwcy.html

C#:   public override string Greet() => "admin";
来源：http://hz.shuidangran.top/gtkksjjhgb.html

[G07] 调用父类方法
来源：http://hz.c1oappe.top/gtxsotshrk.html

Py:   super().greet()
来源：http://hz.nwbrower.top/gtxndmsnec.html

PHP:  parent::greet();
来源：http://hz.guannengcc.top/gtwolfebmq.html

JS:   super.greet();
来源：http://hz.ydzc1.top/gtbjyybtpn.html

TS:   super.greet();
来源：http://hz.aizwys.cn/gtkjgxodev.html

Java: super.greet();
来源：http://hz.cheryme.top/gtmqlrptpa.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.hongshengwenyu.top/gtqfoonlqk.html

Ruby: super
来源：http://hz.hfpthk.cn/gtrjuqgiok.html

C#:   base.Greet();
来源：http://hz.birdmap.top/gtevnexoov.html

[G08] 静态方法与属性
来源：http://hz.guowangkeji.top/gtejfhlvdu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.shzxlz.cn/gtqykphnfm.html

PHP:  public static function f() {}
来源：http://hz.yj20258.top/gtalxpdehs.html

JS:   static f() {}
来源：http://hz.andypj.xyz/gtjpbpthva.html

TS:   static f(): void {}
来源：http://hz.hongshengwenyu.top/gtntoljhrv.html

Java: static void f() {}
来源：http://hz.yuxming.cn/gtzovugsuu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.tanke756.top/gtwzorndmu.html

Ruby: def self.f; end
来源：http://hz.xinyue.icu/gtzvfxlzwk.html

C#:   public static void F() {}
来源：http://hz.shangyingyoupin.top/gtsbqsirpz.html

[G09] 接口 / 抽象类
来源：http://hz.jqgfzy.top/gtwllhstpc.html


<!-- 参考信息 -->