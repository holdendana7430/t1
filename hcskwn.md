代发 wailian999

Go:   strings.Count(s, "a")
来源：http://hz.yanxiufei.cn/gtavzxmoha.html

Ruby: s.count("a")
来源：http://hz.andypj.xyz/gtbhgbhfll.html

C#:   s.Count(c => c == 'a')
来源：http://hz.gotoacloud.top/gteaijkgcl.html

[E13] 逐字符遍历
来源：http://hz.feifeiyinyue.top/gtmgskkqqr.html

Py:   for ch in s: print(ch)
来源：http://hz.yj202588.top/gtfsjberzz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.hfpthk.cn/gtdkclzzio.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.hammf.cn/gtaplzvfxr.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.gogol.net.cn/gtwxolkpog.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.yvedp.cn/gttyzxponu.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.yj20258.top/gtyzmjjfoa.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.yongpay.top/gtimpvezoa.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.xinyue.icu/gtnbslcjib.html

[E14] URL 编码与 Base64
来源：http://hz.hnxiangtu.top/gtizdluzhc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.feifeiyinyue.top/gtltbgpfnv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.tanke756.top/gtwosmngxz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.meibo888.top/gtqezixmxg.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.xingfuxueyuan.xyz/gthtkxchpb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.tianlin.xyz/gtkxdgqhqu.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.nanxinkj.top/gtjvyuijqk.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.nwbrower.top/gtewpwjlce.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.gaohongyu789.top/gtuduklmlv.html

[E15] HTML 转义 / 反转义
来源：http://hz.xingfuxueyuan.xyz/gtftlbquja.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.zycfv.cn/gthaltmqfk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.zhixingplan.top/gtddfodcwg.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.hnxiangtu.top/gtissofxza.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.jinqigufen.top/gtfcrhntjh.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.xziqi.cn/gtcbygpbxs.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.meibo888.top/gtqboffzpm.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.ybcxt.top/gtqpxdxamw.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.cdnleiting.top/gtvorodvoc.html

[E16] 数字千分位
来源：http://hz.andypj.xyz/gttchdrkfd.html

Py:   f"{1234567:,}"
来源：http://hz.mhx1999.top/gtbklfcofe.html

PHP:  number_format(1234567);
来源：http://hz.xuetiantiany.cn/gtpsjcvtwi.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.ppjwa.cn/gtpochddcq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.feifeiyinyue.top/gtcqmpgdsw.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.tian-w.cn/gtjizabflo.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.meibo888.top/gtvqjwfrdk.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.jinyuanbaomall.cn/gtgjvvcfrh.html

C#:   1234567.ToString("N0")
来源：http://hz.zdqjudy.top/gtzfbdettt.html

[E17] 首字母大写
来源：http://hz.yj20258.top/gtiqwovsia.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.sxryk.cn/gtvvfhbykr.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.kuanghao11.cn/gtwivgmrly.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.0kj1m.cn/gtmkclnrys.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jqgfzy.top/gttuqliczc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.gogol.net.cn/gttrianczy.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.nanxuanxn.top/gtzoabxlck.html

Ruby: s.capitalize
来源：http://hz.zycfv.cn/gtcxsckqzn.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.andypj.xyz/gtmlvfwama.html

[E18] 模板占位符替换
来源：http://hz.zhixingplan.top/gtgpbcohix.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.ybcxt.top/gtiibqwuvv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.cucudq.cn/gtitbtwnok.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.chenlongwang.top/gtzagompwa.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.snrcjt.cn/gtpvscthik.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.andypj.xyz/gtsszxchgh.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.sysykeji.top/gtdtedcqnw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.xingfuxueyuan.xyz/gtosfabohq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.xuanzx.com/gtkrufoehw.html

[E19] 多行文本按行拆分
来源：http://hz.hywenlv.cn/gtiaudqbro.html

Py:   s.splitlines()
来源：http://hz.jyoumei.cn/gtyvdznjfc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.redwolf501.top/gtxrlqtvng.html

JS:   s.split(/\r?\n/)
来源：http://hz.sufxvd.cn/gtaitbcypf.html

TS:   s.split(/\r?\n/)
来源：http://hz.yongpay.top/gtdiwdifup.html

Java: s.lines().toList()
来源：http://hz.0kj1m.cn/gtysnjczjy.html

Go:   strings.Split(s, "\n")
来源：http://hz.nwbrower.top/gtudvzhips.html

Ruby: s.lines
来源：http://hz.zdqjudy.top/gtvxqjzjov.html

