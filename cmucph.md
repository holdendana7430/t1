代发 wailian999

Go:   strings.Count(s, "a")
来源：http://hz.shuidangran.top/gtsakxyztb.html

Ruby: s.count("a")
来源：http://hz.chenlongwang.top/gtujrybqzi.html

C#:   s.Count(c => c == 'a')
来源：http://hz.yj20258888.top/gtrwjtncnj.html

[E13] 逐字符遍历
来源：http://hz.tian-w.cn/gtpuoafrju.html

Py:   for ch in s: print(ch)
来源：http://hz.ehwqpu.com/gtperfqcwf.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.aizwys.cn/gtxzxljxrh.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yj20258.top/gtrjjgfqba.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.kuanghao11.cn/gtrflkclkp.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.ivvv.top/gtredvhkdb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.xinyue.icu/gtmqivpegm.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.fengsongda.top/gtqlfprgbh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.guowangkeji.top/gtilazygwr.html

[E14] URL 编码与 Base64
来源：http://hz.sufxvd.cn/gtfmyaxkbd.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.zdqjudy.top/gthylijeyp.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.nanxinkj.top/gtnpsavjlm.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.xuetiantiany.cn/gtjcpyonmj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.pengpengdd.cyou/gtfqsrjxuj.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.jiagoushi.top/gtmmeepfbh.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.yueranfly.top/gtdrinrfdw.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.svipenyu.cn/gtmsrepyhz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.zhiwuduotai.top/gtvgapfxmg.html

[E15] HTML 转义 / 反转义
来源：http://hz.yueranfly.top/gtmsdnyjmy.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.bjfxy.top/gtlxeifuil.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.cqqwz.cn/gtzuzntmjl.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.shangyingyoupin.top/gtqpcqnxio.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.jianghu66.top/gtdkinucul.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.hysaishi.cn/gtlwldedqw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.yuanzhike.top/gtiplbhugd.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.aibaodan.cn/gtozntkrkh.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.andypj.xyz/gtvrrasjjb.html

[E16] 数字千分位
来源：http://hz.shzxlz.cn/gtcxcyvdbm.html

Py:   f"{1234567:,}"
来源：http://hz.tanke756.top/gtgmujefhf.html

PHP:  number_format(1234567);
来源：http://hz.xinyue.icu/gtgvxwrnrs.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.hnxiangtu.top/gtryuhkkna.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.quarkkingdee.top/gtkufanyca.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.xuetiantiany.cn/gtslmsgppx.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.yonumen.top/gtqifpidhz.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.hnqzz.top/gtwstteyvy.html

C#:   1234567.ToString("N0")
来源：http://hz.cucudq.cn/gtvybkmdyq.html

[E17] 首字母大写
来源：http://hz.zhiwuduotai.top/gtzptfolts.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.jqgufenzy.top/gtornoicrh.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.xingfuxueyuan.xyz/gtdubhtilq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.shuidangran.top/gtztteddhc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yueranfly.top/gtfeyldrza.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.zhijiandao.cn/gteqtogyva.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.xingfuxueyuan.xyz/gtnpkdhjrs.html

Ruby: s.capitalize
来源：http://hz.jianghu66.top/gttzbybngz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.zhoulong.xyz/gtmqgpffgm.html

[E18] 模板占位符替换
来源：http://hz.havefunace.top/gtudgoxcxc.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.9152youxi.cn/gtuyhpvlrm.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.hnxiangtu.top/gteugxxbuy.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.316326.xyz/gttpzfwlaq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.hammf.cn/gtrewddxza.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.ppjwa.cn/gteauewwlo.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.jqgfzy.top/gtvjpcstcj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.jqgfzy.top/gtpatzcsbf.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.0kj1m.cn/gtuziwghux.html

[E19] 多行文本按行拆分
来源：http://hz.andypj.xyz/gtixerpeir.html

Py:   s.splitlines()
来源：http://hz.hywenlv.cn/gthydnyinp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.yangfankeji.com/gtpbnqejms.html

JS:   s.split(/\r?\n/)
来源：http://hz.yj20258888.top/gtaaivnqvb.html

TS:   s.split(/\r?\n/)
来源：http://hz.svipenyu.cn/gtpiywkosv.html

Java: s.lines().toList()
来源：http://hz.zhiwuduotai.top/gtghkgcfcl.html

Go:   strings.Split(s, "\n")
来源：http://hz.dashuyun.cn/gtnqeujtei.html

Ruby: s.lines
来源：http://hz.chenlongwang.top/gttidhxfdm.html

