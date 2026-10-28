代发 wailian999

PHP:  substr_count($s, "a");
来源：http://hz.feifeiyinyue.top/gtemegjxep.html

JS:   s.split("a").length - 1
来源：http://hz.yvedp.cn/gtrvgrwtkw.html

TS:   s.split("a").length - 1
来源：http://hz.hnqzz.top/gtcftnkfhv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.ywan-chungtsiang.top/gttesjjhwo.html

Go:   strings.Count(s, "a")
来源：http://hz.shangyingyoupin.top/gtmpkxhxml.html

Ruby: s.count("a")
来源：http://hz.guowangkeji.top/gtmvmaofpz.html

C#:   s.Count(c => c == 'a')
来源：http://hz.jqgufenzy.top/gtjiofqnab.html

[E13] 逐字符遍历
来源：http://hz.quarkkingdee.top/gthzuxrweb.html

Py:   for ch in s: print(ch)
来源：http://hz.quarkkingdee.top/gtqfykljim.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.shanyushiyangkeji.top/gthkrvnfqw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.wangdashe.top/gtnfpflcmm.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jlsjyb.cn/gtrmlhpzgx.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.feifeiyinyue.top/gtjxkzlyfj.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.smart0.xyz/gtizazgvww.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.vqdsnc.cn/gtodbkedev.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.yj20258.top/gtyatepici.html

[E14] URL 编码与 Base64
来源：http://hz.cdnleiting.top/gtgbjxjcam.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.yj202588.top/gtcvhtllnc.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.yonumen.top/gtlyflssle.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.nanxuanxn.top/gtixtrqbpu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.zhiwuduotai.top/gtykqzsxpp.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.yj20258888.top/gticervvip.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.tian-w.cn/gtuozifuib.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.jqgufenzy.top/gtoexpsrks.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.tanke756.top/gtgvxeynjm.html

[E15] HTML 转义 / 反转义
来源：http://hz.bjfxy.top/gtmlpgaehu.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.feifeiyinyue.top/gtclooqrrl.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.haohaochexian.top/gtsybedxxq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yj202588.top/gtahncerxu.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.zhaomingkeji.xyz/gtbyloolkz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.fengsongda.top/gtldqfbqgh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.tanke756.top/gtqlhaditr.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.bjfxy.top/gtbpuasecf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.yanxiufei.cn/gtaduosnag.html

[E16] 数字千分位
来源：http://hz.jinqigufen.top/gtgqybpuuc.html

Py:   f"{1234567:,}"
来源：http://hz.fzhhl.top/gtzcqevnuw.html

PHP:  number_format(1234567);
来源：http://hz.quarkkingdee.top/gtjitvltti.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.kuanghao11.cn/gtsohuppqa.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.shangyingyoupin.top/gtldopfwox.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.wangdashe.top/gtcntpxitf.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.pengpengdd.cyou/gtafneaqnj.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.ppjwa.cn/gtunusfzcv.html

C#:   1234567.ToString("N0")
来源：http://hz.chenjidiqi.icu/gtwktyrloi.html

[E17] 首字母大写
来源：http://hz.52xcode.cn/gtxylvtlwq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.zhaomingkeji.xyz/gtoffygoli.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.hywenlv.cn/gtvepsgeil.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.pengpengdd.cyou/gtcuuthuln.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.tianlin.xyz/gtcnvuneix.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.shangyingyoupin.top/gtsyafwfck.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.nanxinkj.top/gtqcdofwff.html

Ruby: s.capitalize
来源：http://hz.zhijiandao.cn/gtokphxscb.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.tianlin.xyz/gtayqjjinq.html

[E18] 模板占位符替换
来源：http://hz.jiagoushi.top/gtyerkottg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.xziqi.cn/gthzfmvkbf.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.zhijiandao.cn/gttwfourqk.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.cashguo.top/gtrrhlvvyo.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.gaohongyu789.top/gtrqwhlpga.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.jqgfzy.top/gtgszuvttd.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.chenlongwang.top/gthkgkmyvd.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.vqdsnc.cn/gtgtpaefhm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.ydzc1.top/gtsvvkdfcx.html

[E19] 多行文本按行拆分
来源：http://hz.nwbrower.top/gtgrsgexym.html

Py:   s.splitlines()
来源：http://hz.yj20258888.top/gtibluwlra.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.ydjk.org.cn/gtdtbjgmhr.html

JS:   s.split(/\r?\n/)
来源：http://hz.hongshengwenyu.top/gtiyplxyah.html

