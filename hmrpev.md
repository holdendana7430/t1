代发 wailian999

Py:   for ch in s: print(ch)
来源：http://hz.vqdsnc.cn/gtzzxgefco.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.xziqi.cn/gtelxvrjnj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.guowangkeji.top/gtaubepvpl.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.hnxiangtu.top/gtdwbabwbb.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.ybcxt.top/gtmjrdepph.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.haohaochexian.top/gtnxacjnhp.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.yuxming.cn/gtzbwqlmko.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.nanxinkj.top/gtlybbxkzd.html

[E14] URL 编码与 Base64
来源：http://hz.yj202588.top/gtzkfbxidg.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.shangyingyoupin.top/gtuveyvefc.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.yanxiufei.cn/gtbmwzfwys.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.ywan-chungtsiang.top/gtvjjrgidh.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.jinqigfzy.top/gtfefhlaup.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.cdnleiting.top/gtemxkajah.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.dashuyun.cn/gtuynncvkd.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.zdqjudy.top/gtonoqdgcz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.birdmap.top/gtontlamvn.html

[E15] HTML 转义 / 反转义
来源：http://hz.sxryk.cn/gtuzbrbdhb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.jinyuanbaomall.cn/gtcftxdcnm.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.tian-w.cn/gtrunjgcnm.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.sweek.top/gtbviwrmth.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.chenlongwang.top/gtdlsutsjz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.snrcjt.cn/gtbxmsdkgd.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.sweek.top/gtulzugvaa.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.xinyue.icu/gtdujazuyf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.dashuyun.cn/gtqiywidbb.html

[E16] 数字千分位
来源：http://hz.jqgfzy.top/gtbsrwaxob.html

Py:   f"{1234567:,}"
来源：http://hz.yj202588.top/gtqceejeuc.html

PHP:  number_format(1234567);
来源：http://hz.jqgufenzy.top/gtqvgekitj.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.birdmap.top/gtqfgwdeer.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.ivvv.top/gtkabumvvh.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.jinqigfzy.top/gttykvlywu.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.zhoulong.xyz/gtddlepicf.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.daxiang520.top/gtzhqowhtg.html

C#:   1234567.ToString("N0")
来源：http://hz.yangfankeji.com/gthvsvekuw.html

[E17] 首字母大写
来源：http://hz.ydzc1.top/gthfruipan.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.xuetiantiany.cn/gttbxzhzgu.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.wangdashe.top/gtcxmjqidu.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.hnxiangtu.top/gtucxbdrhc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ppjwa.cn/gtbbrjcudz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.guowangkeji.top/gtzzcwjwpn.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.sufxvd.cn/gtjwtcqfvv.html

Ruby: s.capitalize
来源：http://hz.nwbrower.top/gteausrpqt.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.ydzc1.top/gtkwhufhkr.html

[E18] 模板占位符替换
来源：http://hz.daxiang520.top/gtpndtgnjy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.yanxiufei.cn/gtnrxjmgge.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.yvedp.cn/gtsbqbogsg.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.hongshengwenyu.top/gtxmhnleuu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.fengsongda.top/gtfuvmatzh.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.svipenyu.cn/gtvmkjmjby.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.zhijiandao.cn/gttmijfjgq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.zhijiandao.cn/gtaacqajhe.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.jinyuanbaomall.cn/gtaeptcklu.html

[E19] 多行文本按行拆分
来源：http://hz.shanyushiyangtech.top/gtuxbonbhy.html

Py:   s.splitlines()
来源：http://hz.yj202588.top/gttohaotne.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.quarkkingdee.top/gthdrbbthb.html

JS:   s.split(/\r?\n/)
来源：http://hz.yj20258888.top/gtftcfbttf.html

TS:   s.split(/\r?\n/)
来源：http://hz.zhengqikj.top/gttfvjggcm.html

Java: s.lines().toList()
来源：http://hz.yangfankeji.com/gtlrvzxqna.html

Go:   strings.Split(s, "\n")
来源：http://hz.gaohongyu789.top/gtrngjflfq.html

Ruby: s.lines
来源：http://hz.jyoumei.cn/gtzwulmuyo.html

C#:   s.Split('\n')
来源：http://hz.shuidangran.top/gtsphaexdb.html

[E20] 判断字符串是否为空
来源：http://hz.gotoacloud.top/gtiopqggzo.html

Py:   if not s:
来源：http://hz.chenjidiqi.icu/gtlilzjads.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.gaohongyu789.top/gtcfurgjsz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.ywan-chungtsiang.top/gtwmxvapvr.html