C#:   s.Split('\n')
来源：http://hz.iojbl.cn/gtxuhtkuty.html

[E20] 判断字符串是否为空
来源：http://hz.jlsjyb.cn/gtfdwsxtap.html

Py:   if not s:
来源：http://hz.yanxiufei.cn/gtigqeeifi.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.aizwys.cn/gtemzqidvp.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.haohaochexian.top/gtzmkmwoas.html

TS:   if (s === "") {}
来源：http://hz.pengpengdd.cyou/gtpbznimlj.html

Java: if (s.isEmpty()) {}
来源：http://hz.52xcode.cn/gtvzbtyehh.html

Go:   if s == "" {}
来源：http://hz.jyoumei.cn/gtjqatktgt.html

Ruby: if s.empty?
来源：http://hz.cdnleiting.top/gttzgjkzcf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.ydzc1.top/gtnflnnlty.html

[E21] 超长截断加省略号
来源：http://hz.jiagoushi.top/gtwzmizabw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.hongshengwenyu.top/gtpvbwgald.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.nanxuanxn.top/gtqabtmblj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.pycfn.com/gtrkekokol.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jinghuilouyu.cn/gtqteihrle.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.xziqi.cn/gtgzhbflpe.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.hnqzz.top/gtdojqgmhd.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.jinqigfzy.top/gtqumdvqfg.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.haohaochexian.top/gtcuckgjmx.html

[E22] 字节长度与字符长度
来源：http://hz.316326.xyz/gtvyzimxuk.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.xuetiantiany.cn/gtgnnjfcui.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ppjwa.cn/gtltxdlmpi.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.meibo888.top/gtafdrcdrw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.birdmap.top/gtzlfjqwvh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.iojbl.cn/gtgufjgabf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.jinyuanbaomall.cn/gtzwvsfuxf.html

Ruby: s.bytesize;  s.length
来源：http://hz.ehwqpu.com/gtizzjkafh.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.yanxiufei.cn/gtbsoaizxc.html

================================================================================
来源：http://hz.aibaodan.cn/gticfvzvzu.html

F. 文件与目录
来源：http://hz.jyoumei.cn/gtspdjugtp.html

================================================================================
来源：http://hz.shuidangran.top/gtumnhdxjf.html

[F01] 读取整个文件
来源：http://hz.cdnleiting.top/gtwokfnutb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.aizwys.cn/gtvcdqisfp.html

PHP:  file_get_contents("a.txt");
来源：http://hz.nwbrower.top/gtlcnobddp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.kuanghao11.cn/gtghmusjrb.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.daxiang520.top/gthkbnizzn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.cucudq.cn/gtwvolirtk.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zhijiandao.cn/gtduaefosb.html

Ruby: File.read("a.txt")
来源：http://hz.daria6918.cn/gtvkiukkns.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.52xcode.cn/gtfavkkpyq.html

[F02] 逐行读取文件
来源：http://hz.smart0.xyz/gtmnqqjbec.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.nanxinkj.top/gtazsojsim.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.gaohongyu789.top/gtplxasmuz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.sysykeji.top/gtlxtcloxz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jqgfzy.top/gtkhlriygr.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.zdqjudy.top/gtlyblexgb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.jqgufenzy.top/gtswbphxbf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.jianghu66.top/gtthnuzwvf.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.hnqzz.top/gtpypiuull.html

[F03] 写入文件（覆盖）
来源：http://hz.zhoulong.xyz/gtdwwatvla.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.gogol.net.cn/gtkplpoikf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.jinqigufen.top/gtdqggxkef.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.xuetiantiany.cn/gtpyzuekhz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.sysykeji.top/gtkaylwrdx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.jianghu66.top/gtlftslzhq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.nanxuanxn.top/gtrytwhmzh.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.tianlin.xyz/gtknjqculw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.fzhhl.top/gtvjighmcl.html

[F04] 追加写入文件
来源：http://hz.yvedp.cn/gtngbmbvfc.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.tianlin.xyz/gtxrhvingv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.shanyushiyangtech.top/gtaxalgbtb.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jinghuilouyu.cn/gtypcckssj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.redwolf501.top/gtwiybhrcd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.dianchejie.cn/gthivtnzer.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.fengsongda.top/gtjcblzlzf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.ywan-chungtsiang.top/gtkaozohou.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.feifeiyinyue.top/gtsstlmfcj.html

[F05] 判断文件或目录是否存在
来源：http://hz.chenlongwang.top/gtmfxuwbwv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.snrcjt.cn/gtvdppdrmt.html

