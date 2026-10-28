代发 wailian999

PHP:  substr_count($s, "a");
来源：http://hz.sufxvd.cn/gtvjbdkfbm.html

JS:   s.split("a").length - 1
来源：http://hz.quarkkingdee.top/gtadzijfie.html

TS:   s.split("a").length - 1
来源：http://hz.xylfe.cn/gtmapvdogf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.pengpengdd.cyou/gtxvuirxjw.html

Go:   strings.Count(s, "a")
来源：http://hz.xingfuxueyuan.xyz/gtpbxnpjlp.html

Ruby: s.count("a")
来源：http://hz.iojbl.cn/gtqawoxyly.html

C#:   s.Count(c => c == 'a')
来源：http://hz.birdmap.top/gtjjusmlno.html

[E13] 逐字符遍历
来源：http://hz.hnqzz.top/gtrcsatlmw.html

Py:   for ch in s: print(ch)
来源：http://hz.shanyushiyangtech.top/gthlwtrtlj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.zhongyouzk.top/gtsrktasua.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.c1oappe.top/gtijjbkwjh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.gogol.net.cn/gtlryhbpcw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.chenzaomai.com/gtyootwfte.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.yanxiufei.cn/gtlzceqrtu.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.zhongyouzk.top/gtgwidqjnt.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.bjfxy.top/gthaovqxtj.html

[E14] URL 编码与 Base64
来源：http://hz.smart0.xyz/gtnaonehak.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.zdqjudy.top/gttngjtinn.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.chenjidiqi.icu/gtonniojfo.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.zhaomingkeji.xyz/gtdcuiakcz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.jqgufenzy.top/gtetpqwvtx.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.zhengqikj.top/gtbjmaipft.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.tanke756.top/gtunbykwaa.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.jinghuilouyu.cn/gtrlkofnme.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.shanyushiyangtech.top/gtdnmwzrmp.html

[E15] HTML 转义 / 反转义
来源：http://hz.nwbrower.top/gtsdpajapa.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.wangdashe.top/gtjftzcglv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.cqqwz.cn/gtrpsdroql.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.cashguo.top/gtoeswoveo.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.dianchejie.cn/gtcirubegy.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.zhijiandao.cn/gtphysuawh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.cqqwz.cn/gtqwyfvlhb.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.jianghu66.top/gthtblptvb.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.ydzc1.top/gtysjtiaew.html

[E16] 数字千分位
来源：http://hz.tianlin.xyz/gtkzdxkbpx.html

Py:   f"{1234567:,}"
来源：http://hz.hnqzz.top/gtgahxnjst.html

PHP:  number_format(1234567);
来源：http://hz.nanxuanxn.top/gtolmanyek.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.c1oappe.top/gtgutpudim.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.hnqzz.top/gteciyogmf.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.guannengcc.top/gttontwmrw.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.jinghuilouyu.cn/gtcuxuwhzv.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.nwbrower.top/gtwupslcyo.html

C#:   1234567.ToString("N0")
来源：http://hz.xinyue.icu/gtiyndgach.html

[E17] 首字母大写
来源：http://hz.gotoacloud.top/gtobvkytoc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.ydjk.org.cn/gteyzjxpba.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.jqgfzy.top/gtngmazieg.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.sxryk.cn/gtjnwfiglw.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.chenjidiqi.icu/gtthbtrkch.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.c1oappe.top/gtthzeysbs.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.hnqzz.top/gtznmfhasi.html

Ruby: s.capitalize
来源：http://hz.hfpthk.cn/gtoyudbrkg.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.sysykeji.top/gtqllrjxbh.html

[E18] 模板占位符替换
来源：http://hz.ppjwa.cn/gtgohyoyvc.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.redwolf501.top/gtkwhkgckt.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.sufxvd.cn/gtbnijsvbq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.haohaochexian.top/gtbluuegdp.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.0kj1m.cn/gtsexhyyhe.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.hywenlv.cn/gtjqbrasep.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.xziqi.cn/gtuxxsnemh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.hywenlv.cn/gtyjlffbvi.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.xuetiantiany.cn/gtwxovpfdp.html

[E19] 多行文本按行拆分
来源：http://hz.zycfv.cn/gtqqrqxsyr.html

Py:   s.splitlines()
来源：http://hz.cucudq.cn/gtxydnpcms.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.c1oappe.top/gtzqirgtzn.html

JS:   s.split(/\r?\n/)
来源：http://hz.zhixingplan.top/gtdttzvmkx.html

