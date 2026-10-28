代发 wailian999

JS:   [...s].reverse().join("")
来源：http://hz.ydjk.org.cn/gtsbycypgm.html

TS:   [...s].reverse().join("")
来源：http://hz.jianghu66.top/gtwssfsmey.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.nanxinkj.top/gtamizrtnn.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.wangdashe.top/gtxcsdqveu.html

Ruby: s.reverse
来源：http://hz.xingfuxueyuan.xyz/gtmrdxgexr.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.yueranfly.top/gtxumkbuqk.html

[E12] 统计某字符出现次数
来源：http://hz.zhongyouzk.top/gtcignxmhh.html

Py:   s.count("a")
来源：http://hz.sufxvd.cn/gttikrklfu.html

PHP:  substr_count($s, "a");
来源：http://hz.hnqzz.top/gtrgfedfuu.html

JS:   s.split("a").length - 1
来源：http://hz.jiagoushi.top/gthxpostba.html

TS:   s.split("a").length - 1
来源：http://hz.wangshuangyany.cn/gtsbvkevjo.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.jiagoushi.top/gtqfspbgws.html

Go:   strings.Count(s, "a")
来源：http://hz.redwolf501.top/gtkfqjrnlj.html

Ruby: s.count("a")
来源：http://hz.hnqzz.top/gtpoqdqczc.html

C#:   s.Count(c => c == 'a')
来源：http://hz.jinqigufen.top/gtomhbejme.html

[E13] 逐字符遍历
来源：http://hz.xziqi.cn/gtrhnmmape.html

Py:   for ch in s: print(ch)
来源：http://hz.smart0.xyz/gtqcoqqsuc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.jinghuilouyu.cn/gtjgnycafx.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yj20258888.top/gtrijbgxad.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.tian-w.cn/gtuhnlsqau.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.hammf.cn/gtlkrpvufu.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.xuanzx.com/gtugocosgj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.yueranfly.top/gtdwrnfogr.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.sxryk.cn/gtdzloqrwx.html

[E14] URL 编码与 Base64
来源：http://hz.xuetiantiany.cn/gtxkbyvfib.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.yongpay.top/gtungdxcyy.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.tianlin.xyz/gtyijbufsd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.svipenyu.cn/gtzleantzr.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.dianchejie.cn/gtbegfldah.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.chenjidiqi.icu/gtsaeheaoc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.havefunace.top/gtnovxafjp.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.cheryme.top/gtmgecbzuk.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.jqgfzy.top/gtvuwrtzhv.html

[E15] HTML 转义 / 反转义
来源：http://hz.zhixingplan.top/gtknoauqem.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.hammf.cn/gthgdjoqkn.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.yvedp.cn/gtztjaynmi.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.ywan-chungtsiang.top/gtzbudahkv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.yj20258888.top/gtjklmcqtg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.jlsjyb.cn/gtcsxgqmuk.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.guannengcc.top/gtfjvyhkst.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.ydzc1.top/gtugbvqniv.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.yueranfly.top/gtipjvctzy.html

[E16] 数字千分位
来源：http://hz.ivvv.top/gtnvgtidrt.html

Py:   f"{1234567:,}"
来源：http://hz.kuanghao11.cn/gtrdoowjjv.html

PHP:  number_format(1234567);
来源：http://hz.sufxvd.cn/gtvkvcynpd.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.shanyushiyangtech.top/gtekmfprhr.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.shanyushiyangkeji.top/gtbcsjfeuk.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.fzhhl.top/gtviwmnhve.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.c1oappe.top/gtctlzlohc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.jyoumei.cn/gtkrlqwdrq.html

C#:   1234567.ToString("N0")
来源：http://hz.yj202588.top/gtojrqueso.html

[E17] 首字母大写
来源：http://hz.zhijiandao.cn/gtlovnwxyc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.feifeiyinyue.top/gtcvuufflo.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.hnxiangtu.top/gtftfvduvk.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.mhx1999.top/gtgaliihtd.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.guannengcc.top/gtnczoppli.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.52xcode.cn/gtjhslugjl.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.yj20258888.top/gtlewivhwj.html

Ruby: s.capitalize
来源：http://hz.havefunace.top/gtdesqvlre.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.nanxinkj.top/gtjlyjibhz.html

[E18] 模板占位符替换
来源：http://hz.vqdsnc.cn/gtgbbytctk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.sweek.top/gtkcvlacji.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.mhx1999.top/gtdmjddtvu.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.hnxiangtu.top/gtpmhrslxo.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.ppjwa.cn/gtpmsfgyvf.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.cashguo.top/gtdyjxmiym.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.jqgfzy.top/gtyjxadwqr.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.yj20258.top/gtmzfgveiw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.sysykeji.top/gtxyzpmedp.html

