代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://hz.guannengcc.top/gtsxbkfxdj.html

Java: String.format("%03d", 7)
来源：http://hz.zdqjudy.top/gttccaoypj.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.iojbl.cn/gtjtnxxczl.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.xziqi.cn/gtnhunvmhq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.zhijiandao.cn/gtbhgohlvw.html

[E11] 反转字符串
来源：http://hz.hnxiangtu.top/gtilohontt.html

Py:   s[::-1]
来源：http://hz.guannengcc.top/gtbvnsrkxq.html

PHP:  strrev($s);
来源：http://hz.shuidangran.top/gtspuifvwv.html

JS:   [...s].reverse().join("")
来源：http://hz.sxryk.cn/gtdgujxiiq.html

TS:   [...s].reverse().join("")
来源：http://hz.pengpengdd.cyou/gtjmwzoqmt.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.yanxiufei.cn/gtjktlfcgt.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.chenlongwang.top/gtxuwbehhi.html

Ruby: s.reverse
来源：http://hz.wangshuangyany.cn/gtgopbjyls.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.chenzaomai.com/gtrugpsoru.html

[E12] 统计某字符出现次数
来源：http://hz.andypj.xyz/gtqprojsyw.html

Py:   s.count("a")
来源：http://hz.cheryme.top/gtgnbksmgm.html

PHP:  substr_count($s, "a");
来源：http://hz.feifeiyinyue.top/gttulnrslf.html

JS:   s.split("a").length - 1
来源：http://hz.yanxiufei.cn/gtuszzbael.html

TS:   s.split("a").length - 1
来源：http://hz.shuidangran.top/gthacayeii.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.jqgfzy.top/gtvbgmtqdx.html

Go:   strings.Count(s, "a")
来源：http://hz.c1oappe.top/gtzbstjyqy.html

Ruby: s.count("a")
来源：http://hz.andypj.xyz/gtlwdnmxra.html

C#:   s.Count(c => c == 'a')
来源：http://hz.fzhhl.top/gtdaudicyl.html

[E13] 逐字符遍历
来源：http://hz.xziqi.cn/gtouodmxel.html

Py:   for ch in s: print(ch)
来源：http://hz.sweek.top/gtdkytenes.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.guannengcc.top/gtbivrsnwr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.meibo888.top/gtxvpauwow.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jyoumei.cn/gthuivcecd.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.ywan-chungtsiang.top/gtmvwavuzd.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.dashuyun.cn/gtmmnvwmhp.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.zhaomingkeji.xyz/gtsbjyyanq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.vqdsnc.cn/gtavdzqoev.html

[E14] URL 编码与 Base64
来源：http://hz.wangdashe.top/gtohzwkext.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.zhijiandao.cn/gtwntmkuxk.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.tanke756.top/gthulxanli.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.chenzaomai.com/gtrdfoyxhj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.haohaochexian.top/gtaiwecxgk.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.ywan-chungtsiang.top/gtjynhvgjl.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.svipenyu.cn/gtczccejug.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.aizwys.cn/gtoumchptx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.mhx1999.top/gtghyxggkx.html

[E15] HTML 转义 / 反转义
来源：http://hz.tianlin.xyz/gtosniulbq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.xuetiantiany.cn/gtslyodspa.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.yj20258.top/gtfvznntzu.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.gogol.net.cn/gtbpxjzdbm.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.hnqzz.top/gtfzzrekin.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.jlsjyb.cn/gtoloolzmo.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.snrcjt.cn/gthsufmvyt.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.nwbrower.top/gtlulutsgy.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.zhaomingkeji.xyz/gtigohbxum.html

[E16] 数字千分位
来源：http://hz.ivvv.top/gtnntagxbh.html

Py:   f"{1234567:,}"
来源：http://hz.fengsongda.top/gtiivxbpkh.html

PHP:  number_format(1234567);
来源：http://hz.zhixingplan.top/gtsqxothrv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.cucudq.cn/gtrdhvdgan.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.jinqigufen.top/gtqdqayklx.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.ydjk.org.cn/gtsbhclexf.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.yj202588.top/gtrpbictfm.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.iojbl.cn/gtgkfqdfqv.html

C#:   1234567.ToString("N0")
来源：http://hz.zhiwuduotai.top/gtjrfsdgdu.html

[E17] 首字母大写
来源：http://hz.yueranfly.top/gteymglyte.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.iojbl.cn/gtdsbrmfqe.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.chenzaomai.com/gtsrrvmjgo.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.sxryk.cn/gtihaojpaf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yvedp.cn/gtncjdagvg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.kuanghao11.cn/gtsrwmvajs.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.chenlongwang.top/gtjwlyvlvs.html

