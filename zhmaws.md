代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.sxryk.cn/gtbsuganxm.html

[E11] 反转字符串
来源：http://hz.fzhhl.top/gtqtwrkwjb.html

Py:   s[::-1]
来源：http://hz.chenzaomai.com/gtpseptwcg.html

PHP:  strrev($s);
来源：http://hz.vqdsnc.cn/gtgcuulkwn.html

JS:   [...s].reverse().join("")
来源：http://hz.aizwys.cn/gtwvbhiclp.html

TS:   [...s].reverse().join("")
来源：http://hz.zhoulong.xyz/gtpvklftqa.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.svipenyu.cn/gttinnmmak.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.zhoulong.xyz/gtcdgqbyhl.html

Ruby: s.reverse
来源：http://hz.zhaomingkeji.xyz/gtfznqtepj.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.yueranfly.top/gtuovkejfp.html

[E12] 统计某字符出现次数
来源：http://hz.wangshuangyany.cn/gtpzifvwld.html

Py:   s.count("a")
来源：http://hz.wangshuangyany.cn/gtmlqvslij.html

PHP:  substr_count($s, "a");
来源：http://hz.hongshengwenyu.top/gtjjahwsis.html

JS:   s.split("a").length - 1
来源：http://hz.xylfe.cn/gtrflxtweb.html

TS:   s.split("a").length - 1
来源：http://hz.tanke756.top/gtyvdyhvud.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.hnqzz.top/gtnvjutbzk.html

Go:   strings.Count(s, "a")
来源：http://hz.ydjk.org.cn/gtqacuhuhk.html

Ruby: s.count("a")
来源：http://hz.yj20258888.top/gtqmwxvmhf.html

C#:   s.Count(c => c == 'a')
来源：http://hz.hongshengwenyu.top/gtwnavvydx.html

[E13] 逐字符遍历
来源：http://hz.cqqwz.cn/gtclgssqto.html

Py:   for ch in s: print(ch)
来源：http://hz.dashuyun.cn/gtdcbolkmp.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.jinqigufen.top/gtvbntheea.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.tian-w.cn/gtcehpavvc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yanxiufei.cn/gtjbixvvkk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.tianlin.xyz/gtndmzlseu.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.meibo888.top/gthtcogqlt.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.zhixingplan.top/gtnmihkmld.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.jiagoushi.top/gthtlfiojz.html

[E14] URL 编码与 Base64
来源：http://hz.haohaochexian.top/gtwlsysfjg.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.0kj1m.cn/gtgxeithiq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.pengpengdd.cyou/gtfdhubtjy.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.redwolf501.top/gtaocebfxm.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.chenlongwang.top/gtpfgkkvei.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.ppjwa.cn/gtwapulkoo.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.gotoacloud.top/gtuylkyjpt.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.hywenlv.cn/gthczsqary.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.hammf.cn/gtxnsdzkjz.html

[E15] HTML 转义 / 反转义
来源：http://hz.meibo888.top/gtxqsthqfc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.zhongyouzk.top/gtsdkhvutf.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.hysaishi.cn/gtjfmumare.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.jiagoushi.top/gtadhfsbgo.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.hywenlv.cn/gteechpcfc.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.tianlin.xyz/gtbjfrvzyx.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.hfpthk.cn/gtmyhewdbj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.nanxinkj.top/gtvcuvlups.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.jinyuanbaomall.cn/gtarrxlnsi.html

[E16] 数字千分位
来源：http://hz.sxryk.cn/gtkcikggbs.html

Py:   f"{1234567:,}"
来源：http://hz.fengsongda.top/gtkrcqklqc.html

PHP:  number_format(1234567);
来源：http://hz.316326.xyz/gtyrduynpi.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.xuetiantiany.cn/gtdohbflil.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.hammf.cn/gtvtufuslt.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.fengsongda.top/gtxajxnwih.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.feifeiyinyue.top/gtxbtypfoy.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.yvedp.cn/gtofagtxay.html

C#:   1234567.ToString("N0")
来源：http://hz.daxiang520.top/gtzawplfzs.html

[E17] 首字母大写
来源：http://hz.yuanzhike.top/gtxnycfweo.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.hywenlv.cn/gtpginoelg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.dianchejie.cn/gtplxicdtr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.shzxlz.cn/gtidedlbky.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.feifeiyinyue.top/gtcypvztui.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.tian-w.cn/gtyvmjjcuf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.svipenyu.cn/gtxsgczjwg.html

Ruby: s.capitalize
来源：http://hz.yueranfly.top/gtxvpbwgwc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.hywenlv.cn/gtqfchrpuh.html