PHP:  file_exists("a.txt");
来源：http://hz.redwolf501.top/gtpwishrtn.html

JS:   fs.existsSync("a.txt")
来源：http://hz.birdmap.top/gtmtuuonze.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zhaomingkeji.xyz/gtrulyppyl.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.bjfxy.top/gtdzrazxly.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.zycfv.cn/gtvppfjyrz.html

Ruby: File.exist?("a.txt")
来源：http://hz.ydzc1.top/gtymwirtqy.html

C#:   File.Exists("a.txt")
来源：http://hz.feifeiyinyue.top/gtuugdxwwq.html

[F06] 删除文件
来源：http://hz.yuanzhike.top/gtsmqicjaw.html

Py:   os.remove("a.txt")
来源：http://hz.shanyushiyangtech.top/gtlwfcwxxl.html

PHP:  unlink("a.txt");
来源：http://hz.hfpthk.cn/gtpkfkxrbc.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.316326.xyz/gtlkgrvzti.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.jinyuanbaomall.cn/gtyadrbeek.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.smart0.xyz/gtzzrstftt.html

Go:   os.Remove("a.txt")
来源：http://hz.zhaomingkeji.xyz/gtwtbnudkq.html

Ruby: File.delete("a.txt")
来源：http://hz.cashguo.top/gtvnplyfws.html

C#:   File.Delete("a.txt");
来源：http://hz.haohaochexian.top/gtlcdwpuge.html

[F07] 创建目录（含多级）
来源：http://hz.jinqigufen.top/gtjfivkuhz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.hnqzz.top/gtleziuias.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.snrcjt.cn/gtjbccknwp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ywan-chungtsiang.top/gtzoqxarqg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jianghu66.top/gtwjmzolcf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.ydzc1.top/gtrydzspzv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.daxiang520.top/gtcvmrtlds.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.svipenyu.cn/gttlromvzb.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.hywenlv.cn/gtfzmzvvvx.html

[F08] 遍历目录
来源：http://hz.yj20258.top/gteeiasmsx.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.guannengcc.top/gtygpghpsx.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.chenjidiqi.icu/gtgjhmgkgk.html

JS:   fs.readdirSync("dir")
来源：http://hz.jinqigufen.top/gtavvopezm.html

TS:   fs.readdirSync("dir")
来源：http://hz.meibo888.top/gtdziktfsi.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.guowangkeji.top/gtbcjsufcj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.andypj.xyz/gtboepsfrm.html

Ruby: Dir.children("dir")
来源：http://hz.xziqi.cn/gtiiyreofd.html

C#:   Directory.GetFiles("dir")
来源：http://hz.hnqzz.top/gtvyzzboet.html

[F09] 获取文件大小
来源：http://hz.yangfankeji.com/gthdckhgqj.html

Py:   os.path.getsize("a.txt")
来源：http://hz.316326.xyz/gtjttuvhhc.html

PHP:  filesize("a.txt");
来源：http://hz.dashuyun.cn/gtoewdztvv.html

JS:   fs.statSync("a.txt").size
来源：http://hz.shzxlz.cn/gtxkqbjepy.html

TS:   fs.statSync("a.txt").size
来源：http://hz.xziqi.cn/gtfurghdju.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.cashguo.top/gtpjigboiu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.jiagoushi.top/gtxonabpqa.html

Ruby: File.size("a.txt")
来源：http://hz.ivvv.top/gtqtmbscbt.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.cheryme.top/gtrytlvfzx.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yvedp.cn/gtnzsptaai.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.quarkkingdee.top/gtufgtbesc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.mhx1999.top/gtihkygjmd.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.zhijiandao.cn/gtbwxewbab.html

TS:   path.extname("a.txt")
来源：http://hz.hnxiangtu.top/gtdjcszqva.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.shuidangran.top/gthimvbjoq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.havefunace.top/gtdxupxqml.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jinghuilouyu.cn/gtusqendkl.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.shangyingyoupin.top/gtooaoqjlt.html

[F11] 复制与移动文件
来源：http://hz.xziqi.cn/gtysyqsmpf.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.52xcode.cn/gtobklotjs.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.fzhhl.top/gtxduexrhc.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.feifeiyinyue.top/gtqobtrojy.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jinyuanbaomall.cn/gtldqffwmg.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.hongshengwenyu.top/gtkorfuyjr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.tanke756.top/gtestalmuw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.chenlongwang.top/gtvfjwxpxc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.fzhhl.top/gtxqrmcwml.html

