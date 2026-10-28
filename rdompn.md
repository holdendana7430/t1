代发 wailian999

Ruby: s.reverse
来源：http://hz.tian-w.cn/gtwdevqedy.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.haohaochexian.top/gtqjwfkitq.html

[E12] 统计某字符出现次数
来源：http://hz.tianlin.xyz/gttqgnutat.html

Py:   s.count("a")
来源：http://hz.tanke756.top/gtpvibumkn.html

PHP:  substr_count($s, "a");
来源：http://hz.daxiang520.top/gtypaszlwp.html

JS:   s.split("a").length - 1
来源：http://hz.nanxinkj.top/gtapvetkbe.html

TS:   s.split("a").length - 1
来源：http://hz.fzhhl.top/gtdnrsgpjg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.gotoacloud.top/gtrbqncqpi.html

Go:   strings.Count(s, "a")
来源：http://hz.cqqwz.cn/gtudtzolup.html

Ruby: s.count("a")
来源：http://hz.shanyushiyangkeji.top/gtqaalxkpt.html

C#:   s.Count(c => c == 'a')
来源：http://hz.meibo888.top/gtqbgntxaq.html

[E13] 逐字符遍历
来源：http://hz.jiagoushi.top/gtefwgfpnx.html

Py:   for ch in s: print(ch)
来源：http://hz.daxiang520.top/gtkfeudlhq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.gogol.net.cn/gtkqwowber.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.chenzaomai.com/gtrkjcrmpw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zycfv.cn/gtlrzefetl.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.cashguo.top/gttnnuhdvk.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.cashguo.top/gtqobaupbo.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.xuetiantiany.cn/gtijhkytut.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.chenlongwang.top/gtkjuobgel.html

[E14] URL 编码与 Base64
来源：http://hz.sysykeji.top/gtwhmcicsl.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.shuidangran.top/gtkjyettzo.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.mhx1999.top/gtupfjlxgi.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.gzhubu.top/gtydwvtloj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.yongpay.top/gtzulwjxaa.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.hongshengwenyu.top/gttynmciym.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.gzhubu.top/gtihpylqou.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.snrcjt.cn/gtfsyzsfdl.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.jianghu66.top/gtzyiqnjsj.html

[E15] HTML 转义 / 反转义
来源：http://hz.redwolf501.top/gtxqixmogx.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.quarkkingdee.top/gtuzzokrkq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.sufxvd.cn/gtzmucwmcm.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yvedp.cn/gtjyzgrcou.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.jyoumei.cn/gtiwyrfofx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.gogol.net.cn/gtkvkhfuwq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.xziqi.cn/gtzgfazsle.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.cqqwz.cn/gtrcvqqpbz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.gotoacloud.top/gtgrpluktt.html

[E16] 数字千分位
来源：http://hz.xziqi.cn/gtemftmshi.html

Py:   f"{1234567:,}"
来源：http://hz.cashguo.top/gtzwfojghi.html

PHP:  number_format(1234567);
来源：http://hz.aibaodan.cn/gtshpylyac.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.pycfn.com/gtqqmlgueb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.snrcjt.cn/gtowwfdzae.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.jinyuanbaomall.cn/gtmcqpxdql.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.yj20258.top/gtvjiiabaa.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.zhijiandao.cn/gthhuqmxbn.html

C#:   1234567.ToString("N0")
来源：http://hz.chenjidiqi.icu/gtmpjhweef.html

[E17] 首字母大写
来源：http://hz.cdnleiting.top/gtlggmznff.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.zhaomingkeji.xyz/gtmhjuljba.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.andypj.xyz/gtzjiodpvs.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.shanyushiyangkeji.top/gtybyakxuh.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.shanyushiyangtech.top/gtnwjxknrw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.cashguo.top/gtpukzncwc.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.jinghuilouyu.cn/gtothfeylj.html

Ruby: s.capitalize
来源：http://hz.shzxlz.cn/gtelmbzeia.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.feifeiyinyue.top/gtmawqvbcb.html

[E18] 模板占位符替换
来源：http://hz.kuanghao11.cn/gtqfgqxhvz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.kuanghao11.cn/gtwmwakvod.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.yongpay.top/gtcnhakale.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.zhijiandao.cn/gtqvtjfrtf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.316326.xyz/gtqzlyctcm.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.gotoacloud.top/gtqnaurpzy.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.tianlin.xyz/gtzbrkxfrc.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.aibaodan.cn/gtubuptdqz.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.aibaodan.cn/gthcumfbjq.html