TS:   s.split(/\r?\n/)
来源：http://hz.hfpthk.cn/gtpoaqsmjf.html

Java: s.lines().toList()
来源：http://hz.316326.xyz/gtzqmfxjoi.html

Go:   strings.Split(s, "\n")
来源：http://hz.zhixingplan.top/gtjkztdgju.html

Ruby: s.lines
来源：http://hz.shangyingyoupin.top/gtzsjxcrgt.html

C#:   s.Split('\n')
来源：http://hz.zhiwuduotai.top/gtrdgafgkf.html

[E20] 判断字符串是否为空
来源：http://hz.dianchejie.cn/gtowbipvke.html

Py:   if not s:
来源：http://hz.hfpthk.cn/gtaczcsebw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.316326.xyz/gtjgbpxcds.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.cucudq.cn/gtvxcqfnco.html

TS:   if (s === "") {}
来源：http://hz.daxiang520.top/gtmqgxbphr.html

Java: if (s.isEmpty()) {}
来源：http://hz.guannengcc.top/gtbqltkiut.html

Go:   if s == "" {}
来源：http://hz.ybcxt.top/gtpreggfrz.html

Ruby: if s.empty?
来源：http://hz.xziqi.cn/gtzqzpotmr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.xylfe.cn/gtwublkisd.html

[E21] 超长截断加省略号
来源：http://hz.zdqjudy.top/gttifcnwrv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.gzhubu.top/gtzcylltks.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.sxryk.cn/gttqomkuxw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.daxiang520.top/gtvvzarsun.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ywan-chungtsiang.top/gtvhiteeji.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.316326.xyz/gttibgvytf.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.gaohongyu789.top/gtaeptkklf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.ppjwa.cn/gtjcevnuwu.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.0kj1m.cn/gtfxovwzqh.html

[E22] 字节长度与字符长度
来源：http://hz.cdnleiting.top/gtavorcslr.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.zhiwuduotai.top/gtbueribic.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yangfankeji.com/gtpwdxcqbp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yueranfly.top/gtmojwleti.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jqgfzy.top/gtgidrhqqj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.yongpay.top/gtcdwzldkw.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.kuanghao11.cn/gtoebaqdlb.html

Ruby: s.bytesize;  s.length
来源：http://hz.dianchejie.cn/gtehnlrkxl.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.zhoulong.xyz/gtauxnvxak.html

================================================================================
来源：http://hz.cheryme.top/gtowoetpsm.html

F. 文件与目录
来源：http://hz.ydzc1.top/gtkjojdbzz.html

================================================================================
来源：http://hz.ydjk.org.cn/gtppctzolr.html

[F01] 读取整个文件
来源：http://hz.gaohongyu789.top/gtlitnfmww.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.iojbl.cn/gtttblljkc.html

PHP:  file_get_contents("a.txt");
来源：http://hz.snrcjt.cn/gtrbslgkyt.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.gzhubu.top/gtmelsqnqd.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.bjfxy.top/gtfejqguqa.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.jinqigfzy.top/gtidgtshew.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.yuanzhike.top/gtjosufsom.html

Ruby: File.read("a.txt")
来源：http://hz.sweek.top/gtbrslpsod.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.kuanghao11.cn/gtfmetilmm.html

[F02] 逐行读取文件
来源：http://hz.yj20258888.top/gtlhjlvzha.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.meibo888.top/gthnmaykrq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.sweek.top/gtupvvrdmc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhengqikj.top/gttwfxhduq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.sxryk.cn/gtyilthrom.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.hywenlv.cn/gtkymdmhlh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.andypj.xyz/gtcgcyeckx.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.cqqwz.cn/gtzgyztgpu.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.jqgfzy.top/gteqnaegzh.html

[F03] 写入文件（覆盖）
来源：http://hz.cashguo.top/gtevlzumnd.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.dashuyun.cn/gtolckhxqq.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.hfpthk.cn/gtcgsekaos.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jqgufenzy.top/gtdumxksik.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.pycfn.com/gtzixdipiy.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.sufxvd.cn/gtztnsungr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.chenzaomai.com/gtgwpuinck.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.ppjwa.cn/gtucnbtdxa.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.zhixingplan.top/gttiaygnez.html

[F04] 追加写入文件
来源：http://hz.zhongyouzk.top/gtacpugazo.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.gotoacloud.top/gtdxjmyvrc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.svipenyu.cn/gtwwymqfhd.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ppjwa.cn/gtsfrlkebx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhongyouzk.top/gtzqlsqvgp.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.hammf.cn/gtyxhjmphd.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.ybcxt.top/gthtaxubss.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.havefunace.top/gtampohdww.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.wangshuangyany.cn/gthafqahlq.html