[F12] CSV 读写
来源：http://hz.zhijiandao.cn/gtijupwlgs.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.ydzc1.top/gtxiqkiojg.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.c1oappe.top/gteyviegjn.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.shanyushiyangkeji.top/gtqwvjacbp.html

TS:   // 同上
来源：http://hz.xylfe.cn/gtpvcuwhep.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.yanxiufei.cn/gtdxmqtxew.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.haohaochexian.top/gttqpsjdqo.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.shanyushiyangkeji.top/gtaxwstdvk.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.hongshengwenyu.top/gtfvazbwkj.html

================================================================================
来源：http://hz.vqdsnc.cn/gtmlpyelcl.html

G. 面向对象
来源：http://hz.pycfn.com/gtydmdqfbl.html

================================================================================
来源：http://hz.hammf.cn/gtuwpvfdrs.html

[G01] 定义类
来源：http://hz.shangyingyoupin.top/gtgcyxvtyn.html

Py:   class User: pass
来源：http://hz.jyoumei.cn/gtdpzhgclj.html

PHP:  class User {}
来源：http://hz.nanxinkj.top/gtslfrutcq.html

JS:   class User {}
来源：http://hz.zhiwuduotai.top/gtwmlhaiob.html

TS:   class User { name: string = ""; }
来源：http://hz.snrcjt.cn/gtbfczsowz.html

Java: class User {}
来源：http://hz.gzhubu.top/gtxllmzsnt.html

Go:   type User struct { Name string }
来源：http://hz.hfpthk.cn/gtxuodgmac.html

Ruby: class User; end
来源：http://hz.xuanzx.com/gtjudnpfmw.html

C#:   class User {}
来源：http://hz.mhx1999.top/gtytzmnwwm.html

[G02] 构造函数
来源：http://hz.wangdashe.top/gtkwjfkkqp.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yangfankeji.com/gtxjqnmjlt.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.xziqi.cn/gtgddrliao.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.xuetiantiany.cn/gtrcpdlbod.html

TS:   constructor(public name: string) {}
来源：http://hz.zhiwuduotai.top/gtmplwlovw.html

Java: User(String name) { this.name = name; }
来源：http://hz.zhaomingkeji.xyz/gtrlpxilre.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.sysykeji.top/gteqskwmqn.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.xinyue.icu/gtncsurtdn.html

C#:   public User(string name) { Name = name; }
来源：http://hz.zdqjudy.top/gtkfppipth.html

[G03] 实例属性
来源：http://hz.pycfn.com/gtzalrycqq.html

Py:   self.name = "x"
来源：http://hz.birdmap.top/gtqhybenlk.html

PHP:  public string $name = "x";
来源：http://hz.xuanzx.com/gtrdcjinmk.html

JS:   this.name = "x";
来源：http://hz.nwbrower.top/gtxjlocbvz.html

TS:   name: string = "x";
来源：http://hz.ivvv.top/gtpfjfziei.html

Java: private String name;
来源：http://hz.mhx1999.top/gtxwdixtnh.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.fengsongda.top/gtmlwfuhbh.html

Ruby: @name = "x"
来源：http://hz.yj20258.top/gtmciueawv.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.cdnleiting.top/gtfxnbkeyz.html

[G04] 定义方法
来源：http://hz.52xcode.cn/gtpiaqfqdz.html

Py:   def greet(self): return self.name
来源：http://hz.xinyue.icu/gtmyxzfjvy.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.wangdashe.top/gtwxphtrqf.html

JS:   greet() { return this.name; }
来源：http://hz.jiagoushi.top/gtyluyvmvt.html

TS:   greet(): string { return this.name; }
来源：http://hz.zhijiandao.cn/gtjueoqsxi.html

Java: String greet() { return name; }
来源：http://hz.haohaochexian.top/gthnajpwkt.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.iojbl.cn/gthmnurwij.html

Ruby: def greet; @name; end
来源：http://hz.zhongyouzk.top/gtiawhlqhe.html

C#:   public string Greet() => Name;
来源：http://hz.fzhhl.top/gtvrttyojc.html

[G05] 继承
来源：http://hz.fzhhl.top/gtukxvyoqk.html

Py:   class Admin(User): pass
来源：http://hz.316326.xyz/gtxabzzaip.html

PHP:  class Admin extends User {}
来源：http://hz.yangfankeji.com/gtibqthvvj.html

JS:   class Admin extends User {}
来源：http://hz.sweek.top/gtckdnuqww.html

TS:   class Admin extends User {}
来源：http://hz.cdnleiting.top/gtaepxairc.html