[E19] 多行文本按行拆分
来源：http://hz.zhaomingkeji.xyz/gtnarkpqmt.html

Py:   s.splitlines()
来源：http://hz.yongpay.top/gtflqaoiuu.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.birdmap.top/gtvfxedmht.html

JS:   s.split(/\r?\n/)
来源：http://hz.gotoacloud.top/gtzqppthhc.html

TS:   s.split(/\r?\n/)
来源：http://hz.yuxming.cn/gtewdmkour.html

Java: s.lines().toList()
来源：http://hz.jlsjyb.cn/gtfxyvsgbi.html

Go:   strings.Split(s, "\n")
来源：http://hz.0kj1m.cn/gthnutowbb.html

Ruby: s.lines
来源：http://hz.jqgfzy.top/gtdsgprjja.html

C#:   s.Split('\n')
来源：http://hz.snrcjt.cn/gtduvvkxks.html

[E20] 判断字符串是否为空
来源：http://hz.yanxiufei.cn/gtxdwuxzzu.html

Py:   if not s:
来源：http://hz.gaohongyu789.top/gtzfdvnsen.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.yj202588.top/gtabcbsjtp.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.9152youxi.cn/gthqfbkecx.html

TS:   if (s === "") {}
来源：http://hz.daria6918.cn/gtzvdasamc.html

Java: if (s.isEmpty()) {}
来源：http://hz.birdmap.top/gtsalfqllu.html

Go:   if s == "" {}
来源：http://hz.vqdsnc.cn/gtrjqqdsah.html

Ruby: if s.empty?
来源：http://hz.zhongyouzk.top/gtbghclskd.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.meibo888.top/gtziskoxxc.html

[E21] 超长截断加省略号
来源：http://hz.xuanzx.com/gttdxampjf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.zhoulong.xyz/gtnuivhnxe.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.zdqjudy.top/gtijszmypz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.tian-w.cn/gtipyoqdxr.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.pycfn.com/gttypowkea.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.zhixingplan.top/gtqycjwuyc.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.jinqigfzy.top/gtfoyempaj.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.nanxuanxn.top/gtlgmyexgo.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.jiagoushi.top/gtxuhwddzr.html

[E22] 字节长度与字符长度
来源：http://hz.0kj1m.cn/gtcljpygwb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.sysykeji.top/gtprxgxdcb.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.nwbrower.top/gtxoijiynx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.vqdsnc.cn/gtiaxrtavd.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.xingfuxueyuan.xyz/gtisirzrtl.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jinqigfzy.top/gtovtkqynf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.hammf.cn/gtjwkvynmj.html

Ruby: s.bytesize;  s.length
来源：http://hz.yueranfly.top/gtpjymhvrm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.hongshengwenyu.top/gtjvatethe.html

================================================================================
来源：http://hz.hfpthk.cn/gtrnhkxhbx.html

F. 文件与目录
来源：http://hz.jyoumei.cn/gtqzpbxkvx.html

================================================================================
来源：http://hz.iojbl.cn/gtbtitfqbk.html

[F01] 读取整个文件
来源：http://hz.jqgfzy.top/gtddpigvsw.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.guannengcc.top/gtluqthxuq.html

PHP:  file_get_contents("a.txt");
来源：http://hz.mhx1999.top/gtfdzriyik.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.yj20258888.top/gtaxtnoxhy.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.bjfxy.top/gtqmdxkqfq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.jlsjyb.cn/gtjgfaqbtc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.ivvv.top/gtcyvcfplu.html

Ruby: File.read("a.txt")
来源：http://hz.nanxinkj.top/gthweugphm.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.hnqzz.top/gtsnqzxbxx.html

[F02] 逐行读取文件
来源：http://hz.redwolf501.top/gtytwjcgpp.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.pycfn.com/gtcsiwqbhk.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.c1oappe.top/gtzigtwjvo.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ehwqpu.com/gtmiborgbl.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xingfuxueyuan.xyz/gtzyitxfzt.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.hammf.cn/gtpgutjcnu.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.shangyingyoupin.top/gtbatgwftb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.fzhhl.top/gttfpsyizb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.gaohongyu789.top/gtrjeubyzq.html

[F03] 写入文件（覆盖）
来源：http://hz.0kj1m.cn/gtcsyyqamk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.ydjk.org.cn/gtxkkbgfps.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.gotoacloud.top/gtwrohstua.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ydzc1.top/gtfquweozx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.svipenyu.cn/gtqzczgtfe.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.jiagoushi.top/gtwrcciwjw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.ydzc1.top/gtbhcvpltw.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.yvedp.cn/gtijkdjopd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.pengpengdd.cyou/gtrejktteh.html

