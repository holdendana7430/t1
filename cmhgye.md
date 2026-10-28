代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://hz.0kj1m.cn/gtodckhmwe.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.bjfxy.top/gtjjivyvqz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.mhx1999.top/gtsyvftifh.html

JS:   "7".padStart(3, "0")
来源：http://hz.sweek.top/gtqowmlkqp.html

TS:   "7".padStart(3, "0")
来源：http://hz.havefunace.top/gttndknfye.html

Java: String.format("%03d", 7)
来源：http://hz.cucudq.cn/gtrbpyfgdz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.yuanzhike.top/gtmyhblnfj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.zhixingplan.top/gtulhxxymv.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.zhoulong.xyz/gtrczpiewl.html

[E11] 反转字符串
来源：http://hz.hysaishi.cn/gtgffuzotz.html

Py:   s[::-1]
来源：http://hz.zhaomingkeji.xyz/gtjbvkqjau.html

PHP:  strrev($s);
来源：http://hz.kuanghao11.cn/gtzuspomoa.html

JS:   [...s].reverse().join("")
来源：http://hz.bjfxy.top/gtqfdsqzat.html

TS:   [...s].reverse().join("")
来源：http://hz.jianghu66.top/gtbdgrkafg.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.tianlin.xyz/gtyhbxusdy.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.fzhhl.top/gtkyeyotbr.html

Ruby: s.reverse
来源：http://hz.shanyushiyangtech.top/gtbqymnygx.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.yj20258.top/gtoimoouds.html

[E12] 统计某字符出现次数
来源：http://hz.zhoulong.xyz/gtakfkuyna.html

Py:   s.count("a")
来源：http://hz.hammf.cn/gtblfdphdi.html

PHP:  substr_count($s, "a");
来源：http://hz.nanxinkj.top/gtcgwiygbf.html

JS:   s.split("a").length - 1
来源：http://hz.ppjwa.cn/gtahqlnpfs.html

TS:   s.split("a").length - 1
来源：http://hz.daxiang520.top/gtwzlorlpx.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.yj20258888.top/gtsjjonlmp.html

Go:   strings.Count(s, "a")
来源：http://hz.jqgufenzy.top/gtyxxgdbwx.html

Ruby: s.count("a")
来源：http://hz.gaohongyu789.top/gtrouzgcqy.html

C#:   s.Count(c => c == 'a')
来源：http://hz.shuidangran.top/gtexgjmgdg.html

[E13] 逐字符遍历
来源：http://hz.shanyushiyangkeji.top/gtyyondnxp.html

Py:   for ch in s: print(ch)
来源：http://hz.ppjwa.cn/gtwfbfjrwl.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.jinqigufen.top/gtujcihabx.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.c1oappe.top/gtuklatmrh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.hfpthk.cn/gtmiyhewca.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.hnxiangtu.top/gtuqgydvcu.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.jqgufenzy.top/gtbivffqyq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.jinyuanbaomall.cn/gtwyjoksku.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.fzhhl.top/gtfxyyheme.html

[E14] URL 编码与 Base64
来源：http://hz.zdqjudy.top/gtkyzgraky.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.zhixingplan.top/gtvtprbwsi.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.smart0.xyz/gtgryzlxtu.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.316326.xyz/gthqvkgcvb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.zdqjudy.top/gtkypzglig.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.aibaodan.cn/gtbrrajuev.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.yangfankeji.com/gtbavmwbfm.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.guannengcc.top/gtfpmxmnch.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.sweek.top/gtxveiodqg.html

[E15] HTML 转义 / 反转义
来源：http://hz.zhijiandao.cn/gtnahaywkx.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.jinghuilouyu.cn/gtzdgkpucu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.xuetiantiany.cn/gttbzvmqhx.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.xuanzx.com/gtzygmejor.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.yueranfly.top/gtofjvwdik.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.52xcode.cn/gtfyravbem.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.hammf.cn/gtynkspmeq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.yuanzhike.top/gtiglpiqlj.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.zhongyouzk.top/gtdpdplqxn.html

[E16] 数字千分位
来源：http://hz.zhoulong.xyz/gtxmuvcwat.html

Py:   f"{1234567:,}"
来源：http://hz.tanke756.top/gtcetetzeu.html

PHP:  number_format(1234567);
来源：http://hz.shuidangran.top/gtxbadqafw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.yuxming.cn/gtaqdjtbhq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.chenjidiqi.icu/gtvgnlfubg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.redwolf501.top/gthlppjyyp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.gaohongyu789.top/gtlilxoiif.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.zhijiandao.cn/gtpkeiagbu.html