[E19] 多行文本按行拆分
来源：http://hz.gzhubu.top/gtkpujmjrs.html

Py:   s.splitlines()
来源：http://hz.xinyue.icu/gtswvcyelh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.hongshengwenyu.top/gtxmspmmxw.html

JS:   s.split(/\r?\n/)
来源：http://hz.ybcxt.top/gtbweqhxyy.html

TS:   s.split(/\r?\n/)
来源：http://hz.haohaochexian.top/gtycdfxrqf.html

Java: s.lines().toList()
来源：http://hz.yonumen.top/gtybmagrxg.html

Go:   strings.Split(s, "\n")
来源：http://hz.vqdsnc.cn/gtjmkbpcpj.html

Ruby: s.lines
来源：http://hz.aibaodan.cn/gtlacrnuwf.html

C#:   s.Split('\n')
来源：http://hz.gogol.net.cn/gtbjwnvslt.html

[E20] 判断字符串是否为空
来源：http://hz.gotoacloud.top/gtamvovivy.html

Py:   if not s:
来源：http://hz.hywenlv.cn/gtymzkgjie.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.ydjk.org.cn/gtmfexeaoh.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.jqgfzy.top/gtmtwokazw.html

TS:   if (s === "") {}
来源：http://hz.wangshuangyany.cn/gtmcptluvf.html

Java: if (s.isEmpty()) {}
来源：http://hz.sxryk.cn/gthjhvjihi.html

Go:   if s == "" {}
来源：http://hz.ydzc1.top/gtwkxzjpwu.html

Ruby: if s.empty?
来源：http://hz.pycfn.com/gtrhztlhlt.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.daxiang520.top/gtpagqhrxt.html

[E21] 超长截断加省略号
来源：http://hz.mhx1999.top/gtttuabejz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.cucudq.cn/gtaupojexz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.yj20258.top/gtmeglszhe.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.hywenlv.cn/gtnxhnfhre.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.xylfe.cn/gtpeeyicnv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.snrcjt.cn/gtvincjdjq.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.jqgfzy.top/gtktrznwjc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.hnqzz.top/gtpllgygck.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.52xcode.cn/gtnblqhlro.html

[E22] 字节长度与字符长度
来源：http://hz.hongshengwenyu.top/gthiyoaocj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.316326.xyz/gtcxuinfph.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.cqqwz.cn/gtgcgbruvy.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.meibo888.top/gtvnlmkcmt.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.tanke756.top/gtibrawgij.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.quarkkingdee.top/gtmrqshgph.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.haohaochexian.top/gtnmgsfoiq.html

Ruby: s.bytesize;  s.length
来源：http://hz.snrcjt.cn/gtkldgkdgj.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.jyoumei.cn/gtsppucsvl.html

================================================================================
来源：http://hz.cashguo.top/gtuemloznw.html

F. 文件与目录
来源：http://hz.yj202588.top/gtovyrktvs.html

================================================================================
来源：http://hz.svipenyu.cn/gtirxqjxkd.html

[F01] 读取整个文件
来源：http://hz.zycfv.cn/gtilbnbegu.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.cucudq.cn/gtxjtrgtck.html

PHP:  file_get_contents("a.txt");
来源：http://hz.chenzaomai.com/gtedifuaib.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.daria6918.cn/gtxciypdoc.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.ydzc1.top/gtohmxeyld.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.yj20258.top/gtjjbschud.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.hongshengwenyu.top/gtcctmludo.html

Ruby: File.read("a.txt")
来源：http://hz.c1oappe.top/gtekeddcfj.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.cqqwz.cn/gtufhmurnv.html

[F02] 逐行读取文件
来源：http://hz.zdqjudy.top/gtdqzdvvxh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.vqdsnc.cn/gtdophberg.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.yangfankeji.com/gtbdrasrff.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jqgfzy.top/gtiigrsyhr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xuetiantiany.cn/gtzrfpbpvs.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.316326.xyz/gtedxejkum.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.ydjk.org.cn/gtpntmlscp.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.birdmap.top/gtedmldwag.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.yj202588.top/gtjthvanzm.html