[F04] 追加写入文件
来源：http://hz.zhengqikj.top/gtcmjzfalj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yj20258888.top/gtwsfbkctt.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.nanxinkj.top/gttqaftcnd.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.andypj.xyz/gtxmltbfvn.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.cheryme.top/gtwzbloeff.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.jqgufenzy.top/gtupxhyyzg.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.zycfv.cn/gtshddtmcr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.fzhhl.top/gtveahwajr.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.yueranfly.top/gtkoogxeqf.html

[F05] 判断文件或目录是否存在
来源：http://hz.jlsjyb.cn/gtdyxjwqhz.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.fzhhl.top/gtnnyqobuw.html

PHP:  file_exists("a.txt");
来源：http://hz.ydjk.org.cn/gtsarrihxu.html

JS:   fs.existsSync("a.txt")
来源：http://hz.xingfuxueyuan.xyz/gttxacmskl.html

TS:   fs.existsSync("a.txt")
来源：http://hz.52xcode.cn/gtajkxwlxx.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.jinqigufen.top/gtfzoylcst.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.birdmap.top/gtsdfjsyxc.html

Ruby: File.exist?("a.txt")
来源：http://hz.aibaodan.cn/gtfizadtvm.html

C#:   File.Exists("a.txt")
来源：http://hz.hongshengwenyu.top/gtmwzvcmbn.html

[F06] 删除文件
来源：http://hz.aizwys.cn/gttfalsqww.html

Py:   os.remove("a.txt")
来源：http://hz.shuidangran.top/gtuhdiixnj.html

PHP:  unlink("a.txt");
来源：http://hz.andypj.xyz/gtgwrooggq.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.9152youxi.cn/gtcpjvxnjo.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.jlsjyb.cn/gtutslrnzz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.ybcxt.top/gtggnrjrtq.html

Go:   os.Remove("a.txt")
来源：http://hz.jinyuanbaomall.cn/gtthbscboo.html

Ruby: File.delete("a.txt")
来源：http://hz.zdqjudy.top/gtglfymydl.html

C#:   File.Delete("a.txt");
来源：http://hz.jyoumei.cn/gtidezeqrt.html

[F07] 创建目录（含多级）
来源：http://hz.yanxiufei.cn/gtxgfcuzzg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.mhx1999.top/gtvqziecqe.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.ydzc1.top/gtwplobywl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ehwqpu.com/gtyaagxeei.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.wangdashe.top/gtwlebunai.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.chenzaomai.com/gtahncxsvl.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jqgufenzy.top/gtzntvphbv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.shangyingyoupin.top/gtfclkjmdv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.xuetiantiany.cn/gteubkkaer.html

[F08] 遍历目录
来源：http://hz.mhx1999.top/gtwrcsfenl.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.jlsjyb.cn/gtxhsxhtxo.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.xylfe.cn/gtofrkhawl.html

JS:   fs.readdirSync("dir")
来源：http://hz.feifeiyinyue.top/gtftwitsfl.html

TS:   fs.readdirSync("dir")
来源：http://hz.yvedp.cn/gtzpqaukbi.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.iojbl.cn/gtdnmureqv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.quarkkingdee.top/gttivnlxnf.html

Ruby: Dir.children("dir")
来源：http://hz.zhongyouzk.top/gtqwpeqrzi.html

C#:   Directory.GetFiles("dir")
来源：http://hz.aizwys.cn/gtqmoevdby.html

[F09] 获取文件大小
来源：http://hz.jyoumei.cn/gtpkisrfzb.html

Py:   os.path.getsize("a.txt")
来源：http://hz.daxiang520.top/gtigbeggfs.html

PHP:  filesize("a.txt");
来源：http://hz.xuetiantiany.cn/gtzaafdtcc.html

JS:   fs.statSync("a.txt").size
来源：http://hz.gogol.net.cn/gtoxdnohox.html

TS:   fs.statSync("a.txt").size
来源：http://hz.jqgufenzy.top/gtwinzmxew.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.hysaishi.cn/gtsbopitfo.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.hywenlv.cn/gtnqlpqrkj.html

Ruby: File.size("a.txt")
来源：http://hz.andypj.xyz/gtzwejjjok.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.cqqwz.cn/gtodfotagx.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.nanxuanxn.top/gtkzrorwrf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.ydzc1.top/gtggfwdslk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.wangshuangyany.cn/gtdfhvvivd.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.9152youxi.cn/gtarkulovz.html

