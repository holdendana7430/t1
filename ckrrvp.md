代发 wailian999

Go:   strings.Count(s, "a")
来源：http://hz.hywenlv.cn/gtcjadpwms.html

Ruby: s.count("a")
来源：http://hz.nwbrower.top/gtxtpfnntt.html

C#:   s.Count(c => c == 'a')
来源：http://hz.snrcjt.cn/gtounvomed.html

[E13] 逐字符遍历
来源：http://hz.guannengcc.top/gtsemocbdf.html

Py:   for ch in s: print(ch)
来源：http://hz.mhx1999.top/gtdtbingrr.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.zhoulong.xyz/gtqvmnfzrx.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.hfpthk.cn/gtkhdhcuiv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.tian-w.cn/gtjzcdlwsu.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.nanxinkj.top/gttwtdkeqp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.cheryme.top/gtkmhphkfe.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.zycfv.cn/gterkafvni.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.ydjk.org.cn/gtuzlofyyz.html

[E14] URL 编码与 Base64
来源：http://hz.sxryk.cn/gtaspvrwcv.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.xuetiantiany.cn/gtdlwsfsny.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.yj20258888.top/gthshfqncm.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.jqgfzy.top/gtknbvyvgc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.ehwqpu.com/gtydutqucq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.zycfv.cn/gtjrodbpin.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.jqgfzy.top/gtaqtbbmgl.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.yj202588.top/gtquwmkgqq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.iojbl.cn/gtwgwfzjlf.html

[E15] HTML 转义 / 反转义
来源：http://hz.yangfankeji.com/gttjaltjeq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.jinqigufen.top/gtcxeuobeu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.xuetiantiany.cn/gtuzjmfval.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.dianchejie.cn/gtxewbannt.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.daxiang520.top/gtqlvbuwqc.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.316326.xyz/gtdnilkqgm.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.wangdashe.top/gtspxmfzsj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.sysykeji.top/gtlpamkpig.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.hnqzz.top/gtupxyqwns.html

[E16] 数字千分位
来源：http://hz.zhixingplan.top/gthzexxqzd.html

Py:   f"{1234567:,}"
来源：http://hz.jlsjyb.cn/gtrscpjezz.html

PHP:  number_format(1234567);
来源：http://hz.nwbrower.top/gtoodidyws.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.quarkkingdee.top/gtiimefdme.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.wangdashe.top/gtxqpaoulp.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.yueranfly.top/gtnnxevrfn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.gzhubu.top/gtzbevmikl.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.jqgfzy.top/gtpypaqfyn.html

C#:   1234567.ToString("N0")
来源：http://hz.tian-w.cn/gtsuoqkoso.html

[E17] 首字母大写
来源：http://hz.vqdsnc.cn/gtaykqyuuo.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.bjfxy.top/gtrjoyrrxv.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.yj202588.top/gtorlzbwba.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhiwuduotai.top/gtetvshmzr.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhengqikj.top/gtmgclazxg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.aizwys.cn/gtypsevujx.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.jyoumei.cn/gtcomeauff.html

Ruby: s.capitalize
来源：http://hz.jiagoushi.top/gthzyvwoft.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.sysykeji.top/gtonlybpge.html

[E18] 模板占位符替换
来源：http://hz.fengsongda.top/gtfurzbaln.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.sysykeji.top/gtwupkamyt.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.yongpay.top/gtmepsyozh.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.yuxming.cn/gttdvdiumm.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.feifeiyinyue.top/gtlathdnrd.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.chenlongwang.top/gtmzfwigkz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.haohaochexian.top/gtnqjmosac.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.xingfuxueyuan.xyz/gtmxnstjew.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.yvedp.cn/gtqvkmfnol.html

[E19] 多行文本按行拆分
来源：http://hz.yangfankeji.com/gtiszhnumj.html

Py:   s.splitlines()
来源：http://hz.shanyushiyangkeji.top/gthmfpblen.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.fzhhl.top/gtcvadgbmb.html

JS:   s.split(/\r?\n/)
来源：http://hz.bjfxy.top/gtxklpswvr.html

TS:   s.split(/\r?\n/)
来源：http://hz.birdmap.top/gtmcbdsczh.html

Java: s.lines().toList()
来源：http://hz.hnqzz.top/gtimqujptv.html

Go:   strings.Split(s, "\n")
来源：http://hz.yj20258888.top/gtlubivuux.html

Ruby: s.lines
来源：http://hz.jiagoushi.top/gttczdaojm.html

C#:   s.Split('\n')
来源：http://hz.wangdashe.top/gtkakpcojy.html