TS:   s.split(/\r?\n/)
来源：http://hz.52xcode.cn/gtkxndrvmg.html

Java: s.lines().toList()
来源：http://hz.yj20258888.top/gtqxrscvzx.html

Go:   strings.Split(s, "\n")
来源：http://hz.zhiwuduotai.top/gtvedzbvsb.html

Ruby: s.lines
来源：http://hz.yongpay.top/gtswrtzwds.html

C#:   s.Split('\n')
来源：http://hz.yj20258.top/gtowlinfsj.html

[E20] 判断字符串是否为空
来源：http://hz.yangfankeji.com/gtmiitrbmn.html

Py:   if not s:
来源：http://hz.sysykeji.top/gtudwhrnbr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.zdqjudy.top/gtxvlsxvtb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.jyoumei.cn/gteyushcnq.html

TS:   if (s === "") {}
来源：http://hz.ywan-chungtsiang.top/gtvjhqljym.html

Java: if (s.isEmpty()) {}
来源：http://hz.kuanghao11.cn/gtgpnowsju.html

Go:   if s == "" {}
来源：http://hz.yangfankeji.com/gtkkikploy.html

Ruby: if s.empty?
来源：http://hz.xuetiantiany.cn/gtlbmoxexk.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.0kj1m.cn/gtjnrnnjkw.html

[E21] 超长截断加省略号
来源：http://hz.shzxlz.cn/gtzdpsxjzi.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.xuanzx.com/gtbmsjpbzo.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.chenzaomai.com/gtmlgqghut.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.daria6918.cn/gtvmxdbdct.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.iojbl.cn/gtrlefxunv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.xziqi.cn/gtlideousd.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.yj20258888.top/gtjxmfdzga.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.tianlin.xyz/gthuozwbfg.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.gotoacloud.top/gtxgburndk.html

[E22] 字节长度与字符长度
来源：http://hz.yj202588.top/gtfmgtdmjx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.yuanzhike.top/gtruvmjsew.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.svipenyu.cn/gtqbqobjat.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hnqzz.top/gthbmahitj.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.xuanzx.com/gtuknlqebt.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.hammf.cn/gtdjlnlntg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.zhixingplan.top/gtolpoqeja.html

Ruby: s.bytesize;  s.length
来源：http://hz.daria6918.cn/gtscahvrue.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.hywenlv.cn/gtixkuzobf.html

================================================================================
来源：http://hz.mhx1999.top/gtxsolsvwa.html

F. 文件与目录
来源：http://hz.9152youxi.cn/gtcrafzeou.html

================================================================================
来源：http://hz.fzhhl.top/gtudaaozld.html

[F01] 读取整个文件
来源：http://hz.zhixingplan.top/gtehnkrybu.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.chenjidiqi.icu/gtikbfcurd.html

PHP:  file_get_contents("a.txt");
来源：http://hz.chenzaomai.com/gtmuiqvexl.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.gotoacloud.top/gtkgrgshuz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.redwolf501.top/gtzvmnffps.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.xuetiantiany.cn/gtuxgnsbvi.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.guowangkeji.top/gtqabdrfvb.html

Ruby: File.read("a.txt")
来源：http://hz.yvedp.cn/gtcdmfltzo.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.vqdsnc.cn/gtbshchbnn.html

[F02] 逐行读取文件
来源：http://hz.ehwqpu.com/gtafxjxjaj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.guannengcc.top/gtiefhwonn.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.ppjwa.cn/gtskbdonxb.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hongshengwenyu.top/gtwerzgdtp.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhengqikj.top/gtfgrthlee.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.jinqigufen.top/gtnfxzudrp.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.nanxinkj.top/gtxjbwehxm.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.zhengqikj.top/gtmrpinngz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.hammf.cn/gtyhclwind.html

[F03] 写入文件（覆盖）
来源：http://hz.daxiang520.top/gtjhmpsica.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.xuanzx.com/gtzflxpswb.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.zhongyouzk.top/gtessfkzck.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.birdmap.top/gtftaovrab.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yongpay.top/gthksdkhde.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.ivvv.top/gtuizgdukl.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.ybcxt.top/gtenykanar.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.hywenlv.cn/gtqlostgud.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.yj202588.top/gtremtmjtp.html

[F04] 追加写入文件
来源：http://hz.yj20258.top/gtpnqsugxa.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.snrcjt.cn/gtsjabddfx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.tanke756.top/gtifetvbyx.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.mhx1999.top/gtodokplkv.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.shanyushiyangtech.top/gtqxqzqgzn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.zhengqikj.top/gtgdgrpiun.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.gzhubu.top/gtnhqgiyvx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.vqdsnc.cn/gtzwknyuwj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.shzxlz.cn/gthpygltmq.html