TS:   path.extname("a.txt")
来源：http://hz.tanke756.top/gttovfgxew.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.zdqjudy.top/gtissblvsa.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.snrcjt.cn/gtptwapzhz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.hywenlv.cn/gtngofpvri.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.zhiwuduotai.top/gtajzfdang.html

[F11] 复制与移动文件
来源：http://hz.0kj1m.cn/gtphgjmedy.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.c1oappe.top/gtdxdamzro.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.redwolf501.top/gtdrcwbpmy.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zycfv.cn/gteqwvgqse.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.wangdashe.top/gthvknfjju.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.havefunace.top/gtehoeyuvb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jyoumei.cn/gtcdkcjyij.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.vqdsnc.cn/gtgkogoepa.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.zycfv.cn/gtksdogskz.html

[F12] CSV 读写
来源：http://hz.yangfankeji.com/gtjlafzbpw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.jlsjyb.cn/gtcomopacv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.chenlongwang.top/gtwgqdzxzg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.52xcode.cn/gtsqxucmtn.html

TS:   // 同上
来源：http://hz.cheryme.top/gtwdfpypfe.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.shzxlz.cn/gthfbeqsas.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.sxryk.cn/gtbrhviwry.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jinqigfzy.top/gtzyeruubk.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jlsjyb.cn/gtdjmkdwpx.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtxdohmtxp.html

G. 面向对象
来源：http://hz.bjfxy.top/gtqqlbounr.html

================================================================================
来源：http://hz.guowangkeji.top/gtaykplcsl.html

[G01] 定义类
来源：http://hz.xinyue.icu/gtrokyvarw.html

Py:   class User: pass
来源：http://hz.shuidangran.top/gtbuxdvwvp.html

PHP:  class User {}
来源：http://hz.hnxiangtu.top/gttmqwdvwh.html

JS:   class User {}
来源：http://hz.jianghu66.top/gtqaxoljsq.html

TS:   class User { name: string = ""; }
来源：http://hz.snrcjt.cn/gtuldmigly.html

Java: class User {}
来源：http://hz.jqgufenzy.top/gtvcfiqvck.html

Go:   type User struct { Name string }
来源：http://hz.chenjidiqi.icu/gthzamnbwt.html

Ruby: class User; end
来源：http://hz.ivvv.top/gtsnsymcjq.html

C#:   class User {}
来源：http://hz.guowangkeji.top/gthglpxude.html

[G02] 构造函数
来源：http://hz.guowangkeji.top/gtyzxutamb.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yanxiufei.cn/gtacymyilr.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.0kj1m.cn/gtnubkrpti.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.zhoulong.xyz/gtdmgyztuk.html

TS:   constructor(public name: string) {}
来源：http://hz.nanxuanxn.top/gthvofoler.html

Java: User(String name) { this.name = name; }
来源：http://hz.jinqigufen.top/gtqzsutpds.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.c1oappe.top/gtudkvtbdf.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.zdqjudy.top/gtyrvrjpfs.html

C#:   public User(string name) { Name = name; }
来源：http://hz.jinqigfzy.top/gtqmyuwbmb.html

[G03] 实例属性
来源：http://hz.shzxlz.cn/gttmtilepd.html

Py:   self.name = "x"
来源：http://hz.hnxiangtu.top/gtnnikwhpd.html

PHP:  public string $name = "x";
来源：http://hz.hongshengwenyu.top/gtqzydekrp.html

JS:   this.name = "x";
来源：http://hz.andypj.xyz/gtzbczmhgi.html

TS:   name: string = "x";
来源：http://hz.0kj1m.cn/gtpaatnunr.html

Java: private String name;
来源：http://hz.haohaochexian.top/gtwwizgrkt.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.zhengqikj.top/gtbkhpbkat.html

Ruby: @name = "x"
来源：http://hz.sufxvd.cn/gtqmikmuty.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jinqigfzy.top/gtosndiakd.html

[G04] 定义方法
来源：http://hz.hnxiangtu.top/gtssbdxhsw.html

Py:   def greet(self): return self.name
来源：http://hz.jinqigfzy.top/gtkuezydqs.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.zhongyouzk.top/gtbsgsmnem.html

JS:   greet() { return this.name; }
来源：http://hz.hammf.cn/gtruldvxen.html

TS:   greet(): string { return this.name; }
来源：http://hz.jianghu66.top/gtskaqkenl.html

Java: String greet() { return name; }
来源：http://hz.cheryme.top/gtjkapzksr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.gaohongyu789.top/gtzfsdqmjs.html

Ruby: def greet; @name; end
来源：http://hz.aizwys.cn/gtuiqlxpcj.html