[F05] 判断文件或目录是否存在
来源：http://hz.jqgfzy.top/gtpcfehxfo.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.mhx1999.top/gtorcwqrsl.html

PHP:  file_exists("a.txt");
来源：http://hz.jinyuanbaomall.cn/gtlmpmjrss.html

JS:   fs.existsSync("a.txt")
来源：http://hz.ywan-chungtsiang.top/gtdrzvlhwz.html

TS:   fs.existsSync("a.txt")
来源：http://hz.ivvv.top/gtshukahmu.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.hysaishi.cn/gtgsxqoetd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.shanyushiyangkeji.top/gtivcpkkyk.html

Ruby: File.exist?("a.txt")
来源：http://hz.hywenlv.cn/gtvgetbxep.html

C#:   File.Exists("a.txt")
来源：http://hz.sufxvd.cn/gtgpawxxvo.html

[F06] 删除文件
来源：http://hz.gaohongyu789.top/gtelqioyrl.html

Py:   os.remove("a.txt")
来源：http://hz.quarkkingdee.top/gtemfocqvz.html

PHP:  unlink("a.txt");
来源：http://hz.hammf.cn/gtbthvspcm.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yj202588.top/gtlwpmwpbk.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.fzhhl.top/gtvzomyisv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.tianlin.xyz/gtxlvyggfj.html

Go:   os.Remove("a.txt")
来源：http://hz.meibo888.top/gtetbbivsf.html

Ruby: File.delete("a.txt")
来源：http://hz.smart0.xyz/gtkasuydfe.html

C#:   File.Delete("a.txt");
来源：http://hz.sysykeji.top/gtbvczcnfv.html

[F07] 创建目录（含多级）
来源：http://hz.nanxinkj.top/gtygtizzom.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.tanke756.top/gtwqxuhmzd.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.jinqigufen.top/gtmfcreusw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.wangdashe.top/gtkuwjyutd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.chenzaomai.com/gtdabutjpw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.gaohongyu789.top/gtnslnxsdc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.havefunace.top/gtyrnbhkrv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.zhongyouzk.top/gtvjqnzmea.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.haohaochexian.top/gtgijadvvp.html

[F08] 遍历目录
来源：http://hz.shanyushiyangtech.top/gtbtudzjly.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.smart0.xyz/gtfluxtqqd.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.zhijiandao.cn/gtwdhqixvm.html

JS:   fs.readdirSync("dir")
来源：http://hz.ydjk.org.cn/gtjotnvjfh.html

TS:   fs.readdirSync("dir")
来源：http://hz.nanxinkj.top/gtdkenblhm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.hnqzz.top/gtvizgiueh.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.0kj1m.cn/gtpazbjjdo.html

Ruby: Dir.children("dir")
来源：http://hz.ydjk.org.cn/gtmlxqptzk.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yueranfly.top/gtzxegfpyc.html

[F09] 获取文件大小
来源：http://hz.aibaodan.cn/gtpbckzkvf.html

Py:   os.path.getsize("a.txt")
来源：http://hz.jinqigufen.top/gtywbbrlit.html

PHP:  filesize("a.txt");
来源：http://hz.yongpay.top/gtfkbvktrb.html

JS:   fs.statSync("a.txt").size
来源：http://hz.hywenlv.cn/gtfikjpmda.html

TS:   fs.statSync("a.txt").size
来源：http://hz.gogol.net.cn/gtxpyasrfm.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.feifeiyinyue.top/gtmnimzron.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.tianlin.xyz/gtgyhrfotk.html

Ruby: File.size("a.txt")
来源：http://hz.andypj.xyz/gtpweqvkjc.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.fengsongda.top/gtnpfpqypr.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.xziqi.cn/gtnsoohecl.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.hysaishi.cn/gtermddkpw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.yuanzhike.top/gtiwetbpbr.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.dashuyun.cn/gtockkbalx.html

TS:   path.extname("a.txt")
来源：http://hz.ydzc1.top/gtzlkcjtng.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.feifeiyinyue.top/gtbukggzhu.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.cashguo.top/gtlvtckffp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.cheryme.top/gtupyretkx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.bjfxy.top/gtfdddmrto.html

