代发 wailian999

Go:   strings.Count(s, "a")
来源：http://hz.birdmap.top/gtzgswttay.html

Ruby: s.count("a")
来源：http://hz.yj20258.top/gtcscijcjd.html

C#:   s.Count(c => c == 'a')
来源：http://hz.daria6918.cn/gtkccaihcm.html

[E13] 逐字符遍历
来源：http://hz.yangfankeji.com/gtvrgozspk.html

Py:   for ch in s: print(ch)
来源：http://hz.316326.xyz/gtlclthtsh.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.hysaishi.cn/gtwkrmwhqt.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.nanxuanxn.top/gtymmpieyo.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.aizwys.cn/gtcjfamzmi.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.xingfuxueyuan.xyz/gtljkzgjai.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.yuanzhike.top/gtjdtdwenr.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.wangdashe.top/gthvowhncg.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.xinyue.icu/gtyccdujii.html

[E14] URL 编码与 Base64
来源：http://hz.yuxming.cn/gtstjflzwy.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.iojbl.cn/gtatdqqrrx.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.gzhubu.top/gtnkhihsfh.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.xuanzx.com/gtzufcrduw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.zycfv.cn/gtvmhnqxrw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.jqgufenzy.top/gtcrartirp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.shuidangran.top/gtcxkknyqx.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.cashguo.top/gtfdcjkjzk.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yuanzhike.top/gtgzgdccah.html

[E15] HTML 转义 / 反转义
来源：http://hz.jqgfzy.top/gtxozpmshd.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.jinghuilouyu.cn/gtymdthpqr.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.zhongyouzk.top/gtcesjwscd.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.sufxvd.cn/gtvwmqzrqi.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.tianlin.xyz/gtjdzuwodr.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.ehwqpu.com/gtuwqqwige.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.svipenyu.cn/gtrxikhuqf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.zhongyouzk.top/gtrfjcyfjn.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.daxiang520.top/gtfulvkjqk.html

[E16] 数字千分位
来源：http://hz.feifeiyinyue.top/gtmibleetk.html

Py:   f"{1234567:,}"
来源：http://hz.cucudq.cn/gtuziapfpc.html

PHP:  number_format(1234567);
来源：http://hz.yuanzhike.top/gtiqnosuyj.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.daria6918.cn/gtrnwifkxx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.sweek.top/gtflhmfhxr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.nanxuanxn.top/gtptyyxsmp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.dashuyun.cn/gtlcfbdivt.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.jyoumei.cn/gtwgeddcwl.html

C#:   1234567.ToString("N0")
来源：http://hz.ehwqpu.com/gtftoyxqyt.html

[E17] 首字母大写
来源：http://hz.tian-w.cn/gttmcqrmhp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.cashguo.top/gtcdgdqycf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.hywenlv.cn/gtoizrkubo.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.havefunace.top/gtgrluynrx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.sxryk.cn/gtbhxjyuts.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.quarkkingdee.top/gtlfsbizli.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.yj20258.top/gtmfbffdoh.html

Ruby: s.capitalize
来源：http://hz.gotoacloud.top/gtjxnhmeio.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yuxming.cn/gtivumrgnx.html

[E18] 模板占位符替换
来源：http://hz.andypj.xyz/gtwgowuele.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.shangyingyoupin.top/gtzveplxws.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.shuidangran.top/gtkfbogglw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.shzxlz.cn/gtcqmhkgxg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.zdqjudy.top/gtifinvatu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.jqgufenzy.top/gtqmruwuhb.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.shanyushiyangtech.top/gtilmlteah.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.sxryk.cn/gtnkflwims.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.haohaochexian.top/gtvnqnfmbl.html

[E19] 多行文本按行拆分
来源：http://hz.ivvv.top/gtedhgelym.html

Py:   s.splitlines()
来源：http://hz.xuanzx.com/gtoibcbofl.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.yuxming.cn/gtftusdhyu.html

JS:   s.split(/\r?\n/)
来源：http://hz.yanxiufei.cn/gtophrxojl.html

TS:   s.split(/\r?\n/)
来源：http://hz.chenlongwang.top/gttvhgmxaw.html

Java: s.lines().toList()
来源：http://hz.dashuyun.cn/gtgympaxtg.html

Go:   strings.Split(s, "\n")
来源：http://hz.shangyingyoupin.top/gtybtfbmmh.html

Ruby: s.lines
来源：http://hz.bjfxy.top/gtgiidyhvy.html

C#:   s.Split('\n')
来源：http://hz.wangdashe.top/gtyqqibqfv.html