C#:   1234567.ToString("N0")
来源：http://hz.daxiang520.top/gtsgaovysx.html

[E17] 首字母大写
来源：http://hz.zdqjudy.top/gtaenyynbs.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.wangshuangyany.cn/gtlvyjapak.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.dianchejie.cn/gtrsesalxy.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.chenjidiqi.icu/gtorsdjnub.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.tianlin.xyz/gttqqlricv.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.sxryk.cn/gtdppvssfp.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.sweek.top/gtrzwjyjbi.html

Ruby: s.capitalize
来源：http://hz.sxryk.cn/gtxxlysbts.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.jiagoushi.top/gtechzkptb.html

[E18] 模板占位符替换
来源：http://hz.daxiang520.top/gtcsbrbhzw.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.fengsongda.top/gtfoczkldw.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.aibaodan.cn/gtdbppjkvw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.havefunace.top/gtiqxvlwxa.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.gotoacloud.top/gttltkywda.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.bjfxy.top/gtooglguuo.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.hnqzz.top/gtgokrtatn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.aizwys.cn/gtvggjqyta.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.jianghu66.top/gthoebxfte.html

[E19] 多行文本按行拆分
来源：http://hz.zycfv.cn/gterrzscgz.html

Py:   s.splitlines()
来源：http://hz.tian-w.cn/gtrwxivdke.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.birdmap.top/gtlutiezke.html

JS:   s.split(/\r?\n/)
来源：http://hz.feifeiyinyue.top/gtzxbqqcsv.html

TS:   s.split(/\r?\n/)
来源：http://hz.cheryme.top/gtqmjygysa.html

Java: s.lines().toList()
来源：http://hz.ybcxt.top/gttqtqnxzs.html

Go:   strings.Split(s, "\n")
来源：http://hz.yvedp.cn/gtwknzrnmb.html

Ruby: s.lines
来源：http://hz.andypj.xyz/gtciacjptt.html

C#:   s.Split('\n')
来源：http://hz.yvedp.cn/gtroelcjgn.html

[E20] 判断字符串是否为空
来源：http://hz.cashguo.top/gtmxhkzlit.html

Py:   if not s:
来源：http://hz.chenzaomai.com/gtffkteqem.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.hnxiangtu.top/gteghdtvtw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.0kj1m.cn/gtqdpefqbm.html

TS:   if (s === "") {}
来源：http://hz.ywan-chungtsiang.top/gthqjvmnwj.html

Java: if (s.isEmpty()) {}
来源：http://hz.dianchejie.cn/gtxktxcaud.html

Go:   if s == "" {}
来源：http://hz.yj20258.top/gtvahminpy.html

Ruby: if s.empty?
来源：http://hz.cqqwz.cn/gtyysqncht.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.hywenlv.cn/gtvkieprbs.html

[E21] 超长截断加省略号
来源：http://hz.wangshuangyany.cn/gtjrxdhrje.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.gogol.net.cn/gtoidsstev.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.hongshengwenyu.top/gtnadcnpmx.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.svipenyu.cn/gtmjamsxmv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.nanxinkj.top/gtnsasvwld.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.hongshengwenyu.top/gtjxzuybhx.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.redwolf501.top/gteeyeickl.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.kuanghao11.cn/gtitrdydzj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.birdmap.top/gtmeyujtjc.html

[E22] 字节长度与字符长度
来源：http://hz.xuanzx.com/gtmbyvlbvq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.52xcode.cn/gtcibbocrh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.shanyushiyangtech.top/gtnggcalbp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.xingfuxueyuan.xyz/gtojhpsmgy.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.mhx1999.top/gtfzsyowtn.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.nanxuanxn.top/gteoahmgri.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.cashguo.top/gtosoeohxu.html

Ruby: s.bytesize;  s.length
来源：http://hz.xinyue.icu/gtckeripsc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.yj20258.top/gtygivyeic.html

================================================================================
来源：http://hz.ydzc1.top/gtkwqgiygk.html

F. 文件与目录
来源：http://hz.nanxinkj.top/gtogfwzasa.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtgzqrqmkv.html

[F01] 读取整个文件
来源：http://hz.dianchejie.cn/gttnkjbbgw.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.haohaochexian.top/gtvcxfojfy.html

PHP:  file_get_contents("a.txt");
来源：http://hz.sxryk.cn/gtlituswca.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.nanxinkj.top/gthfmowubm.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.ywan-chungtsiang.top/gtttqzidni.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.xziqi.cn/gtukibflyr.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.ydjk.org.cn/gtogtcmtac.html