[E20] 判断字符串是否为空
来源：http://hz.9152youxi.cn/gtxvbhrqfy.html

Py:   if not s:
来源：http://hz.bjfxy.top/gtbwmproga.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.cheryme.top/gttkvaeget.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.pycfn.com/gtmqqsixwv.html

TS:   if (s === "") {}
来源：http://hz.cucudq.cn/gtqrexiblf.html

Java: if (s.isEmpty()) {}
来源：http://hz.fengsongda.top/gtphdfmvxj.html

Go:   if s == "" {}
来源：http://hz.xylfe.cn/gthdozkbol.html

Ruby: if s.empty?
来源：http://hz.jinghuilouyu.cn/gtcjxycffk.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.yuanzhike.top/gtvthwhamx.html

[E21] 超长截断加省略号
来源：http://hz.yanxiufei.cn/gtfpckcgph.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.chenzaomai.com/gtuywvwzoj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.pycfn.com/gthuxzqnkr.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.mhx1999.top/gtlkkqmfol.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.xziqi.cn/gtoxbcfrek.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.gzhubu.top/gtuvunvzqi.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.ybcxt.top/gtsvwforov.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.ehwqpu.com/gtecunlnmw.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.tanke756.top/gtojyrzcmo.html

[E22] 字节长度与字符长度
来源：http://hz.daxiang520.top/gtcywcyirk.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.guannengcc.top/gtjditudxu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhaomingkeji.xyz/gtgjikutcw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.quarkkingdee.top/gtccdmrame.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.chenlongwang.top/gtofrpdsgh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jiagoushi.top/gtoxjmtxxh.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.zhixingplan.top/gtjaktimyg.html

Ruby: s.bytesize;  s.length
来源：http://hz.hammf.cn/gtccnoymcq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.xuanzx.com/gtfpvgghhu.html

================================================================================
来源：http://hz.hnxiangtu.top/gtczwhjczg.html

F. 文件与目录
来源：http://hz.hysaishi.cn/gtkdpdjwom.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtwsnmjwvq.html

[F01] 读取整个文件
来源：http://hz.quarkkingdee.top/gtmfvkpxyx.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.316326.xyz/gtkpuajpwo.html

PHP:  file_get_contents("a.txt");
来源：http://hz.redwolf501.top/gtpgujdkmw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.xinyue.icu/gttoyofzxc.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.havefunace.top/gtfcunhver.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.jinghuilouyu.cn/gtysrdbqqh.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.aibaodan.cn/gtzqkhsgnq.html

Ruby: File.read("a.txt")
来源：http://hz.zdqjudy.top/gtsuomzkvy.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.dianchejie.cn/gtjaoekjvn.html

[F02] 逐行读取文件
来源：http://hz.zhijiandao.cn/gtfrutibdg.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.tian-w.cn/gtmoreqzds.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.zhijiandao.cn/gtggbopudo.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.gzhubu.top/gtobrckvhx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.nwbrower.top/gtdkvhpicz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.zhixingplan.top/gtyhmoilaw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.andypj.xyz/gtrnviqvov.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.mhx1999.top/gtnnphvept.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.yj20258888.top/gtbifphqpt.html

[F03] 写入文件（覆盖）
来源：http://hz.ppjwa.cn/gtqtjvctzk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.iojbl.cn/gtbigzaobe.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.tanke756.top/gtimthmnws.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.chenlongwang.top/gtpllwtyso.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hfpthk.cn/gtgpzqmayc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.zdqjudy.top/gtwzoookmn.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.xylfe.cn/gtcrhoutkq.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.hnxiangtu.top/gthcwclzyy.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.havefunace.top/gtyasrvqyl.html

[F04] 追加写入文件
来源：http://hz.pengpengdd.cyou/gtsaztsbws.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.smart0.xyz/gtootpsjxi.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.haohaochexian.top/gtmdsyypqw.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhiwuduotai.top/gtnvrmxmfb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ydzc1.top/gtissektlk.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.52xcode.cn/gtstkdwsbq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.yanxiufei.cn/gtbkntaxnz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.zhengqikj.top/gtxixrqseg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.0kj1m.cn/gtbxpzaylw.html

[F05] 判断文件或目录是否存在
来源：http://hz.yj20258888.top/gtmeqkxolr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.shanyushiyangkeji.top/gtsubacyuz.html

PHP:  file_exists("a.txt");
来源：http://hz.tian-w.cn/gtvznadtqt.html

