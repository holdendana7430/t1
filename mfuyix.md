代发 wailian999

Py:   for ch in s: print(ch)
来源：http://hz.quarkkingdee.top/gtjjnnwmiv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.havefunace.top/gtcsuvhguh.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xingfuxueyuan.xyz/gtqqpswdhu.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xuetiantiany.cn/gthpktlnxu.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.redwolf501.top/gtqcjodlng.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.fengsongda.top/gtzhgcjgwx.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.jinqigufen.top/gtwlygskxy.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.fzhhl.top/gtbukqdzny.html

[E14] URL 编码与 Base64
来源：http://hz.9152youxi.cn/gtgsggefmc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.jinqigufen.top/gtxzoodgpz.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.hywenlv.cn/gtjojcptcq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.nwbrower.top/gtwiyrtnxu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.smart0.xyz/gtpouuvbed.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.gzhubu.top/gtbysahozj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.sxryk.cn/gtoiebeuus.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.ehwqpu.com/gtjtseielt.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.hnxiangtu.top/gtzxmjjooh.html

[E15] HTML 转义 / 反转义
来源：http://hz.0kj1m.cn/gtgxgydaiv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.shuidangran.top/gtkbaebmsg.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.guannengcc.top/gtkvltmaev.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yonumen.top/gtxptportj.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.nwbrower.top/gtkrfqraqp.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.hnxiangtu.top/gtbruojthp.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.snrcjt.cn/gtqzhidedl.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.hywenlv.cn/gtdnzadhkr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.ivvv.top/gtrmlucnji.html

[E16] 数字千分位
来源：http://hz.sufxvd.cn/gtkwovtjpr.html

Py:   f"{1234567:,}"
来源：http://hz.xinyue.icu/gtachkajyr.html

PHP:  number_format(1234567);
来源：http://hz.feifeiyinyue.top/gtypzfasfx.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.shzxlz.cn/gtbjkzfvty.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.jinqigfzy.top/gtukqrqezk.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.birdmap.top/gtkbfriwap.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.pycfn.com/gtmewnkgrp.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.jinqigfzy.top/gtrfazjyji.html

C#:   1234567.ToString("N0")
来源：http://hz.ivvv.top/gtaxzbrzrn.html

[E17] 首字母大写
来源：http://hz.tian-w.cn/gtpogejplf.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.jinqigufen.top/gtraeiesdu.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.zhiwuduotai.top/gtlszjehho.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.shanyushiyangkeji.top/gtokrbewnc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.chenzaomai.com/gtuwgzxibz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.jinghuilouyu.cn/gtquzxeyjp.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.wangdashe.top/gteshjhpju.html

Ruby: s.capitalize
来源：http://hz.jyoumei.cn/gtvcdpdgre.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.cucudq.cn/gtddbbrddc.html

[E18] 模板占位符替换
来源：http://hz.jinghuilouyu.cn/gtaythwfam.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.316326.xyz/gtulfrvzej.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.nanxinkj.top/gtlducqhus.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.birdmap.top/gtueuylghq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.xuanzx.com/gtqzhmuejc.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.9152youxi.cn/gtiqxngaek.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.shzxlz.cn/gtztldcegw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.xingfuxueyuan.xyz/gttumskxor.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.tanke756.top/gthqfhjpmq.html

[E19] 多行文本按行拆分
来源：http://hz.hammf.cn/gttvlqfsng.html

Py:   s.splitlines()
来源：http://hz.shangyingyoupin.top/gthoiqxvlm.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jinqigufen.top/gtwfhbmfie.html

JS:   s.split(/\r?\n/)
来源：http://hz.aizwys.cn/gtukmieqby.html

TS:   s.split(/\r?\n/)
来源：http://hz.c1oappe.top/gtkufsciil.html

Java: s.lines().toList()
来源：http://hz.hywenlv.cn/gtwdnknkti.html

Go:   strings.Split(s, "\n")
来源：http://hz.zhixingplan.top/gtrfazhvvw.html

Ruby: s.lines
来源：http://hz.andypj.xyz/gtsnjfmkyk.html

C#:   s.Split('\n')
来源：http://hz.ppjwa.cn/gtzzhkgtyx.html

[E20] 判断字符串是否为空
来源：http://hz.zhixingplan.top/gtljxyyuho.html

Py:   if not s:
来源：http://hz.hfpthk.cn/gtbtltymwy.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.ivvv.top/gtijnrxswg.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.chenlongwang.top/gtcsvynhxb.html

