代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.chenlongwang.top/gtmkyauknt.html

[E11] 反转字符串
来源：http://hz.haohaochexian.top/gtmsgzwdru.html

Py:   s[::-1]
来源：http://hz.gaohongyu789.top/gtzfooqukf.html

PHP:  strrev($s);
来源：http://hz.ivvv.top/gtmzjvyshu.html

JS:   [...s].reverse().join("")
来源：http://hz.sxryk.cn/gtozmompwi.html

TS:   [...s].reverse().join("")
来源：http://hz.yj20258888.top/gtlfqwctug.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.yonumen.top/gtybvdvgjw.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.chenjidiqi.icu/gtbhyhrmgy.html

Ruby: s.reverse
来源：http://hz.c1oappe.top/gthcnlykmd.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.dianchejie.cn/gtiayuhngf.html

[E12] 统计某字符出现次数
来源：http://hz.yangfankeji.com/gtjewjyrlf.html

Py:   s.count("a")
来源：http://hz.gzhubu.top/gtqxtosvcn.html

PHP:  substr_count($s, "a");
来源：http://hz.jianghu66.top/gtnjjhdncg.html

JS:   s.split("a").length - 1
来源：http://hz.chenjidiqi.icu/gtghyxcjwi.html

TS:   s.split("a").length - 1
来源：http://hz.smart0.xyz/gtojppeimu.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.sysykeji.top/gtwdkgmwbg.html

Go:   strings.Count(s, "a")
来源：http://hz.sysykeji.top/gtkgcvrbon.html

Ruby: s.count("a")
来源：http://hz.sweek.top/gtbufigokx.html

C#:   s.Count(c => c == 'a')
来源：http://hz.fzhhl.top/gtzwsxsyxa.html

[E13] 逐字符遍历
来源：http://hz.kuanghao11.cn/gtoswheyxx.html

Py:   for ch in s: print(ch)
来源：http://hz.jinqigfzy.top/gtsybjhjvs.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.jqgfzy.top/gtxnyoyprm.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.cqqwz.cn/gtgwyuxmze.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.nwbrower.top/gtqxldkepa.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.yangfankeji.com/gtzxglpqmn.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.ybcxt.top/gtuzffbigp.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.jlsjyb.cn/gtagasrfkn.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.yj202588.top/gtphwldtnn.html

[E14] URL 编码与 Base64
来源：http://hz.yangfankeji.com/gttjmppcel.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.feifeiyinyue.top/gtdmpeeitv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.fzhhl.top/gtuydcsxdt.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.wangdashe.top/gtrjmojkil.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.aibaodan.cn/gtroqwpkup.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.zhaomingkeji.xyz/gtdredrdeh.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.ivvv.top/gtdrlsmboe.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.yj20258888.top/gtxqtserwn.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.jiagoushi.top/gthfgczmye.html

[E15] HTML 转义 / 反转义
来源：http://hz.shangyingyoupin.top/gtkpeioncj.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.sufxvd.cn/gtrdiitheq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.shzxlz.cn/gtzlvxbqza.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.9152youxi.cn/gthotiuxrp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.hnqzz.top/gtebllzguq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.yuxming.cn/gtoifdbpwn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.daxiang520.top/gtxzyqoaum.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.hnxiangtu.top/gtsqvrjmug.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.xinyue.icu/gtltmabvlm.html

[E16] 数字千分位
来源：http://hz.havefunace.top/gtyhmwzhvn.html

Py:   f"{1234567:,}"
来源：http://hz.aizwys.cn/gtexokzbsv.html

PHP:  number_format(1234567);
来源：http://hz.ehwqpu.com/gtydeljgsk.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.yj20258888.top/gtulkwsmee.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.hnqzz.top/gtzgsceobh.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.chenzaomai.com/gtpbfetmkb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.yj202588.top/gtiwyudyvu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.tanke756.top/gtfrywfyho.html

C#:   1234567.ToString("N0")
来源：http://hz.dianchejie.cn/gteksvefgd.html

[E17] 首字母大写
来源：http://hz.guowangkeji.top/gtzmhfnhfz.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.hongshengwenyu.top/gtujawtika.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.kuanghao11.cn/gtibsxnxan.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yj202588.top/gtjcyavvja.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.sxryk.cn/gtoktinbxy.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.xziqi.cn/gtebrhzoql.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.xingfuxueyuan.xyz/gtzzjgnmgq.html

Ruby: s.capitalize
来源：http://hz.wangdashe.top/gtkxdftmcn.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.hammf.cn/gtbvrkrwna.html