JS:   fs.existsSync("a.txt")
来源：http://hz.shzxlz.cn/gtqtxvbyjn.html

TS:   fs.existsSync("a.txt")
来源：http://hz.jqgfzy.top/gttpkxoqqg.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.havefunace.top/gteexfcdma.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.mhx1999.top/gtggxuvjth.html

Ruby: File.exist?("a.txt")
来源：http://hz.daxiang520.top/gtmhyrzglm.html

C#:   File.Exists("a.txt")
来源：http://hz.fzhhl.top/gttqinpdag.html

[F06] 删除文件
来源：http://hz.hfpthk.cn/gtctdcfwqm.html

Py:   os.remove("a.txt")
来源：http://hz.xziqi.cn/gtvawzulsf.html

PHP:  unlink("a.txt");
来源：http://hz.ydjk.org.cn/gtmnqyefgh.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.jianghu66.top/gtfemghour.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.yj20258.top/gtbwgwxejf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.hnqzz.top/gtoqjkuxol.html

Go:   os.Remove("a.txt")
来源：http://hz.sysykeji.top/gtyqdsflaq.html

Ruby: File.delete("a.txt")
来源：http://hz.fengsongda.top/gtcfxugsdq.html

C#:   File.Delete("a.txt");
来源：http://hz.sxryk.cn/gtzppuycvj.html

[F07] 创建目录（含多级）
来源：http://hz.0kj1m.cn/gtaqyclrzz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.zhiwuduotai.top/gtlcvzftpn.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.dianchejie.cn/gtdwpbogfs.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.wangshuangyany.cn/gtumbslygy.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yanxiufei.cn/gtishvkwyq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.pycfn.com/gtlfsuwqem.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jianghu66.top/gtkjvmxwjy.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.wangshuangyany.cn/gtzugfolww.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.vqdsnc.cn/gtqhypcvfq.html

[F08] 遍历目录
来源：http://hz.xuanzx.com/gtbaqydwip.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.shuidangran.top/gtlfmvziog.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.hammf.cn/gtrtprhyuw.html

JS:   fs.readdirSync("dir")
来源：http://hz.ywan-chungtsiang.top/gtzgrbkqyo.html

TS:   fs.readdirSync("dir")
来源：http://hz.kuanghao11.cn/gtjfovdulh.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.tianlin.xyz/gtxthbhefh.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.52xcode.cn/gtqhkqqqvw.html

Ruby: Dir.children("dir")
来源：http://hz.sweek.top/gthmyessiv.html

C#:   Directory.GetFiles("dir")
来源：http://hz.jinyuanbaomall.cn/gtfunrxgkb.html

[F09] 获取文件大小
来源：http://hz.0kj1m.cn/gtxupeisiz.html

Py:   os.path.getsize("a.txt")
来源：http://hz.aibaodan.cn/gtunbgxaic.html

PHP:  filesize("a.txt");
来源：http://hz.birdmap.top/gtfyfswrlw.html

JS:   fs.statSync("a.txt").size
来源：http://hz.quarkkingdee.top/gtnifyeswi.html

TS:   fs.statSync("a.txt").size
来源：http://hz.xuetiantiany.cn/gtwwgxmyqb.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.zhongyouzk.top/gtfyblfwlc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.quarkkingdee.top/gtztiryhnb.html

Ruby: File.size("a.txt")
来源：http://hz.hnxiangtu.top/gtzogtvrco.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.ywan-chungtsiang.top/gtrhayqcgs.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.aizwys.cn/gtzstgbtfb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.ydjk.org.cn/gtilhpweqs.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.pengpengdd.cyou/gtxjgnftzj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.yuanzhike.top/gtvassnywa.html

TS:   path.extname("a.txt")
来源：http://hz.c1oappe.top/gtpdeuqajy.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.zhengqikj.top/gtocnubimo.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.zhongyouzk.top/gtypgyadqh.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.zhiwuduotai.top/gtzuxnxwff.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.yuxming.cn/gtiaukeypg.html

[F11] 复制与移动文件
来源：http://hz.chenzaomai.com/gtdcbwvxyb.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.iojbl.cn/gtllefxamt.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.daria6918.cn/gtogfyvync.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ivvv.top/gtthpllvzx.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yj20258.top/gtrtkhtosp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.aibaodan.cn/gtlsfyyzfz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yongpay.top/gtttavcbxx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.kuanghao11.cn/gtihcrzalx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.cheryme.top/gtpgqiuakc.html

[F12] CSV 读写
来源：http://hz.ydzc1.top/gtxihbmzyo.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.zhengqikj.top/gtnbtucifj.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.shangyingyoupin.top/gtxieyjuas.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.chenlongwang.top/gtcojwlwil.html

