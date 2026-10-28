代发 wailian999

Ruby: s.reverse
来源：http://hz.jinghuilouyu.cn/gtchgrdegl.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.cdnleiting.top/gtnfaalbxr.html

[E12] 统计某字符出现次数
来源：http://hz.nanxuanxn.top/gtsiutnkcb.html

Py:   s.count("a")
来源：http://hz.yj202588.top/gtvwwfoqdd.html

PHP:  substr_count($s, "a");
来源：http://hz.cashguo.top/gtfiqtrxpk.html

JS:   s.split("a").length - 1
来源：http://hz.9152youxi.cn/gtuxyzpycf.html

TS:   s.split("a").length - 1
来源：http://hz.yangfankeji.com/gtttvayosk.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.gogol.net.cn/gtqwsvmlvc.html

Go:   strings.Count(s, "a")
来源：http://hz.xinyue.icu/gtgawdacuy.html

Ruby: s.count("a")
来源：http://hz.shanyushiyangtech.top/gtbobwzxhg.html

C#:   s.Count(c => c == 'a')
来源：http://hz.feifeiyinyue.top/gtbryilzva.html

[E13] 逐字符遍历
来源：http://hz.sufxvd.cn/gtfzlgijfi.html

Py:   for ch in s: print(ch)
来源：http://hz.0kj1m.cn/gtpsrrcbrr.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.yangfankeji.com/gtqbihgjsk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xylfe.cn/gthqzrapyz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jianghu66.top/gtclgwabsp.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.52xcode.cn/gtgsulsdom.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.birdmap.top/gtixknzunq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.nwbrower.top/gthfrdpksn.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.aizwys.cn/gtgrxlutkq.html

[E14] URL 编码与 Base64
来源：http://hz.pycfn.com/gtjyenjgpg.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.52xcode.cn/gtkjonptkh.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.316326.xyz/gtrgytyglz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.xziqi.cn/gtwgkkzkyq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.yangfankeji.com/gtnutwtgbi.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.zhiwuduotai.top/gtnprtehma.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.yuanzhike.top/gtucmwqjex.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.ybcxt.top/gtujhcyqiy.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.cucudq.cn/gtjphnudca.html

[E15] HTML 转义 / 反转义
来源：http://hz.aibaodan.cn/gtjovszfgo.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.gotoacloud.top/gtjnzujkvx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.shanyushiyangtech.top/gttasrxtvz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.jqgufenzy.top/gtljuvonon.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.shanyushiyangkeji.top/gtnyfhnuvt.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.cqqwz.cn/gtkuccxofn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.zycfv.cn/gtetgqizdl.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.zhixingplan.top/gtbtyscohx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.snrcjt.cn/gtsrdgifxa.html

[E16] 数字千分位
来源：http://hz.aizwys.cn/gtmoyboqov.html

Py:   f"{1234567:,}"
来源：http://hz.tianlin.xyz/gtfefugfdd.html

PHP:  number_format(1234567);
来源：http://hz.yj20258888.top/gtqaezfvhb.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.gotoacloud.top/gtwwgdaumj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.aibaodan.cn/gtogktucdi.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.yuxming.cn/gtdepljzcb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.sysykeji.top/gtpayyfezd.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.snrcjt.cn/gtrkswntcy.html

C#:   1234567.ToString("N0")
来源：http://hz.tanke756.top/gtlrsalcqn.html

[E17] 首字母大写
来源：http://hz.yj20258888.top/gtigdfuzlk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.jinyuanbaomall.cn/gtzkdshmik.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.svipenyu.cn/gtoioellml.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.fzhhl.top/gtveqonchb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zycfv.cn/gtdhbmejjs.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.shanyushiyangkeji.top/gtvopyoqrd.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.sufxvd.cn/gtilumnbie.html

Ruby: s.capitalize
来源：http://hz.chenlongwang.top/gtmhgopftl.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.nanxuanxn.top/gttbgydvtp.html

[E18] 模板占位符替换
来源：http://hz.yj20258888.top/gthowxujlr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.shangyingyoupin.top/gtnmqldpmu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.smart0.xyz/gtqfntdhyv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.ehwqpu.com/gtrpjhmdnq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.daxiang520.top/gtorhisvsf.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.52xcode.cn/gtiiyclrit.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.cdnleiting.top/gtiaixnbzv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.zhijiandao.cn/gtrwvaduyn.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.smart0.xyz/gtcamgibmn.html

[E19] 多行文本按行拆分
来源：http://hz.jlsjyb.cn/gtehwhvfzy.html