[E18] 模板占位符替换
来源：http://hz.yj202588.top/gttitxnwpy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.yonumen.top/gtqnpvtope.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.hnxiangtu.top/gtugmkkfsz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.yvedp.cn/gtkimcmekn.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.xuetiantiany.cn/gtlvxckcfx.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.fzhhl.top/gtjexdduzb.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.shuidangran.top/gtprpndrtj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.bjfxy.top/gtzadchhvs.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.hywenlv.cn/gtqdzvyqma.html

[E19] 多行文本按行拆分
来源：http://hz.daria6918.cn/gtnjzknnwo.html

Py:   s.splitlines()
来源：http://hz.dashuyun.cn/gtwkspgfap.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.yj20258888.top/gtxtbwicuj.html

JS:   s.split(/\r?\n/)
来源：http://hz.haohaochexian.top/gttewkipnv.html

TS:   s.split(/\r?\n/)
来源：http://hz.yvedp.cn/gtoyrbnyqa.html

Java: s.lines().toList()
来源：http://hz.wangshuangyany.cn/gtwibmixbz.html

Go:   strings.Split(s, "\n")
来源：http://hz.iojbl.cn/gtzqemzmto.html

Ruby: s.lines
来源：http://hz.aibaodan.cn/gtruvfjfuw.html

C#:   s.Split('\n')
来源：http://hz.cqqwz.cn/gtwmmapmwn.html

[E20] 判断字符串是否为空
来源：http://hz.sxryk.cn/gtmlxgmivc.html

Py:   if not s:
来源：http://hz.yj202588.top/gtqdkzpsqz.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.meibo888.top/gtfpqeebel.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.wangshuangyany.cn/gtbqfwlqvr.html

TS:   if (s === "") {}
来源：http://hz.ybcxt.top/gtcahnipzl.html

Java: if (s.isEmpty()) {}
来源：http://hz.sweek.top/gtxeijnzks.html

Go:   if s == "" {}
来源：http://hz.jinghuilouyu.cn/gtuycmfrlg.html

Ruby: if s.empty?
来源：http://hz.pycfn.com/gthnqygfnc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.aibaodan.cn/gtlpxlesbw.html

[E21] 超长截断加省略号
来源：http://hz.chenzaomai.com/gtpmygaund.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.ppjwa.cn/gtnyfehwdg.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.wangdashe.top/gtetjpjyeh.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jinqigfzy.top/gteajuesjw.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.cucudq.cn/gtystbrigm.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yj202588.top/gtilpzpbvf.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.tianlin.xyz/gteolxvtpp.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.chenjidiqi.icu/gtcbabmwgn.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.xziqi.cn/gtmmmxhwgd.html

[E22] 字节长度与字符长度
来源：http://hz.hongshengwenyu.top/gtqsrbfdnv.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.andypj.xyz/gtbygshngo.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ybcxt.top/gtiiznldgi.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.kuanghao11.cn/gtyjwtkehi.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.gzhubu.top/gtgrxysybz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.gaohongyu789.top/gtcxzlzahm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.yj20258.top/gtfburmgov.html

Ruby: s.bytesize;  s.length
来源：http://hz.hnqzz.top/gtjovzbieb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.jqgufenzy.top/gtyiqtynpl.html

================================================================================
来源：http://hz.xuanzx.com/gtnsodqvwe.html

F. 文件与目录
来源：http://hz.hongshengwenyu.top/gtlrqcyscr.html

================================================================================
来源：http://hz.yvedp.cn/gtcibkqmgj.html

[F01] 读取整个文件
来源：http://hz.yuanzhike.top/gttimeiqcw.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.cashguo.top/gtjjwucsao.html

PHP:  file_get_contents("a.txt");
来源：http://hz.9152youxi.cn/gtvzrgjbab.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.zhengqikj.top/gtdoiyuikz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.jinqigufen.top/gtaqkctipc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.nwbrower.top/gtuyyewlvi.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.ydjk.org.cn/gtymletlif.html

Ruby: File.read("a.txt")
来源：http://hz.gogol.net.cn/gtgymucncz.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.ppjwa.cn/gtabhjazwj.html

[F02] 逐行读取文件
来源：http://hz.nwbrower.top/gtsnorrzvp.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.tian-w.cn/gtuhizxkyu.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.tianlin.xyz/gtsgbhzsrx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.pycfn.com/gtweqfwvck.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.shuidangran.top/gtgxnpzayi.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.zhoulong.xyz/gtlrkshnla.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.tianlin.xyz/gtpkiuszhc.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.fzhhl.top/gtsktjajlg.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.gzhubu.top/gtykyliogf.html