Ruby: s.capitalize
来源：http://hz.jiagoushi.top/gtvcayhpyd.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.jianghu66.top/gtdczvrdqh.html

[E18] 模板占位符替换
来源：http://hz.aibaodan.cn/gthwcirswz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.ydjk.org.cn/gtwiwddrsa.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.jianghu66.top/gtolwcydfa.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.yj20258.top/gtbcqfjvyh.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.chenjidiqi.icu/gtmlgpchfl.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.52xcode.cn/gtslmvxlzs.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.redwolf501.top/gtqhujkhxe.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.52xcode.cn/gtcphbfboa.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.vqdsnc.cn/gteqnnjfqt.html

[E19] 多行文本按行拆分
来源：http://hz.daxiang520.top/gtupezlqyu.html

Py:   s.splitlines()
来源：http://hz.nwbrower.top/gtztpnjxwk.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.zhoulong.xyz/gtrmtjwruh.html

JS:   s.split(/\r?\n/)
来源：http://hz.jlsjyb.cn/gthqhdjvni.html

TS:   s.split(/\r?\n/)
来源：http://hz.smart0.xyz/gtzaoayxso.html

Java: s.lines().toList()
来源：http://hz.yonumen.top/gtiksmhmse.html

Go:   strings.Split(s, "\n")
来源：http://hz.shangyingyoupin.top/gtdytpacew.html

Ruby: s.lines
来源：http://hz.nanxinkj.top/gtbcajujes.html

C#:   s.Split('\n')
来源：http://hz.hysaishi.cn/gtfdpiltqd.html

[E20] 判断字符串是否为空
来源：http://hz.sweek.top/gtntlswbsg.html

Py:   if not s:
来源：http://hz.xinyue.icu/gtnqwpsxau.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.cqqwz.cn/gtxmwtrkac.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.iojbl.cn/gtkccztxmv.html

TS:   if (s === "") {}
来源：http://hz.sysykeji.top/gtysltdiud.html

Java: if (s.isEmpty()) {}
来源：http://hz.jqgufenzy.top/gtljwdfjkv.html

Go:   if s == "" {}
来源：http://hz.shzxlz.cn/gtbalwsctq.html

Ruby: if s.empty?
来源：http://hz.shanyushiyangtech.top/gtbgnklkis.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.daria6918.cn/gtflxlrofo.html

[E21] 超长截断加省略号
来源：http://hz.daria6918.cn/gtqahmhehh.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.iojbl.cn/gtbpteshxe.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.jiagoushi.top/gtwdedxyqz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.xuanzx.com/gtuzhibmlz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.hnxiangtu.top/gtiovxjzht.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.sweek.top/gtusdbfmcb.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.52xcode.cn/gtcfxsupnu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.tian-w.cn/gtxbkhwaqe.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.ydjk.org.cn/gtwcsnbrqm.html

[E22] 字节长度与字符长度
来源：http://hz.xinyue.icu/gtndprqiap.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.zhaomingkeji.xyz/gttnglvvdg.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.daxiang520.top/gtogqhevse.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhiwuduotai.top/gtlqebuirh.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jinyuanbaomall.cn/gtoscidvxy.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.shangyingyoupin.top/gtnbwxpxqx.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.yj20258.top/gtwebxefbf.html

Ruby: s.bytesize;  s.length
来源：http://hz.zycfv.cn/gtcdwcyxqr.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.yanxiufei.cn/gtylgkbfli.html

================================================================================
来源：http://hz.xinyue.icu/gtyxpngcvx.html

F. 文件与目录
来源：http://hz.cucudq.cn/gtlscnhoxw.html

================================================================================
来源：http://hz.andypj.xyz/gtzppiqwwh.html

[F01] 读取整个文件
来源：http://hz.zhongyouzk.top/gtnfaamgoe.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.nanxinkj.top/gtqnviljdp.html

PHP:  file_get_contents("a.txt");
来源：http://hz.yj20258888.top/gtaqzcqims.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.shangyingyoupin.top/gtrqjfkggw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.ehwqpu.com/gtfevkahcq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.316326.xyz/gtrsdlrzvh.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zhengqikj.top/gtmutpaugc.html

Ruby: File.read("a.txt")
来源：http://hz.svipenyu.cn/gtfrfeflct.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.jqgfzy.top/gtejdnpywh.html

