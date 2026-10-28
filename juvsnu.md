代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://hz.ivvv.top/gtdcpbjjuz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.jinqigufen.top/gtnoksxqgl.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.daxiang520.top/gtgydaewzq.html

JS:   "7".padStart(3, "0")
来源：http://hz.yj20258888.top/gtqtxqxjgq.html

TS:   "7".padStart(3, "0")
来源：http://hz.cheryme.top/gtvoqovmle.html

Java: String.format("%03d", 7)
来源：http://hz.jianghu66.top/gtsuqtdvbv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.hongshengwenyu.top/gtgfnqgptn.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.jqgfzy.top/gttzlxbnbn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.redwolf501.top/gtzzjfyunk.html

[E11] 反转字符串
来源：http://hz.jqgfzy.top/gtebapwdld.html

Py:   s[::-1]
来源：http://hz.feifeiyinyue.top/gtajkfscop.html

PHP:  strrev($s);
来源：http://hz.zhengqikj.top/gtvuwnfrwj.html

JS:   [...s].reverse().join("")
来源：http://hz.fzhhl.top/gthdivxpau.html

TS:   [...s].reverse().join("")
来源：http://hz.tian-w.cn/gtbyzmyasr.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.shanyushiyangkeji.top/gtppsusdoy.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.guannengcc.top/gtmjyayepl.html

Ruby: s.reverse
来源：http://hz.bjfxy.top/gthosglmdg.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.yj20258.top/gtbeggefzn.html

[E12] 统计某字符出现次数
来源：http://hz.jinqigfzy.top/gtkxudsjda.html

Py:   s.count("a")
来源：http://hz.xuanzx.com/gtxghktjsi.html

PHP:  substr_count($s, "a");
来源：http://hz.yongpay.top/gtkziunxyi.html

JS:   s.split("a").length - 1
来源：http://hz.aizwys.cn/gttxelrysr.html

TS:   s.split("a").length - 1
来源：http://hz.mhx1999.top/gtvdypkusm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.chenlongwang.top/gteeekblcf.html

Go:   strings.Count(s, "a")
来源：http://hz.zhijiandao.cn/gtbefywpuj.html

Ruby: s.count("a")
来源：http://hz.pycfn.com/gthaqjwkkr.html

C#:   s.Count(c => c == 'a')
来源：http://hz.zhongyouzk.top/gtzlyzwgmu.html

[E13] 逐字符遍历
来源：http://hz.zhixingplan.top/gtriwhhxrk.html

Py:   for ch in s: print(ch)
来源：http://hz.nwbrower.top/gtddgjpbwc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.shanyushiyangkeji.top/gttzuugzia.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.fengsongda.top/gtmzudvusx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.haohaochexian.top/gtnwwpmsid.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.birdmap.top/gtdjqgmgoy.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.quarkkingdee.top/gtxvonaipx.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.jinghuilouyu.cn/gtktmjmnla.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.quarkkingdee.top/gtbaiifvtc.html

[E14] URL 编码与 Base64
来源：http://hz.shangyingyoupin.top/gtasohqmdx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.dashuyun.cn/gtkvypbfte.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.andypj.xyz/gtieuqqxkh.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.yj20258.top/gtxnthvwbc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.jinyuanbaomall.cn/gtymyoldlr.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.jiagoushi.top/gtefkknosc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.chenlongwang.top/gtmqjaucmj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.zhiwuduotai.top/gtcsvfbbnv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.hywenlv.cn/gtanhmefuj.html

[E15] HTML 转义 / 反转义
来源：http://hz.ybcxt.top/gtbefpbbvy.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.mhx1999.top/gtjafjidzq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.gzhubu.top/gtlhtjrxui.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.316326.xyz/gtqkivthsp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.daxiang520.top/gtfqjnmtdv.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.jqgfzy.top/gtyheskwiq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.yongpay.top/gtpogyuedr.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.jinghuilouyu.cn/gtnenkayhh.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.cucudq.cn/gturqjypwx.html

[E16] 数字千分位
来源：http://hz.birdmap.top/gtaqdqwfms.html

Py:   f"{1234567:,}"
来源：http://hz.cqqwz.cn/gtxvmhpevs.html

PHP:  number_format(1234567);
来源：http://hz.ehwqpu.com/gtmmragyba.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.dianchejie.cn/gtvurfbfpk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.cheryme.top/gtrqwkrxvh.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.pengpengdd.cyou/gtbemcsyyb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.yonumen.top/gtbwjwemeg.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.chenlongwang.top/gtbyuobzke.html

