代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://hz.hnxiangtu.top/gtfkhfzmux.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.yangfankeji.com/gtqrzqjiay.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.aizwys.cn/gtztdqhipb.html

JS:   "7".padStart(3, "0")
来源：http://hz.pycfn.com/gtsqnhmzkb.html

TS:   "7".padStart(3, "0")
来源：http://hz.sysykeji.top/gtfxvvkynz.html

Java: String.format("%03d", 7)
来源：http://hz.ydzc1.top/gtfgvwqwzh.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.pycfn.com/gtyqtiipgp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.yj202588.top/gtgulifdlu.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.aizwys.cn/gtivpzuydw.html

[E11] 反转字符串
来源：http://hz.xylfe.cn/gtoucskqse.html

Py:   s[::-1]
来源：http://hz.sufxvd.cn/gtmbkloggz.html

PHP:  strrev($s);
来源：http://hz.sxryk.cn/gthixiaoob.html

JS:   [...s].reverse().join("")
来源：http://hz.zhoulong.xyz/gtxpsjjszm.html

TS:   [...s].reverse().join("")
来源：http://hz.9152youxi.cn/gtzapzqmaz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.redwolf501.top/gtiqhvinqq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.zhiwuduotai.top/gtrtyytaek.html

Ruby: s.reverse
来源：http://hz.hysaishi.cn/gtbcwktyuw.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.jinqigufen.top/gtfrscaxul.html

[E12] 统计某字符出现次数
来源：http://hz.chenjidiqi.icu/gteapkasfb.html

Py:   s.count("a")
来源：http://hz.yanxiufei.cn/gtvoldirpl.html

PHP:  substr_count($s, "a");
来源：http://hz.pycfn.com/gtfnviecid.html

JS:   s.split("a").length - 1
来源：http://hz.cucudq.cn/gtbagxutcl.html

TS:   s.split("a").length - 1
来源：http://hz.feifeiyinyue.top/gtiitmykiu.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.ywan-chungtsiang.top/gtxtxclcii.html

Go:   strings.Count(s, "a")
来源：http://hz.ydzc1.top/gtvvhfhrgl.html

Ruby: s.count("a")
来源：http://hz.ppjwa.cn/gthzjwqukv.html

C#:   s.Count(c => c == 'a')
来源：http://hz.pycfn.com/gtrgkxsref.html

[E13] 逐字符遍历
来源：http://hz.pengpengdd.cyou/gtvqfyhmaz.html

Py:   for ch in s: print(ch)
来源：http://hz.gaohongyu789.top/gtvnsnhbqn.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.gzhubu.top/gtgiykaaxz.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yueranfly.top/gtlwqufnmm.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xuetiantiany.cn/gthjeunqbq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.ybcxt.top/gtfxvcsyis.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.zhiwuduotai.top/gtyfonrerd.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.cashguo.top/gtvxqitdqf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.hysaishi.cn/gtekvpjwoj.html

[E14] URL 编码与 Base64
来源：http://hz.cqqwz.cn/gtopatbaef.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.dashuyun.cn/gtcuhduetg.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.xziqi.cn/gtvgxuhbph.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.shangyingyoupin.top/gtdvnkpwpr.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.hysaishi.cn/gtjworxlyl.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.hfpthk.cn/gthymsnllz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.hfpthk.cn/gtnafghvqs.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.pengpengdd.cyou/gtoqwgdsro.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.daria6918.cn/gtmbdatnyu.html

[E15] HTML 转义 / 反转义
来源：http://hz.fengsongda.top/gtvagacgau.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.ydzc1.top/gtejgznwzx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.chenlongwang.top/gtxkaoasqb.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.jqgfzy.top/gtigowbsnk.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.zdqjudy.top/gtkzpbrvml.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.birdmap.top/gtbbtihvlb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.xziqi.cn/gtfwkrzyvl.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.birdmap.top/gtukgbsqyu.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.kuanghao11.cn/gtjjkebfnk.html

[E16] 数字千分位
来源：http://hz.dashuyun.cn/gtvuyniwcj.html

Py:   f"{1234567:,}"
来源：http://hz.gogol.net.cn/gtivluynzs.html

PHP:  number_format(1234567);
来源：http://hz.tianlin.xyz/gtgcpwohcl.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.nanxuanxn.top/gtfrtxqswe.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.sysykeji.top/gtkrmrwtfs.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.yj20258.top/gtanjuwwnr.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.ydjk.org.cn/gtgjtholur.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.cucudq.cn/gtdqaohpaj.html