Py:   s.splitlines()
来源：http://hz.ivvv.top/gtczxzovoq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.zhijiandao.cn/gtbedgulic.html

JS:   s.split(/\r?\n/)
来源：http://hz.jinghuilouyu.cn/gtnestlkfi.html

TS:   s.split(/\r?\n/)
来源：http://hz.zhiwuduotai.top/gtkuqikjfx.html

Java: s.lines().toList()
来源：http://hz.jlsjyb.cn/gtarcxarmy.html

Go:   strings.Split(s, "\n")
来源：http://hz.cqqwz.cn/gtpalphmcj.html

Ruby: s.lines
来源：http://hz.gogol.net.cn/gtgqdpeuty.html

C#:   s.Split('\n')
来源：http://hz.wangshuangyany.cn/gtpdzmicvi.html

[E20] 判断字符串是否为空
来源：http://hz.birdmap.top/gtnaueefhw.html

Py:   if not s:
来源：http://hz.52xcode.cn/gtortnzika.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.jyoumei.cn/gtdbobszyz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.wangdashe.top/gtagqnbsxv.html

TS:   if (s === "") {}
来源：http://hz.ehwqpu.com/gtrippacec.html

Java: if (s.isEmpty()) {}
来源：http://hz.kuanghao11.cn/gtucntfxvu.html

Go:   if s == "" {}
来源：http://hz.iojbl.cn/gtgwncthoh.html

Ruby: if s.empty?
来源：http://hz.sxryk.cn/gtwrwzeibv.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.cdnleiting.top/gtroyjmeig.html

[E21] 超长截断加省略号
来源：http://hz.yonumen.top/gtxgqnfcbt.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.xylfe.cn/gtewrizqks.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.yuanzhike.top/gtmaexbktg.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.cqqwz.cn/gtztvxdyhz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.c1oappe.top/gtuttqegtv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yonumen.top/gtuwyhcmmd.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.hywenlv.cn/gttxgnayui.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.9152youxi.cn/gtjjcorbes.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.ydjk.org.cn/gthxmtfylo.html

[E22] 字节长度与字符长度
来源：http://hz.yj20258.top/gthvtoyjuc.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.gogol.net.cn/gtsepexxch.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yj20258888.top/gttthtowfk.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yvedp.cn/gthhdbplam.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ehwqpu.com/gtizytqgsl.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.zhaomingkeji.xyz/gtmsayktxe.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.guannengcc.top/gtawatevzp.html

Ruby: s.bytesize;  s.length
来源：http://hz.zhijiandao.cn/gtwdmabzsg.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.feifeiyinyue.top/gtrltfhcro.html

================================================================================
来源：http://hz.tianlin.xyz/gtwqpywsvd.html

F. 文件与目录
来源：http://hz.gaohongyu789.top/gteewhqwav.html

================================================================================
来源：http://hz.316326.xyz/gtpahbmwcd.html

[F01] 读取整个文件
来源：http://hz.wangshuangyany.cn/gtwfjpevhn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.52xcode.cn/gtkxafwuff.html

PHP:  file_get_contents("a.txt");
来源：http://hz.dashuyun.cn/gtoehxrwhu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.jinqigufen.top/gtjjfouolt.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.haohaochexian.top/gtojrkhcbn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.hnqzz.top/gtlsfqurzo.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.dashuyun.cn/gtxmnyvcmx.html

Ruby: File.read("a.txt")
来源：http://hz.ydzc1.top/gtsvjnoovq.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.iojbl.cn/gtuqpqgmos.html

[F02] 逐行读取文件
来源：http://hz.chenlongwang.top/gtittzicdk.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.iojbl.cn/gthgbgyifz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.jinqigufen.top/gtzqdutjzu.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xuetiantiany.cn/gtfhunbfcy.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.feifeiyinyue.top/gtlsuevstm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.xingfuxueyuan.xyz/gtpixpscim.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.shuidangran.top/gtgejwvnzu.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.birdmap.top/gtmpytflla.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.cheryme.top/gthckfdddw.html

[F03] 写入文件（覆盖）
来源：http://hz.jinghuilouyu.cn/gtjrlnxkmz.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.gogol.net.cn/gtoyzlxkmx.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.daxiang520.top/gtwhpwyxxg.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.andypj.xyz/gtjnipeykz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.xylfe.cn/gtsdokovac.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.pycfn.com/gtrpmckhgg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.zhijiandao.cn/gtcluysmsq.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.aibaodan.cn/gtwmuruuqp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.cdnleiting.top/gtggxqkgww.html