[E18] 模板占位符替换
来源：http://hz.tianlin.xyz/gtvpfozemh.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.cashguo.top/gtkpuujjdd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.hfpthk.cn/gterdghrrw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.jinqigfzy.top/gtgtyhxrwe.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.havefunace.top/gteblwwmbp.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.tian-w.cn/gtdyimatpw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.jinqigufen.top/gtabywedeq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.nwbrower.top/gtmavmbfey.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.jinqigufen.top/gtkxvatden.html

[E19] 多行文本按行拆分
来源：http://hz.pycfn.com/gtkdxvfdgc.html

Py:   s.splitlines()
来源：http://hz.zdqjudy.top/gtewjkjlmj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.cucudq.cn/gtxynccfwg.html

JS:   s.split(/\r?\n/)
来源：http://hz.xuanzx.com/gtvcvfnqkw.html

TS:   s.split(/\r?\n/)
来源：http://hz.316326.xyz/gtyjlmsrgn.html

Java: s.lines().toList()
来源：http://hz.pengpengdd.cyou/gtmmboshtm.html

Go:   strings.Split(s, "\n")
来源：http://hz.shanyushiyangtech.top/gtxozqwuns.html

Ruby: s.lines
来源：http://hz.zdqjudy.top/gtbiwsgkcp.html

C#:   s.Split('\n')
来源：http://hz.havefunace.top/gtpmqnyqtr.html

[E20] 判断字符串是否为空
来源：http://hz.cdnleiting.top/gttgsbqnwy.html

Py:   if not s:
来源：http://hz.gaohongyu789.top/gtwhcbanhc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.yangfankeji.com/gtsbapfmyn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.xuanzx.com/gtxmfdbcwa.html

TS:   if (s === "") {}
来源：http://hz.gzhubu.top/gtuwopodzw.html

Java: if (s.isEmpty()) {}
来源：http://hz.feifeiyinyue.top/gtdaligtag.html

Go:   if s == "" {}
来源：http://hz.yj202588.top/gtiwcknjfq.html

Ruby: if s.empty?
来源：http://hz.hammf.cn/gthfmcihdv.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.redwolf501.top/gtarhqbsiz.html

[E21] 超长截断加省略号
来源：http://hz.smart0.xyz/gttpvdwsvb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.yanxiufei.cn/gtuoaunnbq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.hywenlv.cn/gtrgibrlgc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.andypj.xyz/gtlgnymxix.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.52xcode.cn/gtlrvatpcj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.ydzc1.top/gtauutinys.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.shangyingyoupin.top/gtaxskkngu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.yj20258888.top/gtkqidvygx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.dianchejie.cn/gtwhorowjh.html

[E22] 字节长度与字符长度
来源：http://hz.nwbrower.top/gtjcqltiqx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.meibo888.top/gtzerdgqid.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.birdmap.top/gtdxwuphcw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.cheryme.top/gthicwdyqo.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.shanyushiyangtech.top/gtlbpdzrwf.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.dianchejie.cn/gtgxvmkkll.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.xinyue.icu/gtshcgvzgh.html

Ruby: s.bytesize;  s.length
来源：http://hz.yueranfly.top/gtkkklkutr.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.gogol.net.cn/gtefxgplof.html

================================================================================
来源：http://hz.ehwqpu.com/gtofrvxnxz.html

F. 文件与目录
来源：http://hz.yuxming.cn/gtplkrvrwb.html

================================================================================
来源：http://hz.yuanzhike.top/gtsrawvzra.html

[F01] 读取整个文件
来源：http://hz.jyoumei.cn/gtlfqmouhi.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.mhx1999.top/gtzkbjktkr.html

PHP:  file_get_contents("a.txt");
来源：http://hz.aibaodan.cn/gtatjjnefr.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.hammf.cn/gthveywvny.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.wangshuangyany.cn/gtfjuhtnxm.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.shangyingyoupin.top/gtlavscafq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zhaomingkeji.xyz/gtruipqjxu.html

Ruby: File.read("a.txt")
来源：http://hz.wangdashe.top/gtghmxaalg.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yvedp.cn/gtyoblvqwx.html

[F02] 逐行读取文件
来源：http://hz.zhixingplan.top/gtpmxllibz.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.andypj.xyz/gtpqsxwkpd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.cucudq.cn/gthmsnmldk.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jinyuanbaomall.cn/gtustqxrom.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hnxiangtu.top/gtrnoeytkb.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.redwolf501.top/gtbckqrhlu.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.daria6918.cn/gtinhpoyqj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.cashguo.top/gtlffjvajj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.cashguo.top/gtxuqnwdfx.html