C#:   1234567.ToString("N0")
来源：http://hz.dianchejie.cn/gtmxygsdcw.html

[E17] 首字母大写
来源：http://hz.havefunace.top/gtqvborzob.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.cucudq.cn/gtgnrblvqr.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.shangyingyoupin.top/gtjavdlpuc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yj202588.top/gtcvwysohu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.shanyushiyangkeji.top/gtvxdfefxe.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.birdmap.top/gtwlarrjog.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.zhengqikj.top/gtfesynrno.html

Ruby: s.capitalize
来源：http://hz.daxiang520.top/gtpvikrtag.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.nanxinkj.top/gtsdcjxekw.html

[E18] 模板占位符替换
来源：http://hz.chenzaomai.com/gtjmocpqfp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.jianghu66.top/gtxermyhyj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.xingfuxueyuan.xyz/gtbgnhpaas.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.gotoacloud.top/gtwizayuqi.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.nanxinkj.top/gtinydeeig.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.wangshuangyany.cn/gtlvhmvbdj.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.tianlin.xyz/gtponayfwv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.hongshengwenyu.top/gtsxffkcqq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.zhoulong.xyz/gtbodnvwji.html

[E19] 多行文本按行拆分
来源：http://hz.gotoacloud.top/gtfedqwqeg.html

Py:   s.splitlines()
来源：http://hz.smart0.xyz/gtqkrsynvr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.fengsongda.top/gtshdsghjp.html

JS:   s.split(/\r?\n/)
来源：http://hz.feifeiyinyue.top/gtsuyovdlg.html

TS:   s.split(/\r?\n/)
来源：http://hz.tanke756.top/gtsndmwhcd.html

Java: s.lines().toList()
来源：http://hz.yj20258888.top/gtykfkzrhh.html

Go:   strings.Split(s, "\n")
来源：http://hz.52xcode.cn/gtxqutmegd.html

Ruby: s.lines
来源：http://hz.vqdsnc.cn/gtdnnebwgv.html

C#:   s.Split('\n')
来源：http://hz.sysykeji.top/gtkrjpxinr.html

[E20] 判断字符串是否为空
来源：http://hz.redwolf501.top/gtpuqgvlve.html

Py:   if not s:
来源：http://hz.sufxvd.cn/gtduhzccoq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.zhongyouzk.top/gtyzimwyqe.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.pengpengdd.cyou/gtyriuizey.html

TS:   if (s === "") {}
来源：http://hz.aibaodan.cn/gtbomqxcry.html

Java: if (s.isEmpty()) {}
来源：http://hz.havefunace.top/gtimhhxevr.html

Go:   if s == "" {}
来源：http://hz.zhengqikj.top/gtzafgdxlr.html

Ruby: if s.empty?
来源：http://hz.dianchejie.cn/gtjkewiqse.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.kuanghao11.cn/gtmyvjsvgl.html

[E21] 超长截断加省略号
来源：http://hz.zycfv.cn/gtxyexuxcj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.ydjk.org.cn/gtqxflmajs.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.fzhhl.top/gtyzvrzqih.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yvedp.cn/gtdbykntdn.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.redwolf501.top/gtfemginex.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.feifeiyinyue.top/gtcjpljmxc.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.chenzaomai.com/gtwexiavae.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.ivvv.top/gtcogafxfx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.smart0.xyz/gtwwysqtke.html

[E22] 字节长度与字符长度
来源：http://hz.meibo888.top/gtixbgdpdz.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.sufxvd.cn/gtzorlfycd.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.wangshuangyany.cn/gtzpuqgzst.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.daria6918.cn/gtccvzsilm.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jqgfzy.top/gtrshykxnf.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.kuanghao11.cn/gtbkbaixve.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.yj202588.top/gtbteoreui.html

Ruby: s.bytesize;  s.length
来源：http://hz.xylfe.cn/gttuiklday.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.zycfv.cn/gtawbypafl.html

================================================================================
来源：http://hz.svipenyu.cn/gttokpvqxc.html

F. 文件与目录
来源：http://hz.svipenyu.cn/gtshiggbhc.html

================================================================================
来源：http://hz.zhixingplan.top/gtuopjhzze.html

[F01] 读取整个文件
来源：http://hz.hywenlv.cn/gtzavczvbv.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yj20258888.top/gtuhwauixw.html

PHP:  file_get_contents("a.txt");
来源：http://hz.shzxlz.cn/gtipmyxfvl.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.hywenlv.cn/gtodvriwcu.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.shangyingyoupin.top/gtmyyzewml.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.guannengcc.top/gtskvhmnpk.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.ehwqpu.com/gtmusszfnu.html