[F11] 复制与移动文件
来源：http://hz.shzxlz.cn/gtjnrbwewz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.ydzc1.top/gtkbhqqept.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yanxiufei.cn/gtvptxgbck.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.smart0.xyz/gtsrirfqdv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.sxryk.cn/gtmiskoaxr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.shangyingyoupin.top/gtzdubzlcr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.cucudq.cn/gtzqdqrcpc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.cashguo.top/gtvewyvygy.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.shanyushiyangtech.top/gtwggzurzs.html

[F12] CSV 读写
来源：http://hz.zhixingplan.top/gtkardsoit.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.fengsongda.top/gtznyuovhb.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.zycfv.cn/gtcniocyms.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.zhixingplan.top/gtmfgdryog.html

TS:   // 同上
来源：http://hz.aizwys.cn/gtxthgddjp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.yangfankeji.com/gtuzndtrvx.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.wangdashe.top/gthnwiuwcy.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.cheryme.top/gteqweaynr.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.zycfv.cn/gthqalflwz.html

================================================================================
来源：http://hz.316326.xyz/gtxuuqpcae.html

G. 面向对象
来源：http://hz.xingfuxueyuan.xyz/gtrgmjgawn.html

================================================================================
来源：http://hz.aizwys.cn/gtriatwhes.html

[G01] 定义类
来源：http://hz.jlsjyb.cn/gtucwpjjke.html

Py:   class User: pass
来源：http://hz.meibo888.top/gtuhjojbww.html

PHP:  class User {}
来源：http://hz.xziqi.cn/gtdkpoaqqg.html

JS:   class User {}
来源：http://hz.guowangkeji.top/gtmpftburm.html

TS:   class User { name: string = ""; }
来源：http://hz.xziqi.cn/gtxscdhxij.html

Java: class User {}
来源：http://hz.chenzaomai.com/gtgiutgvcb.html

Go:   type User struct { Name string }
来源：http://hz.quarkkingdee.top/gtofitnxfo.html

Ruby: class User; end
来源：http://hz.kuanghao11.cn/gtcbthjvca.html

C#:   class User {}
来源：http://hz.tianlin.xyz/gtdcizcbse.html

[G02] 构造函数
来源：http://hz.hysaishi.cn/gtftmygdtq.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.jyoumei.cn/gtsarthrwv.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.cqqwz.cn/gtchofjgyv.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.zhixingplan.top/gtfnhjrhmk.html

TS:   constructor(public name: string) {}
来源：http://hz.smart0.xyz/gtuibpondd.html

Java: User(String name) { this.name = name; }
来源：http://hz.yj20258.top/gtbbknscre.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.guowangkeji.top/gtbadxajyk.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.jlsjyb.cn/gtobznnzul.html

C#:   public User(string name) { Name = name; }
来源：http://hz.wangshuangyany.cn/gtzvqixdbd.html

[G03] 实例属性
来源：http://hz.hnxiangtu.top/gtbtfelmrs.html

Py:   self.name = "x"
来源：http://hz.ywan-chungtsiang.top/gtdzyowmyd.html

PHP:  public string $name = "x";
来源：http://hz.bjfxy.top/gtjyjfipph.html

JS:   this.name = "x";
来源：http://hz.cdnleiting.top/gtaeavwxpo.html

TS:   name: string = "x";
来源：http://hz.hfpthk.cn/gtevfawcdl.html

Java: private String name;
来源：http://hz.redwolf501.top/gtvotstqcb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.havefunace.top/gtfgmgtvfh.html

Ruby: @name = "x"
来源：http://hz.cdnleiting.top/gtwxhuihhk.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.hysaishi.cn/gtguapbzws.html

[G04] 定义方法
来源：http://hz.yonumen.top/gtymshketh.html

Py:   def greet(self): return self.name
来源：http://hz.xingfuxueyuan.xyz/gtzfxplklr.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yongpay.top/gthkulzzei.html

JS:   greet() { return this.name; }
来源：http://hz.jqgufenzy.top/gtovpvxsjm.html

TS:   greet(): string { return this.name; }
来源：http://hz.aizwys.cn/gtgywmuncw.html

Java: String greet() { return name; }
来源：http://hz.0kj1m.cn/gtwddzqgzy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.yj20258888.top/gtfjitldyw.html

Ruby: def greet; @name; end
来源：http://hz.dianchejie.cn/gtyyuaohzf.html

C#:   public string Greet() => Name;
来源：http://hz.zhixingplan.top/gtgvfxkryf.html

[G05] 继承
来源：http://hz.316326.xyz/gtfqmcqgga.html

Py:   class Admin(User): pass
来源：http://hz.smart0.xyz/gtdgrwlkqt.html