[F03] 写入文件（覆盖）
来源：http://hz.kuanghao11.cn/gtgjtcqntj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.yanxiufei.cn/gtoddqskzs.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.hnqzz.top/gtcxymsyta.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.sxryk.cn/gtqzeuohew.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.sysykeji.top/gtkliniwjl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.ydjk.org.cn/gtwlavuujv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.hongshengwenyu.top/gtyywqqpmu.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.fengsongda.top/gtknpjznvz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.xuanzx.com/gtftszwrwj.html

[F04] 追加写入文件
来源：http://hz.jinghuilouyu.cn/gtqquitfix.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.316326.xyz/gtffqoqyoz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.zycfv.cn/gtzucxoeus.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yongpay.top/gttlqbvwvi.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.hnqzz.top/gtyuxeczzf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.chenlongwang.top/gtbuflwklt.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.hfpthk.cn/gtqnzfhdjw.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yongpay.top/gtgnkwuowf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.cqqwz.cn/gtcpsmbyuy.html

[F05] 判断文件或目录是否存在
来源：http://hz.hywenlv.cn/gtdmrsuvom.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.cheryme.top/gtpxbmnhrn.html

PHP:  file_exists("a.txt");
来源：http://hz.shuidangran.top/gtavczlnyn.html

JS:   fs.existsSync("a.txt")
来源：http://hz.jlsjyb.cn/gtdtmewhfy.html

TS:   fs.existsSync("a.txt")
来源：http://hz.tian-w.cn/gtuerkvraj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.jinqigufen.top/gtubwzjysp.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.shuidangran.top/gtrkjbfeut.html

Ruby: File.exist?("a.txt")
来源：http://hz.shanyushiyangkeji.top/gtepqjhvii.html

C#:   File.Exists("a.txt")
来源：http://hz.cqqwz.cn/gtgkltddlo.html

[F06] 删除文件
来源：http://hz.0kj1m.cn/gtojevahgs.html

Py:   os.remove("a.txt")
来源：http://hz.yangfankeji.com/gtubvsgxga.html

PHP:  unlink("a.txt");
来源：http://hz.daxiang520.top/gtapxqufau.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.shanyushiyangkeji.top/gtupvzhcia.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.yanxiufei.cn/gtmwcjlfqv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.jinqigfzy.top/gtbhfdkixq.html

Go:   os.Remove("a.txt")
来源：http://hz.hammf.cn/gthkybfbto.html

Ruby: File.delete("a.txt")
来源：http://hz.zhongyouzk.top/gtkukksodd.html

C#:   File.Delete("a.txt");
来源：http://hz.gotoacloud.top/gtvxxetbap.html

[F07] 创建目录（含多级）
来源：http://hz.jinyuanbaomall.cn/gtusturvzn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.hywenlv.cn/gtaqmyzayc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.zhixingplan.top/gtyvfvuknm.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhijiandao.cn/gtphkzrdfe.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jyoumei.cn/gtgxuejqqb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.hfpthk.cn/gtarmlvkkb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.yongpay.top/gtifhhluhi.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.havefunace.top/gthismafcu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.andypj.xyz/gtwwlgiwln.html

[F08] 遍历目录
来源：http://hz.shanyushiyangkeji.top/gtybwwwayk.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.9152youxi.cn/gtsqmyrhjp.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.jyoumei.cn/gtqjrwhsqw.html

JS:   fs.readdirSync("dir")
来源：http://hz.svipenyu.cn/gtaoeupghk.html

TS:   fs.readdirSync("dir")
来源：http://hz.guowangkeji.top/gtzylgwjiw.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.yj20258.top/gtjgopwimk.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.daria6918.cn/gtwrmaysad.html

Ruby: Dir.children("dir")
来源：http://hz.cucudq.cn/gtisxvqxih.html

C#:   Directory.GetFiles("dir")
来源：http://hz.xylfe.cn/gtiimxlkkv.html

[F09] 获取文件大小
来源：http://hz.hnqzz.top/gtptemtswz.html

Py:   os.path.getsize("a.txt")
来源：http://hz.cheryme.top/gtpyeqiguq.html

PHP:  filesize("a.txt");
来源：http://hz.guowangkeji.top/gthffvzikq.html

JS:   fs.statSync("a.txt").size
来源：http://hz.zhijiandao.cn/gtvttfpdhm.html

TS:   fs.statSync("a.txt").size
来源：http://hz.nanxuanxn.top/gtohrucezg.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.ppjwa.cn/gtrjmmohqa.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.jianghu66.top/gtvqtvtlwx.html