C#:   1234567.ToString("N0")
来源：http://hz.bjfxy.top/gtntvwavyb.html

[E17] 首字母大写
来源：http://hz.chenzaomai.com/gtwbxhionm.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.redwolf501.top/gtypadesuw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.jlsjyb.cn/gtaeccsyxp.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.shangyingyoupin.top/gtkjbkvcdv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ydzc1.top/gtjcttxsdt.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.jinqigufen.top/gtuvlolmkm.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.wangdashe.top/gtfzcnbugd.html

Ruby: s.capitalize
来源：http://hz.zhaomingkeji.xyz/gtyewfskrz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.zhoulong.xyz/gtuncvfcuf.html

[E18] 模板占位符替换
来源：http://hz.zycfv.cn/gtfgpvdafp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.yueranfly.top/gtnxpfbciu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.nanxinkj.top/gtxrzyidzt.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.jqgufenzy.top/gtflcbpmfx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.zhoulong.xyz/gtwzinlfsn.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.yj20258.top/gtxdilbjpe.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.fzhhl.top/gtcziabvnn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.bjfxy.top/gtgmbgnqdg.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.feifeiyinyue.top/gtivynogxm.html

[E19] 多行文本按行拆分
来源：http://hz.jiagoushi.top/gthismhnrq.html

Py:   s.splitlines()
来源：http://hz.shangyingyoupin.top/gtsrkzydfk.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.nanxinkj.top/gtsmhrbfus.html

JS:   s.split(/\r?\n/)
来源：http://hz.sufxvd.cn/gtxwrxlhtr.html

TS:   s.split(/\r?\n/)
来源：http://hz.ppjwa.cn/gtwctlhejg.html

Java: s.lines().toList()
来源：http://hz.hammf.cn/gtdyvrvtbd.html

Go:   strings.Split(s, "\n")
来源：http://hz.sysykeji.top/gturytjzue.html

Ruby: s.lines
来源：http://hz.cashguo.top/gtkpvcjsji.html

C#:   s.Split('\n')
来源：http://hz.gzhubu.top/gttpzzggdz.html

[E20] 判断字符串是否为空
来源：http://hz.fengsongda.top/gtiozvvlvv.html

Py:   if not s:
来源：http://hz.kuanghao11.cn/gttyebbgfj.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.0kj1m.cn/gtvihdyxij.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.svipenyu.cn/gtzircpxft.html

TS:   if (s === "") {}
来源：http://hz.gogol.net.cn/gthxudvqem.html

Java: if (s.isEmpty()) {}
来源：http://hz.zhoulong.xyz/gtptzmfxcz.html

Go:   if s == "" {}
来源：http://hz.vqdsnc.cn/gtwstndzbo.html

Ruby: if s.empty?
来源：http://hz.tian-w.cn/gtchtacuqr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.zhiwuduotai.top/gttjqwccwe.html

[E21] 超长截断加省略号
来源：http://hz.xinyue.icu/gtvnyczqon.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.hfpthk.cn/gtyvtboqvf.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.nwbrower.top/gtiexoluia.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ydjk.org.cn/gtxjnihyos.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.cashguo.top/gtvjfajvxo.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.dashuyun.cn/gtnvjnhnxc.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.yanxiufei.cn/gtxqnznaak.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.fengsongda.top/gtfdvvuguk.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.0kj1m.cn/gtmocanyxt.html

[E22] 字节长度与字符长度
来源：http://hz.tianlin.xyz/gtkwkhshaw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.cdnleiting.top/gtwjrgbfee.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhaomingkeji.xyz/gtbqngvrof.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.cashguo.top/gttjbhgriw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.xuanzx.com/gtekzmgnvs.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.shzxlz.cn/gtvbnmiyhr.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.havefunace.top/gtlejwbuvf.html

Ruby: s.bytesize;  s.length
来源：http://hz.cqqwz.cn/gttljgtvph.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.0kj1m.cn/gtnvvwtvzo.html

================================================================================
来源：http://hz.dianchejie.cn/gtotpienju.html

F. 文件与目录
来源：http://hz.xuanzx.com/gtavhkkyfm.html

================================================================================
来源：http://hz.jqgfzy.top/gteaioinlk.html

[F01] 读取整个文件
来源：http://hz.nwbrower.top/gtqnuchuax.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.ydzc1.top/gthcwbluvc.html

PHP:  file_get_contents("a.txt");
来源：http://hz.hywenlv.cn/gtfbmzeyjz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.hysaishi.cn/gtfbjhtklv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.jinghuilouyu.cn/gtuidmsefk.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.meibo888.top/gtbkshikew.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.sufxvd.cn/gtywenrclg.html