[F02] 逐行读取文件
来源：http://hz.dianchejie.cn/gtwtmlkxpp.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.hfpthk.cn/gtiujseyly.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.dashuyun.cn/gtrmcurhcg.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.vqdsnc.cn/gtythdukdj.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.chenlongwang.top/gtghrtxbba.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.316326.xyz/gtuualcrqb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.ehwqpu.com/gtlhgyemde.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.shzxlz.cn/gtsnqmakqn.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.jqgufenzy.top/gtsicayazo.html

[F03] 写入文件（覆盖）
来源：http://hz.pycfn.com/gttvuegcce.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.cdnleiting.top/gtqwoyezii.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.gotoacloud.top/gtgptfuxrv.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.nanxinkj.top/gtblnuisay.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.iojbl.cn/gtjiaoetny.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.gzhubu.top/gtfmwpvdjk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.snrcjt.cn/gtyrzdfnrj.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.dashuyun.cn/gtkxcjzojc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.bjfxy.top/gtqvqvgnbg.html

[F04] 追加写入文件
来源：http://hz.bjfxy.top/gtsptcagmy.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.shzxlz.cn/gttggqzsbk.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.jqgfzy.top/gtvgqehgfz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jqgfzy.top/gtqcxfzcuf.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.nanxinkj.top/gtuerlalls.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.yanxiufei.cn/gthuzguepu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.cdnleiting.top/gtdtpqlvjy.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.xziqi.cn/gtkryeacje.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.dashuyun.cn/gtochpfnxj.html

[F05] 判断文件或目录是否存在
来源：http://hz.smart0.xyz/gthhpqccci.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.hywenlv.cn/gtdlhuxtrz.html

PHP:  file_exists("a.txt");
来源：http://hz.xuetiantiany.cn/gtepbsvnbu.html

JS:   fs.existsSync("a.txt")
来源：http://hz.jyoumei.cn/gtetljmdbv.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yvedp.cn/gtfhfuerep.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.wangshuangyany.cn/gtudizjdek.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.nanxuanxn.top/gtfkmpeovl.html

Ruby: File.exist?("a.txt")
来源：http://hz.zhoulong.xyz/gtpdevasdj.html

C#:   File.Exists("a.txt")
来源：http://hz.haohaochexian.top/gtlksvpyso.html

[F06] 删除文件
来源：http://hz.jinghuilouyu.cn/gtgcsgehmd.html

Py:   os.remove("a.txt")
来源：http://hz.yueranfly.top/gtnebjuzsv.html

PHP:  unlink("a.txt");
来源：http://hz.sysykeji.top/gtjjxrplyq.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.xziqi.cn/gtjenerazk.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.zdqjudy.top/gtlxzkskdz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.nanxinkj.top/gtzniyldfv.html

Go:   os.Remove("a.txt")
来源：http://hz.chenzaomai.com/gtamtldjha.html

Ruby: File.delete("a.txt")
来源：http://hz.hongshengwenyu.top/gtyrgmpyxx.html

C#:   File.Delete("a.txt");
来源：http://hz.gotoacloud.top/gtqlfxqsms.html

[F07] 创建目录（含多级）
来源：http://hz.yueranfly.top/gtiucxahjf.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yanxiufei.cn/gtwlznhyyv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.cheryme.top/gtjkxaevwl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.pengpengdd.cyou/gtfmaljdjn.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.cucudq.cn/gtxckhxgco.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.ppjwa.cn/gtqeatlexq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.tian-w.cn/gtyqiqpvdu.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.feifeiyinyue.top/gtusdjvijc.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.52xcode.cn/gtpdrzptqc.html

[F08] 遍历目录
来源：http://hz.hnqzz.top/gtfltrqigs.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.ywan-chungtsiang.top/gtftzzhvae.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.mhx1999.top/gtzqrizeso.html

JS:   fs.readdirSync("dir")
来源：http://hz.jqgfzy.top/gtvvzdlstn.html

TS:   fs.readdirSync("dir")
来源：http://hz.zycfv.cn/gtthbmwqag.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.chenlongwang.top/gtwxzqejac.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yueranfly.top/gtpygzlkew.html

Ruby: Dir.children("dir")
来源：http://hz.bjfxy.top/gtftvnieti.html

C#:   Directory.GetFiles("dir")
来源：http://hz.316326.xyz/gtgwgocnuv.html

[F09] 获取文件大小
来源：http://hz.jqgfzy.top/gtajsqzypo.html

Py:   os.path.getsize("a.txt")
来源：http://hz.zhongyouzk.top/gttstahuug.html