[F03] 写入文件（覆盖）
来源：http://hz.yj202588.top/gtbxfbxufo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.shanyushiyangkeji.top/gttfobpxhd.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.fengsongda.top/gtwfoguowj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.sufxvd.cn/gtskwzqcxq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhiwuduotai.top/gtbztdbgtw.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.redwolf501.top/gtkaxhplob.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.gogol.net.cn/gtnkrdlqgj.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.sxryk.cn/gtsoyxwjql.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.jyoumei.cn/gtllnviqbx.html

[F04] 追加写入文件
来源：http://hz.chenlongwang.top/gtqpggwrug.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yj20258888.top/gtienbctye.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.mhx1999.top/gtefctpxee.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.mhx1999.top/gtxljbpvcg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yuxming.cn/gtifeqjphx.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.haohaochexian.top/gtxmxkznug.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.feifeiyinyue.top/gtwtevpnzi.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.chenjidiqi.icu/gtfqgjaajq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.zdqjudy.top/gtwlrbyocl.html

[F05] 判断文件或目录是否存在
来源：http://hz.yangfankeji.com/gtbkpuzsga.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.fzhhl.top/gtmoawmmsp.html

PHP:  file_exists("a.txt");
来源：http://hz.ivvv.top/gtxtfzyyca.html

JS:   fs.existsSync("a.txt")
来源：http://hz.nanxuanxn.top/gtqxdtexvh.html

TS:   fs.existsSync("a.txt")
来源：http://hz.pycfn.com/gtruwshpmo.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.feifeiyinyue.top/gtntnzwwfh.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.zdqjudy.top/gtemlewwet.html

Ruby: File.exist?("a.txt")
来源：http://hz.jyoumei.cn/gtsqhydwtx.html

C#:   File.Exists("a.txt")
来源：http://hz.316326.xyz/gthgwlunfo.html

[F06] 删除文件
来源：http://hz.9152youxi.cn/gtxtuvkvbk.html

Py:   os.remove("a.txt")
来源：http://hz.xylfe.cn/gtewqqzsic.html

PHP:  unlink("a.txt");
来源：http://hz.yj202588.top/gtnstogtpf.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.dashuyun.cn/gtpgpbcejp.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.cqqwz.cn/gtildcpekc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.jinghuilouyu.cn/gtqxnfnwci.html

Go:   os.Remove("a.txt")
来源：http://hz.yueranfly.top/gtpnpayrdt.html

Ruby: File.delete("a.txt")
来源：http://hz.fengsongda.top/gtnnabkksm.html

C#:   File.Delete("a.txt");
来源：http://hz.nwbrower.top/gtfwxgbdih.html

[F07] 创建目录（含多级）
来源：http://hz.hywenlv.cn/gtvacvsewj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.jqgufenzy.top/gttvliynvm.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.hysaishi.cn/gtdtfgoems.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hammf.cn/gtgfdsjilp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhaomingkeji.xyz/gtaxuczgke.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.meibo888.top/gttuhwqkem.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.gzhubu.top/gtcfrsvmcz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.316326.xyz/gtgzbzlegq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.zhengqikj.top/gtdtsivxia.html

[F08] 遍历目录
来源：http://hz.snrcjt.cn/gttcwzbdrp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.jqgufenzy.top/gtlvqxuaza.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.jinghuilouyu.cn/gtuosvfyfp.html

JS:   fs.readdirSync("dir")
来源：http://hz.c1oappe.top/gtbicfkava.html

TS:   fs.readdirSync("dir")
来源：http://hz.wangshuangyany.cn/gtadzevzzu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.daxiang520.top/gtepagdglz.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.hfpthk.cn/gtrddcxvxx.html

Ruby: Dir.children("dir")
来源：http://hz.aizwys.cn/gtakqkkhbt.html

C#:   Directory.GetFiles("dir")
来源：http://hz.kuanghao11.cn/gtqfihubyr.html

[F09] 获取文件大小
来源：http://hz.xuetiantiany.cn/gtporuwamt.html

Py:   os.path.getsize("a.txt")
来源：http://hz.xinyue.icu/gtohbkhfad.html

PHP:  filesize("a.txt");
来源：http://hz.jinyuanbaomall.cn/gtjtmzfegx.html

JS:   fs.statSync("a.txt").size
来源：http://hz.cqqwz.cn/gtjujqdccf.html