[F05] 判断文件或目录是否存在
来源：http://hz.aizwys.cn/gtgetcatqn.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.wangshuangyany.cn/gtmvqbxcba.html

PHP:  file_exists("a.txt");
来源：http://hz.cdnleiting.top/gtjnucwauy.html

JS:   fs.existsSync("a.txt")
来源：http://hz.xziqi.cn/gtptcumkrq.html

TS:   fs.existsSync("a.txt")
来源：http://hz.hysaishi.cn/gtufzwgcia.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.yonumen.top/gtcutnxwry.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.ywan-chungtsiang.top/gtmxvzyuez.html

Ruby: File.exist?("a.txt")
来源：http://hz.smart0.xyz/gtdsxmzdks.html

C#:   File.Exists("a.txt")
来源：http://hz.0kj1m.cn/gtibcfhifg.html

[F06] 删除文件
来源：http://hz.jyoumei.cn/gtnsmhiqys.html

Py:   os.remove("a.txt")
来源：http://hz.316326.xyz/gtkfwoxyvg.html

PHP:  unlink("a.txt");
来源：http://hz.shzxlz.cn/gtxmvgrucs.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.xziqi.cn/gtcbangcwe.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.gzhubu.top/gtqtujkpln.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.fengsongda.top/gtiyselezh.html

Go:   os.Remove("a.txt")
来源：http://hz.sweek.top/gtmleurwic.html

Ruby: File.delete("a.txt")
来源：http://hz.chenjidiqi.icu/gtglyufblg.html

C#:   File.Delete("a.txt");
来源：http://hz.birdmap.top/gtivjboqiu.html

[F07] 创建目录（含多级）
来源：http://hz.gotoacloud.top/gtnwzdoljt.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.jinghuilouyu.cn/gtrngwgtcc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.hongshengwenyu.top/gtfwiiucqv.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.aizwys.cn/gtyzwnijaj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.gotoacloud.top/gtmhyqupgw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.c1oappe.top/gtyucurbgu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.yuxming.cn/gtijtzjbpr.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.tian-w.cn/gtjghvajpo.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.nanxinkj.top/gtcxisyfbb.html

[F08] 遍历目录
来源：http://hz.smart0.xyz/gtxhsxcynw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.ybcxt.top/gtpscocuir.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.cqqwz.cn/gtyhonadtv.html

JS:   fs.readdirSync("dir")
来源：http://hz.iojbl.cn/gtvxxnbztm.html

TS:   fs.readdirSync("dir")
来源：http://hz.jianghu66.top/gtdvbfbukm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.hysaishi.cn/gtqvpdzukg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.sufxvd.cn/gtnlukyhdo.html

Ruby: Dir.children("dir")
来源：http://hz.jlsjyb.cn/gtzhbsjdqt.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yvedp.cn/gtcnoddqzk.html

[F09] 获取文件大小
来源：http://hz.c1oappe.top/gtcakqmzeb.html

Py:   os.path.getsize("a.txt")
来源：http://hz.yj20258888.top/gtvpbdkvuh.html

PHP:  filesize("a.txt");
来源：http://hz.yanxiufei.cn/gtcjbdlpyd.html

JS:   fs.statSync("a.txt").size
来源：http://hz.hywenlv.cn/gtgmqehins.html

TS:   fs.statSync("a.txt").size
来源：http://hz.andypj.xyz/gtbvtoprxr.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.chenlongwang.top/gtmemwfdul.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.ivvv.top/gtfpubbwxs.html

Ruby: File.size("a.txt")
来源：http://hz.xuetiantiany.cn/gtfuubkytj.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.jinqigufen.top/gtwkvjnrxu.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.gzhubu.top/gtudaqhuyb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.sweek.top/gtpypedvjk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.daxiang520.top/gtvuqklylu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.aibaodan.cn/gtcnipulpo.html

TS:   path.extname("a.txt")
来源：http://hz.yuxming.cn/gtvzpbhpxw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.zhengqikj.top/gtaifitpap.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.wangdashe.top/gtfzsnrpxe.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.dashuyun.cn/gtazyweaai.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.jinyuanbaomall.cn/gtqxgedxop.html