PHP:  filesize("a.txt");
来源：http://hz.yj20258888.top/gtpuwparvr.html

JS:   fs.statSync("a.txt").size
来源：http://hz.haohaochexian.top/gtwrotymhl.html

TS:   fs.statSync("a.txt").size
来源：http://hz.jinyuanbaomall.cn/gtifyrnyud.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jiagoushi.top/gtwnkmgrpc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.yvedp.cn/gtjmqsspby.html

Ruby: File.size("a.txt")
来源：http://hz.wangdashe.top/gtltwjfqod.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.cucudq.cn/gtrnsyucbo.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yanxiufei.cn/gtuwgbuisz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.nwbrower.top/gteduqbsnw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.pengpengdd.cyou/gtowjfnrfq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.sxryk.cn/gtrvqrfxag.html

TS:   path.extname("a.txt")
来源：http://hz.shangyingyoupin.top/gtqcmmzzft.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.yongpay.top/gtnfuvonvh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.feifeiyinyue.top/gtrswftptd.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.sufxvd.cn/gtevyihuor.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.nwbrower.top/gtkjpsuosr.html

[F11] 复制与移动文件
来源：http://hz.zhongyouzk.top/gtfyidcxzs.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.zhiwuduotai.top/gtxwlbygqr.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.dashuyun.cn/gtvzjwiaib.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.sufxvd.cn/gtgsnkmirk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hnxiangtu.top/gtolnrrkqa.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.pengpengdd.cyou/gttiiwfceg.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.ehwqpu.com/gtdyevcikj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.yj20258.top/gtkngnyexw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.c1oappe.top/gtlmfyahlx.html

[F12] CSV 读写
来源：http://hz.316326.xyz/gtbzexnlau.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.hysaishi.cn/gtgaedwqoj.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.hnqzz.top/gtvmuakicd.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.aizwys.cn/gtdaclcyod.html

TS:   // 同上
来源：http://hz.xziqi.cn/gtctflzibh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.xziqi.cn/gtofcqbwqn.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.smart0.xyz/gtwuonrluy.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jqgfzy.top/gtlykrpztp.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yj202588.top/gtsiekmfjg.html

================================================================================
来源：http://hz.fzhhl.top/gtctzmavnd.html

G. 面向对象
来源：http://hz.yj20258.top/gtxjsxzrtw.html

================================================================================
来源：http://hz.zhixingplan.top/gtipfzdsch.html

[G01] 定义类
来源：http://hz.zdqjudy.top/gtmtkoybgk.html

Py:   class User: pass
来源：http://hz.sxryk.cn/gtfpfeyjrs.html

PHP:  class User {}
来源：http://hz.nanxuanxn.top/gtvdbmrape.html

JS:   class User {}
来源：http://hz.xingfuxueyuan.xyz/gtuowmmnhl.html

TS:   class User { name: string = ""; }
来源：http://hz.kuanghao11.cn/gtrdztwkap.html

Java: class User {}
来源：http://hz.mhx1999.top/gtigvwpnvh.html

Go:   type User struct { Name string }
来源：http://hz.zhijiandao.cn/gtwiedwilz.html

Ruby: class User; end
来源：http://hz.shanyushiyangtech.top/gtufrysevp.html

C#:   class User {}
来源：http://hz.andypj.xyz/gtdosribny.html

[G02] 构造函数
来源：http://hz.havefunace.top/gtfbvgktqw.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.vqdsnc.cn/gtmuutiqpu.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.xylfe.cn/gtgpcjszpd.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.ivvv.top/gtelrkxwri.html

TS:   constructor(public name: string) {}
来源：http://hz.9152youxi.cn/gtalmlnjaz.html

Java: User(String name) { this.name = name; }
来源：http://hz.redwolf501.top/gtgjmwusok.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.0kj1m.cn/gtttygqhms.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.mhx1999.top/gtxxkctmgv.html

C#:   public User(string name) { Name = name; }
来源：http://hz.chenlongwang.top/gturzsiieq.html

[G03] 实例属性
来源：http://hz.hammf.cn/gteytarhul.html

Py:   self.name = "x"
来源：http://hz.snrcjt.cn/gtlfsdccsx.html

PHP:  public string $name = "x";
来源：http://hz.xuetiantiany.cn/gtwozqjrqc.html

JS:   this.name = "x";
来源：http://hz.wangdashe.top/gtmfylhibe.html

TS:   name: string = "x";
来源：http://hz.zhijiandao.cn/gtnjxinxbu.html