TS:   if (s === "") {}
来源：http://hz.zhixingplan.top/gtdxvnmaes.html

Java: if (s.isEmpty()) {}
来源：http://hz.guowangkeji.top/gtfmtahobs.html

Go:   if s == "" {}
来源：http://hz.gotoacloud.top/gtixtvqlpe.html

Ruby: if s.empty?
来源：http://hz.ehwqpu.com/gtumrlrztq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.yangfankeji.com/gtdscawcuz.html

[E21] 超长截断加省略号
来源：http://hz.xinyue.icu/gtvhrwsnwz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.zhaomingkeji.xyz/gtozileakj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.aibaodan.cn/gthjevnpqy.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.fengsongda.top/gtnisqacig.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.c1oappe.top/gtzxztlvui.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.ehwqpu.com/gtjroiwuzi.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.xinyue.icu/gtmryoobyo.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.snrcjt.cn/gtonwmlpjb.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.hongshengwenyu.top/gteudbtmhj.html

[E22] 字节长度与字符长度
来源：http://hz.jinghuilouyu.cn/gtlzsszjue.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.gotoacloud.top/gtmqtqwgqo.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.cdnleiting.top/gtwxtfwwwq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.havefunace.top/gtoiztvlnz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.9152youxi.cn/gtrthvucuh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jqgufenzy.top/gtarltvgmr.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.smart0.xyz/gtpcfflcqd.html

Ruby: s.bytesize;  s.length
来源：http://hz.hywenlv.cn/gtmoczhrrn.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.aibaodan.cn/gtrlziucse.html

================================================================================
来源：http://hz.xylfe.cn/gtdcbmrioq.html

F. 文件与目录
来源：http://hz.pengpengdd.cyou/gtcabrakrk.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtytsreufh.html

[F01] 读取整个文件
来源：http://hz.sxryk.cn/gtzhhijpqw.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.nanxinkj.top/gtsjoekftg.html

PHP:  file_get_contents("a.txt");
来源：http://hz.yonumen.top/gtkwbrzfgc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.daria6918.cn/gtoieyclwb.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.zhaomingkeji.xyz/gtetzbryka.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.zhoulong.xyz/gtipwcfulx.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.wangshuangyany.cn/gtnmzplouk.html

Ruby: File.read("a.txt")
来源：http://hz.yongpay.top/gtvrndtkba.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.feifeiyinyue.top/gtbmnlxpdt.html

[F02] 逐行读取文件
来源：http://hz.zhiwuduotai.top/gttojgtxoa.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.yueranfly.top/gtuiwrcrle.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.yueranfly.top/gtfatjiahi.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.dianchejie.cn/gtephcrotj.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yuanzhike.top/gtgbaakflc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.fengsongda.top/gtodtfpjty.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.yuanzhike.top/gtdywynmrt.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yj202588.top/gteqppvphx.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.xingfuxueyuan.xyz/gtyswrdjnc.html

[F03] 写入文件（覆盖）
来源：http://hz.gotoacloud.top/gtrxjkqftr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.tanke756.top/gtgjbzifgz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.jinghuilouyu.cn/gtfqdezdra.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.nanxuanxn.top/gtrqziijgp.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.gaohongyu789.top/gtrepscenp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.andypj.xyz/gtqgykamrf.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.feifeiyinyue.top/gtjkytxjdj.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.jiagoushi.top/gtnfdttojc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.ehwqpu.com/gtnwxnkezp.html

[F04] 追加写入文件
来源：http://hz.gotoacloud.top/gtlizgglqj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.redwolf501.top/gtkzyalmod.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.daria6918.cn/gtwuhvfwbh.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.sufxvd.cn/gtuqibzklq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.nanxinkj.top/gtjtenwekz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.tanke756.top/gtxctomxuz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.redwolf501.top/gtqaxgjdxa.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.shanyushiyangkeji.top/gtsqgqbjwr.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.redwolf501.top/gtnywndmtp.html

[F05] 判断文件或目录是否存在
来源：http://hz.sxryk.cn/gtaieerjcv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.jqgfzy.top/gtdlypqfml.html

PHP:  file_exists("a.txt");
来源：http://hz.dashuyun.cn/gtqxjezsng.html

JS:   fs.existsSync("a.txt")
来源：http://hz.zhoulong.xyz/gtwamqphbk.html

TS:   fs.existsSync("a.txt")
来源：http://hz.snrcjt.cn/gtbxdbpxld.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.shanyushiyangkeji.top/gtpmklhqiz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.nanxinkj.top/gtmbryoapo.html