TS:   if (s === "") {}
来源：http://hz.nanxuanxn.top/gtlkvtvoww.html

Java: if (s.isEmpty()) {}
来源：http://hz.chenjidiqi.icu/gtawsfwche.html

Go:   if s == "" {}
来源：http://hz.cheryme.top/gtglirkzrw.html

Ruby: if s.empty?
来源：http://hz.yuanzhike.top/gtaazddzml.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.chenjidiqi.icu/gtcosbjjtd.html

[E21] 超长截断加省略号
来源：http://hz.zhaomingkeji.xyz/gtvczhoato.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.sysykeji.top/gtbrojgweb.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.ehwqpu.com/gtgfordbcd.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yanxiufei.cn/gtmgfodnfy.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.pycfn.com/gtbexldsvi.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.daria6918.cn/gtgwvvjyqk.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.yongpay.top/gttdisioga.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.andypj.xyz/gtnhldkayh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.cashguo.top/gtbrddbdyi.html

[E22] 字节长度与字符长度
来源：http://hz.jqgufenzy.top/gtuaxwzgpk.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.gzhubu.top/gtnmvyqbih.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.birdmap.top/gtakodznch.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.316326.xyz/gtyvapdswd.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.guowangkeji.top/gtfkrfnztc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jinqigufen.top/gtzrwklqnd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.jqgfzy.top/gtgvxbgmsl.html

Ruby: s.bytesize;  s.length
来源：http://hz.xuetiantiany.cn/gtipufqdgu.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.quarkkingdee.top/gtafynqoiw.html

================================================================================
来源：http://hz.yongpay.top/gtflhsaciu.html

F. 文件与目录
来源：http://hz.xylfe.cn/gttvwoalau.html

================================================================================
来源：http://hz.zycfv.cn/gtrhamzkxh.html

[F01] 读取整个文件
来源：http://hz.quarkkingdee.top/gtrxrvccup.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.daxiang520.top/gtpnfdzqtc.html

PHP:  file_get_contents("a.txt");
来源：http://hz.meibo888.top/gtkrqttzfd.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.guannengcc.top/gttbmuzqkz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.shanyushiyangkeji.top/gtoxeslfxa.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.hysaishi.cn/gteahanhpi.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.cashguo.top/gtuxobcyyq.html

Ruby: File.read("a.txt")
来源：http://hz.hammf.cn/gtbukvcdbf.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.fzhhl.top/gtlpcvfzap.html

[F02] 逐行读取文件
来源：http://hz.dashuyun.cn/gtkbjsegef.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.jiagoushi.top/gtixcqsqol.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.sweek.top/gtxtljnacl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.c1oappe.top/gtlsdygepz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.smart0.xyz/gtqzlexviz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.yongpay.top/gtblwspmqh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.52xcode.cn/gtgngystqt.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.tanke756.top/gtsqzrbglx.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.chenjidiqi.icu/gtgivgauzd.html

[F03] 写入文件（覆盖）
来源：http://hz.gotoacloud.top/gtqjbsfuis.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.aizwys.cn/gtimwiglmz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.yvedp.cn/gtrfmvapjd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.xuanzx.com/gtoltnxjdp.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yj202588.top/gthlcxzpbe.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.hnqzz.top/gtevidxjpi.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.yonumen.top/gtxfrreiba.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.wangshuangyany.cn/gttllpcqyt.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.nwbrower.top/gtqdumrlsj.html

[F04] 追加写入文件
来源：http://hz.zhiwuduotai.top/gtaslholay.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.ydjk.org.cn/gtggoxekgs.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.bjfxy.top/gtarfmrtyt.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.xuanzx.com/gtvsajsysf.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.fzhhl.top/gtxbkajkwb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.cheryme.top/gtmtoxlzre.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.yvedp.cn/gtfqfrsrpu.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.xuetiantiany.cn/gtdctpkgpc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.vqdsnc.cn/gtpxibaejs.html

[F05] 判断文件或目录是否存在
来源：http://hz.xingfuxueyuan.xyz/gtjytxrdzv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.daxiang520.top/gtdbqflsmc.html

PHP:  file_exists("a.txt");
来源：http://hz.havefunace.top/gtlrlcspdx.html

JS:   fs.existsSync("a.txt")
来源：http://hz.snrcjt.cn/gtibjlfghx.html

TS:   fs.existsSync("a.txt")
来源：http://hz.xuetiantiany.cn/gtnjakcgtq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.haohaochexian.top/gtupjdcqyz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.nanxinkj.top/gtcotqhdsk.html