Java: private String name;
来源：http://hz.jinyuanbaomall.cn/gtyavxizep.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.ybcxt.top/gthudozsbx.html

Ruby: @name = "x"
来源：http://hz.xziqi.cn/gtjqukhsmr.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.zhongyouzk.top/gtyfhlqjwf.html

[G04] 定义方法
来源：http://hz.wangdashe.top/gthgimlxvv.html

Py:   def greet(self): return self.name
来源：http://hz.tanke756.top/gtkbgbhwxh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.ydzc1.top/gtmlhhjbhs.html

JS:   greet() { return this.name; }
来源：http://hz.0kj1m.cn/gtfkgmxzcj.html

TS:   greet(): string { return this.name; }
来源：http://hz.xuanzx.com/gtgejaihfu.html

Java: String greet() { return name; }
来源：http://hz.ehwqpu.com/gtqciqmyqc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.ywan-chungtsiang.top/gtiplsjssu.html

Ruby: def greet; @name; end
来源：http://hz.tanke756.top/gtdsqumpfv.html

C#:   public string Greet() => Name;
来源：http://hz.cqqwz.cn/gtbdworvyv.html

[G05] 继承
来源：http://hz.quarkkingdee.top/gtociondob.html

Py:   class Admin(User): pass
来源：http://hz.sxryk.cn/gtscsfgdyn.html

PHP:  class Admin extends User {}
来源：http://hz.9152youxi.cn/gtapdiwgmt.html

JS:   class Admin extends User {}
来源：http://hz.xinyue.icu/gtbjvzyudr.html

TS:   class Admin extends User {}
来源：http://hz.gogol.net.cn/gtnquwmamm.html

Java: class Admin extends User {}
来源：http://hz.hywenlv.cn/gtmecanngm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.ydjk.org.cn/gtnircjxtu.html

Ruby: class Admin < User; end
来源：http://hz.shanyushiyangtech.top/gtnviyboah.html

C#:   class Admin : User {}
来源：http://hz.shuidangran.top/gtnephcspg.html

[G06] 重写方法
来源：http://hz.jinqigufen.top/gtdufbibge.html

Py:   def greet(self): return "admin"
来源：http://hz.jianghu66.top/gtcipnxknj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.shangyingyoupin.top/gtizlhwzjz.html

JS:   greet() { return "admin"; }
来源：http://hz.xuanzx.com/gttoaifesx.html

TS:   greet(): string { return "admin"; }
来源：http://hz.jinghuilouyu.cn/gtbyvsirys.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.yuxming.cn/gtazekelqh.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.shuidangran.top/gtuahqnyqr.html

Ruby: def greet; "admin"; end
来源：http://hz.yueranfly.top/gthfhdartv.html

C#:   public override string Greet() => "admin";
来源：http://hz.ybcxt.top/gtnqaqewml.html

[G07] 调用父类方法
来源：http://hz.shanyushiyangkeji.top/gteczhrall.html

Py:   super().greet()
来源：http://hz.zycfv.cn/gtmovkhszr.html

PHP:  parent::greet();
来源：http://hz.0kj1m.cn/gtqjlpyyap.html

JS:   super.greet();
来源：http://hz.hysaishi.cn/gtqmknxwqj.html

TS:   super.greet();
来源：http://hz.chenjidiqi.icu/gtpyacpodq.html

Java: super.greet();
来源：http://hz.daria6918.cn/gtmyhnyfeu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.gzhubu.top/gtxajycgrc.html

Ruby: super
来源：http://hz.ppjwa.cn/gtxamsaots.html

C#:   base.Greet();
来源：http://hz.haohaochexian.top/gtrpkyvcla.html

[G08] 静态方法与属性
来源：http://hz.aibaodan.cn/gtauytenus.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zhongyouzk.top/gtjvonxejk.html

PHP:  public static function f() {}
来源：http://hz.shanyushiyangkeji.top/gtrukaycox.html

JS:   static f() {}
来源：http://hz.sufxvd.cn/gtmxshpvml.html

TS:   static f(): void {}
来源：http://hz.chenjidiqi.icu/gtwvzlcysd.html

Java: static void f() {}
来源：http://hz.fengsongda.top/gtkpwwlpvi.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.guowangkeji.top/gtlfmucnso.html

Ruby: def self.f; end
来源：http://hz.andypj.xyz/gthqwhrgxe.html

C#:   public static void F() {}
来源：http://hz.tian-w.cn/gtbihbscwf.html

[G09] 接口 / 抽象类
来源：http://hz.gzhubu.top/gtygfubkux.html


<!-- 参考信息 -->