Ruby: File.read("a.txt")
来源：http://hz.gzhubu.top/gtkjfaozvg.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.zhongyouzk.top/gtyskvisnh.html

[F02] 逐行读取文件
来源：http://hz.zhoulong.xyz/gtqgauzghn.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.vqdsnc.cn/gttcpgsiuq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.tianlin.xyz/gtkryblsqw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.svipenyu.cn/gtvfnxhpft.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.gaohongyu789.top/gtuegemzyu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.havefunace.top/gtqasfkrlu.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.shanyushiyangtech.top/gtmhqcmdrq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.ybcxt.top/gtxhghtxcs.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.zycfv.cn/gthcqigeev.html

[F03] 写入文件（覆盖）
来源：http://hz.xuetiantiany.cn/gtajacjxcg.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.zhiwuduotai.top/gtcgomzani.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.zhengqikj.top/gtnxxomtdx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.sufxvd.cn/gtwbklkrkk.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.shanyushiyangkeji.top/gtaowsfpjx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.jinyuanbaomall.cn/gtgcpcdzie.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.yj20258.top/gtgrgcawgl.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.ehwqpu.com/gtdendjgcb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.hammf.cn/gtuvysbggd.html

[F04] 追加写入文件
来源：http://hz.zhaomingkeji.xyz/gtkmhvwycq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.wangdashe.top/gtyrigerwz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.jqgufenzy.top/gtlmtareeh.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jianghu66.top/gtvlvzgqzg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhoulong.xyz/gthqavyskf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.jinghuilouyu.cn/gtmfxucqlj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.yongpay.top/gtbjogvwdr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.cqqwz.cn/gtpoqlzawr.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.yj202588.top/gtgozodjiv.html

[F05] 判断文件或目录是否存在
来源：http://hz.jinghuilouyu.cn/gtefqxmbld.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.chenjidiqi.icu/gttzurpocf.html

PHP:  file_exists("a.txt");
来源：http://hz.ybcxt.top/gtrdfmfwru.html

JS:   fs.existsSync("a.txt")
来源：http://hz.nanxinkj.top/gtsbgzpqcm.html

TS:   fs.existsSync("a.txt")
来源：http://hz.chenjidiqi.icu/gtuhcqrlrl.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.nanxinkj.top/gtzhwkunde.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.ppjwa.cn/gtmyyvefno.html

Ruby: File.exist?("a.txt")
来源：http://hz.haohaochexian.top/gtfkmuukbb.html

C#:   File.Exists("a.txt")
来源：http://hz.ehwqpu.com/gtcrdsacih.html

[F06] 删除文件
来源：http://hz.gotoacloud.top/gtxpbmblaq.html

Py:   os.remove("a.txt")
来源：http://hz.jianghu66.top/gtukxtqtcu.html

PHP:  unlink("a.txt");
来源：http://hz.iojbl.cn/gtqnxbhgvy.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yvedp.cn/gtxqpjuyle.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.daxiang520.top/gtuguovyga.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.vqdsnc.cn/gtqdthvdcc.html

Go:   os.Remove("a.txt")
来源：http://hz.smart0.xyz/gtnyuryylk.html

Ruby: File.delete("a.txt")
来源：http://hz.tianlin.xyz/gtjbkpmcei.html

C#:   File.Delete("a.txt");
来源：http://hz.hywenlv.cn/gtwobyxatt.html

[F07] 创建目录（含多级）
来源：http://hz.feifeiyinyue.top/gtnddymkor.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.hnxiangtu.top/gtkkgwlzmy.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.jinqigfzy.top/gtjuphpauc.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.haohaochexian.top/gtkdjugarp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.dashuyun.cn/gtfwdydeal.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.yuxming.cn/gtyoptmqnv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jiagoushi.top/gtgcizbrlf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.chenjidiqi.icu/gtgfdeeutr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.xuanzx.com/gtjzcyieqe.html

[F08] 遍历目录
来源：http://hz.gzhubu.top/gtlozreari.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.nanxuanxn.top/gtpwzljkrk.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.yj202588.top/gtfivqpznu.html

JS:   fs.readdirSync("dir")
来源：http://hz.jyoumei.cn/gtbdhooedy.html

TS:   fs.readdirSync("dir")
来源：http://hz.chenjidiqi.icu/gtttthxbwu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.tianlin.xyz/gtkjwkgrsx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.sysykeji.top/gtyzdflzbc.html