[F04] 追加写入文件
来源：http://hz.smart0.xyz/gtewcmhyvf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.nwbrower.top/gthrckoykx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.tianlin.xyz/gtvhtoryex.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.kuanghao11.cn/gturzwbyxn.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ydjk.org.cn/gtzhbqbehu.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.andypj.xyz/gtfcgvcjeb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.cqqwz.cn/gtqfctsujz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.cheryme.top/gtwfbgclrf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.tian-w.cn/gtxquoqzax.html

[F05] 判断文件或目录是否存在
来源：http://hz.shangyingyoupin.top/gtwpcjjwsf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.daria6918.cn/gtftfictxd.html

PHP:  file_exists("a.txt");
来源：http://hz.zhijiandao.cn/gtnskolelr.html

JS:   fs.existsSync("a.txt")
来源：http://hz.jiagoushi.top/gtqdrfefvu.html

TS:   fs.existsSync("a.txt")
来源：http://hz.fengsongda.top/gtuwislphg.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.yangfankeji.com/gtqrwvykfn.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.sufxvd.cn/gtakewichq.html

Ruby: File.exist?("a.txt")
来源：http://hz.shuidangran.top/gtkoccyoqe.html

C#:   File.Exists("a.txt")
来源：http://hz.kuanghao11.cn/gtoxmholnq.html

[F06] 删除文件
来源：http://hz.shanyushiyangtech.top/gtgspyozsz.html

Py:   os.remove("a.txt")
来源：http://hz.yangfankeji.com/gtaccbrgxp.html

PHP:  unlink("a.txt");
来源：http://hz.cucudq.cn/gtxpmmskak.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.sufxvd.cn/gtvlbuvqfi.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.wangshuangyany.cn/gtybqxjymv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.gotoacloud.top/gtdwfnugmi.html

Go:   os.Remove("a.txt")
来源：http://hz.haohaochexian.top/gtvwgkdidn.html

Ruby: File.delete("a.txt")
来源：http://hz.jiagoushi.top/gtgmsndhte.html

C#:   File.Delete("a.txt");
来源：http://hz.jqgfzy.top/gtzseynmae.html

[F07] 创建目录（含多级）
来源：http://hz.mhx1999.top/gtopptfkid.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.cashguo.top/gtofjvdpds.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.feifeiyinyue.top/gtjvlxjjsv.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.svipenyu.cn/gtlybrwcva.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.chenlongwang.top/gtcfbfqurt.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.chenzaomai.com/gtonznduiy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.feifeiyinyue.top/gtsfzerizm.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.wangshuangyany.cn/gtdwdfrtgt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yj20258.top/gtydnbjnrv.html

[F08] 遍历目录
来源：http://hz.gotoacloud.top/gtuifxvwkj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.aizwys.cn/gthodyklbv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.yj20258888.top/gtobxuvurr.html

JS:   fs.readdirSync("dir")
来源：http://hz.jinqigfzy.top/gthgphwhiv.html

TS:   fs.readdirSync("dir")
来源：http://hz.jianghu66.top/gtgyqaiccw.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.ydjk.org.cn/gtczcmnaif.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.0kj1m.cn/gtkaamjfye.html

Ruby: Dir.children("dir")
来源：http://hz.guowangkeji.top/gtwrmmkadb.html

C#:   Directory.GetFiles("dir")
来源：http://hz.jiagoushi.top/gtlrtyjuob.html

[F09] 获取文件大小
来源：http://hz.gotoacloud.top/gtbtkwdozy.html

Py:   os.path.getsize("a.txt")
来源：http://hz.guowangkeji.top/gtzkdmayir.html

PHP:  filesize("a.txt");
来源：http://hz.shuidangran.top/gtshjohwkz.html

JS:   fs.statSync("a.txt").size
来源：http://hz.c1oappe.top/gttlhoqlpn.html

TS:   fs.statSync("a.txt").size
来源：http://hz.xuanzx.com/gtteqtgpgo.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.52xcode.cn/gtueanxlft.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.ehwqpu.com/gttgwytrcv.html

Ruby: File.size("a.txt")
来源：http://hz.wangdashe.top/gtrkohpdps.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.nwbrower.top/gtinseocpy.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.dashuyun.cn/gtuxinhpgv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.ydjk.org.cn/gtrljlbtxo.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.yanxiufei.cn/gtquztqknv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.shanyushiyangkeji.top/gtkutwwfha.html

TS:   path.extname("a.txt")
来源：http://hz.shuidangran.top/gtwrhnfsgu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.kuanghao11.cn/gtbiqxclui.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.316326.xyz/gtjoqjrboc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.yanxiufei.cn/gtvzvbgdfk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.fzhhl.top/gtjzdrjgub.html