Ruby: File.read("a.txt")
来源：http://hz.zhixingplan.top/gteushphyu.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yuanzhike.top/gtfgzdgxog.html

[F02] 逐行读取文件
来源：http://hz.hammf.cn/gthrdncbcy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.yuxming.cn/gtafhpmfhw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.yuanzhike.top/gtylnwuanj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hnqzz.top/gtcemuuybc.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jlsjyb.cn/gtkcsdwxex.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.hongshengwenyu.top/gtkcjxdrqn.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.sxryk.cn/gtgkrreyki.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.daria6918.cn/gtrjvqkfxv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.dianchejie.cn/gtgzgcudoq.html

[F03] 写入文件（覆盖）
来源：http://hz.jinqigufen.top/gttrfhaath.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.yuanzhike.top/gtccubiocw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.316326.xyz/gtyryxxupi.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhongyouzk.top/gtemnljerg.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.tian-w.cn/gtsgcnqsms.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.jinyuanbaomall.cn/gtuupqpbjh.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.gzhubu.top/gtgitqoqzi.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.yj202588.top/gtdymkowdx.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.nanxuanxn.top/gtqiwntirf.html

[F04] 追加写入文件
来源：http://hz.jyoumei.cn/gtqtdufxio.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.guowangkeji.top/gtgmmzfbso.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.xinyue.icu/gtobedbwcg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.cdnleiting.top/gtupnyokvg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.quarkkingdee.top/gtavwuonvv.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.yj202588.top/gtyhxihprf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.wangdashe.top/gtpjvqwrms.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.xuanzx.com/gtjnyalfhh.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.yvedp.cn/gtmlvatwdk.html

[F05] 判断文件或目录是否存在
来源：http://hz.jqgufenzy.top/gtiyjxroir.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.fengsongda.top/gtmzvmvqvd.html

PHP:  file_exists("a.txt");
来源：http://hz.aibaodan.cn/gtsynlzmbq.html

JS:   fs.existsSync("a.txt")
来源：http://hz.xylfe.cn/gtamtzsxmj.html

TS:   fs.existsSync("a.txt")
来源：http://hz.ywan-chungtsiang.top/gtshqbtttm.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.yuxming.cn/gtgpsulwto.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.jianghu66.top/gtotahpmdb.html

Ruby: File.exist?("a.txt")
来源：http://hz.yanxiufei.cn/gtunlnqmqv.html

C#:   File.Exists("a.txt")
来源：http://hz.52xcode.cn/gtczfomjfd.html

[F06] 删除文件
来源：http://hz.yangfankeji.com/gtndmmqioj.html

Py:   os.remove("a.txt")
来源：http://hz.shanyushiyangtech.top/gteopdwqtj.html

PHP:  unlink("a.txt");
来源：http://hz.guowangkeji.top/gtasngwril.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.pycfn.com/gtfjlfvbnl.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.9152youxi.cn/gtshbqgwds.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.meibo888.top/gtzfxvijnk.html

Go:   os.Remove("a.txt")
来源：http://hz.hongshengwenyu.top/gtdhpxpmpj.html

Ruby: File.delete("a.txt")
来源：http://hz.tanke756.top/gtsmgpawzs.html

C#:   File.Delete("a.txt");
来源：http://hz.tian-w.cn/gtgjainqnj.html

[F07] 创建目录（含多级）
来源：http://hz.52xcode.cn/gtfwnnrsen.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.havefunace.top/gtyzhrjxfi.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.jqgufenzy.top/gteoeglsvg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yangfankeji.com/gtylcapcaj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.xziqi.cn/gtngvcvtgk.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.zhixingplan.top/gthapekugz.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jlsjyb.cn/gtdbsipuxd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.mhx1999.top/gtljfqigqj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.wangdashe.top/gtxdpidfht.html

[F08] 遍历目录
来源：http://hz.hywenlv.cn/gttyuoiuek.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.kuanghao11.cn/gtphdtavhl.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.sufxvd.cn/gtwtikjnlg.html

JS:   fs.readdirSync("dir")
来源：http://hz.vqdsnc.cn/gtmkeswjei.html

TS:   fs.readdirSync("dir")
来源：http://hz.fengsongda.top/gtvmsvzmvz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.hnqzz.top/gtnggstlrz.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yueranfly.top/gttaflwycn.html

Ruby: Dir.children("dir")
来源：http://hz.hammf.cn/gtieeikmhb.html