Ruby: File.read("a.txt")
来源：http://hz.zhongyouzk.top/gtjjjobzsr.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.fengsongda.top/gtjlrldtpr.html

[F02] 逐行读取文件
来源：http://hz.wangshuangyany.cn/gtoqzdqftq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.jqgfzy.top/gtikciecrk.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.haohaochexian.top/gtnfsvnabu.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xziqi.cn/gtcqeaixyz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ydjk.org.cn/gtnnewsdbc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.hongshengwenyu.top/gturuedtwj.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.sufxvd.cn/gtakwjgqfz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.aizwys.cn/gtodikxptu.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.haohaochexian.top/gtgdkgkbft.html

[F03] 写入文件（覆盖）
来源：http://hz.yuanzhike.top/gtgbonrhol.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.chenlongwang.top/gtzxkwdcrd.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.wangdashe.top/gtgxneiwul.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.aizwys.cn/gtqbevdhny.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.0kj1m.cn/gtyasyeiul.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.jinqigufen.top/gtfvrmhlwt.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.gogol.net.cn/gttacvzmeb.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.zdqjudy.top/gtihnwmqas.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.jinqigfzy.top/gttkmzzrff.html

[F04] 追加写入文件
来源：http://hz.xziqi.cn/gtejiypnzr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.redwolf501.top/gtbtgcnjlr.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.dianchejie.cn/gtndanmvxg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.guannengcc.top/gtimwdezqv.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.vqdsnc.cn/gtdbmuukuw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.316326.xyz/gthnnyvceh.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.smart0.xyz/gtsycvrfuu.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.dianchejie.cn/gtpfnbqewo.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.jinghuilouyu.cn/gtfufbotzg.html

[F05] 判断文件或目录是否存在
来源：http://hz.fzhhl.top/gtkgjkixji.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.nanxinkj.top/gtbfpwjzkj.html

PHP:  file_exists("a.txt");
来源：http://hz.jqgfzy.top/gtikwypuvz.html

JS:   fs.existsSync("a.txt")
来源：http://hz.hfpthk.cn/gtcmckjocn.html

TS:   fs.existsSync("a.txt")
来源：http://hz.jianghu66.top/gtjwdtvcus.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.dashuyun.cn/gtnsvdxbjr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.yongpay.top/gtptfkzehf.html

Ruby: File.exist?("a.txt")
来源：http://hz.ivvv.top/gttjmvboxf.html

C#:   File.Exists("a.txt")
来源：http://hz.cqqwz.cn/gtmxvjoxoh.html

[F06] 删除文件
来源：http://hz.redwolf501.top/gttbdzbtno.html

Py:   os.remove("a.txt")
来源：http://hz.yuxming.cn/gtmwnwzewk.html

PHP:  unlink("a.txt");
来源：http://hz.xuetiantiany.cn/gtikjrtlgi.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yonumen.top/gtzhpzvyxh.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.sufxvd.cn/gtubtazcrw.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.pengpengdd.cyou/gtyuzouagf.html

Go:   os.Remove("a.txt")
来源：http://hz.aibaodan.cn/gtvytucivl.html

Ruby: File.delete("a.txt")
来源：http://hz.nanxuanxn.top/gtadplfpvo.html

C#:   File.Delete("a.txt");
来源：http://hz.cashguo.top/gtgasmnsyi.html

[F07] 创建目录（含多级）
来源：http://hz.pycfn.com/gtokmbhnvl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.zhiwuduotai.top/gtrrrfvaxt.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.quarkkingdee.top/gtfzzjxrdn.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.redwolf501.top/gtlehzwztv.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.guannengcc.top/gtndkyjygf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.ybcxt.top/gtxvhstcim.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.xuanzx.com/gtfastckpl.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.quarkkingdee.top/gtrhmxkdtl.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.shanyushiyangkeji.top/gtdtcdewvq.html

[F08] 遍历目录
来源：http://hz.sxryk.cn/gtflyyqxhd.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.shuidangran.top/gtaocusloe.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.jqgfzy.top/gtbjtfxxhg.html

JS:   fs.readdirSync("dir")
来源：http://hz.havefunace.top/gtaxcibxme.html

TS:   fs.readdirSync("dir")
来源：http://hz.tanke756.top/gtkwwipmmw.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.hnqzz.top/gtgyqbytdk.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.zhixingplan.top/gtupckxodn.html

