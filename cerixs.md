代发 wailian999

JS:   [...s].reverse().join("")
来源：http://hz.yj20258888.top/gtwzqnmuvt.html

TS:   [...s].reverse().join("")
来源：http://hz.andypj.xyz/gtinqlhpom.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.xingfuxueyuan.xyz/gttkiaxhck.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.tianlin.xyz/gtokmovotd.html

Ruby: s.reverse
来源：http://hz.shanyushiyangtech.top/gtntusnmvr.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.jqgufenzy.top/gtclcjuxvb.html

[E12] 统计某字符出现次数
来源：http://hz.jinyuanbaomall.cn/gtiusiffsu.html

Py:   s.count("a")
来源：http://hz.jinyuanbaomall.cn/gttniurqxe.html

PHP:  substr_count($s, "a");
来源：http://hz.ivvv.top/gtyoutarqj.html

JS:   s.split("a").length - 1
来源：http://hz.gzhubu.top/gtegzdiqwe.html

TS:   s.split("a").length - 1
来源：http://hz.cqqwz.cn/gtgcsfsasg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.cheryme.top/gthjsjgdgf.html

Go:   strings.Count(s, "a")
来源：http://hz.birdmap.top/gtoteryrdi.html

Ruby: s.count("a")
来源：http://hz.xuanzx.com/gtzclvigor.html

C#:   s.Count(c => c == 'a')
来源：http://hz.aizwys.cn/gtlwuxeqtl.html

[E13] 逐字符遍历
来源：http://hz.chenjidiqi.icu/gtmdxmszqx.html

Py:   for ch in s: print(ch)
来源：http://hz.c1oappe.top/gtiaxbfdry.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.birdmap.top/gtpvbfpxnh.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yuxming.cn/gtcqrmsuot.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jiagoushi.top/gtczxbtbnl.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.vqdsnc.cn/gtkhxtfkgd.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.zhiwuduotai.top/gtajutunlp.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.shanyushiyangkeji.top/gtshhrglac.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.havefunace.top/gtcafrkwsb.html

[E14] URL 编码与 Base64
来源：http://hz.cheryme.top/gtcsridnrc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.hysaishi.cn/gthxcmmutz.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.ydzc1.top/gteqdeibfq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.zhengqikj.top/gtkujrqtgv.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.dashuyun.cn/gtjhbitwxd.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.316326.xyz/gtwnkbydxu.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.shanyushiyangtech.top/gtungnuklj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.quarkkingdee.top/gtisdkxina.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.birdmap.top/gttwfmstcy.html

[E15] HTML 转义 / 反转义
来源：http://hz.gzhubu.top/gtrcjljbcn.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.sxryk.cn/gtqgblgsqx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.shanyushiyangkeji.top/gtqesrynzd.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yonumen.top/gtxkxbjxzl.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.vqdsnc.cn/gtzqojqply.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.yj202588.top/gtaxaxmzqq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.jinghuilouyu.cn/gtubnvkoez.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.yuxming.cn/gtonvmeggm.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.chenjidiqi.icu/gtgnbvfkda.html

[E16] 数字千分位
来源：http://hz.aizwys.cn/gtuqgwrgzx.html

Py:   f"{1234567:,}"
来源：http://hz.0kj1m.cn/gttxshgtie.html

PHP:  number_format(1234567);
来源：http://hz.wangshuangyany.cn/gthcnekhqa.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.aizwys.cn/gtblmvzsms.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.0kj1m.cn/gtfatbhqii.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.zhixingplan.top/gtkbyhbgrs.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.tian-w.cn/gtgzweasuw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.316326.xyz/gtbmmxuagk.html

C#:   1234567.ToString("N0")
来源：http://hz.zdqjudy.top/gttjvfubng.html

[E17] 首字母大写
来源：http://hz.tian-w.cn/gtmpkxpvlp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.sysykeji.top/gtzfhbnuma.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.aizwys.cn/gtfhudnpvg.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.xinyue.icu/gtnsqgudta.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yuanzhike.top/gtvfrlpalu.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.yonumen.top/gttjmvswew.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.hnqzz.top/gtxqzpiyah.html

Ruby: s.capitalize
来源：http://hz.wangdashe.top/gtrlwrtqdj.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.kuanghao11.cn/gtniaxznaw.html