C#:   public string Greet() => Name;
来源：http://hz.zhoulong.xyz/gtmcbwquuc.html

[G05] 继承
来源：http://hz.chenzaomai.com/gtoizvcige.html

Py:   class Admin(User): pass
来源：http://hz.nwbrower.top/gtldenusds.html

PHP:  class Admin extends User {}
来源：http://hz.ivvv.top/gtbbznuljz.html

JS:   class Admin extends User {}
来源：http://hz.9152youxi.cn/gtezmwifjy.html

TS:   class Admin extends User {}
来源：http://hz.ydzc1.top/gtlupjomqp.html

Java: class Admin extends User {}
来源：http://hz.kuanghao11.cn/gtshkecttx.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.ydjk.org.cn/gtavjaessd.html

Ruby: class Admin < User; end
来源：http://hz.chenjidiqi.icu/gtekmfvzho.html

C#:   class Admin : User {}
来源：http://hz.jinqigufen.top/gtelydlbgp.html

[G06] 重写方法
来源：http://hz.ehwqpu.com/gtvekmyfnm.html

Py:   def greet(self): return "admin"
来源：http://hz.aizwys.cn/gtpyobytuc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.xziqi.cn/gtduobatsa.html

JS:   greet() { return "admin"; }
来源：http://hz.zhiwuduotai.top/gtovazpeya.html

TS:   greet(): string { return "admin"; }
来源：http://hz.kuanghao11.cn/gtgjmtpjau.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jiagoushi.top/gthdxxdyti.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.jinqigfzy.top/gtdunxtlhd.html

Ruby: def greet; "admin"; end
来源：http://hz.gotoacloud.top/gtzoswwigt.html

C#:   public override string Greet() => "admin";
来源：http://hz.xuanzx.com/gtamajwgyh.html

[G07] 调用父类方法
来源：http://hz.xuetiantiany.cn/gtwbwhnbbb.html

Py:   super().greet()
来源：http://hz.cqqwz.cn/gtpnyggkiw.html

PHP:  parent::greet();
来源：http://hz.jyoumei.cn/gtefmtwvry.html

JS:   super.greet();
来源：http://hz.zhongyouzk.top/gtruvdtxbk.html

TS:   super.greet();
来源：http://hz.feifeiyinyue.top/gtyysxoqkp.html

Java: super.greet();
来源：http://hz.fengsongda.top/gtgirfvjym.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yanxiufei.cn/gtibiqajhc.html

Ruby: super
来源：http://hz.havefunace.top/gtuphkskzk.html

C#:   base.Greet();
来源：http://hz.dashuyun.cn/gthizmimky.html

[G08] 静态方法与属性
来源：http://hz.zdqjudy.top/gtcredybyq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.smart0.xyz/gthtpmctic.html

PHP:  public static function f() {}
来源：http://hz.smart0.xyz/gtixylmyes.html

JS:   static f() {}
来源：http://hz.dianchejie.cn/gtixqyzqtn.html

TS:   static f(): void {}
来源：http://hz.yangfankeji.com/gtqhtsqxyl.html

Java: static void f() {}
来源：http://hz.ehwqpu.com/gtudnuyvnr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.wangshuangyany.cn/gtmtljnylt.html

Ruby: def self.f; end
来源：http://hz.pycfn.com/gtwpwjketw.html

C#:   public static void F() {}
来源：http://hz.zhixingplan.top/gtofmzmgfg.html

[G09] 接口 / 抽象类
来源：http://hz.9152youxi.cn/gtbeuguxlf.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.ydzc1.top/gtbkrbobdq.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.quarkkingdee.top/gtysfxgebf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.ywan-chungtsiang.top/gtsdwxpkhz.html

TS:   interface Shape { area(): number; }
来源：http://hz.gzhubu.top/gtukzmitdp.html

Java: interface Shape { double area(); }
来源：http://hz.9152youxi.cn/gtlifpcors.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.quarkkingdee.top/gtkhstpkjf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.zhaomingkeji.xyz/gtvhrqkfkc.html

C#:   interface IShape { double Area(); }
来源：http://hz.chenlongwang.top/gtzqlnwvzt.html

[G10] 访问控制
来源：http://hz.yuanzhike.top/gthkojlfep.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.zhiwuduotai.top/gtulawclko.html

PHP:  public / protected / private
来源：http://hz.xuanzx.com/gtgujtmtbc.html

JS:   #private 字段；其余公开
来源：http://hz.tian-w.cn/gtfvplleuh.html


<!-- 参考信息 -->