[E20] 判断字符串是否为空
来源：http://hz.wangshuangyany.cn/gtnycrnrlf.html

Py:   if not s:
来源：http://hz.jlsjyb.cn/gtujxzersg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.zhiwuduotai.top/gtgnevgmjl.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.cucudq.cn/gtfzzxjmvf.html

TS:   if (s === "") {}
来源：http://hz.zhoulong.xyz/gtydqxoxhh.html

Java: if (s.isEmpty()) {}
来源：http://hz.shanyushiyangkeji.top/gtvnhaqrhx.html

Go:   if s == "" {}
来源：http://hz.ybcxt.top/gtzdjsjuuh.html

Ruby: if s.empty?
来源：http://hz.shangyingyoupin.top/gtobrgxymp.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.cashguo.top/gtsuhoikio.html

[E21] 超长截断加省略号
来源：http://hz.birdmap.top/gtyexbzvmu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.52xcode.cn/gtpmjrvxfg.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.cheryme.top/gtshfipuol.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.shzxlz.cn/gteypemron.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jyoumei.cn/gtrhqmwggr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.xuetiantiany.cn/gtfxyvfrwu.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.fzhhl.top/gtfnhncyrc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.havefunace.top/gttwbbzrvt.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.shangyingyoupin.top/gtwdsbifbo.html

[E22] 字节长度与字符长度
来源：http://hz.xingfuxueyuan.xyz/gthgrcaehr.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.yuxming.cn/gtuktqvfuv.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.redwolf501.top/gtcbuqxyef.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.sxryk.cn/gtmbskfuur.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.gzhubu.top/gtjjqbpppm.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.nanxinkj.top/gtopssorof.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.cheryme.top/gtskpiixox.html

Ruby: s.bytesize;  s.length
来源：http://hz.xziqi.cn/gtgqutfhbb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.iojbl.cn/gtsndnhmum.html

================================================================================
来源：http://hz.kuanghao11.cn/gtscgfqffx.html

F. 文件与目录
来源：http://hz.hysaishi.cn/gtsuerdgai.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtujehomou.html

[F01] 读取整个文件
来源：http://hz.cucudq.cn/gtrtluqfby.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.shanyushiyangkeji.top/gtgzkchsfx.html

PHP:  file_get_contents("a.txt");
来源：http://hz.yonumen.top/gtpblyuwvv.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.ehwqpu.com/gtytokwcwr.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.chenjidiqi.icu/gtyxuwminr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.chenzaomai.com/gtlsvjonvz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.nanxuanxn.top/gtmidpcqfb.html

Ruby: File.read("a.txt")
来源：http://hz.zhixingplan.top/gttxqpfmbu.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.daxiang520.top/gtneyotkkz.html

[F02] 逐行读取文件
来源：http://hz.fzhhl.top/gthltzjkqa.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.ybcxt.top/gtkpvnewrl.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.yj20258888.top/gttmdeyflm.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.shuidangran.top/gtpjmgwhcu.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zdqjudy.top/gtjsnnjxoq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.gotoacloud.top/gtrtrexonv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.aibaodan.cn/gtpyycxjcf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.c1oappe.top/gtueknibar.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.zhiwuduotai.top/gtocwditfn.html

[F03] 写入文件（覆盖）
来源：http://hz.smart0.xyz/gtwsbzxbrn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.yanxiufei.cn/gtakqnzyid.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.dashuyun.cn/gttiiwddow.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zdqjudy.top/gtclmlmbtd.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.smart0.xyz/gtkakedajm.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.ppjwa.cn/gtbtkigidm.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.wangdashe.top/gtxnskcqzy.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.jqgufenzy.top/gtddmcurko.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.jyoumei.cn/gtbwdeqxxf.html

[F04] 追加写入文件
来源：http://hz.xinyue.icu/gtyjxkultq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.aibaodan.cn/gteymkqajy.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.cucudq.cn/gtrhcljggg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ivvv.top/gtwnmkotke.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.aizwys.cn/gtcmmtbayd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.yj20258888.top/gtnvpojhcv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.jinqigufen.top/gtsmcttsrx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.hysaishi.cn/gtigpkhvxc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.tianlin.xyz/gtwtxexgzo.html

[F05] 判断文件或目录是否存在
来源：http://hz.ywan-chungtsiang.top/gtairoupkz.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.xylfe.cn/gtxkepajjx.html

PHP:  file_exists("a.txt");
来源：http://hz.havefunace.top/gtvhaowmcg.html