TS:   fs.statSync("a.txt").size
来源：http://hz.zhiwuduotai.top/gterlacact.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.9152youxi.cn/gtibsthobq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.xuanzx.com/gtmiqsqebm.html

Ruby: File.size("a.txt")
来源：http://hz.vqdsnc.cn/gtgmmadjnq.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.tian-w.cn/gtluqoywtt.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.andypj.xyz/gtlibbougw.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.wangdashe.top/gtldhpfgun.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.yvedp.cn/gtqhdxevbu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.yongpay.top/gttljuyxwg.html

TS:   path.extname("a.txt")
来源：http://hz.ydzc1.top/gtjnvthjrg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.ppjwa.cn/gtkbugetmf.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.chenjidiqi.icu/gtzeihzkfa.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.hysaishi.cn/gteccklsxt.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.mhx1999.top/gtxuhckotz.html

[F11] 复制与移动文件
来源：http://hz.hnqzz.top/gtwijxhpun.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.cashguo.top/gtdjyjfttx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.ehwqpu.com/gtzaxfjmzx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.iojbl.cn/gtjaolwwpu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.guowangkeji.top/gtxsavshiu.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.c1oappe.top/gtcepgpatw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jinqigufen.top/gtthwkhezs.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.mhx1999.top/gtkvefwkco.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.hnqzz.top/gtpcwedakn.html

[F12] CSV 读写
来源：http://hz.aibaodan.cn/gtfcvwfbgl.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.sxryk.cn/gtsabnkqps.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.chenjidiqi.icu/gttffpewoa.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.zhongyouzk.top/gtpggwkpkv.html

TS:   // 同上
来源：http://hz.zdqjudy.top/gtjjqwrdcd.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.quarkkingdee.top/gtmlyhsdyl.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.andypj.xyz/gttgnushfv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.shanyushiyangkeji.top/gtvsbnsokd.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.tian-w.cn/gtisxztahx.html

================================================================================
来源：http://hz.shzxlz.cn/gtclzzswfy.html

G. 面向对象
来源：http://hz.tian-w.cn/gtwootgafd.html

================================================================================
来源：http://hz.haohaochexian.top/gtqdyzwhmr.html

[G01] 定义类
来源：http://hz.yvedp.cn/gtiloyesfc.html

Py:   class User: pass
来源：http://hz.gotoacloud.top/gtjyjarrno.html

PHP:  class User {}
来源：http://hz.iojbl.cn/gtuqkkbpne.html

JS:   class User {}
来源：http://hz.tian-w.cn/gtctofsren.html

TS:   class User { name: string = ""; }
来源：http://hz.aizwys.cn/gtiwuflrzs.html

Java: class User {}
来源：http://hz.hfpthk.cn/gtyrivbggo.html

Go:   type User struct { Name string }
来源：http://hz.yj20258.top/gtyetwsvzk.html

Ruby: class User; end
来源：http://hz.jlsjyb.cn/gtvnydjpfx.html

C#:   class User {}
来源：http://hz.havefunace.top/gtyhqlsxuv.html

[G02] 构造函数
来源：http://hz.yvedp.cn/gtcexazwuf.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zhongyouzk.top/gtgxbszzpn.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.xziqi.cn/gtpuhyghrt.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.haohaochexian.top/gtaqkcrjqo.html

TS:   constructor(public name: string) {}
来源：http://hz.pengpengdd.cyou/gtewcxykfl.html

Java: User(String name) { this.name = name; }
来源：http://hz.9152youxi.cn/gtqfreoine.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.haohaochexian.top/gtnbfzrplp.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.xinyue.icu/gtimtislix.html

C#:   public User(string name) { Name = name; }
来源：http://hz.daria6918.cn/gtddsvwfps.html

[G03] 实例属性
来源：http://hz.tanke756.top/gtcnxhpftt.html

Py:   self.name = "x"
来源：http://hz.cdnleiting.top/gtuuwlnytw.html

PHP:  public string $name = "x";
来源：http://hz.xinyue.icu/gtptopajuq.html

JS:   this.name = "x";
来源：http://hz.ivvv.top/gtjjfijqbh.html

TS:   name: string = "x";
来源：http://hz.316326.xyz/gtnkgjauqi.html

Java: private String name;
来源：http://hz.zhengqikj.top/gtkcteyiys.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.smart0.xyz/gtmsnwdbod.html

Ruby: @name = "x"
来源：http://hz.yueranfly.top/gtjlljuazc.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.zhijiandao.cn/gtbtxjsojb.html

[G04] 定义方法
来源：http://hz.zdqjudy.top/gtqyexsvsd.html