Ruby: File.size("a.txt")
来源：http://hz.zhiwuduotai.top/gtsoskjmmj.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.xuanzx.com/gtatgnrgqi.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.hfpthk.cn/gtshfwwkpu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.fengsongda.top/gtyfvxjsqj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.cucudq.cn/gtsqisgeut.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.jianghu66.top/gtunrgosqh.html

TS:   path.extname("a.txt")
来源：http://hz.jinqigfzy.top/gtmicusabv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.yongpay.top/gtmwvnocbz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.nanxinkj.top/gtiqludutc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.tian-w.cn/gtwkiuozdr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.shanyushiyangkeji.top/gtvgbyojgo.html

[F11] 复制与移动文件
来源：http://hz.tianlin.xyz/gtvlblliit.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.cdnleiting.top/gtitfskzqh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.zhongyouzk.top/gtwewhnpvx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhiwuduotai.top/gtolsleuxb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.sysykeji.top/gtstprcmju.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.jyoumei.cn/gtoyzmkamb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.tianlin.xyz/gtqbfljkzw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.daria6918.cn/gtinyuxpyh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.yongpay.top/gtrmcplbbr.html

[F12] CSV 读写
来源：http://hz.jinqigufen.top/gttldauxrd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.chenzaomai.com/gtrykafqlm.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.yongpay.top/gtmfyeinpd.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.sufxvd.cn/gtofcoaask.html

TS:   // 同上
来源：http://hz.jyoumei.cn/gtawejxgbc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.fzhhl.top/gtasxefuyl.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.fzhhl.top/gtzioyscpd.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.xziqi.cn/gtdnmvgbvd.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.ppjwa.cn/gtrrmogixw.html

================================================================================
来源：http://hz.hfpthk.cn/gtpisvxdpw.html

G. 面向对象
来源：http://hz.ydzc1.top/gtrcxshkyr.html

================================================================================
来源：http://hz.cheryme.top/gtrdtuitti.html

[G01] 定义类
来源：http://hz.cashguo.top/gtagcooxmh.html

Py:   class User: pass
来源：http://hz.shangyingyoupin.top/gtvpsilqxq.html

PHP:  class User {}
来源：http://hz.yongpay.top/gtsezowhtx.html

JS:   class User {}
来源：http://hz.iojbl.cn/gtmusoffrr.html

TS:   class User { name: string = ""; }
来源：http://hz.gzhubu.top/gtkpfxnqkf.html

Java: class User {}
来源：http://hz.316326.xyz/gthiisievy.html

Go:   type User struct { Name string }
来源：http://hz.zhaomingkeji.xyz/gtwwcenbyw.html

Ruby: class User; end
来源：http://hz.hongshengwenyu.top/gtmrvopitm.html

C#:   class User {}
来源：http://hz.cqqwz.cn/gtowsnlvnn.html

[G02] 构造函数
来源：http://hz.jinqigfzy.top/gtfjjiqwwa.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.jyoumei.cn/gtqwgaddvc.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.shzxlz.cn/gtuybqvjlf.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.hfpthk.cn/gtnbhqkgzc.html

TS:   constructor(public name: string) {}
来源：http://hz.cqqwz.cn/gtlobjibdx.html

Java: User(String name) { this.name = name; }
来源：http://hz.jinqigufen.top/gtzpfibhzo.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.feifeiyinyue.top/gtdrxjobag.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.svipenyu.cn/gtuohkqxjf.html

C#:   public User(string name) { Name = name; }
来源：http://hz.cashguo.top/gtjaopslnq.html

[G03] 实例属性
来源：http://hz.quarkkingdee.top/gtbzxrngza.html

Py:   self.name = "x"
来源：http://hz.sysykeji.top/gtgduoupbd.html

PHP:  public string $name = "x";
来源：http://hz.c1oappe.top/gtlctxwngr.html

JS:   this.name = "x";
来源：http://hz.zhijiandao.cn/gtjczkgohu.html

TS:   name: string = "x";
来源：http://hz.andypj.xyz/gtxeusncsb.html

Java: private String name;
来源：http://hz.yanxiufei.cn/gtklaysfde.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.shuidangran.top/gtyajlptlm.html

Ruby: @name = "x"
来源：http://hz.hammf.cn/gtdheqkmdh.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.zhiwuduotai.top/gtkdgmwbpd.html

[G04] 定义方法
来源：http://hz.yangfankeji.com/gtwaodekzr.html

Py:   def greet(self): return self.name
来源：http://hz.yanxiufei.cn/gtjtwwprsz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.andypj.xyz/gtiujgzzkr.html

JS:   greet() { return this.name; }
来源：http://hz.ywan-chungtsiang.top/gttxkugpix.html