JS:   fs.existsSync("a.txt")
来源：http://hz.tianlin.xyz/gtqbnqpssp.html

TS:   fs.existsSync("a.txt")
来源：http://hz.cdnleiting.top/gtbhxwqfcz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.zhiwuduotai.top/gtwgtwtjao.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.hfpthk.cn/gtzafklpww.html

Ruby: File.exist?("a.txt")
来源：http://hz.cucudq.cn/gtixlytcyh.html

C#:   File.Exists("a.txt")
来源：http://hz.iojbl.cn/gtoffzoiop.html

[F06] 删除文件
来源：http://hz.zhiwuduotai.top/gtmrvqznje.html

Py:   os.remove("a.txt")
来源：http://hz.snrcjt.cn/gteyvcibzx.html

PHP:  unlink("a.txt");
来源：http://hz.316326.xyz/gtkprunzke.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.ydjk.org.cn/gtlgybkgdh.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.zhixingplan.top/gtfhkuffir.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.shanyushiyangkeji.top/gthftdrcjd.html

Go:   os.Remove("a.txt")
来源：http://hz.xuetiantiany.cn/gtgkegoudd.html

Ruby: File.delete("a.txt")
来源：http://hz.jlsjyb.cn/gtvyjtusph.html

C#:   File.Delete("a.txt");
来源：http://hz.hnxiangtu.top/gtivlruqii.html

[F07] 创建目录（含多级）
来源：http://hz.zdqjudy.top/gtmtyzutyf.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.vqdsnc.cn/gtfzwxubko.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.guannengcc.top/gtnhnambes.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.snrcjt.cn/gtoneiciqb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhoulong.xyz/gtronpynlk.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.sxryk.cn/gtumashlsh.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jianghu66.top/gtjychczfn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.zhongyouzk.top/gtdurtcilr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.dashuyun.cn/gtmskkifgm.html

[F08] 遍历目录
来源：http://hz.tianlin.xyz/gtpgaaifpu.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.hammf.cn/gtvuqnonxb.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.guowangkeji.top/gtrdphxxky.html

JS:   fs.readdirSync("dir")
来源：http://hz.ybcxt.top/gtbrrbacld.html

TS:   fs.readdirSync("dir")
来源：http://hz.tanke756.top/gtcjxkmuul.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.shangyingyoupin.top/gtnnhcocxw.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.andypj.xyz/gtnpcedgrc.html

Ruby: Dir.children("dir")
来源：http://hz.vqdsnc.cn/gtvkdmgdls.html

C#:   Directory.GetFiles("dir")
来源：http://hz.jqgufenzy.top/gtbtrchrmt.html

[F09] 获取文件大小
来源：http://hz.hongshengwenyu.top/gtsagkkklt.html

Py:   os.path.getsize("a.txt")
来源：http://hz.sxryk.cn/gtqbmxxcoy.html

PHP:  filesize("a.txt");
来源：http://hz.svipenyu.cn/gtrcytbywy.html

JS:   fs.statSync("a.txt").size
来源：http://hz.iojbl.cn/gtapmrxhvf.html

TS:   fs.statSync("a.txt").size
来源：http://hz.jlsjyb.cn/gtoraarkrs.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.kuanghao11.cn/gtdoxlzwgs.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.andypj.xyz/gtildslzzz.html

Ruby: File.size("a.txt")
来源：http://hz.snrcjt.cn/gtwcraxjna.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.redwolf501.top/gtkhsyspyk.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yanxiufei.cn/gtehdvgmjj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.0kj1m.cn/gtdujsmcto.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.jqgfzy.top/gtkrrmoqxx.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.0kj1m.cn/gtjnckxpvl.html

TS:   path.extname("a.txt")
来源：http://hz.tian-w.cn/gtwebdhwps.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.kuanghao11.cn/gtwxxvklgz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.zhoulong.xyz/gtwsjteauc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.zhixingplan.top/gtzipedyhz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.jinghuilouyu.cn/gtzytifhvk.html

[F11] 复制与移动文件
来源：http://hz.shuidangran.top/gtaidbnffa.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.ppjwa.cn/gtsdrqydwx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.zdqjudy.top/gtbcfkjrjl.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.daria6918.cn/gtqolvmrsc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.feifeiyinyue.top/gtxaqlcoxq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.zycfv.cn/gtkbvjjwft.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.chenlongwang.top/gtxnljnfqm.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.pycfn.com/gtioidgqdz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.xinyue.icu/gtrituaylu.html