Ruby: File.exist?("a.txt")
来源：http://hz.tian-w.cn/gtspaeksjm.html

C#:   File.Exists("a.txt")
来源：http://hz.shanyushiyangtech.top/gtkjnjuqow.html

[F06] 删除文件
来源：http://hz.smart0.xyz/gtfjxsyees.html

Py:   os.remove("a.txt")
来源：http://hz.zhengqikj.top/gtrzqxyajx.html

PHP:  unlink("a.txt");
来源：http://hz.ywan-chungtsiang.top/gtarmslnmt.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yangfankeji.com/gtnphfrxrh.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.quarkkingdee.top/gtggqkvbrq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.cheryme.top/gtbxvwxdwv.html

Go:   os.Remove("a.txt")
来源：http://hz.jianghu66.top/gtuptxiake.html

Ruby: File.delete("a.txt")
来源：http://hz.andypj.xyz/gtrbwxgqzb.html

C#:   File.Delete("a.txt");
来源：http://hz.shuidangran.top/gtftdhwbat.html

[F07] 创建目录（含多级）
来源：http://hz.hnxiangtu.top/gtntiusidj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.jinqigufen.top/gtqwwjkznr.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.cucudq.cn/gttfnvepdh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.cqqwz.cn/gtrsiauxus.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ehwqpu.com/gtqmqoifeu.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.tianlin.xyz/gtawlwxdzb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.nanxinkj.top/gtietwecmi.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.yanxiufei.cn/gthwneknjz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.pycfn.com/gtsomkjoqy.html

[F08] 遍历目录
来源：http://hz.feifeiyinyue.top/gtjyzbhwpa.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.shzxlz.cn/gtmbwclacg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.chenlongwang.top/gtrzgowdry.html

JS:   fs.readdirSync("dir")
来源：http://hz.sufxvd.cn/gtuynjyugt.html

TS:   fs.readdirSync("dir")
来源：http://hz.zdqjudy.top/gthlevjgjg.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.iojbl.cn/gtjzzxclsl.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.zhixingplan.top/gtehdfvnes.html

Ruby: Dir.children("dir")
来源：http://hz.hnqzz.top/gtrwrkbrrh.html

C#:   Directory.GetFiles("dir")
来源：http://hz.jqgufenzy.top/gtqyllgniy.html

[F09] 获取文件大小
来源：http://hz.jianghu66.top/gtotxkiyjg.html

Py:   os.path.getsize("a.txt")
来源：http://hz.xuanzx.com/gthgcxveaq.html

PHP:  filesize("a.txt");
来源：http://hz.hnxiangtu.top/gtcxavqhqa.html

JS:   fs.statSync("a.txt").size
来源：http://hz.c1oappe.top/gtqtqinuzc.html

TS:   fs.statSync("a.txt").size
来源：http://hz.vqdsnc.cn/gtclxlolfw.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.ydjk.org.cn/gtxhjxlhdd.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.fzhhl.top/gtldobondg.html

Ruby: File.size("a.txt")
来源：http://hz.yj20258.top/gtfwekjfeg.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yongpay.top/gtldzhkjcs.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.jyoumei.cn/gthlgxvtxb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.shuidangran.top/gtzkzffufv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.yj20258888.top/gtlfmntekc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.cqqwz.cn/gtqujnyajn.html

TS:   path.extname("a.txt")
来源：http://hz.jiagoushi.top/gtsmtshzwu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.hywenlv.cn/gtnjzeqdcx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.sweek.top/gtnkndkbtu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.shangyingyoupin.top/gthelgqxgl.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.gotoacloud.top/gtrpgklkod.html

[F11] 复制与移动文件
来源：http://hz.tianlin.xyz/gtvgwhxcfa.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.zycfv.cn/gtdxphrwya.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.jinqigfzy.top/gtfsnxelkx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.dianchejie.cn/gtjbkoxked.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jinqigfzy.top/gtjtspptss.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.ydjk.org.cn/gtivtxsole.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.zhongyouzk.top/gtwevwcgzf.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.aizwys.cn/gteuwdcyaw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.yongpay.top/gtyyojazfo.html

[F12] CSV 读写
来源：http://hz.yanxiufei.cn/gtrtabmxwj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.svipenyu.cn/gtcwjjrosc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.tian-w.cn/gtuwssgsvy.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.hnxiangtu.top/gtuwfhdhep.html

TS:   // 同上
来源：http://hz.haohaochexian.top/gtwzycpetk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.hysaishi.cn/gtdxlnsuil.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.jinyuanbaomall.cn/gtaynpsfid.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.chenzaomai.com/gtchrifrxf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.hysaishi.cn/gtsolnexkc.html