[F03] 写入文件（覆盖）
来源：http://hz.zhixingplan.top/gtqzbnmnng.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.yvedp.cn/gtqztcqpfm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.jqgfzy.top/gtsjtmehhq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhengqikj.top/gtwoecdssz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.xingfuxueyuan.xyz/gthzlplghd.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.hysaishi.cn/gtswngcovx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.zhengqikj.top/gtzcqamfuu.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.cheryme.top/gtagregqkn.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.redwolf501.top/gtnobydvdg.html

[F04] 追加写入文件
来源：http://hz.svipenyu.cn/gthjmbtopw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.vqdsnc.cn/gtgeuvgwoh.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.daria6918.cn/gtiaecwuxg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.andypj.xyz/gtvlukkbrl.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.aizwys.cn/gtxtqtehib.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.sweek.top/gtvfiyyhha.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.chenjidiqi.icu/gtrvrjjrqr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.svipenyu.cn/gttdxavpkz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.cucudq.cn/gtjsgvdxgq.html

[F05] 判断文件或目录是否存在
来源：http://hz.xuetiantiany.cn/gtodquyrib.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.andypj.xyz/gtjqnioxel.html

PHP:  file_exists("a.txt");
来源：http://hz.redwolf501.top/gtzgnsxacy.html

JS:   fs.existsSync("a.txt")
来源：http://hz.c1oappe.top/gtgjsyrheo.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zhoulong.xyz/gtyvcvobgn.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.hysaishi.cn/gtwfbzpepd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.iojbl.cn/gtiqcsjdob.html

Ruby: File.exist?("a.txt")
来源：http://hz.gaohongyu789.top/gtzmualkwq.html

C#:   File.Exists("a.txt")
来源：http://hz.zhaomingkeji.xyz/gtgxizzhth.html

[F06] 删除文件
来源：http://hz.chenjidiqi.icu/gtlfembhdd.html

Py:   os.remove("a.txt")
来源：http://hz.yanxiufei.cn/gtdktgosap.html

PHP:  unlink("a.txt");
来源：http://hz.dianchejie.cn/gtwolkenoq.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.tanke756.top/gtzmjqygbf.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.yvedp.cn/gtewjulvsf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.dianchejie.cn/gtqhbchijh.html

Go:   os.Remove("a.txt")
来源：http://hz.yuanzhike.top/gtujrqtevf.html

Ruby: File.delete("a.txt")
来源：http://hz.vqdsnc.cn/gttrbcccqn.html

C#:   File.Delete("a.txt");
来源：http://hz.zhengqikj.top/gthoxvhqxb.html

[F07] 创建目录（含多级）
来源：http://hz.shanyushiyangtech.top/gtpqoyfefg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.smart0.xyz/gtbwlkipxu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.redwolf501.top/gtvdupsjml.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.redwolf501.top/gtsgiywene.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.daria6918.cn/gtmzesgojf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.yj20258888.top/gtieaanhxq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.hnxiangtu.top/gtbbabnoxc.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.hnxiangtu.top/gtpbtkgxql.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.redwolf501.top/gtsgchlnbz.html

[F08] 遍历目录
来源：http://hz.ydzc1.top/gtokbqmupv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.xingfuxueyuan.xyz/gtptjemtvg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.yj20258.top/gtallfutat.html

JS:   fs.readdirSync("dir")
来源：http://hz.quarkkingdee.top/gtuebjjrwb.html

TS:   fs.readdirSync("dir")
来源：http://hz.zhaomingkeji.xyz/gtfvkzyntj.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.cheryme.top/gtslklapqr.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.jyoumei.cn/gttotwhbje.html

Ruby: Dir.children("dir")
来源：http://hz.daxiang520.top/gtwjhtsnck.html

C#:   Directory.GetFiles("dir")
来源：http://hz.jinqigufen.top/gtdczzzhae.html

[F09] 获取文件大小
来源：http://hz.nanxinkj.top/gtyrnpilcx.html

Py:   os.path.getsize("a.txt")
来源：http://hz.chenzaomai.com/gtcjuqblzi.html

PHP:  filesize("a.txt");
来源：http://hz.xylfe.cn/gtebimsicv.html

JS:   fs.statSync("a.txt").size
来源：http://hz.mhx1999.top/gthfmkcaog.html