[F12] CSV 读写
来源：http://hz.fzhhl.top/gtdjnpeutc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.ydzc1.top/gttwhrjhpo.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.ppjwa.cn/gthstjsvvq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.iojbl.cn/gtbmhtacix.html

TS:   // 同上
来源：http://hz.cdnleiting.top/gtpmfahgqd.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.ybcxt.top/gtrknscuno.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.xylfe.cn/gtyojastkh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.fengsongda.top/gtkesczulf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yongpay.top/gtfgpfnufz.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtljviidxs.html

G. 面向对象
来源：http://hz.yanxiufei.cn/gtqbywulaf.html

================================================================================
来源：http://hz.svipenyu.cn/gtcbriexjs.html

[G01] 定义类
来源：http://hz.tianlin.xyz/gtlzzuvvby.html

Py:   class User: pass
来源：http://hz.jqgufenzy.top/gthyvvvudt.html

PHP:  class User {}
来源：http://hz.jinyuanbaomall.cn/gtnjupkdsm.html

JS:   class User {}
来源：http://hz.yj20258.top/gtfzjcqoio.html

TS:   class User { name: string = ""; }
来源：http://hz.meibo888.top/gtxzpdbdqn.html

Java: class User {}
来源：http://hz.52xcode.cn/gtrcrwarbr.html

Go:   type User struct { Name string }
来源：http://hz.jinghuilouyu.cn/gtsaagvimb.html

Ruby: class User; end
来源：http://hz.zhixingplan.top/gtczofzfwy.html

C#:   class User {}
来源：http://hz.gzhubu.top/gtqclqjhcb.html

[G02] 构造函数
来源：http://hz.zhongyouzk.top/gtrvhnvywc.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.hywenlv.cn/gtlsrwglst.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.nanxuanxn.top/gtlnnwtfkc.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.chenjidiqi.icu/gtagvfuqdb.html

TS:   constructor(public name: string) {}
来源：http://hz.c1oappe.top/gtghplogbu.html

Java: User(String name) { this.name = name; }
来源：http://hz.zhengqikj.top/gttvamfrii.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.pengpengdd.cyou/gtkqxbaxug.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.52xcode.cn/gtaqtvzyot.html

C#:   public User(string name) { Name = name; }
来源：http://hz.pycfn.com/gtouqjkxve.html

[G03] 实例属性
来源：http://hz.shzxlz.cn/gtpxujneqk.html

Py:   self.name = "x"
来源：http://hz.jyoumei.cn/gtwxtttskg.html

PHP:  public string $name = "x";
来源：http://hz.zdqjudy.top/gtlxyvnwmq.html

JS:   this.name = "x";
来源：http://hz.pengpengdd.cyou/gtneuxgdol.html

TS:   name: string = "x";
来源：http://hz.ybcxt.top/gtcblaagwm.html

Java: private String name;
来源：http://hz.zhengqikj.top/gtgbzbiarp.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.cashguo.top/gthsavqatf.html

Ruby: @name = "x"
来源：http://hz.chenzaomai.com/gtbwbehcym.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.guowangkeji.top/gtxobmwqiz.html

[G04] 定义方法
来源：http://hz.aibaodan.cn/gtaxltpcea.html

Py:   def greet(self): return self.name
来源：http://hz.9152youxi.cn/gtdanvpyxa.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yueranfly.top/gtosgflfew.html

JS:   greet() { return this.name; }
来源：http://hz.hongshengwenyu.top/gtndcoowwn.html

TS:   greet(): string { return this.name; }
来源：http://hz.yuxming.cn/gtyppxtege.html

Java: String greet() { return name; }
来源：http://hz.hnxiangtu.top/gtgirdplbb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.zhaomingkeji.xyz/gtdhbhliui.html

Ruby: def greet; @name; end
来源：http://hz.smart0.xyz/gtdrmumjov.html

C#:   public string Greet() => Name;
来源：http://hz.haohaochexian.top/gtfwltjuxo.html

[G05] 继承
来源：http://hz.xylfe.cn/gtrfsxafcd.html

Py:   class Admin(User): pass
来源：http://hz.shangyingyoupin.top/gtdaoyxlnq.html

PHP:  class Admin extends User {}
来源：http://hz.gotoacloud.top/gtqkvpqujx.html

JS:   class Admin extends User {}
来源：http://hz.ydzc1.top/gtahoommmn.html

TS:   class Admin extends User {}
来源：http://hz.pycfn.com/gttbsfriaa.html

Java: class Admin extends User {}
来源：http://hz.chenzaomai.com/gtnvbtktfh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.0kj1m.cn/gtqzuzmoiz.html