Ruby: File.exist?("a.txt")
来源：http://hz.kuanghao11.cn/gtliefasui.html

C#:   File.Exists("a.txt")
来源：http://hz.pycfn.com/gtwiemvkvd.html

[F06] 删除文件
来源：http://hz.kuanghao11.cn/gtnygfjiir.html

Py:   os.remove("a.txt")
来源：http://hz.cashguo.top/gtndkwvvgs.html

PHP:  unlink("a.txt");
来源：http://hz.daria6918.cn/gtbiurlich.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.zhaomingkeji.xyz/gtuwmtnlim.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.xylfe.cn/gtxsiichyo.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.birdmap.top/gtfqorrouz.html

Go:   os.Remove("a.txt")
来源：http://hz.0kj1m.cn/gtqjzjzmoj.html

Ruby: File.delete("a.txt")
来源：http://hz.vqdsnc.cn/gthexjptxd.html

C#:   File.Delete("a.txt");
来源：http://hz.hnxiangtu.top/gtxtborecv.html

[F07] 创建目录（含多级）
来源：http://hz.xingfuxueyuan.xyz/gtniwziwte.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.xuanzx.com/gtwncstajb.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.xziqi.cn/gtevypiebq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ydzc1.top/gtqxkeghix.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yvedp.cn/gtdaqrnczp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.yj20258.top/gtlmwnerwn.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.xingfuxueyuan.xyz/gtsryluivm.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.ppjwa.cn/gtnrshmend.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.dashuyun.cn/gtahuyxemz.html

[F08] 遍历目录
来源：http://hz.zhoulong.xyz/gtjvbxjdgd.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.hnqzz.top/gtxizywike.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.yvedp.cn/gtdklsbdye.html

JS:   fs.readdirSync("dir")
来源：http://hz.wangdashe.top/gttioctiid.html

TS:   fs.readdirSync("dir")
来源：http://hz.xuetiantiany.cn/gtofegvose.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.zhixingplan.top/gtuhbccyjf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.aizwys.cn/gtbbxbxtcu.html

Ruby: Dir.children("dir")
来源：http://hz.gotoacloud.top/gtygdrbpdt.html

C#:   Directory.GetFiles("dir")
来源：http://hz.zhixingplan.top/gtzzkshifr.html

[F09] 获取文件大小
来源：http://hz.hnxiangtu.top/gtrbxnpzgi.html

Py:   os.path.getsize("a.txt")
来源：http://hz.yvedp.cn/gthxkacnzk.html

PHP:  filesize("a.txt");
来源：http://hz.svipenyu.cn/gtbukedfhu.html

JS:   fs.statSync("a.txt").size
来源：http://hz.jlsjyb.cn/gtfpujfutl.html

TS:   fs.statSync("a.txt").size
来源：http://hz.aizwys.cn/gtcxgzrobp.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.daria6918.cn/gteglwkzuh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.9152youxi.cn/gtjthdykmm.html

Ruby: File.size("a.txt")
来源：http://hz.hnqzz.top/gtuxbnfbqq.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.tianlin.xyz/gtvdohijcr.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.andypj.xyz/gtlhwgixhw.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.svipenyu.cn/gtnjrgkcts.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.svipenyu.cn/gtofvulkkq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.fzhhl.top/gtudobrseu.html