[E18] 模板占位符替换
来源：http://hz.daxiang520.top/gtbplhxenu.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.xinyue.icu/gtbbhmsdxe.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.fzhhl.top/gtjsfneqzy.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.ybcxt.top/gtxwbhqrsl.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.snrcjt.cn/gtwtwzolnq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.cashguo.top/gtejdjjazx.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.jqgfzy.top/gtgbvqdsin.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.snrcjt.cn/gtobelovxd.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.andypj.xyz/gtfljzjbfy.html

[E19] 多行文本按行拆分
来源：http://hz.dashuyun.cn/gtmmezqgrs.html

Py:   s.splitlines()
来源：http://hz.cashguo.top/gtzslpatuk.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.xylfe.cn/gtpkmtqijx.html

JS:   s.split(/\r?\n/)
来源：http://hz.xinyue.icu/gtoddsukyk.html

TS:   s.split(/\r?\n/)
来源：http://hz.cashguo.top/gthfbkkulx.html

Java: s.lines().toList()
来源：http://hz.chenlongwang.top/gtiikdbdzm.html

Go:   strings.Split(s, "\n")
来源：http://hz.yonumen.top/gtxgwadhju.html

Ruby: s.lines
来源：http://hz.kuanghao11.cn/gtomgbkrsm.html

C#:   s.Split('\n')
来源：http://hz.jiagoushi.top/gtvrbjbwen.html

[E20] 判断字符串是否为空
来源：http://hz.sweek.top/gtqsiretgu.html

Py:   if not s:
来源：http://hz.ehwqpu.com/gtdvakbtyp.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.xuanzx.com/gtlzwhcdnf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.tian-w.cn/gttsgbojzw.html

TS:   if (s === "") {}
来源：http://hz.haohaochexian.top/gtwvxhiglz.html

Java: if (s.isEmpty()) {}
来源：http://hz.xingfuxueyuan.xyz/gtyfvhmxsv.html

Go:   if s == "" {}
来源：http://hz.aibaodan.cn/gtegxitvby.html

Ruby: if s.empty?
来源：http://hz.xinyue.icu/gtxdalhhtl.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.birdmap.top/gtetcrvxxf.html

[E21] 超长截断加省略号
来源：http://hz.hywenlv.cn/gtqqncejxl.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.jiagoushi.top/gtnmcbgwwr.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.9152youxi.cn/gtvxurbymx.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.wangdashe.top/gtsqdpdnce.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jyoumei.cn/gtrsoxqltu.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.zycfv.cn/gtuyzltoeq.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.ydjk.org.cn/gtfkuyrszw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.chenzaomai.com/gtlozdphnm.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.svipenyu.cn/gtlszdgfoa.html

[E22] 字节长度与字符长度
来源：http://hz.snrcjt.cn/gttpbwqsiw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.fengsongda.top/gtoxnhckjc.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.shuidangran.top/gtdavlozkp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.fengsongda.top/gttqzxacjd.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ydzc1.top/gtobeszrng.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.feifeiyinyue.top/gtbedtgzyj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.smart0.xyz/gttdmxfcyk.html

Ruby: s.bytesize;  s.length
来源：http://hz.jinqigufen.top/gtkflpcqal.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.wangshuangyany.cn/gtviadrynt.html

================================================================================
来源：http://hz.iojbl.cn/gtlrhxbqwq.html

F. 文件与目录
来源：http://hz.yj202588.top/gtmhmehafi.html

================================================================================
来源：http://hz.tian-w.cn/gtpbqpqprv.html

[F01] 读取整个文件
来源：http://hz.jinqigfzy.top/gtfodomxvb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.ivvv.top/gtouhuxpkq.html

PHP:  file_get_contents("a.txt");
来源：http://hz.yvedp.cn/gtxtgknbnr.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.gzhubu.top/gtwfyhoywu.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.zhixingplan.top/gtrobistwu.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.mhx1999.top/gthxfaoyxd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.shuidangran.top/gtciufxhxa.html

Ruby: File.read("a.txt")
来源：http://hz.shanyushiyangkeji.top/gtpmamuotq.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.dianchejie.cn/gtxhfjawui.html

[F02] 逐行读取文件
来源：http://hz.gogol.net.cn/gtpvurcant.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.52xcode.cn/gtykroedtr.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.snrcjt.cn/gtiylpwsff.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.316326.xyz/gtrnjbsnjb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ivvv.top/gthvqbrels.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.shzxlz.cn/gtkyzrfdwa.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.jinqigfzy.top/gtkapacvaa.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.jinqigfzy.top/gtizgesziv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.xuanzx.com/gttzidcgdv.html