Ruby: class Admin < User; end
来源：http://hz.zhongyouzk.top/gtjwehsfvp.html

C#:   class Admin : User {}
来源：http://hz.haohaochexian.top/gtrcukjeyc.html

[G06] 重写方法
来源：http://hz.c1oappe.top/gtdrpyguax.html

Py:   def greet(self): return "admin"
来源：http://hz.hammf.cn/gtrunaeilh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.zhengqikj.top/gtgznxmdkn.html

JS:   greet() { return "admin"; }
来源：http://hz.vqdsnc.cn/gtmhtffeem.html

TS:   greet(): string { return "admin"; }
来源：http://hz.xuetiantiany.cn/gtabqclffu.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.chenjidiqi.icu/gtmkexxldq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.aizwys.cn/gttynjgqxb.html

Ruby: def greet; "admin"; end
来源：http://hz.gzhubu.top/gtduelosal.html

C#:   public override string Greet() => "admin";
来源：http://hz.zhijiandao.cn/gtfmzbfrnk.html

[G07] 调用父类方法
来源：http://hz.havefunace.top/gtyjujaagf.html

Py:   super().greet()
来源：http://hz.aibaodan.cn/gtmrafbcyo.html

PHP:  parent::greet();
来源：http://hz.guannengcc.top/gtvpfnevsc.html

JS:   super.greet();
来源：http://hz.jinqigfzy.top/gtohmmjgbd.html

TS:   super.greet();
来源：http://hz.shangyingyoupin.top/gtbjbwygnn.html

Java: super.greet();
来源：http://hz.xuetiantiany.cn/gtfillzmgc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.52xcode.cn/gtanuxngts.html

Ruby: super
来源：http://hz.guowangkeji.top/gtgylqgxhh.html

C#:   base.Greet();
来源：http://hz.yueranfly.top/gtfzecavha.html

[G08] 静态方法与属性
来源：http://hz.bjfxy.top/gtvbxcxshl.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.sufxvd.cn/gttyaocftr.html

PHP:  public static function f() {}
来源：http://hz.ydjk.org.cn/gtxbhqtcgc.html

JS:   static f() {}
来源：http://hz.daxiang520.top/gtlsrhwhvs.html

TS:   static f(): void {}
来源：http://hz.wangdashe.top/gtasuwtbcf.html

Java: static void f() {}
来源：http://hz.zhaomingkeji.xyz/gtnqiznkns.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.zhixingplan.top/gtmxjooiku.html

Ruby: def self.f; end
来源：http://hz.kuanghao11.cn/gtyczroiho.html

C#:   public static void F() {}
来源：http://hz.haohaochexian.top/gtzlovqzuw.html

[G09] 接口 / 抽象类
来源：http://hz.cheryme.top/gtviyzavbi.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yonumen.top/gtjpyysmqt.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jinqigfzy.top/gtcdtjzdfb.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.yj202588.top/gtgnwwvctj.html

TS:   interface Shape { area(): number; }
来源：http://hz.ybcxt.top/gtpsjbpuwr.html

Java: interface Shape { double area(); }
来源：http://hz.aizwys.cn/gtrxnkbqee.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.aizwys.cn/gtrxhcfaoz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.zhixingplan.top/gtuwodjhbh.html

C#:   interface IShape { double Area(); }
来源：http://hz.yueranfly.top/gthahxwrgu.html

[G10] 访问控制
来源：http://hz.wangshuangyany.cn/gtqcziwhyh.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.daria6918.cn/gtxyzgbrxf.html

PHP:  public / protected / private
来源：http://hz.mhx1999.top/gtcilqrmxf.html

JS:   #private 字段；其余公开
来源：http://hz.chenzaomai.com/gtlvarbgtr.html

TS:   public / protected / private
来源：http://hz.yvedp.cn/gttqccmrue.html

Java: public / protected / private / 默认包级
来源：http://hz.nanxuanxn.top/gtnfntkors.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.chenlongwang.top/gtsftbropb.html

Ruby: public / protected / private
来源：http://hz.nanxinkj.top/gtblsmttsm.html

C#:   public / protected / private / internal
来源：http://hz.hnqzz.top/gtrkqqtsyu.html

[G11] getter / setter
来源：http://hz.vqdsnc.cn/gtixjsgbbj.html

Py:   @property 与 @x.setter
来源：http://hz.ydjk.org.cn/gtghxciukk.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.sufxvd.cn/gtaxsrmaxr.html


<!-- 参考信息 -->