TS:   path.extname("a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtieqcwdwi.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.gogol.net.cn/gtpcygtosf.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.sxryk.cn/gtcrnunnyw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.hnqzz.top/gtenyvqflu.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.havefunace.top/gtbqmuzskd.html

[F11] 复制与移动文件
来源：http://hz.ydjk.org.cn/gtdxfneuwz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.xylfe.cn/gtszqvbist.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.redwolf501.top/gtsrehwdbb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.aibaodan.cn/gtetmspsig.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.9152youxi.cn/gtrxpimepa.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.redwolf501.top/gtjlnumieg.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.zycfv.cn/gtunojpqvi.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.jianghu66.top/gtzcgaavba.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.xuanzx.com/gtieydfrax.html

[F12] CSV 读写
来源：http://hz.haohaochexian.top/gtsqonqpyj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.9152youxi.cn/gtbgocycwp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.jiagoushi.top/gtbrrbmzwa.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.mhx1999.top/gtxubntpqv.html

TS:   // 同上
来源：http://hz.dashuyun.cn/gtlqoamqqc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.quarkkingdee.top/gtetuszqdy.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.9152youxi.cn/gtichrvjjy.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.chenzaomai.com/gtcgofolcj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yanxiufei.cn/gtkyzaakkr.html

================================================================================
来源：http://hz.jiagoushi.top/gtrsewamuv.html

G. 面向对象
来源：http://hz.hnxiangtu.top/gteuewkmyn.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtctbgxpmh.html

[G01] 定义类
来源：http://hz.feifeiyinyue.top/gtowhaxaqp.html

Py:   class User: pass
来源：http://hz.xuetiantiany.cn/gtllxyguip.html

PHP:  class User {}
来源：http://hz.chenlongwang.top/gtfovshfjl.html

JS:   class User {}
来源：http://hz.shuidangran.top/gtylavrzpk.html

TS:   class User { name: string = ""; }
来源：http://hz.yanxiufei.cn/gtwjdsxdac.html

Java: class User {}
来源：http://hz.hywenlv.cn/gtkvyjadft.html

Go:   type User struct { Name string }
来源：http://hz.yueranfly.top/gtzqsyucpw.html

Ruby: class User; end
来源：http://hz.yj202588.top/gtorxhtcfs.html

C#:   class User {}
来源：http://hz.aibaodan.cn/gtahlxkhbs.html

[G02] 构造函数
来源：http://hz.kuanghao11.cn/gtgeyahetn.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.ehwqpu.com/gtedygdpuu.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.xinyue.icu/gtvvamjtnf.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.zhengqikj.top/gtygfgrqhb.html

TS:   constructor(public name: string) {}
来源：http://hz.hywenlv.cn/gtytcntowl.html

Java: User(String name) { this.name = name; }
来源：http://hz.yuxming.cn/gtpjlkodvq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.ppjwa.cn/gtiyzffuok.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.gzhubu.top/gtzeeuymcp.html

C#:   public User(string name) { Name = name; }
来源：http://hz.hongshengwenyu.top/gtnagzaotp.html

[G03] 实例属性
来源：http://hz.hongshengwenyu.top/gtnmsjcnzt.html

Py:   self.name = "x"
来源：http://hz.smart0.xyz/gtqopdrwis.html

PHP:  public string $name = "x";
来源：http://hz.yongpay.top/gtifsnoxpr.html

JS:   this.name = "x";
来源：http://hz.jinghuilouyu.cn/gthqmsrupi.html

TS:   name: string = "x";
来源：http://hz.ppjwa.cn/gteztidoax.html

Java: private String name;
来源：http://hz.pycfn.com/gtjntorcec.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.hongshengwenyu.top/gtdilbtlwm.html

Ruby: @name = "x"
来源：http://hz.cheryme.top/gtunbdiefa.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.xuanzx.com/gtybauifiu.html

[G04] 定义方法
来源：http://hz.yj20258888.top/gtsjgwrhnl.html

Py:   def greet(self): return self.name
来源：http://hz.vqdsnc.cn/gtmjnmzjia.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.ywan-chungtsiang.top/gtlwztoizj.html

JS:   greet() { return this.name; }
来源：http://hz.snrcjt.cn/gtifmararv.html

TS:   greet(): string { return this.name; }
来源：http://hz.zhiwuduotai.top/gtjkcxgiid.html

Java: String greet() { return name; }
来源：http://hz.mhx1999.top/gtcllacuzt.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.hongshengwenyu.top/gtrmwlysum.html

Ruby: def greet; @name; end
来源：http://hz.hongshengwenyu.top/gtnamhzxim.html

C#:   public string Greet() => Name;
来源：http://hz.yonumen.top/gtirpbvwkx.html

[G05] 继承
来源：http://hz.xingfuxueyuan.xyz/gtycjteocc.html

Py:   class Admin(User): pass
来源：http://hz.zycfv.cn/gtzsbmqzvm.html

PHP:  class Admin extends User {}
来源：http://hz.gotoacloud.top/gtwhgrvmkz.html

JS:   class Admin extends User {}
来源：http://hz.sweek.top/gtldneilwq.html

TS:   class Admin extends User {}
来源：http://hz.aizwys.cn/gtefixwrxb.html

Java: class Admin extends User {}
来源：http://hz.yuxming.cn/gtfqubkfmf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.zhengqikj.top/gtcqguwazn.html

Ruby: class Admin < User; end
来源：http://hz.yvedp.cn/gtixbpzsjn.html

C#:   class Admin : User {}
来源：http://hz.ppjwa.cn/gtevaelzma.html

[G06] 重写方法
来源：http://hz.zhijiandao.cn/gttscbpnjp.html

Py:   def greet(self): return "admin"
来源：http://hz.shuidangran.top/gtcumbxfjn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jiagoushi.top/gtukupzxkw.html

JS:   greet() { return "admin"; }
来源：http://hz.aibaodan.cn/gtfwyuuvqa.html

TS:   greet(): string { return "admin"; }
来源：http://hz.yueranfly.top/gtszciysue.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.sufxvd.cn/gtomicbklb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.ehwqpu.com/gtftarjlkd.html

Ruby: def greet; "admin"; end
来源：http://hz.9152youxi.cn/gtymhpwsvh.html

C#:   public override string Greet() => "admin";
来源：http://hz.chenzaomai.com/gtvrgrguwr.html

[G07] 调用父类方法
来源：http://hz.birdmap.top/gtirbalntw.html

Py:   super().greet()
来源：http://hz.yongpay.top/gtmsargtiv.html

PHP:  parent::greet();
来源：http://hz.sufxvd.cn/gteidcwcbi.html

JS:   super.greet();
来源：http://hz.jiagoushi.top/gtgruflkab.html

TS:   super.greet();
来源：http://hz.zhijiandao.cn/gtnytebrmj.html

Java: super.greet();
来源：http://hz.gogol.net.cn/gtdsqkdcff.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.xuetiantiany.cn/gtivogofev.html

Ruby: super
来源：http://hz.gzhubu.top/gtumbycobo.html

C#:   base.Greet();
来源：http://hz.nanxinkj.top/gttfvttmgh.html

[G08] 静态方法与属性
来源：http://hz.dashuyun.cn/gtmkpvjwis.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.birdmap.top/gtkhyufrob.html

PHP:  public static function f() {}
来源：http://hz.shzxlz.cn/gtevqxsedy.html

JS:   static f() {}
来源：http://hz.shanyushiyangtech.top/gtubpcphpy.html

TS:   static f(): void {}
来源：http://hz.hywenlv.cn/gtllgpihrr.html

Java: static void f() {}
来源：http://hz.chenjidiqi.icu/gtsfaqblwk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.fengsongda.top/gtbwgvtagj.html

Ruby: def self.f; end
来源：http://hz.havefunace.top/gthxadmbsc.html

C#:   public static void F() {}
来源：http://hz.daria6918.cn/gteqsknaih.html

[G09] 接口 / 抽象类
来源：http://hz.mhx1999.top/gtzivocexh.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.jiagoushi.top/gtosznqcgf.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.zhongyouzk.top/gtmwduaupe.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.svipenyu.cn/gtxdmjjxhh.html

TS:   interface Shape { area(): number; }
来源：http://hz.9152youxi.cn/gtxghiconp.html

Java: interface Shape { double area(); }
来源：http://hz.aibaodan.cn/gtguebteye.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.shuidangran.top/gtpvbjmyrx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jyoumei.cn/gtyahfween.html

C#:   interface IShape { double Area(); }
来源：http://hz.pengpengdd.cyou/gtuoqfzbdf.html

[G10] 访问控制
来源：http://hz.nanxuanxn.top/gtutlxhths.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.xuetiantiany.cn/gtjluqqzna.html

PHP:  public / protected / private
来源：http://hz.52xcode.cn/gtmuuwfkqu.html

JS:   #private 字段；其余公开
来源：http://hz.9152youxi.cn/gtpiznnohb.html

TS:   public / protected / private
来源：http://hz.havefunace.top/gtqngnavah.html

Java: public / protected / private / 默认包级
来源：http://hz.ybcxt.top/gtaxacxysj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.iojbl.cn/gtnczskadf.html

Ruby: public / protected / private
来源：http://hz.jinyuanbaomall.cn/gtvlluyobd.html

C#:   public / protected / private / internal
来源：http://hz.xuetiantiany.cn/gtfiwmuosc.html

[G11] getter / setter
来源：http://hz.0kj1m.cn/gtaoyxllvt.html

Py:   @property 与 @x.setter
来源：http://hz.cqqwz.cn/gtgikxcyjg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.hysaishi.cn/gtwyjgaosx.html

JS:   get name() { return this._name; }
来源：http://hz.yj20258888.top/gtwbgjseys.html

TS:   get name(): string { return this._name; }
来源：http://hz.sufxvd.cn/gtzlcefbrs.html

Java: public String getName() { return name; }
来源：http://hz.xinyue.icu/gthyauhoku.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.xylfe.cn/gtcwmtragv.html


<!-- 参考信息 -->