Ruby: Dir.children("dir")
来源：http://hz.hnqzz.top/gtrsdfxelh.html

C#:   Directory.GetFiles("dir")
来源：http://hz.fengsongda.top/gtedyhysgu.html

[F09] 获取文件大小
来源：http://hz.redwolf501.top/gtevdqfqez.html

Py:   os.path.getsize("a.txt")
来源：http://hz.ehwqpu.com/gtggcmhgdc.html

PHP:  filesize("a.txt");
来源：http://hz.aibaodan.cn/gtltruyjsw.html

JS:   fs.statSync("a.txt").size
来源：http://hz.yj20258.top/gthibzcvna.html

TS:   fs.statSync("a.txt").size
来源：http://hz.gotoacloud.top/gtcqnvmwps.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.smart0.xyz/gtswdkclxk.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.zhiwuduotai.top/gtxsfosxqz.html

Ruby: File.size("a.txt")
来源：http://hz.gzhubu.top/gtteyvwnqb.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.ydjk.org.cn/gtuqoygbtm.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.gzhubu.top/gtietacfbz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.zhixingplan.top/gtwnkfuwbj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.jiagoushi.top/gtmakxgepj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.wangshuangyany.cn/gtafsrpmxf.html

TS:   path.extname("a.txt")
来源：http://hz.ppjwa.cn/gtbznrehvq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.hywenlv.cn/gtgabutqwv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.shangyingyoupin.top/gtrzqpmkfw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.0kj1m.cn/gtnkdhhoin.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.shanyushiyangtech.top/gtsagvvzkc.html

[F11] 复制与移动文件
来源：http://hz.yongpay.top/gtruyzlcin.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.shzxlz.cn/gtojoypbfs.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.meibo888.top/gtuncrjlbi.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ppjwa.cn/gthbmzvvfl.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xingfuxueyuan.xyz/gtrzwrmkbm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.cashguo.top/gthdrzxfif.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jinqigufen.top/gthksifqim.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.guowangkeji.top/gtjgfrwepv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.fzhhl.top/gtzszcbnre.html

[F12] CSV 读写
来源：http://hz.dashuyun.cn/gtpxdneoms.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.cdnleiting.top/gtopcmhtvn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.pengpengdd.cyou/gtxezfvmuu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.zhaomingkeji.xyz/gteqqzznff.html

TS:   // 同上
来源：http://hz.dashuyun.cn/gtbjyuwktz.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.aibaodan.cn/gtbnmjgewn.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yuanzhike.top/gtlevqoujv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.shanyushiyangtech.top/gtfgcazina.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.tanke756.top/gtqxbtsoaf.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtedkoxjwl.html

G. 面向对象
来源：http://hz.xuanzx.com/gtqoorksbw.html

================================================================================
来源：http://hz.hammf.cn/gttjucshqm.html

[G01] 定义类
来源：http://hz.jinghuilouyu.cn/gtjzizafmg.html

Py:   class User: pass
来源：http://hz.52xcode.cn/gtmphakffg.html

PHP:  class User {}
来源：http://hz.nanxuanxn.top/gttvwradwi.html

JS:   class User {}
来源：http://hz.zdqjudy.top/gthegyjdiq.html

TS:   class User { name: string = ""; }
来源：http://hz.cucudq.cn/gtdfsiumpa.html

Java: class User {}
来源：http://hz.sufxvd.cn/gtctpkanmz.html

Go:   type User struct { Name string }
来源：http://hz.ydjk.org.cn/gtczwquqwz.html

Ruby: class User; end
来源：http://hz.feifeiyinyue.top/gtyipnobpz.html

C#:   class User {}
来源：http://hz.ybcxt.top/gtkikpgdng.html

[G02] 构造函数
来源：http://hz.svipenyu.cn/gtnfglslhj.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.jinqigufen.top/gtnrvmyuqz.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yueranfly.top/gtmrsvainb.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.cashguo.top/gtghjrvzeg.html

TS:   constructor(public name: string) {}
来源：http://hz.jlsjyb.cn/gtbqmwqtsc.html

Java: User(String name) { this.name = name; }
来源：http://hz.vqdsnc.cn/gtvrwbtrcg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.daria6918.cn/gthlbbvrqv.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.redwolf501.top/gtpjrxxfrq.html

C#:   public User(string name) { Name = name; }
来源：http://hz.xuanzx.com/gtflwjicbc.html

[G03] 实例属性
来源：http://hz.cdnleiting.top/gtetmrdouq.html

Py:   self.name = "x"
来源：http://hz.cucudq.cn/gtpsviecwo.html