TS:   fs.statSync("a.txt").size
来源：http://hz.redwolf501.top/gtmveclwjs.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.gzhubu.top/gtlhrsmxfz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.daxiang520.top/gtfhirvfqu.html

Ruby: File.size("a.txt")
来源：http://hz.zhongyouzk.top/gtfcdujlfs.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yvedp.cn/gtpardasyk.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.jyoumei.cn/gtjqeftpyt.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.vqdsnc.cn/gtooaebvng.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.jinqigufen.top/gtyvfziyio.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.jinqigfzy.top/gtznpjstbz.html

TS:   path.extname("a.txt")
来源：http://hz.hywenlv.cn/gtbpjmcutl.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.tanke756.top/gtwuumydux.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.hnqzz.top/gtsdaxgsav.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.zhixingplan.top/gtpmpjcyhl.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.cashguo.top/gtvskfbspb.html

[F11] 复制与移动文件
来源：http://hz.andypj.xyz/gtsadfqfyd.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.daria6918.cn/gtxumcctvc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.tanke756.top/gtsazqnkua.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhaomingkeji.xyz/gtyaemmkfl.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhongyouzk.top/gtpkpqsxyg.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.cdnleiting.top/gtxmgqzsbz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.aibaodan.cn/gtbbvdtmcm.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.hnxiangtu.top/gtbezodimd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.jiagoushi.top/gtbpdywbha.html

[F12] CSV 读写
来源：http://hz.smart0.xyz/gtrfjqjaeb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.jqgfzy.top/gtnwbxanxt.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.pengpengdd.cyou/gtxqouemdc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.dashuyun.cn/gtjwlwuufx.html

TS:   // 同上
来源：http://hz.hongshengwenyu.top/gtjbcbgnjb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.birdmap.top/gtkoikqjym.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.svipenyu.cn/gtgdncvfmc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.316326.xyz/gtwalcsppl.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.bjfxy.top/gtxtqvpzgb.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtrkegoobb.html

G. 面向对象
来源：http://hz.meibo888.top/gtabxbqcch.html

================================================================================
来源：http://hz.yj20258.top/gtiyfvviil.html

[G01] 定义类
来源：http://hz.fzhhl.top/gtzuoveypf.html

Py:   class User: pass
来源：http://hz.hnxiangtu.top/gtbzbkfczc.html

PHP:  class User {}
来源：http://hz.birdmap.top/gtgoiiasoz.html

JS:   class User {}
来源：http://hz.shangyingyoupin.top/gtdqhjfwie.html

TS:   class User { name: string = ""; }
来源：http://hz.tanke756.top/gtskalpjgw.html

Java: class User {}
来源：http://hz.wangshuangyany.cn/gtzoszkoxs.html

Go:   type User struct { Name string }
来源：http://hz.fengsongda.top/gteybkgatg.html

Ruby: class User; end
来源：http://hz.svipenyu.cn/gtocayxhyy.html

C#:   class User {}
来源：http://hz.hfpthk.cn/gtjxbnamlw.html

[G02] 构造函数
来源：http://hz.ehwqpu.com/gtmikfwosz.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.daria6918.cn/gtwgqstrna.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.sxryk.cn/gtxigapcvy.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.gaohongyu789.top/gtfcahykmw.html

TS:   constructor(public name: string) {}
来源：http://hz.jqgufenzy.top/gtmuxhdlvt.html

Java: User(String name) { this.name = name; }
来源：http://hz.sysykeji.top/gtjdgvptgb.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.sweek.top/gtwujdocac.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.ydzc1.top/gtfjflrgks.html

C#:   public User(string name) { Name = name; }
来源：http://hz.dianchejie.cn/gtcdxzaqol.html

[G03] 实例属性
来源：http://hz.0kj1m.cn/gtqvhwyyod.html

Py:   self.name = "x"
来源：http://hz.dashuyun.cn/gtbkttiwvi.html

PHP:  public string $name = "x";
来源：http://hz.shanyushiyangtech.top/gtrxugrnty.html

JS:   this.name = "x";
来源：http://hz.pengpengdd.cyou/gtapspojfa.html

TS:   name: string = "x";
来源：http://hz.quarkkingdee.top/gtwoeueyyt.html

Java: private String name;
来源：http://hz.shuidangran.top/gtyljrnzxl.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.cashguo.top/gtvwsxhzca.html

Ruby: @name = "x"
来源：http://hz.shangyingyoupin.top/gtsbepidkn.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.meibo888.top/gtqehpifbd.html

[G04] 定义方法
来源：http://hz.aibaodan.cn/gttrnwkokr.html