[F11] 复制与移动文件
来源：http://hz.316326.xyz/gtsmyvvxus.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.hammf.cn/gtcflhduos.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.guannengcc.top/gtxqgrwyqb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.meibo888.top/gtakpqxvwt.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.haohaochexian.top/gthmfjoosn.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.hongshengwenyu.top/gtywecprkx.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.shzxlz.cn/gtogszliui.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.yj202588.top/gtzodyqbbk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.redwolf501.top/gtrchkpfbj.html

[F12] CSV 读写
来源：http://hz.9152youxi.cn/gtwyhfstxj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.jinyuanbaomall.cn/gtwjoiqwqy.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.shangyingyoupin.top/gtmsvqvofd.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.chenzaomai.com/gtqzgolayx.html

TS:   // 同上
来源：http://hz.ehwqpu.com/gtuqypyyfr.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.chenzaomai.com/gtgtmyavsc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.gzhubu.top/gtnoagaqoq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.snrcjt.cn/gtcfshgfxi.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.hongshengwenyu.top/gtvpwnkank.html

================================================================================
来源：http://hz.jiagoushi.top/gtuemjgpfw.html

G. 面向对象
来源：http://hz.yongpay.top/gtiadiatnp.html

================================================================================
来源：http://hz.hywenlv.cn/gtixfawuuj.html

[G01] 定义类
来源：http://hz.nanxinkj.top/gteieuzwaj.html

Py:   class User: pass
来源：http://hz.hfpthk.cn/gtyqikzcjo.html

PHP:  class User {}
来源：http://hz.vqdsnc.cn/gtsbuknuhj.html

JS:   class User {}
来源：http://hz.yuanzhike.top/gtzmmbtkwf.html

TS:   class User { name: string = ""; }
来源：http://hz.wangshuangyany.cn/gtbiygbflf.html

Java: class User {}
来源：http://hz.chenzaomai.com/gtycugjpod.html

Go:   type User struct { Name string }
来源：http://hz.zycfv.cn/gtpylsmnqr.html

Ruby: class User; end
来源：http://hz.zycfv.cn/gtjruqbass.html

C#:   class User {}
来源：http://hz.tanke756.top/gtbkxjtayo.html

[G02] 构造函数
来源：http://hz.kuanghao11.cn/gtjijrkxzp.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.pycfn.com/gtzzszrnlb.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.sweek.top/gtdneesuuc.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.cashguo.top/gtccuyojys.html

TS:   constructor(public name: string) {}
来源：http://hz.jinyuanbaomall.cn/gtducubasz.html

Java: User(String name) { this.name = name; }
来源：http://hz.sufxvd.cn/gtcooyevyr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jinghuilouyu.cn/gthjddjzte.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yuanzhike.top/gtgtsyeniu.html

C#:   public User(string name) { Name = name; }
来源：http://hz.gzhubu.top/gtgzzohode.html

[G03] 实例属性
来源：http://hz.wangdashe.top/gtvaxcpzkj.html

Py:   self.name = "x"
来源：http://hz.xziqi.cn/gtlsazdcjx.html

PHP:  public string $name = "x";
来源：http://hz.jinghuilouyu.cn/gtvrfwuhui.html

JS:   this.name = "x";
来源：http://hz.jinqigfzy.top/gtbjwveexm.html

TS:   name: string = "x";
来源：http://hz.xziqi.cn/gtmsxcqqav.html

Java: private String name;
来源：http://hz.cdnleiting.top/gtgdyoifey.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.jinqigufen.top/gtzafcomll.html

Ruby: @name = "x"
来源：http://hz.haohaochexian.top/gtvkrjlfnn.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.vqdsnc.cn/gtmdarfvxz.html

[G04] 定义方法
来源：http://hz.hywenlv.cn/gtbtxedpxa.html

Py:   def greet(self): return self.name
来源：http://hz.sysykeji.top/gtpstvlyvk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.tian-w.cn/gtcftcanrb.html

JS:   greet() { return this.name; }
来源：http://hz.kuanghao11.cn/gtyawpadsy.html

TS:   greet(): string { return this.name; }
来源：http://hz.pycfn.com/gtdhujcsdb.html

Java: String greet() { return name; }
来源：http://hz.hfpthk.cn/gtaigtowtp.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.gogol.net.cn/gtmngtcdlw.html

Ruby: def greet; @name; end
来源：http://hz.gogol.net.cn/gthbzyxctf.html

C#:   public string Greet() => Name;
来源：http://hz.hfpthk.cn/gtyteejwgf.html

[G05] 继承
来源：http://hz.guannengcc.top/gtcvankcvs.html

Py:   class Admin(User): pass
来源：http://hz.aizwys.cn/gtlapmxuch.html