[F03] 写入文件（覆盖）
来源：http://hz.pycfn.com/gtceqctbqo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.yuanzhike.top/gtkddzclvr.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.hnxiangtu.top/gteaxgwncj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.sysykeji.top/gtiqvwdvag.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.bjfxy.top/gtpnzbvkmw.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.bjfxy.top/gtkwpwkcyb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.yvedp.cn/gtztpdycyv.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.gotoacloud.top/gtraakvalc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.yuanzhike.top/gtiyskeawn.html

[F04] 追加写入文件
来源：http://hz.c1oappe.top/gtqkcuvtxm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.dashuyun.cn/gtdwuywows.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.ywan-chungtsiang.top/gtnrhtvwns.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.shanyushiyangtech.top/gtvguomjyo.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.sxryk.cn/gttwjgdkof.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.tianlin.xyz/gthzcsdjkr.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.shanyushiyangkeji.top/gtockcgpid.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.zhoulong.xyz/gtzluhjtci.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.jinghuilouyu.cn/gthqacomru.html

[F05] 判断文件或目录是否存在
来源：http://hz.andypj.xyz/gtwfftyebw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.yongpay.top/gtwdinhlmm.html

PHP:  file_exists("a.txt");
来源：http://hz.zdqjudy.top/gtiltonoxo.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yanxiufei.cn/gtjeigiznj.html

TS:   fs.existsSync("a.txt")
来源：http://hz.shangyingyoupin.top/gtfiygrkev.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.havefunace.top/gtyntppaxc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.daria6918.cn/gtipuevrgj.html

Ruby: File.exist?("a.txt")
来源：http://hz.hammf.cn/gtdesqylzg.html

C#:   File.Exists("a.txt")
来源：http://hz.yuanzhike.top/gtorbtcjak.html

[F06] 删除文件
来源：http://hz.ydjk.org.cn/gtmmrogaof.html

Py:   os.remove("a.txt")
来源：http://hz.feifeiyinyue.top/gtidefohoq.html

PHP:  unlink("a.txt");
来源：http://hz.yvedp.cn/gtufjkbzxs.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.jinghuilouyu.cn/gtteqyxxzi.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.tianlin.xyz/gtyohyyycu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.yuxming.cn/gtryoonyzy.html

Go:   os.Remove("a.txt")
来源：http://hz.nwbrower.top/gtodnauxyu.html

Ruby: File.delete("a.txt")
来源：http://hz.cqqwz.cn/gtxzvhknxc.html

C#:   File.Delete("a.txt");
来源：http://hz.feifeiyinyue.top/gtbgnpgqum.html

[F07] 创建目录（含多级）
来源：http://hz.quarkkingdee.top/gtzygtaddh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.hnqzz.top/gtdsbjnahu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.sufxvd.cn/gtwdikqahd.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhaomingkeji.xyz/gtymxyxwzi.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.svipenyu.cn/gtdqcmucrt.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.sweek.top/gtpwlsddsm.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.ywan-chungtsiang.top/gtoardhprz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.chenjidiqi.icu/gtpyxribnt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.aibaodan.cn/gtsacybuix.html

[F08] 遍历目录
来源：http://hz.yuxming.cn/gtvodtwyvl.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.sxryk.cn/gtprjuupqw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.gaohongyu789.top/gtnjejwaso.html

JS:   fs.readdirSync("dir")
来源：http://hz.jyoumei.cn/gtypsfyuaw.html

TS:   fs.readdirSync("dir")
来源：http://hz.yueranfly.top/gtwxagevvq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.sweek.top/gtpsaojrmz.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.jianghu66.top/gtvzsmpziu.html

Ruby: Dir.children("dir")
来源：http://hz.aibaodan.cn/gtysrdptnl.html

C#:   Directory.GetFiles("dir")
来源：http://hz.andypj.xyz/gtvojzwbkh.html

[F09] 获取文件大小
来源：http://hz.hywenlv.cn/gtwwvuzvqf.html

Py:   os.path.getsize("a.txt")
来源：http://hz.zhongyouzk.top/gtgvtkkudh.html

PHP:  filesize("a.txt");
来源：http://hz.gaohongyu789.top/gtkgewbxxl.html

JS:   fs.statSync("a.txt").size
来源：http://hz.zhoulong.xyz/gtbwcadvcg.html

TS:   fs.statSync("a.txt").size
来源：http://hz.svipenyu.cn/gtnbapuvux.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.xziqi.cn/gtbyzqhrik.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.yj202588.top/gtxfxrnqka.html