PHP:  class Admin extends User {}
来源：http://hz.jlsjyb.cn/gtepyaxkaa.html

JS:   class Admin extends User {}
来源：http://hz.nwbrower.top/gtxchqnioz.html

TS:   class Admin extends User {}
来源：http://hz.daria6918.cn/gtbskvzuih.html

Java: class Admin extends User {}
来源：http://hz.daxiang520.top/gtwapuzwci.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.fengsongda.top/gtsyhywffn.html

Ruby: class Admin < User; end
来源：http://hz.jqgfzy.top/gtowwhrvzn.html

C#:   class Admin : User {}
来源：http://hz.svipenyu.cn/gtzrmtqbqy.html

[G06] 重写方法
来源：http://hz.haohaochexian.top/gtfidzbbzg.html

Py:   def greet(self): return "admin"
来源：http://hz.yj20258888.top/gthgurfigp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.snrcjt.cn/gtasepyakh.html

JS:   greet() { return "admin"; }
来源：http://hz.xziqi.cn/gtfxlctidv.html

TS:   greet(): string { return "admin"; }
来源：http://hz.shzxlz.cn/gtkdqayuis.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.redwolf501.top/gtmmldgvsu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.gzhubu.top/gtwsuszbnc.html

Ruby: def greet; "admin"; end
来源：http://hz.iojbl.cn/gtkkodjvqz.html

C#:   public override string Greet() => "admin";
来源：http://hz.yueranfly.top/gtldwbhcbz.html

[G07] 调用父类方法
来源：http://hz.shzxlz.cn/gtarzxmjul.html

Py:   super().greet()
来源：http://hz.aibaodan.cn/gtgnzcqahq.html

PHP:  parent::greet();
来源：http://hz.yj20258888.top/gtjofzzttt.html

JS:   super.greet();
来源：http://hz.52xcode.cn/gtzzevvnva.html

TS:   super.greet();
来源：http://hz.ywan-chungtsiang.top/gtbdpfjpob.html

Java: super.greet();
来源：http://hz.zhiwuduotai.top/gtugqkuzsp.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.zhixingplan.top/gtckpfirts.html

Ruby: super
来源：http://hz.cashguo.top/gtpblevgpq.html

C#:   base.Greet();
来源：http://hz.chenzaomai.com/gtwhzylmyg.html

[G08] 静态方法与属性
来源：http://hz.jqgfzy.top/gtneuyhjyw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.yanxiufei.cn/gtoppbogpj.html

PHP:  public static function f() {}
来源：http://hz.cdnleiting.top/gtnkzjwvzc.html

JS:   static f() {}
来源：http://hz.zhongyouzk.top/gtxdsdhjtw.html

TS:   static f(): void {}
来源：http://hz.c1oappe.top/gtgddfrbiu.html

Java: static void f() {}
来源：http://hz.zhiwuduotai.top/gtsrkllsot.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.wangshuangyany.cn/gtdplsazmn.html

Ruby: def self.f; end
来源：http://hz.yuanzhike.top/gtohrzoyrp.html

C#:   public static void F() {}
来源：http://hz.sufxvd.cn/gtajzffjcr.html

[G09] 接口 / 抽象类
来源：http://hz.jinyuanbaomall.cn/gttkfgxkmm.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.ehwqpu.com/gtzjujzhac.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.bjfxy.top/gtpygvkklf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.quarkkingdee.top/gtphgrupis.html

TS:   interface Shape { area(): number; }
来源：http://hz.zycfv.cn/gtosnakwll.html

Java: interface Shape { double area(); }
来源：http://hz.guannengcc.top/gtnbenfodh.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.9152youxi.cn/gtknsmmkmb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.hammf.cn/gtkhjksiyg.html

C#:   interface IShape { double Area(); }
来源：http://hz.wangdashe.top/gtbdusbfjq.html

[G10] 访问控制
来源：http://hz.haohaochexian.top/gttajmcnkp.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.jlsjyb.cn/gtyhyfugma.html

PHP:  public / protected / private
来源：http://hz.hammf.cn/gtxxhzroay.html

JS:   #private 字段；其余公开
来源：http://hz.hnxiangtu.top/gtgvxfgilt.html

TS:   public / protected / private
来源：http://hz.guannengcc.top/gtnccwdsal.html

Java: public / protected / private / 默认包级
来源：http://hz.shangyingyoupin.top/gtomtvuouf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.feifeiyinyue.top/gtmmqbkgwh.html

Ruby: public / protected / private
来源：http://hz.zycfv.cn/gtzkrttsws.html


<!-- 参考信息 -->