C#:   s.Split('\n')
来源：http://hz.jinghuilouyu.cn/gtfshbmvcn.html

[E20] 判断字符串是否为空
来源：http://hz.aibaodan.cn/gtkwixcfux.html

Py:   if not s:
来源：http://hz.hnxiangtu.top/gtjsijjztp.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.ppjwa.cn/gtrkrvuyfr.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.tanke756.top/gttwipwpnm.html

TS:   if (s === "") {}
来源：http://hz.yongpay.top/gthyzuyeme.html

Java: if (s.isEmpty()) {}
来源：http://hz.aibaodan.cn/gtqjbwmzvq.html

Go:   if s == "" {}
来源：http://hz.birdmap.top/gtkzzqgjwf.html

Ruby: if s.empty?
来源：http://hz.chenlongwang.top/gtrqhohohz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.zycfv.cn/gtaxlooerb.html

[E21] 超长截断加省略号
来源：http://hz.ivvv.top/gtoqfgyknf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.dianchejie.cn/gtwmeajify.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.daxiang520.top/gtjdaazyfl.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.chenjidiqi.icu/gtqvygstnj.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.tanke756.top/gtgjcixvbj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yangfankeji.com/gtgkjalctg.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.hnqzz.top/gtwpyrebzt.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.tanke756.top/gthigbxxbf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.wangshuangyany.cn/gtjwtsisaz.html

[E22] 字节长度与字符长度
来源：http://hz.ybcxt.top/gthzxbioec.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.daxiang520.top/gtwsvpnfzg.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.gaohongyu789.top/gtjmcpviqi.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.dashuyun.cn/gtwuqeizxq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.fzhhl.top/gtghurihdm.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.yj20258.top/gtnhyqxwis.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.0kj1m.cn/gtbpqblzms.html

Ruby: s.bytesize;  s.length
来源：http://hz.daxiang520.top/gtyuluhhvl.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.feifeiyinyue.top/gtvekbkrvm.html

================================================================================
来源：http://hz.haohaochexian.top/gtegmaobxi.html

F. 文件与目录
来源：http://hz.ehwqpu.com/gtkovfcxhx.html

================================================================================
来源：http://hz.aizwys.cn/gtcqmdicwv.html

[F01] 读取整个文件
来源：http://hz.wangdashe.top/gtdyeqjuln.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.snrcjt.cn/gtrghaykvw.html

PHP:  file_get_contents("a.txt");
来源：http://hz.yangfankeji.com/gtisbngbus.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.pycfn.com/gtdidsbwex.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.jqgufenzy.top/gtdlybajhd.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.pycfn.com/gtsjkncnkh.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.kuanghao11.cn/gtoptyvqnp.html

Ruby: File.read("a.txt")
来源：http://hz.zhoulong.xyz/gtkvhlsiyw.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.daria6918.cn/gtkslgsbev.html

[F02] 逐行读取文件
来源：http://hz.sufxvd.cn/gtatpzbnpn.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.yuanzhike.top/gtahqshvjc.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.chenjidiqi.icu/gttsrmzgcq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jlsjyb.cn/gtmjaajixv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.chenjidiqi.icu/gtupcfwtry.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.birdmap.top/gtinqzbebr.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.sxryk.cn/gtrcnsxjly.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.quarkkingdee.top/gtpgdpfxqd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.vqdsnc.cn/gtdolketsn.html

[F03] 写入文件（覆盖）
来源：http://hz.yongpay.top/gtnzfssxon.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.shanyushiyangkeji.top/gtjmaypqmm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.gaohongyu789.top/gttxcuaoub.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.birdmap.top/gttsmudbzt.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.snrcjt.cn/gthbjascfu.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.zycfv.cn/gtxkstlkjv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.yongpay.top/gtswffkihc.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.xuetiantiany.cn/gtutvngvjn.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.nwbrower.top/gtuvzybolo.html

[F04] 追加写入文件
来源：http://hz.jyoumei.cn/gtcumtnmxi.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.hywenlv.cn/gtqitkbtpl.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.iojbl.cn/gtsqpdnmzo.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.hywenlv.cn/gtysqbjzst.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.smart0.xyz/gtkulvyqud.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.jinqigufen.top/gtcsmrcpzp.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.redwolf501.top/gtrlvwswgo.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.cdnleiting.top/gtqbpjwgws.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.chenlongwang.top/gtroeoctrl.html

[F05] 判断文件或目录是否存在
来源：http://hz.shanyushiyangkeji.top/gtffddyylj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.hongshengwenyu.top/gtkfspmggc.html