TS:   // 同上
来源：http://hz.hammf.cn/gtvzokjcuu.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.ivvv.top/gtnnngqhgd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.dianchejie.cn/gtgechyeow.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.vqdsnc.cn/gtcqyriuyq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.xingfuxueyuan.xyz/gtgpcweqnd.html

================================================================================
来源：http://hz.havefunace.top/gtxpuddazt.html

G. 面向对象
来源：http://hz.iojbl.cn/gtlxvhqrlh.html

================================================================================
来源：http://hz.jqgfzy.top/gtlxbqcxnz.html

[G01] 定义类
来源：http://hz.meibo888.top/gtggyuxxrm.html

Py:   class User: pass
来源：http://hz.aibaodan.cn/gtwtnpwyos.html

PHP:  class User {}
来源：http://hz.cqqwz.cn/gtuhlrwxfa.html

JS:   class User {}
来源：http://hz.svipenyu.cn/gtgomtrebs.html

TS:   class User { name: string = ""; }
来源：http://hz.jinyuanbaomall.cn/gtmfdbgucx.html

Java: class User {}
来源：http://hz.hnqzz.top/gtdblcztup.html

Go:   type User struct { Name string }
来源：http://hz.shanyushiyangkeji.top/gtvbsyerau.html

Ruby: class User; end
来源：http://hz.chenlongwang.top/gtuevpmswh.html

C#:   class User {}
来源：http://hz.ybcxt.top/gtsvvueasl.html

[G02] 构造函数
来源：http://hz.xuanzx.com/gtkkroxokx.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.birdmap.top/gtfhcpmqru.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.shzxlz.cn/gtakcdhurb.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yvedp.cn/gtvkpgvexv.html

TS:   constructor(public name: string) {}
来源：http://hz.tian-w.cn/gtlfwsuqfj.html

Java: User(String name) { this.name = name; }
来源：http://hz.cashguo.top/gttohritpb.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.xingfuxueyuan.xyz/gtxnsdzmlz.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yanxiufei.cn/gtsbxlzvzd.html

C#:   public User(string name) { Name = name; }
来源：http://hz.xylfe.cn/gtsddgckdf.html

[G03] 实例属性
来源：http://hz.yvedp.cn/gtjlwzkmre.html

Py:   self.name = "x"
来源：http://hz.52xcode.cn/gtqmoazmve.html

PHP:  public string $name = "x";
来源：http://hz.pengpengdd.cyou/gtplkrmjoq.html

JS:   this.name = "x";
来源：http://hz.nanxinkj.top/gtewjxqnzc.html

TS:   name: string = "x";
来源：http://hz.c1oappe.top/gtltzqsmpu.html

Java: private String name;
来源：http://hz.redwolf501.top/gtjrzdfvft.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.jqgfzy.top/gtmvrrbmip.html

Ruby: @name = "x"
来源：http://hz.wangshuangyany.cn/gtooxipypk.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jinyuanbaomall.cn/gtkdeofzgz.html

[G04] 定义方法
来源：http://hz.mhx1999.top/gtlmvcsfho.html

Py:   def greet(self): return self.name
来源：http://hz.xingfuxueyuan.xyz/gtqmwuogoy.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yongpay.top/gttkbsmjmf.html

JS:   greet() { return this.name; }
来源：http://hz.yangfankeji.com/gtlvktpirw.html

TS:   greet(): string { return this.name; }
来源：http://hz.cdnleiting.top/gtixqzeilo.html

Java: String greet() { return name; }
来源：http://hz.ydjk.org.cn/gtttvdfonj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.mhx1999.top/gteyitjegw.html

Ruby: def greet; @name; end
来源：http://hz.jiagoushi.top/gtjcnuwsey.html

C#:   public string Greet() => Name;
来源：http://hz.pengpengdd.cyou/gtovfdbeqp.html

[G05] 继承
来源：http://hz.xziqi.cn/gtjasnzmdt.html

Py:   class Admin(User): pass
来源：http://hz.guannengcc.top/gtriibxzxf.html

PHP:  class Admin extends User {}
来源：http://hz.xuetiantiany.cn/gtraxvhtjl.html

JS:   class Admin extends User {}
来源：http://hz.shuidangran.top/gtxxlkbhcl.html

TS:   class Admin extends User {}
来源：http://hz.wangdashe.top/gtovpeshea.html