C#:   Directory.GetFiles("dir")
来源：http://hz.quarkkingdee.top/gtvszmwoyz.html

[F09] 获取文件大小
来源：http://hz.yangfankeji.com/gtibzznzbu.html

Py:   os.path.getsize("a.txt")
来源：http://hz.meibo888.top/gtanybkjeh.html

PHP:  filesize("a.txt");
来源：http://hz.gogol.net.cn/gtdjiwowjo.html

JS:   fs.statSync("a.txt").size
来源：http://hz.yvedp.cn/gttfqikltv.html

TS:   fs.statSync("a.txt").size
来源：http://hz.guannengcc.top/gtgdsuvdyd.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.chenzaomai.com/gtslcoktfs.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.zhaomingkeji.xyz/gtcwdwlmfq.html

Ruby: File.size("a.txt")
来源：http://hz.hongshengwenyu.top/gtmeakdgsy.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.guannengcc.top/gthgverhpa.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.sweek.top/gturrlnxps.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtdkotdpqb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.tianlin.xyz/gthwtuliwj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.c1oappe.top/gtuexuuhug.html

TS:   path.extname("a.txt")
来源：http://hz.andypj.xyz/gtbxsgxpxz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.jqgfzy.top/gtxnxyaxjg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yvedp.cn/gtqzaadpqc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.nanxinkj.top/gtkztemkvf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.chenzaomai.com/gtstwvrklb.html

[F11] 复制与移动文件
来源：http://hz.52xcode.cn/gtalnasdpf.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.jinyuanbaomall.cn/gtfedptmhb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.shzxlz.cn/gtkyytsbby.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhaomingkeji.xyz/gtvvoikmsk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.nanxinkj.top/gtazvsvmpv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.yuanzhike.top/gtavivgfzd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.kuanghao11.cn/gttycrjvyp.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.hysaishi.cn/gttpwxetbe.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.hfpthk.cn/gtoshwaboo.html

[F12] CSV 读写
来源：http://hz.kuanghao11.cn/gtbwclflks.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.snrcjt.cn/gtyvxuowcv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.0kj1m.cn/gtdpkvsamu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.0kj1m.cn/gttmlfhqek.html

TS:   // 同上
来源：http://hz.shanyushiyangkeji.top/gtgyvznuff.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.meibo888.top/gtppxzrgzv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yongpay.top/gtzxcgahcr.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.yonumen.top/gtxgahgumi.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.feifeiyinyue.top/gtiorcvrfz.html

================================================================================
来源：http://hz.jiagoushi.top/gtpzfgqvbu.html

G. 面向对象
来源：http://hz.jinghuilouyu.cn/gtzaaecjgz.html

================================================================================
来源：http://hz.smart0.xyz/gteohjqvli.html

[G01] 定义类
来源：http://hz.xuetiantiany.cn/gtezemqfqk.html

Py:   class User: pass
来源：http://hz.gaohongyu789.top/gtooeexhrj.html

PHP:  class User {}
来源：http://hz.zhiwuduotai.top/gtrprgjohz.html

JS:   class User {}
来源：http://hz.xuetiantiany.cn/gtvygtybsb.html

TS:   class User { name: string = ""; }
来源：http://hz.jinghuilouyu.cn/gteuemjncm.html

Java: class User {}
来源：http://hz.daxiang520.top/gtotdptsfa.html

Go:   type User struct { Name string }
来源：http://hz.dashuyun.cn/gtnloqzwjn.html

Ruby: class User; end
来源：http://hz.zycfv.cn/gtuhlfodyj.html

C#:   class User {}
来源：http://hz.yongpay.top/gtycgjllmf.html

[G02] 构造函数
来源：http://hz.daxiang520.top/gtuwgkruiy.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.52xcode.cn/gtwnatgari.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.hfpthk.cn/gtqqsnxuvv.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.ydzc1.top/gtfffkbaap.html

TS:   constructor(public name: string) {}
来源：http://hz.316326.xyz/gtympmmtml.html

Java: User(String name) { this.name = name; }
来源：http://hz.xziqi.cn/gtoskbnxrz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.chenzaomai.com/gtynofptdz.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.ydzc1.top/gtnbsugkdh.html

C#:   public User(string name) { Name = name; }
来源：http://hz.andypj.xyz/gtvmnpelxw.html

[G03] 实例属性
来源：http://hz.havefunace.top/gtmgezteng.html

Py:   self.name = "x"
来源：http://hz.meibo888.top/gtblfktvid.html