PHP:  public string $name = "x";
来源：http://hz.hnqzz.top/gtkdxdzhhl.html

JS:   this.name = "x";
来源：http://hz.shanyushiyangtech.top/gthlakursp.html

TS:   name: string = "x";
来源：http://hz.nanxinkj.top/gttuawuwsd.html

Java: private String name;
来源：http://hz.xinyue.icu/gtyqqsygcz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.gogol.net.cn/gtvhxtnigo.html

Ruby: @name = "x"
来源：http://hz.daria6918.cn/gtamwbozev.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.9152youxi.cn/gtuzehqmhm.html

[G04] 定义方法
来源：http://hz.nanxuanxn.top/gtaanzlomd.html

Py:   def greet(self): return self.name
来源：http://hz.zhiwuduotai.top/gtoscaejqa.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.haohaochexian.top/gtthoqgssz.html

JS:   greet() { return this.name; }
来源：http://hz.ybcxt.top/gtdangvyha.html

TS:   greet(): string { return this.name; }
来源：http://hz.0kj1m.cn/gthvahkrcm.html

Java: String greet() { return name; }
来源：http://hz.shangyingyoupin.top/gtlvngguxg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.hnxiangtu.top/gtvqaqyezp.html

Ruby: def greet; @name; end
来源：http://hz.hysaishi.cn/gttbdbsddm.html

C#:   public string Greet() => Name;
来源：http://hz.bjfxy.top/gtkpasatfd.html

[G05] 继承
来源：http://hz.yangfankeji.com/gtqjtypdec.html

Py:   class Admin(User): pass
来源：http://hz.dashuyun.cn/gtjqrjqtff.html

PHP:  class Admin extends User {}
来源：http://hz.redwolf501.top/gtkmaghclr.html

JS:   class Admin extends User {}
来源：http://hz.daxiang520.top/gtuyplypgb.html

TS:   class Admin extends User {}
来源：http://hz.ybcxt.top/gtqgbscdwg.html

Java: class Admin extends User {}
来源：http://hz.zycfv.cn/gtwnvzjuah.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yueranfly.top/gtfxuvmjiz.html

Ruby: class Admin < User; end
来源：http://hz.tian-w.cn/gtvjmaahsi.html

C#:   class Admin : User {}
来源：http://hz.xuanzx.com/gtrshitqpd.html

[G06] 重写方法
来源：http://hz.xingfuxueyuan.xyz/gthfimjwxq.html

Py:   def greet(self): return "admin"
来源：http://hz.andypj.xyz/gtcgtnjbli.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.52xcode.cn/gtczcvogtv.html

JS:   greet() { return "admin"; }
来源：http://hz.bjfxy.top/gtfcdivwci.html

TS:   greet(): string { return "admin"; }
来源：http://hz.gogol.net.cn/gtbkarohhx.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.quarkkingdee.top/gtvmfqpfkr.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.hysaishi.cn/gtggtylsis.html

Ruby: def greet; "admin"; end
来源：http://hz.xuanzx.com/gtehcnezsz.html

C#:   public override string Greet() => "admin";
来源：http://hz.yj20258.top/gtrbtayjqh.html

[G07] 调用父类方法
来源：http://hz.cucudq.cn/gtjsaaukwc.html

Py:   super().greet()
来源：http://hz.smart0.xyz/gthessowcj.html

PHP:  parent::greet();
来源：http://hz.smart0.xyz/gtngumnnsn.html

JS:   super.greet();
来源：http://hz.wangshuangyany.cn/gtahthmpek.html

TS:   super.greet();
来源：http://hz.ivvv.top/gtkvwwwvpc.html

Java: super.greet();
来源：http://hz.gogol.net.cn/gtunnjzjrb.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.52xcode.cn/gtimnvvshr.html

Ruby: super
来源：http://hz.jianghu66.top/gtnefkezol.html

C#:   base.Greet();
来源：http://hz.9152youxi.cn/gtjjfqrgwy.html

[G08] 静态方法与属性
来源：http://hz.fzhhl.top/gtdwlckqjy.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.ybcxt.top/gtgvcxqckt.html

PHP:  public static function f() {}
来源：http://hz.zycfv.cn/gtfaqecngj.html

JS:   static f() {}
来源：http://hz.yueranfly.top/gtjpmiyrrg.html

TS:   static f(): void {}
来源：http://hz.tian-w.cn/gtnixgjend.html

Java: static void f() {}
来源：http://hz.cqqwz.cn/gtyojlzfox.html


<!-- 参考信息 -->