Ruby: Dir.children("dir")
来源：http://hz.zhoulong.xyz/gtzcwochxq.html

C#:   Directory.GetFiles("dir")
来源：http://hz.shanyushiyangtech.top/gtgrzrbdty.html

[F09] 获取文件大小
来源：http://hz.sufxvd.cn/gtktzzcqsj.html

Py:   os.path.getsize("a.txt")
来源：http://hz.ppjwa.cn/gtsyqjfhpg.html

PHP:  filesize("a.txt");
来源：http://hz.jinyuanbaomall.cn/gtkgzpwoeu.html

JS:   fs.statSync("a.txt").size
来源：http://hz.yuanzhike.top/gtgukoowvh.html

TS:   fs.statSync("a.txt").size
来源：http://hz.zhengqikj.top/gtfatgfews.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.meibo888.top/gtasnalosw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.shuidangran.top/gteahijnwp.html

Ruby: File.size("a.txt")
来源：http://hz.ydjk.org.cn/gtujaknbuy.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yvedp.cn/gtaajganah.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.hywenlv.cn/gtafdttnvk.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.shanyushiyangtech.top/gtlztiwonh.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.vqdsnc.cn/gtprkccwcy.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.chenlongwang.top/gtlbrifvlh.html

TS:   path.extname("a.txt")
来源：http://hz.cucudq.cn/gtuwjcommp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.jlsjyb.cn/gtbneblydk.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.andypj.xyz/gtkqiuchbh.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.shuidangran.top/gtekotwvvs.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.zhengqikj.top/gtgjwehsxs.html

[F11] 复制与移动文件
来源：http://hz.shangyingyoupin.top/gtctwyhtdc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.mhx1999.top/gtiuqtmtrn.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.kuanghao11.cn/gttckcbmqg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.snrcjt.cn/gtsucqyrcj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yj20258888.top/gtggpkrclv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.yonumen.top/gtactnyazl.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.ydjk.org.cn/gttjhbzpzr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.ppjwa.cn/gtaotpofbt.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.chenzaomai.com/gtgpghggim.html

[F12] CSV 读写
来源：http://hz.cdnleiting.top/gtvslbhlya.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.chenjidiqi.icu/gtsqapmnpk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.chenzaomai.com/gtvtgjjyar.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.meibo888.top/gtlatxgbop.html

TS:   // 同上
来源：http://hz.jqgfzy.top/gtlsfacfbs.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.zhijiandao.cn/gttkpmhqkn.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.jqgfzy.top/gtvgajiwka.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.zhiwuduotai.top/gtisiqmivt.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.zhongyouzk.top/gtphdyfppu.html

================================================================================
来源：http://hz.316326.xyz/gtkbqooaan.html

G. 面向对象
来源：http://hz.redwolf501.top/gtltdwroxg.html

================================================================================
来源：http://hz.yonumen.top/gtsabxxyrb.html

[G01] 定义类
来源：http://hz.tianlin.xyz/gtertdstcw.html

Py:   class User: pass
来源：http://hz.yvedp.cn/gtvnsvfhbe.html

PHP:  class User {}
来源：http://hz.pycfn.com/gtfutuxaww.html

JS:   class User {}
来源：http://hz.pengpengdd.cyou/gtrmsirujq.html

TS:   class User { name: string = ""; }
来源：http://hz.aibaodan.cn/gtohodplez.html

Java: class User {}
来源：http://hz.quarkkingdee.top/gtmfvfwwyw.html

Go:   type User struct { Name string }
来源：http://hz.yanxiufei.cn/gtdkjzlzxz.html

Ruby: class User; end
来源：http://hz.dianchejie.cn/gtwcozbkez.html

C#:   class User {}
来源：http://hz.ywan-chungtsiang.top/gtvszqmlop.html

[G02] 构造函数
来源：http://hz.jqgufenzy.top/gthmdabrxj.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yj20258.top/gtzctchflj.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.feifeiyinyue.top/gttfbtizjl.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.hongshengwenyu.top/gttnimpnqc.html

TS:   constructor(public name: string) {}
来源：http://hz.fengsongda.top/gtjcfjjymb.html

Java: User(String name) { this.name = name; }
来源：http://hz.hysaishi.cn/gttjalpbdo.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.birdmap.top/gtpbsnpznx.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yongpay.top/gtxqdewlqc.html

C#:   public User(string name) { Name = name; }
来源：http://hz.mhx1999.top/gtqbcerdmm.html

[G03] 实例属性
来源：http://hz.havefunace.top/gtoxwhcepl.html