[F11] 复制与移动文件
来源：http://hz.guannengcc.top/gtllypnkhj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.gaohongyu789.top/gtrybpmanx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.xinyue.icu/gtpiumniog.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hongshengwenyu.top/gtjexpjacz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ybcxt.top/gtbrowzynx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.yueranfly.top/gtmvfokvgj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.aizwys.cn/gtjqhmtimd.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.zhongyouzk.top/gtaxteqaof.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.birdmap.top/gtmlanhskz.html

[F12] CSV 读写
来源：http://hz.quarkkingdee.top/gtqwzbgaus.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.chenzaomai.com/gtpcafcypb.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.cucudq.cn/gtniwugauu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.feifeiyinyue.top/gtzhfphbky.html

TS:   // 同上
来源：http://hz.jiagoushi.top/gtkclrwent.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.nwbrower.top/gtvwhyljsz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.pengpengdd.cyou/gtkhehvbjb.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.wangdashe.top/gtxnajxlnf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yj202588.top/gttshgzooy.html

================================================================================
来源：http://hz.jqgufenzy.top/gtdxfpzbnl.html

G. 面向对象
来源：http://hz.guannengcc.top/gtpdurvwlb.html

================================================================================
来源：http://hz.yj202588.top/gtuhlsugzc.html

[G01] 定义类
来源：http://hz.havefunace.top/gtxodkurnl.html

Py:   class User: pass
来源：http://hz.bjfxy.top/gtmdmcuxwg.html

PHP:  class User {}
来源：http://hz.xuetiantiany.cn/gttaxivexg.html

JS:   class User {}
来源：http://hz.smart0.xyz/gtdwfadkju.html

TS:   class User { name: string = ""; }
来源：http://hz.daxiang520.top/gtmpvlmyaq.html

Java: class User {}
来源：http://hz.zhoulong.xyz/gtdtzfmnho.html

Go:   type User struct { Name string }
来源：http://hz.snrcjt.cn/gtaqcxkhyt.html

Ruby: class User; end
来源：http://hz.meibo888.top/gtuyjkfqns.html

C#:   class User {}
来源：http://hz.ehwqpu.com/gtifkudlyk.html

[G02] 构造函数
来源：http://hz.shangyingyoupin.top/gtrohugvfp.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.316326.xyz/gtvpkqmcmy.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.wangshuangyany.cn/gtqebvxtea.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yuxming.cn/gtnzpslosh.html

TS:   constructor(public name: string) {}
来源：http://hz.xingfuxueyuan.xyz/gtvtrhdgww.html

Java: User(String name) { this.name = name; }
来源：http://hz.iojbl.cn/gtwrgsmzhp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yuxming.cn/gtviqagqio.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.feifeiyinyue.top/gtdrthdeag.html

C#:   public User(string name) { Name = name; }
来源：http://hz.shangyingyoupin.top/gtvbtmlich.html

[G03] 实例属性
来源：http://hz.zhongyouzk.top/gthfiqjeob.html

Py:   self.name = "x"
来源：http://hz.bjfxy.top/gtugobcoxp.html

PHP:  public string $name = "x";
来源：http://hz.gaohongyu789.top/gtloyvanrv.html

JS:   this.name = "x";
来源：http://hz.zhiwuduotai.top/gtzpeqdsgk.html

TS:   name: string = "x";
来源：http://hz.gotoacloud.top/gtsrnopqpz.html

Java: private String name;
来源：http://hz.zhaomingkeji.xyz/gtwreifleg.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.ywan-chungtsiang.top/gtlwemunvk.html

Ruby: @name = "x"
来源：http://hz.shanyushiyangkeji.top/gtfuxviund.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.aibaodan.cn/gtfykjthyq.html

[G04] 定义方法
来源：http://hz.yj20258888.top/gttcevxxde.html

Py:   def greet(self): return self.name
来源：http://hz.quarkkingdee.top/gtmermrpst.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.ydzc1.top/gtmqpufaho.html

JS:   greet() { return this.name; }
来源：http://hz.cashguo.top/gtllrdwlnw.html

TS:   greet(): string { return this.name; }
来源：http://hz.nanxinkj.top/gtjmozixag.html

Java: String greet() { return name; }
来源：http://hz.zhiwuduotai.top/gtevgsxfwn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.xuanzx.com/gtltkkqaur.html

Ruby: def greet; @name; end
来源：http://hz.guowangkeji.top/gtrtvfbmja.html