Py:   def greet(self): return self.name
来源：http://hz.nwbrower.top/gtrpsgokyo.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.shanyushiyangkeji.top/gtfdxhskxn.html

JS:   greet() { return this.name; }
来源：http://hz.shangyingyoupin.top/gtiwdwuyip.html

TS:   greet(): string { return this.name; }
来源：http://hz.52xcode.cn/gtkaffizdy.html

Java: String greet() { return name; }
来源：http://hz.yongpay.top/gtaiqgtdbi.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.pengpengdd.cyou/gtutaccugp.html

Ruby: def greet; @name; end
来源：http://hz.meibo888.top/gtytddyqvi.html

C#:   public string Greet() => Name;
来源：http://hz.gotoacloud.top/gtotvisovg.html

[G05] 继承
来源：http://hz.andypj.xyz/gtxhavrzkg.html

Py:   class Admin(User): pass
来源：http://hz.sysykeji.top/gtpxevysch.html

PHP:  class Admin extends User {}
来源：http://hz.sxryk.cn/gthrunuzrx.html

JS:   class Admin extends User {}
来源：http://hz.nwbrower.top/gtmnduqvtg.html

TS:   class Admin extends User {}
来源：http://hz.316326.xyz/gtqftxjhqc.html

Java: class Admin extends User {}
来源：http://hz.ehwqpu.com/gtbdovrzqr.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.nwbrower.top/gtisgshpuv.html

Ruby: class Admin < User; end
来源：http://hz.yvedp.cn/gtkhybapcy.html

C#:   class Admin : User {}
来源：http://hz.pycfn.com/gtcudinpod.html

[G06] 重写方法
来源：http://hz.tanke756.top/gtdtviqojn.html

Py:   def greet(self): return "admin"
来源：http://hz.bjfxy.top/gtmdrtsrls.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.iojbl.cn/gtqmvpdclm.html

JS:   greet() { return "admin"; }
来源：http://hz.smart0.xyz/gtigrlmxir.html

TS:   greet(): string { return "admin"; }
来源：http://hz.yuanzhike.top/gtvwjcuigh.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.ywan-chungtsiang.top/gtqdapnndh.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.yvedp.cn/gtetshswie.html

Ruby: def greet; "admin"; end
来源：http://hz.zycfv.cn/gtkrytahqj.html

C#:   public override string Greet() => "admin";
来源：http://hz.0kj1m.cn/gtvoduxpxv.html

[G07] 调用父类方法
来源：http://hz.chenzaomai.com/gthrerdszn.html

Py:   super().greet()
来源：http://hz.shzxlz.cn/gtgmvpzjdj.html

PHP:  parent::greet();
来源：http://hz.tianlin.xyz/gtetcpyrnt.html

JS:   super.greet();
来源：http://hz.ydzc1.top/gtqurdbybt.html

TS:   super.greet();
来源：http://hz.hfpthk.cn/gtuwzackqc.html

Java: super.greet();
来源：http://hz.shanyushiyangtech.top/gtbtktdbzn.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.smart0.xyz/gtusybkrst.html

Ruby: super
来源：http://hz.shanyushiyangtech.top/gthqiluznt.html

C#:   base.Greet();
来源：http://hz.ywan-chungtsiang.top/gtvkqprtim.html

[G08] 静态方法与属性
来源：http://hz.shuidangran.top/gthhkzmydk.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.cdnleiting.top/gtaivopkis.html

PHP:  public static function f() {}
来源：http://hz.ywan-chungtsiang.top/gtwbstaqkl.html

JS:   static f() {}
来源：http://hz.yangfankeji.com/gtotbjwgtz.html

TS:   static f(): void {}
来源：http://hz.meibo888.top/gtfqoponmn.html

Java: static void f() {}
来源：http://hz.yj20258888.top/gtvkugrryj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yueranfly.top/gtedtrvjwx.html

Ruby: def self.f; end
来源：http://hz.sxryk.cn/gtzoqgjuwt.html

C#:   public static void F() {}
来源：http://hz.yanxiufei.cn/gtlzzzfyei.html

[G09] 接口 / 抽象类
来源：http://hz.aizwys.cn/gtwpbzeqlu.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.xziqi.cn/gtwmdjvzek.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.svipenyu.cn/gtbhvyjhkk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.dianchejie.cn/gtxunujktn.html

TS:   interface Shape { area(): number; }
来源：http://hz.xylfe.cn/gtavrexxgp.html


<!-- 参考信息 -->