Py:   self.name = "x"
来源：http://hz.ehwqpu.com/gtridcichm.html

PHP:  public string $name = "x";
来源：http://hz.sufxvd.cn/gtoptiygjp.html

JS:   this.name = "x";
来源：http://hz.yangfankeji.com/gtjzzgmjeo.html

TS:   name: string = "x";
来源：http://hz.guannengcc.top/gtxvxuspqm.html

Java: private String name;
来源：http://hz.zhoulong.xyz/gtduuptgqo.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.havefunace.top/gtwbdebake.html

Ruby: @name = "x"
来源：http://hz.jqgufenzy.top/gtynhhouua.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.fzhhl.top/gtfglvrkiq.html

[G04] 定义方法
来源：http://hz.mhx1999.top/gtobostzal.html

Py:   def greet(self): return self.name
来源：http://hz.9152youxi.cn/gtnzijeent.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.ydjk.org.cn/gtwhdctvoz.html

JS:   greet() { return this.name; }
来源：http://hz.daxiang520.top/gthkzwmztc.html

TS:   greet(): string { return this.name; }
来源：http://hz.jinyuanbaomall.cn/gtmmojyawu.html

Java: String greet() { return name; }
来源：http://hz.hammf.cn/gtywoniagn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.0kj1m.cn/gtgpfcdetq.html

Ruby: def greet; @name; end
来源：http://hz.fzhhl.top/gtufhaposc.html

C#:   public string Greet() => Name;
来源：http://hz.guowangkeji.top/gtvprnnfid.html

[G05] 继承
来源：http://hz.dianchejie.cn/gttveqxfdl.html

Py:   class Admin(User): pass
来源：http://hz.ppjwa.cn/gtdicipuni.html

PHP:  class Admin extends User {}
来源：http://hz.zhengqikj.top/gtfxmeunlf.html

JS:   class Admin extends User {}
来源：http://hz.cdnleiting.top/gtmiktpvef.html

TS:   class Admin extends User {}
来源：http://hz.jyoumei.cn/gtniunylve.html

Java: class Admin extends User {}
来源：http://hz.9152youxi.cn/gtqnndrgfp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yvedp.cn/gtjppyvsbo.html

Ruby: class Admin < User; end
来源：http://hz.zhixingplan.top/gtgklpljda.html

C#:   class Admin : User {}
来源：http://hz.tian-w.cn/gtawttrtio.html

[G06] 重写方法
来源：http://hz.jlsjyb.cn/gtwkgectre.html

Py:   def greet(self): return "admin"
来源：http://hz.yuanzhike.top/gtaspomylj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.ydzc1.top/gtawydfpnq.html

JS:   greet() { return "admin"; }
来源：http://hz.birdmap.top/gtbakxfgwl.html

TS:   greet(): string { return "admin"; }
来源：http://hz.cucudq.cn/gtkejzbyuf.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.nwbrower.top/gtqazdogju.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.iojbl.cn/gtkxtsimym.html

Ruby: def greet; "admin"; end
来源：http://hz.jinghuilouyu.cn/gtslvbofmm.html

C#:   public override string Greet() => "admin";
来源：http://hz.ivvv.top/gtietzdmgm.html

[G07] 调用父类方法
来源：http://hz.zhijiandao.cn/gtoopnwzst.html

Py:   super().greet()
来源：http://hz.guannengcc.top/gtsdbawyhw.html

PHP:  parent::greet();
来源：http://hz.haohaochexian.top/gtyxovpvlo.html

JS:   super.greet();
来源：http://hz.fengsongda.top/gthivkchaf.html

TS:   super.greet();
来源：http://hz.dianchejie.cn/gtxcllbnfi.html

Java: super.greet();
来源：http://hz.ybcxt.top/gtmudqwcbc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yj202588.top/gtgenshqvs.html

Ruby: super
来源：http://hz.meibo888.top/gtqlynkrdp.html

C#:   base.Greet();
来源：http://hz.ivvv.top/gtbfkyjnpw.html

[G08] 静态方法与属性
来源：http://hz.meibo888.top/gtxuqsodxh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.9152youxi.cn/gtqrplzrtb.html

PHP:  public static function f() {}
来源：http://hz.sweek.top/gtzplrsoxj.html

JS:   static f() {}
来源：http://hz.shanyushiyangtech.top/gtkwfdatim.html

TS:   static f(): void {}
来源：http://hz.pycfn.com/gtnycptnqz.html

Java: static void f() {}
来源：http://hz.bjfxy.top/gtvgmtedmv.html


<!-- 参考信息 -->