Ruby: File.size("a.txt")
来源：http://hz.smart0.xyz/gtuticskdx.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yonumen.top/gtavmsunws.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.svipenyu.cn/gttvlmltox.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.9152youxi.cn/gtlrvfyskf.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.smart0.xyz/gtypkzuxdg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.shuidangran.top/gtmxouonyh.html

TS:   path.extname("a.txt")
来源：http://hz.0kj1m.cn/gttpisxlxo.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.daria6918.cn/gtwutvpdtz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.jqgfzy.top/gtrvcivwsc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.haohaochexian.top/gtjckyhlvb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.jiagoushi.top/gthynjvczo.html

[F11] 复制与移动文件
来源：http://hz.316326.xyz/gtzoeccrat.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.jiagoushi.top/gtqwxnpoct.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.shuidangran.top/gtpvahkxpl.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zdqjudy.top/gtdhghqppr.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.sufxvd.cn/gtfrfcqlwn.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.zdqjudy.top/gtrljoyuvz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.redwolf501.top/gtmeqhczxk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.snrcjt.cn/gtqgvsapfk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.ywan-chungtsiang.top/gtcerjbjny.html

[F12] CSV 读写
来源：http://hz.gotoacloud.top/gtbysifibj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.sxryk.cn/gtqidrabsr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.0kj1m.cn/gtqngnmwsm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.jqgufenzy.top/gttudcpzyt.html

TS:   // 同上
来源：http://hz.hongshengwenyu.top/gtzqznggrj.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.zhiwuduotai.top/gtduljttmn.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.xinyue.icu/gtrjcsrice.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.ivvv.top/gthapwybyt.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.aibaodan.cn/gtnqvhupnw.html

================================================================================
来源：http://hz.yanxiufei.cn/gtdqzdmkcd.html

G. 面向对象
来源：http://hz.zhijiandao.cn/gtelqtftze.html

================================================================================
来源：http://hz.jiagoushi.top/gtuzxbljxl.html

[G01] 定义类
来源：http://hz.zhaomingkeji.xyz/gtkzsnurej.html

Py:   class User: pass
来源：http://hz.jinqigfzy.top/gturajmvzn.html

PHP:  class User {}
来源：http://hz.shuidangran.top/gtmlanxgmz.html

JS:   class User {}
来源：http://hz.zhoulong.xyz/gtnczafxmx.html

TS:   class User { name: string = ""; }
来源：http://hz.kuanghao11.cn/gtkfrxqizh.html

Java: class User {}
来源：http://hz.yanxiufei.cn/gtmqxrskbk.html

Go:   type User struct { Name string }
来源：http://hz.hnxiangtu.top/gtarompxwv.html

Ruby: class User; end
来源：http://hz.hnqzz.top/gtwipxseem.html

C#:   class User {}
来源：http://hz.andypj.xyz/gtjlynommg.html

[G02] 构造函数
来源：http://hz.chenzaomai.com/gtwdakmplt.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.sweek.top/gtubvydqxm.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yangfankeji.com/gtjydljfxg.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.xuetiantiany.cn/gtntkthyjl.html

TS:   constructor(public name: string) {}
来源：http://hz.ydzc1.top/gtsmozevwv.html

Java: User(String name) { this.name = name; }
来源：http://hz.pengpengdd.cyou/gtarbnfgbo.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.haohaochexian.top/gtxwzkauoi.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.nanxinkj.top/gtqugmvvhe.html

C#:   public User(string name) { Name = name; }
来源：http://hz.cashguo.top/gtrfykjjle.html

[G03] 实例属性
来源：http://hz.shuidangran.top/gtwfrotfof.html

Py:   self.name = "x"
来源：http://hz.zdqjudy.top/gtzvqascin.html

PHP:  public string $name = "x";
来源：http://hz.shanyushiyangtech.top/gtlkemxwpk.html

JS:   this.name = "x";
来源：http://hz.yj20258888.top/gtazhbbcrr.html

TS:   name: string = "x";
来源：http://hz.daria6918.cn/gtuuqkfsfb.html

Java: private String name;
来源：http://hz.aizwys.cn/gtyrsrquee.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.sweek.top/gtagcxzwac.html

Ruby: @name = "x"
来源：http://hz.aizwys.cn/gtyadhtyil.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.iojbl.cn/gtkpgcfwdv.html

[G04] 定义方法
来源：http://hz.yongpay.top/gtrysquiec.html

Py:   def greet(self): return self.name
来源：http://hz.ywan-chungtsiang.top/gtfxwfqjwu.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.hysaishi.cn/gtdwxxewag.html

JS:   greet() { return this.name; }
来源：http://hz.gogol.net.cn/gtxmfojdjh.html