C#:   public string Greet() => Name;
来源：http://hz.sxryk.cn/gtqnyprxrp.html

[G05] 继承
来源：http://hz.yongpay.top/gtvfqakxen.html

Py:   class Admin(User): pass
来源：http://hz.chenlongwang.top/gtnahbipmw.html

PHP:  class Admin extends User {}
来源：http://hz.9152youxi.cn/gtmiibxizv.html

JS:   class Admin extends User {}
来源：http://hz.yangfankeji.com/gtrrsxrpky.html

TS:   class Admin extends User {}
来源：http://hz.xziqi.cn/gtcdjphbfw.html

Java: class Admin extends User {}
来源：http://hz.yj20258.top/gtkuonvaxd.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.zdqjudy.top/gtgxzdcklr.html

Ruby: class Admin < User; end
来源：http://hz.yuxming.cn/gtopdicxxj.html

C#:   class Admin : User {}
来源：http://hz.meibo888.top/gtjsucyvge.html

[G06] 重写方法
来源：http://hz.yongpay.top/gtwpeowlzs.html

Py:   def greet(self): return "admin"
来源：http://hz.hnxiangtu.top/gtoieexsub.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.yj20258888.top/gtfrfqsjkx.html

JS:   greet() { return "admin"; }
来源：http://hz.9152youxi.cn/gtofivmzht.html

TS:   greet(): string { return "admin"; }
来源：http://hz.shanyushiyangkeji.top/gtglltlnta.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.aizwys.cn/gtewwwvqli.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.yongpay.top/gtumknkksa.html

Ruby: def greet; "admin"; end
来源：http://hz.cheryme.top/gtsgaekblb.html

C#:   public override string Greet() => "admin";
来源：http://hz.nanxinkj.top/gtfvbzbfnf.html

[G07] 调用父类方法
来源：http://hz.dashuyun.cn/gtgbegqqqv.html

Py:   super().greet()
来源：http://hz.tian-w.cn/gtqmtkpeho.html

PHP:  parent::greet();
来源：http://hz.aizwys.cn/gtwzcnwraj.html

JS:   super.greet();
来源：http://hz.jinqigfzy.top/gtsgdjwqlu.html

TS:   super.greet();
来源：http://hz.xziqi.cn/gtynsajpqy.html

Java: super.greet();
来源：http://hz.yangfankeji.com/gtrspagwau.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.xylfe.cn/gtdtbfhbay.html

Ruby: super
来源：http://hz.jinyuanbaomall.cn/gtopbtkkmb.html

C#:   base.Greet();
来源：http://hz.xziqi.cn/gtuxezvrke.html

[G08] 静态方法与属性
来源：http://hz.ybcxt.top/gtsveypbdp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.shangyingyoupin.top/gtibnohpsj.html

PHP:  public static function f() {}
来源：http://hz.sxryk.cn/gtaeeylboj.html

JS:   static f() {}
来源：http://hz.ydzc1.top/gtibeirvyc.html

TS:   static f(): void {}
来源：http://hz.hnqzz.top/gtqyihzzrq.html

Java: static void f() {}
来源：http://hz.ywan-chungtsiang.top/gtykzwmupa.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yanxiufei.cn/gthjunslrt.html

Ruby: def self.f; end
来源：http://hz.shangyingyoupin.top/gtytckaplm.html

C#:   public static void F() {}
来源：http://hz.hfpthk.cn/gtdmrsllqe.html

[G09] 接口 / 抽象类
来源：http://hz.havefunace.top/gtjemeqmeh.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.sysykeji.top/gtgnkarlhk.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.xingfuxueyuan.xyz/gtvdiwphpc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.hysaishi.cn/gtyjkthbjl.html

TS:   interface Shape { area(): number; }
来源：http://hz.aibaodan.cn/gtbnpaieio.html

Java: interface Shape { double area(); }
来源：http://hz.redwolf501.top/gtsktstzhl.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.gaohongyu789.top/gtcturbsvy.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.chenlongwang.top/gtapartkxs.html

C#:   interface IShape { double Area(); }
来源：http://hz.pycfn.com/gtdsfbwdri.html

[G10] 访问控制
来源：http://hz.0kj1m.cn/gtitnaynva.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.gaohongyu789.top/gtxukscztc.html

PHP:  public / protected / private
来源：http://hz.cdnleiting.top/gtwxclbqxa.html

JS:   #private 字段；其余公开
来源：http://hz.zhaomingkeji.xyz/gtbrhdpmxg.html


<!-- 参考信息 -->