TS:   greet(): string { return this.name; }
来源：http://hz.jqgfzy.top/gtwktowuwb.html

Java: String greet() { return name; }
来源：http://hz.zhaomingkeji.xyz/gtbmflqokv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.dianchejie.cn/gtbdbykitp.html

Ruby: def greet; @name; end
来源：http://hz.hnxiangtu.top/gtoaxxjajo.html

C#:   public string Greet() => Name;
来源：http://hz.yueranfly.top/gtqyenvgfw.html

[G05] 继承
来源：http://hz.shuidangran.top/gtufmbrfld.html

Py:   class Admin(User): pass
来源：http://hz.hammf.cn/gtvroutzsh.html

PHP:  class Admin extends User {}
来源：http://hz.wangshuangyany.cn/gtnnslqqec.html

JS:   class Admin extends User {}
来源：http://hz.pycfn.com/gtvszhhvmj.html

TS:   class Admin extends User {}
来源：http://hz.guowangkeji.top/gtwrohpoch.html

Java: class Admin extends User {}
来源：http://hz.hammf.cn/gtalesrsod.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.ydzc1.top/gtuhqxincl.html

Ruby: class Admin < User; end
来源：http://hz.feifeiyinyue.top/gtgsptnyhc.html

C#:   class Admin : User {}
来源：http://hz.cashguo.top/gtllxlqblo.html

[G06] 重写方法
来源：http://hz.guowangkeji.top/gttoolhyuo.html

Py:   def greet(self): return "admin"
来源：http://hz.hnxiangtu.top/gteekqfexh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.sufxvd.cn/gtxexgeokz.html

JS:   greet() { return "admin"; }
来源：http://hz.xingfuxueyuan.xyz/gtvowrxivo.html

TS:   greet(): string { return "admin"; }
来源：http://hz.hysaishi.cn/gtxaxkrypz.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jqgfzy.top/gtmuyvjrfi.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.vqdsnc.cn/gtxbgypmje.html

Ruby: def greet; "admin"; end
来源：http://hz.tian-w.cn/gtdlnesyje.html

C#:   public override string Greet() => "admin";
来源：http://hz.yonumen.top/gtannjkbxm.html

[G07] 调用父类方法
来源：http://hz.zhijiandao.cn/gtcxcibaav.html

Py:   super().greet()
来源：http://hz.cashguo.top/gtadoliyao.html

PHP:  parent::greet();
来源：http://hz.sysykeji.top/gtfwjnlzda.html

JS:   super.greet();
来源：http://hz.ivvv.top/gthjkfibkw.html

TS:   super.greet();
来源：http://hz.cdnleiting.top/gthymezsym.html

Java: super.greet();
来源：http://hz.zdqjudy.top/gtmpvurxtq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.zhoulong.xyz/gtwfycntja.html

Ruby: super
来源：http://hz.xuetiantiany.cn/gthwgledlu.html

C#:   base.Greet();
来源：http://hz.shanyushiyangkeji.top/gtxkaosdqo.html

[G08] 静态方法与属性
来源：http://hz.jianghu66.top/gtnbvoaedj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.nanxinkj.top/gtsbhpkssn.html

PHP:  public static function f() {}
来源：http://hz.xylfe.cn/gteanhydea.html

JS:   static f() {}
来源：http://hz.jinghuilouyu.cn/gtmbvniktp.html

TS:   static f(): void {}
来源：http://hz.xuetiantiany.cn/gtyjuopcrm.html

Java: static void f() {}
来源：http://hz.guannengcc.top/gthamsihzz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.meibo888.top/gtfdmfelru.html

Ruby: def self.f; end
来源：http://hz.iojbl.cn/gtccovfozt.html

C#:   public static void F() {}
来源：http://hz.daria6918.cn/gtocjivcdk.html

[G09] 接口 / 抽象类
来源：http://hz.ppjwa.cn/gtrglbmean.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.xziqi.cn/gtxjeezuji.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.guannengcc.top/gtumqgfall.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.fengsongda.top/gtqohxcujt.html

TS:   interface Shape { area(): number; }
来源：http://hz.dianchejie.cn/gttaqmwcua.html

Java: interface Shape { double area(); }
来源：http://hz.jqgufenzy.top/gtzqwhjroq.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.sweek.top/gtesqybbuy.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.gotoacloud.top/gtwrnzkgqc.html

C#:   interface IShape { double Area(); }
来源：http://hz.mhx1999.top/gtfmxtvjyz.html


<!-- 参考信息 -->