TS:   greet(): string { return this.name; }
来源：http://hz.daria6918.cn/gtrqubekuj.html

Java: String greet() { return name; }
来源：http://hz.xingfuxueyuan.xyz/gtejdhyxfj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.redwolf501.top/gtfiiyayia.html

Ruby: def greet; @name; end
来源：http://hz.wangdashe.top/gtdkevpcnf.html

C#:   public string Greet() => Name;
来源：http://hz.yj20258888.top/gtvhmbmohk.html

[G05] 继承
来源：http://hz.vqdsnc.cn/gtnlaxfkrv.html

Py:   class Admin(User): pass
来源：http://hz.bjfxy.top/gtmgqlvcvl.html

PHP:  class Admin extends User {}
来源：http://hz.gaohongyu789.top/gtcnqyerxo.html

JS:   class Admin extends User {}
来源：http://hz.jinqigfzy.top/gthaalafke.html

TS:   class Admin extends User {}
来源：http://hz.yj20258888.top/gtxdhsajbh.html

Java: class Admin extends User {}
来源：http://hz.chenlongwang.top/gthurslqny.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yj20258.top/gtypudtlpc.html

Ruby: class Admin < User; end
来源：http://hz.yonumen.top/gthdlhzxlu.html

C#:   class Admin : User {}
来源：http://hz.jyoumei.cn/gtldiaqrkg.html

[G06] 重写方法
来源：http://hz.jlsjyb.cn/gtvcnjgtoc.html

Py:   def greet(self): return "admin"
来源：http://hz.gogol.net.cn/gtqpijelmw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.chenjidiqi.icu/gtfrfunfeg.html

JS:   greet() { return "admin"; }
来源：http://hz.xingfuxueyuan.xyz/gtlhzorcli.html

TS:   greet(): string { return "admin"; }
来源：http://hz.gzhubu.top/gtuvrqzxsx.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.aizwys.cn/gtdaxyvxvl.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zhongyouzk.top/gtsgowvsbl.html

Ruby: def greet; "admin"; end
来源：http://hz.hnqzz.top/gtextldnef.html

C#:   public override string Greet() => "admin";
来源：http://hz.yongpay.top/gtetjeedyo.html

[G07] 调用父类方法
来源：http://hz.xingfuxueyuan.xyz/gtkmjlyyyu.html

Py:   super().greet()
来源：http://hz.yueranfly.top/gtclqujoit.html

PHP:  parent::greet();
来源：http://hz.gzhubu.top/gtbarsrdxc.html

JS:   super.greet();
来源：http://hz.iojbl.cn/gtmrsoofkt.html

TS:   super.greet();
来源：http://hz.ivvv.top/gtwkleaavz.html

Java: super.greet();
来源：http://hz.zhengqikj.top/gtlsdhzmxu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.0kj1m.cn/gtobqkoeiz.html

Ruby: super
来源：http://hz.tanke756.top/gtckjsvpia.html

C#:   base.Greet();
来源：http://hz.wangdashe.top/gtddvpipvi.html

[G08] 静态方法与属性
来源：http://hz.cdnleiting.top/gtnflehquv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zhiwuduotai.top/gtgbsyzedi.html

PHP:  public static function f() {}
来源：http://hz.yonumen.top/gtgafccmba.html

JS:   static f() {}
来源：http://hz.cucudq.cn/gtfjwealjn.html

TS:   static f(): void {}
来源：http://hz.dashuyun.cn/gtzpyisjyh.html

Java: static void f() {}
来源：http://hz.meibo888.top/gtvduwrjik.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.chenlongwang.top/gtmwkgxlvf.html

Ruby: def self.f; end
来源：http://hz.fzhhl.top/gtpmtlnvdk.html

C#:   public static void F() {}
来源：http://hz.sxryk.cn/gtmxixyolf.html

[G09] 接口 / 抽象类
来源：http://hz.ybcxt.top/gtjftruceh.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.shuidangran.top/gtphjeypaz.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.52xcode.cn/gtifnmqcxh.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.shuidangran.top/gtbypfhdqq.html

TS:   interface Shape { area(): number; }
来源：http://hz.hongshengwenyu.top/gtfagaqmpf.html

Java: interface Shape { double area(); }
来源：http://hz.cqqwz.cn/gtikaafpin.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.sweek.top/gtcdopskps.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yongpay.top/gtjfgzvxrz.html

C#:   interface IShape { double Area(); }
来源：http://hz.dashuyun.cn/gthnjcbqts.html


<!-- 参考信息 -->