PHP:  public string $name = "x";
来源：http://hz.svipenyu.cn/gtymgbhopb.html

JS:   this.name = "x";
来源：http://hz.pycfn.com/gtfgdzenaz.html

TS:   name: string = "x";
来源：http://hz.feifeiyinyue.top/gtclqumhzh.html

Java: private String name;
来源：http://hz.smart0.xyz/gtdeqjhqnn.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.xinyue.icu/gtxbhookgf.html

Ruby: @name = "x"
来源：http://hz.wangshuangyany.cn/gtganocgls.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.birdmap.top/gtgtkfencx.html

[G04] 定义方法
来源：http://hz.cdnleiting.top/gtqqrllrrw.html

Py:   def greet(self): return self.name
来源：http://hz.yj202588.top/gtmhewuuto.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.chenlongwang.top/gtrigqzvbb.html

JS:   greet() { return this.name; }
来源：http://hz.ydjk.org.cn/gtvzozfmgk.html

TS:   greet(): string { return this.name; }
来源：http://hz.cheryme.top/gthoizguap.html

Java: String greet() { return name; }
来源：http://hz.jqgfzy.top/gticiarupk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.havefunace.top/gtgwsvdtym.html

Ruby: def greet; @name; end
来源：http://hz.pycfn.com/gtoysbcood.html

C#:   public string Greet() => Name;
来源：http://hz.wangshuangyany.cn/gtdmahjssd.html

[G05] 继承
来源：http://hz.jlsjyb.cn/gtbsbsnzwq.html

Py:   class Admin(User): pass
来源：http://hz.xuanzx.com/gtmxgpgwwp.html

PHP:  class Admin extends User {}
来源：http://hz.zhengqikj.top/gtbstdifry.html

JS:   class Admin extends User {}
来源：http://hz.kuanghao11.cn/gtomitesik.html

TS:   class Admin extends User {}
来源：http://hz.hnqzz.top/gtztsyusag.html

Java: class Admin extends User {}
来源：http://hz.zhixingplan.top/gtswpudaqi.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.hnqzz.top/gttmtnaxzj.html

Ruby: class Admin < User; end
来源：http://hz.jlsjyb.cn/gtjfaggpst.html

C#:   class Admin : User {}
来源：http://hz.hnxiangtu.top/gtkrlzwnlj.html

[G06] 重写方法
来源：http://hz.shanyushiyangkeji.top/gtxrguhqdc.html

Py:   def greet(self): return "admin"
来源：http://hz.ywan-chungtsiang.top/gtqzexnhrw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.havefunace.top/gtfwjcqvyd.html

JS:   greet() { return "admin"; }
来源：http://hz.chenlongwang.top/gtigzjsquh.html

TS:   greet(): string { return "admin"; }
来源：http://hz.gogol.net.cn/gtnodfxlja.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.dashuyun.cn/gtaqmjbchm.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.jinghuilouyu.cn/gtygvmfxug.html

Ruby: def greet; "admin"; end
来源：http://hz.jqgufenzy.top/gtwnykkbhb.html

C#:   public override string Greet() => "admin";
来源：http://hz.jinqigfzy.top/gtbfvufpcq.html

[G07] 调用父类方法
来源：http://hz.jianghu66.top/gtfoemayig.html

Py:   super().greet()
来源：http://hz.haohaochexian.top/gteccogase.html

PHP:  parent::greet();
来源：http://hz.jqgufenzy.top/gtghanxiwl.html

JS:   super.greet();
来源：http://hz.pycfn.com/gtyydjxsry.html

TS:   super.greet();
来源：http://hz.jinqigufen.top/gtoaynmbak.html

Java: super.greet();
来源：http://hz.sxryk.cn/gtyranbfpq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jinghuilouyu.cn/gthtztdlxn.html

Ruby: super
来源：http://hz.jinghuilouyu.cn/gtuvibfizx.html

C#:   base.Greet();
来源：http://hz.havefunace.top/gtlyfwbbvd.html

[G08] 静态方法与属性
来源：http://hz.9152youxi.cn/gtrgkqmjpt.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.hammf.cn/gtynpynzfj.html

PHP:  public static function f() {}
来源：http://hz.cheryme.top/gtgqaebxks.html

JS:   static f() {}
来源：http://hz.zhengqikj.top/gtnqduukqh.html

TS:   static f(): void {}
来源：http://hz.smart0.xyz/gtvsodeols.html

Java: static void f() {}
来源：http://hz.birdmap.top/gtodfahqje.html


<!-- 参考信息 -->