Java: class Admin extends User {}
来源：http://hz.wangdashe.top/gtdcahmalo.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.shanyushiyangkeji.top/gtjpfbeepl.html

Ruby: class Admin < User; end
来源：http://hz.ppjwa.cn/gtrcvdhzez.html

C#:   class Admin : User {}
来源：http://hz.xziqi.cn/gtqtspphbu.html

[G06] 重写方法
来源：http://hz.sufxvd.cn/gtrpdsugxw.html

Py:   def greet(self): return "admin"
来源：http://hz.guowangkeji.top/gtqongbeap.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.tanke756.top/gtywrumpdh.html

JS:   greet() { return "admin"; }
来源：http://hz.daxiang520.top/gtgvkpwwgd.html

TS:   greet(): string { return "admin"; }
来源：http://hz.birdmap.top/gtjprzljdq.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.wangshuangyany.cn/gttlgamtmi.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.svipenyu.cn/gtisrxfpna.html

Ruby: def greet; "admin"; end
来源：http://hz.nanxinkj.top/gtqgpegaej.html

C#:   public override string Greet() => "admin";
来源：http://hz.zhengqikj.top/gttpzmxnra.html

[G07] 调用父类方法
来源：http://hz.meibo888.top/gtonwaobwf.html

Py:   super().greet()
来源：http://hz.52xcode.cn/gtxgtgitkc.html

PHP:  parent::greet();
来源：http://hz.9152youxi.cn/gtoalltabj.html

JS:   super.greet();
来源：http://hz.snrcjt.cn/gtdhobsupx.html

TS:   super.greet();
来源：http://hz.yongpay.top/gtsrpszujf.html

Java: super.greet();
来源：http://hz.jiagoushi.top/gtfxvrqzsz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.zhoulong.xyz/gtquhkjxvj.html

Ruby: super
来源：http://hz.fzhhl.top/gtnqfbqqno.html

C#:   base.Greet();
来源：http://hz.xuetiantiany.cn/gtwiqdxlzq.html

[G08] 静态方法与属性
来源：http://hz.ydzc1.top/gtprtnxsbx.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.yangfankeji.com/gtrcwuutam.html

PHP:  public static function f() {}
来源：http://hz.zhoulong.xyz/gtjybxdfop.html

JS:   static f() {}
来源：http://hz.sufxvd.cn/gtlloezoij.html

TS:   static f(): void {}
来源：http://hz.ybcxt.top/gtuqlbudcf.html

Java: static void f() {}
来源：http://hz.svipenyu.cn/gtcbaqyaeu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.tanke756.top/gtlnqwtysm.html

Ruby: def self.f; end
来源：http://hz.xuetiantiany.cn/gtozsvypzs.html

C#:   public static void F() {}
来源：http://hz.ybcxt.top/gtffipfzmk.html

[G09] 接口 / 抽象类
来源：http://hz.ppjwa.cn/gtyiavicnu.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.ivvv.top/gtnfgiphuv.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.ydjk.org.cn/gtsfdcovdb.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.ydjk.org.cn/gthsedoatt.html

TS:   interface Shape { area(): number; }
来源：http://hz.fzhhl.top/gtjyiyvdpp.html

Java: interface Shape { double area(); }
来源：http://hz.jinqigufen.top/gtybyndhdc.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.cqqwz.cn/gttwhaabbr.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.sweek.top/gtzahrkaql.html

C#:   interface IShape { double Area(); }
来源：http://hz.cucudq.cn/gtenxzbsuo.html

[G10] 访问控制
来源：http://hz.chenzaomai.com/gtbivquuex.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.aizwys.cn/gtdedejtgp.html

PHP:  public / protected / private
来源：http://hz.sufxvd.cn/gtrfpoazct.html

JS:   #private 字段；其余公开
来源：http://hz.zhengqikj.top/gtnkybfzcv.html

TS:   public / protected / private
来源：http://hz.ppjwa.cn/gtcyqpqcvg.html

Java: public / protected / private / 默认包级
来源：http://hz.hfpthk.cn/gtfcqpqmdz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.chenjidiqi.icu/gtbjzufrsw.html

Ruby: public / protected / private
来源：http://hz.tian-w.cn/gtvuscclxu.html

C#:   public / protected / private / internal
来源：http://hz.jinyuanbaomall.cn/gtpbanruar.html

[G11] getter / setter
来源：http://hz.xziqi.cn/gteaduzmvi.html

Py:   @property 与 @x.setter
来源：http://hz.zhongyouzk.top/gtmekcfink.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.ehwqpu.com/gtnubzmlcy.html


<!-- 参考信息 -->