PHP:  class Admin extends User {}
来源：http://hz.jqgfzy.top/gtpgwbwxbq.html

JS:   class Admin extends User {}
来源：http://hz.jiagoushi.top/gtljedotrx.html

TS:   class Admin extends User {}
来源：http://hz.xziqi.cn/gtisczjwdk.html

Java: class Admin extends User {}
来源：http://hz.guowangkeji.top/gtrunrupcq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.snrcjt.cn/gtmgcrwwlv.html

Ruby: class Admin < User; end
来源：http://hz.zycfv.cn/gtpsfvirgl.html

C#:   class Admin : User {}
来源：http://hz.bjfxy.top/gtpykginwm.html

[G06] 重写方法
来源：http://hz.yongpay.top/gthehxvfdj.html

Py:   def greet(self): return "admin"
来源：http://hz.xziqi.cn/gtbaybduce.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.zycfv.cn/gtxmdykveh.html

JS:   greet() { return "admin"; }
来源：http://hz.0kj1m.cn/gtogfqdver.html

TS:   greet(): string { return "admin"; }
来源：http://hz.xylfe.cn/gtckofzrpr.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.shuidangran.top/gtodpnjuep.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.sweek.top/gtwmcfzzys.html

Ruby: def greet; "admin"; end
来源：http://hz.yuxming.cn/gtnlqoleyh.html

C#:   public override string Greet() => "admin";
来源：http://hz.xuanzx.com/gtsaxyrefe.html

[G07] 调用父类方法
来源：http://hz.hammf.cn/gtriwcjmeb.html

Py:   super().greet()
来源：http://hz.nanxinkj.top/gtkwcndkod.html

PHP:  parent::greet();
来源：http://hz.haohaochexian.top/gtdnluznek.html

JS:   super.greet();
来源：http://hz.zhoulong.xyz/gtzolpndoj.html

TS:   super.greet();
来源：http://hz.pycfn.com/gtquirinkj.html

Java: super.greet();
来源：http://hz.zycfv.cn/gtoihstbgj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.9152youxi.cn/gttxxmwdvw.html

Ruby: super
来源：http://hz.xingfuxueyuan.xyz/gtvjffoelg.html

C#:   base.Greet();
来源：http://hz.9152youxi.cn/gtkbbttznf.html

[G08] 静态方法与属性
来源：http://hz.smart0.xyz/gtegkdphhz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.dianchejie.cn/gtvpgkhanw.html

PHP:  public static function f() {}
来源：http://hz.chenzaomai.com/gtwyobzquz.html

JS:   static f() {}
来源：http://hz.cashguo.top/gtdpyuzmbq.html

TS:   static f(): void {}
来源：http://hz.wangdashe.top/gtfcroawbt.html

Java: static void f() {}
来源：http://hz.guannengcc.top/gtipjudahy.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yongpay.top/gttdcxynon.html

Ruby: def self.f; end
来源：http://hz.zhiwuduotai.top/gtczmiyxle.html

C#:   public static void F() {}
来源：http://hz.jiagoushi.top/gtufuhfvvp.html

[G09] 接口 / 抽象类
来源：http://hz.xziqi.cn/gtljkpmuvc.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.vqdsnc.cn/gthhwfwqai.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jqgufenzy.top/gtvtbbnzif.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.nanxinkj.top/gttojsiaie.html

TS:   interface Shape { area(): number; }
来源：http://hz.yonumen.top/gtzlmiwckp.html

Java: interface Shape { double area(); }
来源：http://hz.shuidangran.top/gteshbrakr.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.hnxiangtu.top/gtgsvausov.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yongpay.top/gtwsimoyld.html

C#:   interface IShape { double Area(); }
来源：http://hz.wangdashe.top/gtmrwgmmxb.html

[G10] 访问控制
来源：http://hz.chenzaomai.com/gtrvczyptw.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.dashuyun.cn/gtplhcbjmn.html

PHP:  public / protected / private
来源：http://hz.hnxiangtu.top/gtxfxdgcsl.html

JS:   #private 字段；其余公开
来源：http://hz.jlsjyb.cn/gtkdcocyyv.html

TS:   public / protected / private
来源：http://hz.hysaishi.cn/gtfkvpdcww.html

Java: public / protected / private / 默认包级
来源：http://hz.jinghuilouyu.cn/gtnxseryfy.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zhaomingkeji.xyz/gtrljfclcx.html

Ruby: public / protected / private
来源：http://hz.kuanghao11.cn/gtwogmwhiz.html


<!-- 参考信息 -->