================================================================================
来源：http://hz.vqdsnc.cn/gtunnyojft.html

G. 面向对象
来源：http://hz.chenlongwang.top/gtttjgmvzs.html

================================================================================
来源：http://hz.yonumen.top/gtuxmbnoqt.html

[G01] 定义类
来源：http://hz.ydjk.org.cn/gtzjnlnaqk.html

Py:   class User: pass
来源：http://hz.shanyushiyangkeji.top/gtxtljlonk.html

PHP:  class User {}
来源：http://hz.sxryk.cn/gtgjkcxzea.html

JS:   class User {}
来源：http://hz.zycfv.cn/gttxkzkfpd.html

TS:   class User { name: string = ""; }
来源：http://hz.xinyue.icu/gtflblzpzu.html

Java: class User {}
来源：http://hz.birdmap.top/gtpfabbwbt.html

Go:   type User struct { Name string }
来源：http://hz.zhijiandao.cn/gtzqhngdyo.html

Ruby: class User; end
来源：http://hz.yuanzhike.top/gtybupqpnz.html

C#:   class User {}
来源：http://hz.yj20258.top/gtteksiike.html

[G02] 构造函数
来源：http://hz.jqgfzy.top/gtxyvjcbod.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yuanzhike.top/gthxzwddhp.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.hongshengwenyu.top/gtfeqkamkk.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.jianghu66.top/gtqekgftdh.html

TS:   constructor(public name: string) {}
来源：http://hz.redwolf501.top/gtqcoeoegv.html

Java: User(String name) { this.name = name; }
来源：http://hz.316326.xyz/gtbcnspwkn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.316326.xyz/gtauuprhwb.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.jianghu66.top/gtbjvsllrh.html

C#:   public User(string name) { Name = name; }
来源：http://hz.shanyushiyangkeji.top/gtynvwxcvc.html

[G03] 实例属性
来源：http://hz.feifeiyinyue.top/gtqgnexioz.html

Py:   self.name = "x"
来源：http://hz.yongpay.top/gtongragyr.html

PHP:  public string $name = "x";
来源：http://hz.hongshengwenyu.top/gtoqugfyhw.html

JS:   this.name = "x";
来源：http://hz.guannengcc.top/gthtnlmayr.html

TS:   name: string = "x";
来源：http://hz.zycfv.cn/gtcstdqrvb.html

Java: private String name;
来源：http://hz.havefunace.top/gtfzlroxht.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.xuanzx.com/gtldfcqzwe.html

Ruby: @name = "x"
来源：http://hz.316326.xyz/gtwosgbvsi.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yueranfly.top/gtenapoowq.html

[G04] 定义方法
来源：http://hz.smart0.xyz/gtorgxyvtw.html

Py:   def greet(self): return self.name
来源：http://hz.ivvv.top/gtoihmchbo.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.dashuyun.cn/gtiyorvzjp.html

JS:   greet() { return this.name; }
来源：http://hz.shanyushiyangtech.top/gtikwceubf.html

TS:   greet(): string { return this.name; }
来源：http://hz.daxiang520.top/gtaucxillx.html

Java: String greet() { return name; }
来源：http://hz.nanxinkj.top/gtdfnlbtil.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jinghuilouyu.cn/gtrpldagkx.html

Ruby: def greet; @name; end
来源：http://hz.dashuyun.cn/gtlbwwjyyx.html

C#:   public string Greet() => Name;
来源：http://hz.guowangkeji.top/gtwaxhjqxe.html

[G05] 继承
来源：http://hz.tian-w.cn/gtirnzzvri.html

Py:   class Admin(User): pass
来源：http://hz.aibaodan.cn/gtebceitso.html

PHP:  class Admin extends User {}
来源：http://hz.hongshengwenyu.top/gtowmjscrm.html

JS:   class Admin extends User {}
来源：http://hz.yongpay.top/gtgoprjqus.html

TS:   class Admin extends User {}
来源：http://hz.gogol.net.cn/gtxvetdrcw.html

Java: class Admin extends User {}
来源：http://hz.shuidangran.top/gtyyddcrkj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.cdnleiting.top/gtcyqdutta.html

Ruby: class Admin < User; end
来源：http://hz.ydjk.org.cn/gtyqfkuqow.html

C#:   class Admin : User {}
来源：http://hz.zhoulong.xyz/gtkshmqubw.html

[G06] 重写方法
来源：http://hz.ydzc1.top/gtkbtgxiyx.html