PHP:  file_exists("a.txt");
来源：http://hz.meibo888.top/gtsqgqcffv.html

JS:   fs.existsSync("a.txt")
来源：http://hz.smart0.xyz/gtgrxdetqn.html

TS:   fs.existsSync("a.txt")
来源：http://hz.9152youxi.cn/gtmaewiumz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.pycfn.com/gtejlptypv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.redwolf501.top/gtletixepx.html

Ruby: File.exist?("a.txt")
来源：http://hz.yanxiufei.cn/gtylimzjic.html

C#:   File.Exists("a.txt")
来源：http://hz.wangdashe.top/gthjsanteg.html

[F06] 删除文件
来源：http://hz.zhixingplan.top/gtvhjpxoup.html

Py:   os.remove("a.txt")
来源：http://hz.cheryme.top/gtkhawemvp.html

PHP:  unlink("a.txt");
来源：http://hz.jinqigfzy.top/gtreatacfu.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.gaohongyu789.top/gtsrmlduvg.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.xylfe.cn/gtxarhzlro.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.shangyingyoupin.top/gtxdnhnohh.html

Go:   os.Remove("a.txt")
来源：http://hz.hywenlv.cn/gtaqyrcbox.html

Ruby: File.delete("a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtakxfsfug.html

C#:   File.Delete("a.txt");
来源：http://hz.nanxuanxn.top/gtrzkqkdoc.html

[F07] 创建目录（含多级）
来源：http://hz.cashguo.top/gtwavaoqeu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.haohaochexian.top/gtiuxyjxsz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.jyoumei.cn/gtkpodqast.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.quarkkingdee.top/gtajtvljgu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhijiandao.cn/gtizybtkkq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.wangdashe.top/gtczekpyrp.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.tianlin.xyz/gtztggrwxg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.gogol.net.cn/gtlivvtzyx.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.xylfe.cn/gtpwxlcgbv.html

[F08] 遍历目录
来源：http://hz.tianlin.xyz/gtdxmpuvau.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.sxryk.cn/gtcrrikmah.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.birdmap.top/gtqhbzfxci.html

JS:   fs.readdirSync("dir")
来源：http://hz.yj20258.top/gtdursbown.html

TS:   fs.readdirSync("dir")
来源：http://hz.chenlongwang.top/gtycpbodjo.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.yuxming.cn/gtasfitlsk.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.jqgfzy.top/gtioiqgbyz.html

Ruby: Dir.children("dir")
来源：http://hz.yj20258888.top/gthfyjbext.html

C#:   Directory.GetFiles("dir")
来源：http://hz.0kj1m.cn/gttzxvetux.html

[F09] 获取文件大小
来源：http://hz.gaohongyu789.top/gtmlpflqtn.html

Py:   os.path.getsize("a.txt")
来源：http://hz.dashuyun.cn/gtqjlxangf.html

PHP:  filesize("a.txt");
来源：http://hz.redwolf501.top/gtyjxnpmvo.html

JS:   fs.statSync("a.txt").size
来源：http://hz.aibaodan.cn/gtlzvravum.html

TS:   fs.statSync("a.txt").size
来源：http://hz.vqdsnc.cn/gtxvifceit.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.gotoacloud.top/gtryfhrfvt.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.hammf.cn/gtubmjcfzk.html

Ruby: File.size("a.txt")
来源：http://hz.zhongyouzk.top/gtapthobkf.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.zhaomingkeji.xyz/gtmweawkqq.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.zhaomingkeji.xyz/gtkvrtqopd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.zdqjudy.top/gtmshmicbe.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.xingfuxueyuan.xyz/gthkgmhhxc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.jqgfzy.top/gtbsuneumg.html

TS:   path.extname("a.txt")
来源：http://hz.zycfv.cn/gtlkscwpiu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.ppjwa.cn/gtlrubssid.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.pycfn.com/gttvmswltc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.yangfankeji.com/gttyjwmlpz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.zhengqikj.top/gtaqjmqvtb.html

[F11] 复制与移动文件
来源：http://hz.hongshengwenyu.top/gtjcnnxrfg.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.9152youxi.cn/gtmnvshrgu.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.dashuyun.cn/gtlhexjllj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xziqi.cn/gtesmkfwwl.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.wangshuangyany.cn/gtwvwqffqb.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.zhongyouzk.top/gtevhyduai.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.chenjidiqi.icu/gtfltirtte.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.snrcjt.cn/gttizzdben.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.hywenlv.cn/gtvihayivy.html

[F12] CSV 读写
来源：http://hz.zhixingplan.top/gtjimdosiq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.9152youxi.cn/gtsprwmmdk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.shanyushiyangkeji.top/gtvnmfcosn.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.tanke756.top/gtcoqmqbnw.html

TS:   // 同上
来源：http://hz.xuetiantiany.cn/gtjfxpypnl.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.9152youxi.cn/gtoppbsllb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.xinyue.icu/gtjuervgvd.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.zhongyouzk.top/gtzbrytbpe.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.ywan-chungtsiang.top/gtlkrxgmgq.html

================================================================================
来源：http://hz.yj20258888.top/gtlmrwdisg.html

G. 面向对象
来源：http://hz.hongshengwenyu.top/gtiiurhldn.html

================================================================================
来源：http://hz.aibaodan.cn/gtsngcnhyo.html

[G01] 定义类
来源：http://hz.iojbl.cn/gtgsixygbm.html

Py:   class User: pass
来源：http://hz.snrcjt.cn/gtuywxgzdr.html

PHP:  class User {}
来源：http://hz.svipenyu.cn/gtfswdkhln.html

JS:   class User {}
来源：http://hz.cdnleiting.top/gtgqvqhswq.html

TS:   class User { name: string = ""; }
来源：http://hz.daxiang520.top/gtmttfikdh.html

Java: class User {}
来源：http://hz.bjfxy.top/gtvbhbofvx.html

Go:   type User struct { Name string }
来源：http://hz.guowangkeji.top/gtvdlpaoqe.html

Ruby: class User; end
来源：http://hz.dianchejie.cn/gtquafmydb.html

C#:   class User {}
来源：http://hz.316326.xyz/gteviopgtf.html

[G02] 构造函数
来源：http://hz.gzhubu.top/gtmwxiytvu.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yvedp.cn/gtxwhsyfqp.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.zhoulong.xyz/gtmqybkddc.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.dianchejie.cn/gtwdriqjwz.html

TS:   constructor(public name: string) {}
来源：http://hz.iojbl.cn/gtmfglianh.html

Java: User(String name) { this.name = name; }
来源：http://hz.ydzc1.top/gtngxxaqdi.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.cashguo.top/gtlyauplau.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.jqgfzy.top/gtgunwcmwi.html

C#:   public User(string name) { Name = name; }
来源：http://hz.jianghu66.top/gtvrtstlzh.html

[G03] 实例属性
来源：http://hz.svipenyu.cn/gtswxxxrpz.html

Py:   self.name = "x"
来源：http://hz.jqgufenzy.top/gthzuoiouh.html

PHP:  public string $name = "x";
来源：http://hz.yuanzhike.top/gtbkrnjpym.html

JS:   this.name = "x";
来源：http://hz.jiagoushi.top/gtlecxjqdj.html

TS:   name: string = "x";
来源：http://hz.ppjwa.cn/gtvnhykfux.html

Java: private String name;
来源：http://hz.zhijiandao.cn/gtrkfyhgfk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.hfpthk.cn/gtsoagkvsx.html

Ruby: @name = "x"
来源：http://hz.quarkkingdee.top/gteynntnuj.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yj20258888.top/gtkzuxnzdm.html

[G04] 定义方法
来源：http://hz.daria6918.cn/gtfuhscyup.html

Py:   def greet(self): return self.name
来源：http://hz.redwolf501.top/gtkrlcgdva.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.zhaomingkeji.xyz/gtgclqvvxz.html

JS:   greet() { return this.name; }
来源：http://hz.shanyushiyangkeji.top/gtwelofusw.html

TS:   greet(): string { return this.name; }
来源：http://hz.bjfxy.top/gtipjhmaqi.html

Java: String greet() { return name; }
来源：http://hz.nwbrower.top/gtphdiaqps.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.xuetiantiany.cn/gtnbdfavjw.html

Ruby: def greet; @name; end
来源：http://hz.hywenlv.cn/gtzaemayob.html

C#:   public string Greet() => Name;
来源：http://hz.fengsongda.top/gtqmlbmefq.html

[G05] 继承
来源：http://hz.xuetiantiany.cn/gtabryynxu.html

Py:   class Admin(User): pass
来源：http://hz.jinqigufen.top/gthuqgkefv.html

PHP:  class Admin extends User {}
来源：http://hz.cheryme.top/gthxxircva.html

JS:   class Admin extends User {}
来源：http://hz.redwolf501.top/gtnnfwombv.html

TS:   class Admin extends User {}
来源：http://hz.ydjk.org.cn/gtufnxctxp.html

Java: class Admin extends User {}
来源：http://hz.hywenlv.cn/gtwyyknjsa.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.cqqwz.cn/gtsedaxcrl.html

Ruby: class Admin < User; end
来源：http://hz.xziqi.cn/gtkvezwgdv.html

C#:   class Admin : User {}
来源：http://hz.xuetiantiany.cn/gtndkpjuwj.html

[G06] 重写方法
来源：http://hz.hongshengwenyu.top/gtyxycmnvx.html

Py:   def greet(self): return "admin"
来源：http://hz.chenjidiqi.icu/gtofsolgrd.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.zhaomingkeji.xyz/gtddvnvloo.html

JS:   greet() { return "admin"; }
来源：http://hz.svipenyu.cn/gtunyoftoc.html

TS:   greet(): string { return "admin"; }
来源：http://hz.dianchejie.cn/gtmpxpqnbl.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.ivvv.top/gtnkchrsuo.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.fengsongda.top/gtdojwtqkz.html

Ruby: def greet; "admin"; end
来源：http://hz.cashguo.top/gttckibrdc.html

C#:   public override string Greet() => "admin";
来源：http://hz.dashuyun.cn/gtceskurjw.html

[G07] 调用父类方法
来源：http://hz.jqgufenzy.top/gtrsilzovr.html

Py:   super().greet()
来源：http://hz.shanyushiyangtech.top/gtuexxryqr.html

PHP:  parent::greet();
来源：http://hz.jinqigfzy.top/gtldhfvevy.html

JS:   super.greet();
来源：http://hz.ppjwa.cn/gttmlmqqtw.html

TS:   super.greet();
来源：http://hz.ybcxt.top/gtzhqybwql.html

Java: super.greet();
来源：http://hz.yj202588.top/gtprhoguqm.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.kuanghao11.cn/gtdsjbrbzd.html

Ruby: super
来源：http://hz.aibaodan.cn/gtmjrcmikp.html

C#:   base.Greet();
来源：http://hz.chenlongwang.top/gtmhawfate.html

[G08] 静态方法与属性
来源：http://hz.quarkkingdee.top/gtchvqffol.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.cashguo.top/gtjprnzrce.html

PHP:  public static function f() {}
来源：http://hz.shangyingyoupin.top/gtwmpyatkf.html

JS:   static f() {}
来源：http://hz.chenjidiqi.icu/gtlkvhorsu.html

TS:   static f(): void {}
来源：http://hz.smart0.xyz/gtjhdbdufx.html

Java: static void f() {}
来源：http://hz.nanxinkj.top/gtjmiekapk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.ydjk.org.cn/gtmbhlablc.html

Ruby: def self.f; end
来源：http://hz.jinyuanbaomall.cn/gtndqomzkb.html

C#:   public static void F() {}
来源：http://hz.meibo888.top/gtpbpnfavh.html

[G09] 接口 / 抽象类
来源：http://hz.wangshuangyany.cn/gtoounxekp.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.iojbl.cn/gtmocofkxa.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yonumen.top/gtmdkznlme.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.zhijiandao.cn/gtghtttjgl.html

TS:   interface Shape { area(): number; }
来源：http://hz.xuetiantiany.cn/gtpzfblqyv.html

Java: interface Shape { double area(); }
来源：http://hz.hnxiangtu.top/gtanytpyjj.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.xingfuxueyuan.xyz/gtgoxlaldd.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.hammf.cn/gtleqcsvbr.html

C#:   interface IShape { double Area(); }
来源：http://hz.jinqigfzy.top/gtxirouocw.html

[G10] 访问控制
来源：http://hz.yuanzhike.top/gtyivblfls.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.jqgufenzy.top/gttebrueyk.html

PHP:  public / protected / private
来源：http://hz.chenlongwang.top/gtqqmftgkr.html

JS:   #private 字段；其余公开
来源：http://hz.chenzaomai.com/gthsuleoig.html

TS:   public / protected / private
来源：http://hz.snrcjt.cn/gtjonkifgv.html

Java: public / protected / private / 默认包级
来源：http://hz.xylfe.cn/gtbhtxsygb.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.52xcode.cn/gtnqvqkvoj.html

Ruby: public / protected / private
来源：http://hz.jqgufenzy.top/gtuyzsqpsl.html

C#:   public / protected / private / internal
来源：http://hz.aizwys.cn/gtevjxwiwm.html

[G11] getter / setter
来源：http://hz.chenjidiqi.icu/gtmzzqrxtz.html

Py:   @property 与 @x.setter
来源：http://hz.sweek.top/gtfmdvsoon.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jinghuilouyu.cn/gtyfnkhynd.html


<!-- 参考信息 -->