Py:   def greet(self): return self.name
来源：http://hz.jlsjyb.cn/gtcvfipvtx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.jinqigufen.top/gtbteihzzk.html

JS:   greet() { return this.name; }
来源：http://hz.xingfuxueyuan.xyz/gtuditoxrb.html

TS:   greet(): string { return this.name; }
来源：http://hz.jiagoushi.top/gtdwpzsinm.html

Java: String greet() { return name; }
来源：http://hz.sxryk.cn/gtkjlhfqbr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.ppjwa.cn/gtkyubmfga.html

Ruby: def greet; @name; end
来源：http://hz.dianchejie.cn/gtqwjjiusd.html

C#:   public string Greet() => Name;
来源：http://hz.0kj1m.cn/gtjiscwvuu.html

[G05] 继承
来源：http://hz.zhengqikj.top/gtzboryuhg.html

Py:   class Admin(User): pass
来源：http://hz.fzhhl.top/gtoocndkrn.html

PHP:  class Admin extends User {}
来源：http://hz.hnxiangtu.top/gtwvuhpgkc.html

JS:   class Admin extends User {}
来源：http://hz.hammf.cn/gtrxgbrfes.html

TS:   class Admin extends User {}
来源：http://hz.yonumen.top/gttajcixio.html

Java: class Admin extends User {}
来源：http://hz.daxiang520.top/gtruswosxc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.birdmap.top/gtvqpvpnrd.html

Ruby: class Admin < User; end
来源：http://hz.xuetiantiany.cn/gtgciaizom.html

C#:   class Admin : User {}
来源：http://hz.meibo888.top/gtrfxvrmxm.html

[G06] 重写方法
来源：http://hz.shanyushiyangtech.top/gtuyonrbin.html

Py:   def greet(self): return "admin"
来源：http://hz.jqgufenzy.top/gtnibwblyp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.shanyushiyangkeji.top/gtlfdouqez.html

JS:   greet() { return "admin"; }
来源：http://hz.sysykeji.top/gtodlqbano.html

TS:   greet(): string { return "admin"; }
来源：http://hz.havefunace.top/gtgmuqdzfe.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.ybcxt.top/gtppncolpa.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.snrcjt.cn/gtnakcfmzc.html

Ruby: def greet; "admin"; end
来源：http://hz.tian-w.cn/gtzopxkoqk.html

C#:   public override string Greet() => "admin";
来源：http://hz.mhx1999.top/gtsddvjmpx.html

[G07] 调用父类方法
来源：http://hz.zhiwuduotai.top/gtieeqfweb.html

Py:   super().greet()
来源：http://hz.jiagoushi.top/gtadcawidt.html

PHP:  parent::greet();
来源：http://hz.hnxiangtu.top/gtqcuiwxkq.html

JS:   super.greet();
来源：http://hz.0kj1m.cn/gtjqssbish.html

TS:   super.greet();
来源：http://hz.tian-w.cn/gtcznxylwe.html

Java: super.greet();
来源：http://hz.xuetiantiany.cn/gtbiylxizx.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.gaohongyu789.top/gtycjxiqnq.html

Ruby: super
来源：http://hz.zhengqikj.top/gtcvaaaurj.html

C#:   base.Greet();
来源：http://hz.shanyushiyangtech.top/gtuajcwhvl.html

[G08] 静态方法与属性
来源：http://hz.dashuyun.cn/gtvtwwumwh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jyoumei.cn/gtvjbjmgor.html

PHP:  public static function f() {}
来源：http://hz.jinyuanbaomall.cn/gthnxzeyjg.html

JS:   static f() {}
来源：http://hz.tian-w.cn/gtasjnnfvy.html

TS:   static f(): void {}
来源：http://hz.jiagoushi.top/gtyszliufg.html

Java: static void f() {}
来源：http://hz.nanxuanxn.top/gtshpcorex.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.zhongyouzk.top/gtndstztqx.html

Ruby: def self.f; end
来源：http://hz.cqqwz.cn/gtwajpiqpc.html

C#:   public static void F() {}
来源：http://hz.shanyushiyangtech.top/gtrjhynqzk.html

[G09] 接口 / 抽象类
来源：http://hz.bjfxy.top/gtatqmklhi.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.hnxiangtu.top/gtpuagkbde.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.feifeiyinyue.top/gtmujkgrsp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.jiagoushi.top/gthetixwjt.html

TS:   interface Shape { area(): number; }
来源：http://hz.aizwys.cn/gtofknsmxv.html


<!-- 参考信息 -->