Py:   def greet(self): return "admin"
来源：http://hz.yueranfly.top/gtdqvcgnpq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.tanke756.top/gtxyjpbzis.html

JS:   greet() { return "admin"; }
来源：http://hz.ivvv.top/gtmcvbrngu.html

TS:   greet(): string { return "admin"; }
来源：http://hz.dianchejie.cn/gtkqexueid.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jqgfzy.top/gtxfbwttkm.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.chenjidiqi.icu/gtfeguumyi.html

Ruby: def greet; "admin"; end
来源：http://hz.sxryk.cn/gtsenhrdsb.html

C#:   public override string Greet() => "admin";
来源：http://hz.guannengcc.top/gtjhwwgvjc.html

[G07] 调用父类方法
来源：http://hz.cqqwz.cn/gtgztgfyqt.html

Py:   super().greet()
来源：http://hz.nanxinkj.top/gtbayrjgme.html

PHP:  parent::greet();
来源：http://hz.havefunace.top/gtrbjrwbrf.html

JS:   super.greet();
来源：http://hz.cashguo.top/gtfqnqlpbz.html

TS:   super.greet();
来源：http://hz.yj20258.top/gtjaswqxlm.html

Java: super.greet();
来源：http://hz.jinqigfzy.top/gtrdyelgrl.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.chenlongwang.top/gtqtjjrbil.html

Ruby: super
来源：http://hz.chenzaomai.com/gttqbsaxni.html

C#:   base.Greet();
来源：http://hz.pycfn.com/gtuxmfdxwa.html

[G08] 静态方法与属性
来源：http://hz.yongpay.top/gtqxaxzjer.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.shangyingyoupin.top/gtrdnlinez.html

PHP:  public static function f() {}
来源：http://hz.daxiang520.top/gtmrgpbdsw.html

JS:   static f() {}
来源：http://hz.nanxuanxn.top/gtvmzxtrcz.html

TS:   static f(): void {}
来源：http://hz.yvedp.cn/gtuxzkngse.html

Java: static void f() {}
来源：http://hz.zhixingplan.top/gtmqdetuoh.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.hysaishi.cn/gtjkrichfo.html

Ruby: def self.f; end
来源：http://hz.shanyushiyangkeji.top/gtdgjyqljz.html

C#:   public static void F() {}
来源：http://hz.hnqzz.top/gtwqezehzh.html

[G09] 接口 / 抽象类
来源：http://hz.jinghuilouyu.cn/gtzafmmawh.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.0kj1m.cn/gtkghddnmz.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.hfpthk.cn/gtpaanneei.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.zhijiandao.cn/gtcugpvdie.html

TS:   interface Shape { area(): number; }
来源：http://hz.shanyushiyangtech.top/gtgsfcijyy.html

Java: interface Shape { double area(); }
来源：http://hz.zhengqikj.top/gthknmaeky.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.tian-w.cn/gtqnissiqg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.zhijiandao.cn/gtdyltblcl.html

C#:   interface IShape { double Area(); }
来源：http://hz.xinyue.icu/gtjporebbp.html

[G10] 访问控制
来源：http://hz.aibaodan.cn/gteasxhoki.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.hfpthk.cn/gtaryqxxdj.html

PHP:  public / protected / private
来源：http://hz.tianlin.xyz/gtyhtnrzgp.html

JS:   #private 字段；其余公开
来源：http://hz.nanxinkj.top/gtwqtnhoij.html

TS:   public / protected / private
来源：http://hz.havefunace.top/gtxnvqipwy.html

Java: public / protected / private / 默认包级
来源：http://hz.yj20258.top/gtefxsrbry.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.aizwys.cn/gtyuxielqn.html

Ruby: public / protected / private
来源：http://hz.daria6918.cn/gttdtafpau.html

C#:   public / protected / private / internal
来源：http://hz.yangfankeji.com/gtdjtbgqgk.html

[G11] getter / setter
来源：http://hz.hysaishi.cn/gtszbpnycy.html

Py:   @property 与 @x.setter
来源：http://hz.jianghu66.top/gtvgrclink.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.shuidangran.top/gthzinablu.html

JS:   get name() { return this._name; }
来源：http://hz.xuanzx.com/gtvvjvhibj.html

TS:   get name(): string { return this._name; }
来源：http://hz.gzhubu.top/gtxkizkcmh.html

Java: public String getName() { return name; }
来源：http://hz.redwolf501.top/gtuwiwrvft.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.daria6918.cn/gtdfmulifg.html


<!-- 参考信息 -->