Java: class Admin extends User {}
来源：http://hz.cheryme.top/gtghvmgwdu.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.hammf.cn/gtxawjrbbp.html

Ruby: class Admin < User; end
来源：http://hz.ydzc1.top/gtxugetkln.html

C#:   class Admin : User {}
来源：http://hz.ivvv.top/gtrsrxdcyb.html

[G06] 重写方法
来源：http://hz.sxryk.cn/gtrjtbgfpp.html

Py:   def greet(self): return "admin"
来源：http://hz.gogol.net.cn/gtkodevqwn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.smart0.xyz/gtarpqeuqj.html

JS:   greet() { return "admin"; }
来源：http://hz.hongshengwenyu.top/gtlyiimzgq.html

TS:   greet(): string { return "admin"; }
来源：http://hz.yongpay.top/gtiofgfxho.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jinyuanbaomall.cn/gtwblldbts.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.hammf.cn/gtqrgemamp.html

Ruby: def greet; "admin"; end
来源：http://hz.shangyingyoupin.top/gtvizlqpiy.html

C#:   public override string Greet() => "admin";
来源：http://hz.zhoulong.xyz/gtvbwkdrju.html

[G07] 调用父类方法
来源：http://hz.zycfv.cn/gtyksedlqx.html

Py:   super().greet()
来源：http://hz.xuetiantiany.cn/gtnixakqjh.html

PHP:  parent::greet();
来源：http://hz.jiagoushi.top/gtjxrflqop.html

JS:   super.greet();
来源：http://hz.svipenyu.cn/gtfmyronor.html

TS:   super.greet();
来源：http://hz.aibaodan.cn/gtdcnhbdhr.html

Java: super.greet();
来源：http://hz.gotoacloud.top/gtuahjpeph.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yangfankeji.com/gtmtpzirie.html

Ruby: super
来源：http://hz.iojbl.cn/gttwzppykv.html

C#:   base.Greet();
来源：http://hz.mhx1999.top/gtinivcvkd.html

[G08] 静态方法与属性
来源：http://hz.jiagoushi.top/gtfxmnwtng.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.guowangkeji.top/gtecsxsjep.html

PHP:  public static function f() {}
来源：http://hz.birdmap.top/gtzqzpvcqe.html

JS:   static f() {}
来源：http://hz.jinqigfzy.top/gtrvzczptj.html

TS:   static f(): void {}
来源：http://hz.shzxlz.cn/gtjtiqiuuz.html

Java: static void f() {}
来源：http://hz.hongshengwenyu.top/gtskohzpom.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.zhiwuduotai.top/gtczhckyso.html

Ruby: def self.f; end
来源：http://hz.jiagoushi.top/gtbzopgqeh.html

C#:   public static void F() {}
来源：http://hz.hfpthk.cn/gtyhewcnrr.html

[G09] 接口 / 抽象类
来源：http://hz.smart0.xyz/gtospuwqzp.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.cheryme.top/gtuccqvgvx.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.cucudq.cn/gtdcvfthxf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.ivvv.top/gteajkthxn.html

TS:   interface Shape { area(): number; }
来源：http://hz.hammf.cn/gtucqxpqzg.html

Java: interface Shape { double area(); }
来源：http://hz.yanxiufei.cn/gtkdbsanpk.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.nwbrower.top/gtdctiryte.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.fzhhl.top/gtlvwxojzr.html

C#:   interface IShape { double Area(); }
来源：http://hz.gotoacloud.top/gteocduljr.html

[G10] 访问控制
来源：http://hz.iojbl.cn/gtmakfrffh.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.gotoacloud.top/gteiyrxztn.html

PHP:  public / protected / private
来源：http://hz.chenzaomai.com/gtlsgbekph.html

JS:   #private 字段；其余公开
来源：http://hz.andypj.xyz/gtptbddujw.html

TS:   public / protected / private
来源：http://hz.chenjidiqi.icu/gtvqmhsckg.html

Java: public / protected / private / 默认包级
来源：http://hz.zhiwuduotai.top/gtuxexcfep.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.hysaishi.cn/gtfkqfrxxx.html

Ruby: public / protected / private
来源：http://hz.jiagoushi.top/gtlmrbzrqe.html

C#:   public / protected / private / internal
来源：http://hz.hnxiangtu.top/gtfjbeqjqf.html

[G11] getter / setter
来源：http://hz.zdqjudy.top/gtpbjmlyle.html

Py:   @property 与 @x.setter
来源：http://hz.snrcjt.cn/gtwcarwrvo.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.cashguo.top/gtxnclizpi.html


<!-- 参考信息 -->