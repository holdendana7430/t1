代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://hz.xziqi.cn/gtutqfxggg.html

Java: String.format("%03d", 7)
来源：http://hz.tanke756.top/gtztwefkzx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.hfpthk.cn/gtfvqvczkd.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.cucudq.cn/gtkoootjuw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.hfpthk.cn/gtpbnbgkmi.html

[E11] 反转字符串
来源：http://hz.316326.xyz/gtcmxflnye.html

Py:   s[::-1]
来源：http://hz.nwbrower.top/gtebzxbcqk.html

PHP:  strrev($s);
来源：http://hz.jinqigufen.top/gtpcextesu.html

JS:   [...s].reverse().join("")
来源：http://hz.hysaishi.cn/gtaeoekrej.html

TS:   [...s].reverse().join("")
来源：http://hz.dianchejie.cn/gtlmaavzwu.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.kuanghao11.cn/gtkegjzcvc.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.zhongyouzk.top/gtzvgigvsy.html

Ruby: s.reverse
来源：http://hz.vqdsnc.cn/gtbzydmzvs.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.fzhhl.top/gtpgctegkx.html

[E12] 统计某字符出现次数
来源：http://hz.zhaomingkeji.xyz/gtxhimiunr.html

Py:   s.count("a")
来源：http://hz.tianlin.xyz/gtpdevlofb.html

PHP:  substr_count($s, "a");
来源：http://hz.ivvv.top/gtfnvgqave.html

JS:   s.split("a").length - 1
来源：http://hz.jyoumei.cn/gtlmqveven.html

TS:   s.split("a").length - 1
来源：http://hz.zhoulong.xyz/gtgwetumkb.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.nanxuanxn.top/gtdpywglco.html

Go:   strings.Count(s, "a")
来源：http://hz.gogol.net.cn/gtcxahujpb.html

Ruby: s.count("a")
来源：http://hz.cqqwz.cn/gtvfbsmecb.html

C#:   s.Count(c => c == 'a')
来源：http://hz.guannengcc.top/gtfpsdyaxg.html

[E13] 逐字符遍历
来源：http://hz.zhaomingkeji.xyz/gtnbraerkl.html

Py:   for ch in s: print(ch)
来源：http://hz.guowangkeji.top/gtyqygpwck.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.mhx1999.top/gtdhoapmwv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.shangyingyoupin.top/gtxsmzzglh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.gzhubu.top/gthlsheeys.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.quarkkingdee.top/gtravmzzxp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.aibaodan.cn/gtgtqbjoxp.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.chenzaomai.com/gtoonsxfgf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.shangyingyoupin.top/gtcpyyzczp.html

[E14] URL 编码与 Base64
来源：http://hz.nanxinkj.top/gtrpamtxaj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.gaohongyu789.top/gttxougkqm.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.jinqigufen.top/gtfjodxxhn.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.ivvv.top/gtiauqvunx.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.cqqwz.cn/gtcaohwbab.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.redwolf501.top/gtgyxlxuqy.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.jinghuilouyu.cn/gtnlwopzip.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.svipenyu.cn/gtywslquwc.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.xinyue.icu/gtelagycbu.html

[E15] HTML 转义 / 反转义
来源：http://hz.shzxlz.cn/gtxlpjqgmz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.jianghu66.top/gtjlntsgkt.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.cheryme.top/gtuvqosopx.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.xinyue.icu/gtqgqctesu.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.ivvv.top/gtluvytwau.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.fzhhl.top/gtzsiizgtv.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.xziqi.cn/gtpqyckikj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.sxryk.cn/gtpsnuvqmx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.zhaomingkeji.xyz/gtbnnuyhzw.html

[E16] 数字千分位
来源：http://hz.sweek.top/gtopdlhygp.html

Py:   f"{1234567:,}"
来源：http://hz.gaohongyu789.top/gtjbabbacm.html

PHP:  number_format(1234567);
来源：http://hz.zhixingplan.top/gtlcpzjioa.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.kuanghao11.cn/gtqmlamogb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.hnqzz.top/gtrotxfvhm.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.tanke756.top/gtxiwmhytp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.shzxlz.cn/gtpupizurn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.chenlongwang.top/gtkvkvdnhd.html

C#:   1234567.ToString("N0")
来源：http://hz.ybcxt.top/gtmmeculfb.html

[E17] 首字母大写
来源：http://hz.jiagoushi.top/gtjlqnytwu.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.kuanghao11.cn/gtguwzbslj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.zhoulong.xyz/gtmyiweolz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.nanxuanxn.top/gtbifqptds.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.xinyue.icu/gtccbwrmdo.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.yangfankeji.com/gtpsvjilos.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.cdnleiting.top/gtrtpmugku.html

Ruby: s.capitalize
来源：http://hz.svipenyu.cn/gtlrlgczgv.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.redwolf501.top/gtldakrhfx.html

[E18] 模板占位符替换
来源：http://hz.zhongyouzk.top/gtmfzmnefc.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.hywenlv.cn/gtrjprwtbm.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.hysaishi.cn/gtsqhuzmsj.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.quarkkingdee.top/gttjfclibe.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.52xcode.cn/gtancjqnzg.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.vqdsnc.cn/gtpidcbczv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.wangdashe.top/gtfxrnidsl.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.ppjwa.cn/gtaebbpudo.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.vqdsnc.cn/gtxesyghaw.html

[E19] 多行文本按行拆分
来源：http://hz.ehwqpu.com/gtqdeejvfb.html

Py:   s.splitlines()
来源：http://hz.yuxming.cn/gtgqcvbdua.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.haohaochexian.top/gtyewydmab.html

JS:   s.split(/\r?\n/)
来源：http://hz.havefunace.top/gtlzqjlxdk.html

TS:   s.split(/\r?\n/)
来源：http://hz.hysaishi.cn/gtbmfniwmn.html

Java: s.lines().toList()
来源：http://hz.andypj.xyz/gtnnqbbwtj.html

Go:   strings.Split(s, "\n")
来源：http://hz.yj20258888.top/gtzfnhqpus.html

Ruby: s.lines
来源：http://hz.vqdsnc.cn/gthaaxdvpt.html

C#:   s.Split('\n')
来源：http://hz.jyoumei.cn/gtltbicrcy.html

[E20] 判断字符串是否为空
来源：http://hz.ivvv.top/gtfeaikklq.html

Py:   if not s:
来源：http://hz.hywenlv.cn/gtienjpymo.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.kuanghao11.cn/gtwhyzqhgw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.shangyingyoupin.top/gtwlroakwd.html

TS:   if (s === "") {}
来源：http://hz.zhoulong.xyz/gtpsbupjnk.html

Java: if (s.isEmpty()) {}
来源：http://hz.cqqwz.cn/gthothhrpm.html

Go:   if s == "" {}
来源：http://hz.jyoumei.cn/gtxdjtopsp.html

Ruby: if s.empty?
来源：http://hz.snrcjt.cn/gtcgrrqput.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.vqdsnc.cn/gtccrswggu.html

[E21] 超长截断加省略号
来源：http://hz.sxryk.cn/gteppvjesa.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.fzhhl.top/gtuooefsbs.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.pycfn.com/gtbhbsnkxc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.bjfxy.top/gtxrmydgdc.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.hfpthk.cn/gtbtlgfsrk.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.sxryk.cn/gtuofdcecf.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.9152youxi.cn/gtrtnaattx.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.nwbrower.top/gtjewbieoc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.pycfn.com/gtcpkejqfa.html

[E22] 字节长度与字符长度
来源：http://hz.yvedp.cn/gtrzhmslqi.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.gzhubu.top/gtvmjpymjy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.redwolf501.top/gtboiikdet.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hfpthk.cn/gtzarpontn.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.shangyingyoupin.top/gtwsydmxxr.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.quarkkingdee.top/gtnhsjpupg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.zhijiandao.cn/gtucswmsri.html

Ruby: s.bytesize;  s.length
来源：http://hz.cheryme.top/gtcgibsgrj.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.yangfankeji.com/gtjaohatmc.html

================================================================================
来源：http://hz.dashuyun.cn/gtfykzhnyk.html

F. 文件与目录
来源：http://hz.yangfankeji.com/gtgnhazfyl.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtfxvgyfmh.html

[F01] 读取整个文件
来源：http://hz.redwolf501.top/gtqjclxdrl.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.zhengqikj.top/gtpsyjgejo.html

PHP:  file_get_contents("a.txt");
来源：http://hz.aizwys.cn/gtvytrtylu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.birdmap.top/gtuooanhjc.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.svipenyu.cn/gtacglyoii.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.daria6918.cn/gtnceeujdc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.gotoacloud.top/gthucytshw.html

Ruby: File.read("a.txt")
来源：http://hz.hfpthk.cn/gtxfjcngxx.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.sweek.top/gtfhphicmc.html

[F02] 逐行读取文件
来源：http://hz.sufxvd.cn/gtpvjihgll.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.zhoulong.xyz/gtlsyciwdo.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.zhengqikj.top/gtevylwdxz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.nanxuanxn.top/gtbmvxuciw.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.sysykeji.top/gtyifzlsnw.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.jyoumei.cn/gtpgmzmowd.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.hfpthk.cn/gtalxzlhql.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.shzxlz.cn/gtdjmiuoeu.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.guowangkeji.top/gtgskngkor.html

[F03] 写入文件（覆盖）
来源：http://hz.guannengcc.top/gthsnaxgrr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.xuanzx.com/gtznkcnwpz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.haohaochexian.top/gtzyuasnam.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hammf.cn/gttrawpjvu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.gogol.net.cn/gtsrdfhljv.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.nanxuanxn.top/gtuxqkyjku.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.iojbl.cn/gtkoyyehss.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.nanxinkj.top/gtnqpdwysb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.nanxinkj.top/gtfdidehbk.html

[F04] 追加写入文件
来源：http://hz.jianghu66.top/gtmrgnrskx.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.haohaochexian.top/gtsfxrnwdd.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.aibaodan.cn/gtburpjjag.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.316326.xyz/gtrzshmznc.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.shanyushiyangtech.top/gttizyhshl.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.cheryme.top/gtlmsbiern.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.fengsongda.top/gtttedzzui.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.cheryme.top/gtzlqdctrt.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.zhijiandao.cn/gtrstapdts.html

[F05] 判断文件或目录是否存在
来源：http://hz.yj202588.top/gtfnsudgjz.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.daxiang520.top/gtpoemwzyv.html

PHP:  file_exists("a.txt");
来源：http://hz.zhengqikj.top/gtlvfmwcsi.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yj20258.top/gtywebvxuq.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zhiwuduotai.top/gtktndqcca.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.jinqigufen.top/gtzchwgiup.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.zycfv.cn/gtotjdijap.html

Ruby: File.exist?("a.txt")
来源：http://hz.hfpthk.cn/gtgchrtijw.html

C#:   File.Exists("a.txt")
来源：http://hz.zhijiandao.cn/gtmzfyaxvm.html

[F06] 删除文件
来源：http://hz.nanxuanxn.top/gtflzcsadv.html

Py:   os.remove("a.txt")
来源：http://hz.yj202588.top/gtiwfnbajr.html

PHP:  unlink("a.txt");
来源：http://hz.hysaishi.cn/gttafttusd.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.hongshengwenyu.top/gtcdsbmtoi.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.gaohongyu789.top/gtltlucots.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.sysykeji.top/gtjmhnxzfy.html

Go:   os.Remove("a.txt")
来源：http://hz.jyoumei.cn/gtyxdtnhsh.html

Ruby: File.delete("a.txt")
来源：http://hz.cashguo.top/gtcffozvtz.html

C#:   File.Delete("a.txt");
来源：http://hz.yangfankeji.com/gtadhdpvlz.html

[F07] 创建目录（含多级）
来源：http://hz.dashuyun.cn/gtlmolluxi.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.hywenlv.cn/gteonnkova.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.zhijiandao.cn/gtfscajtqe.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ydjk.org.cn/gtuzywjphs.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.smart0.xyz/gtxhoqppdw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.9152youxi.cn/gtckplfglf.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.birdmap.top/gtgjmishgw.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.aizwys.cn/gtspqphhoi.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.feifeiyinyue.top/gtudifoebe.html

[F08] 遍历目录
来源：http://hz.haohaochexian.top/gtfgnpqljq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yuanzhike.top/gtyawnjysv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.jinghuilouyu.cn/gtpsglzrsu.html

JS:   fs.readdirSync("dir")
来源：http://hz.vqdsnc.cn/gtsbthwkyf.html

TS:   fs.readdirSync("dir")
来源：http://hz.hysaishi.cn/gtlnmtyunp.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.shzxlz.cn/gtkmbbdyyn.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.fzhhl.top/gtjqmrgcbs.html

Ruby: Dir.children("dir")
来源：http://hz.gogol.net.cn/gtnmdeakjj.html

C#:   Directory.GetFiles("dir")
来源：http://hz.ppjwa.cn/gtmkbkdzeg.html

[F09] 获取文件大小
来源：http://hz.feifeiyinyue.top/gterwkxdws.html

Py:   os.path.getsize("a.txt")
来源：http://hz.hfpthk.cn/gtlgmcchky.html

PHP:  filesize("a.txt");
来源：http://hz.xylfe.cn/gtmztlmlen.html

JS:   fs.statSync("a.txt").size
来源：http://hz.0kj1m.cn/gttxuzhqnd.html

TS:   fs.statSync("a.txt").size
来源：http://hz.xuetiantiany.cn/gtfjhayedd.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jqgfzy.top/gtayrzmyps.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.yanxiufei.cn/gtjblczcwh.html

Ruby: File.size("a.txt")
来源：http://hz.gogol.net.cn/gtgawpaoub.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.zhiwuduotai.top/gtnbzhvsah.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.chenzaomai.com/gtzvrxxqrp.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.yongpay.top/gthvmwabnk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.sysykeji.top/gtnjgdnlzd.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.zycfv.cn/gtyjsaxnta.html

TS:   path.extname("a.txt")
来源：http://hz.birdmap.top/gtumgnjujz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.haohaochexian.top/gtxnbncxbx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.jqgfzy.top/gtvyqouvhz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.mhx1999.top/gtcgevyrnb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.guannengcc.top/gtwjgvngpg.html

[F11] 复制与移动文件
来源：http://hz.andypj.xyz/gtdfoyqhwy.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.vqdsnc.cn/gtfoeptmkf.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.gzhubu.top/gtnywfngsa.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhongyouzk.top/gtzuitgtvu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.mhx1999.top/gtputqctxe.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.sweek.top/gttodocekr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jqgufenzy.top/gteffhcfwy.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.yj202588.top/gtehcojeah.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.guannengcc.top/gtohllqdah.html

[F12] CSV 读写
来源：http://hz.sxryk.cn/gtuzexnqti.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.gzhubu.top/gtdxeshmmk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.yuxming.cn/gtbiidqklu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.gogol.net.cn/gtuzovalic.html

TS:   // 同上
来源：http://hz.yj20258.top/gtobvzcmqh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.andypj.xyz/gtbcyecbdd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.9152youxi.cn/gtfrbfijrj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.xuetiantiany.cn/gtrjgsmtie.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.tianlin.xyz/gtaekfodvp.html

================================================================================
来源：http://hz.tanke756.top/gtdrypfqcv.html

G. 面向对象
来源：http://hz.jyoumei.cn/gtzkiyvylc.html

================================================================================
来源：http://hz.wangdashe.top/gtxzesjpgo.html

[G01] 定义类
来源：http://hz.mhx1999.top/gttipdfxld.html

Py:   class User: pass
来源：http://hz.shangyingyoupin.top/gtmdljbgbo.html

PHP:  class User {}
来源：http://hz.guannengcc.top/gtfeimntzj.html

JS:   class User {}
来源：http://hz.nwbrower.top/gtgzuvqamf.html

TS:   class User { name: string = ""; }
来源：http://hz.shanyushiyangtech.top/gtyeedchmh.html

Java: class User {}
来源：http://hz.zhiwuduotai.top/gtqmegozev.html

Go:   type User struct { Name string }
来源：http://hz.vqdsnc.cn/gtlbwwfeyn.html

Ruby: class User; end
来源：http://hz.dianchejie.cn/gtwuvwwval.html

C#:   class User {}
来源：http://hz.haohaochexian.top/gtybqhrqtl.html

[G02] 构造函数
来源：http://hz.guowangkeji.top/gtndjratcx.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.316326.xyz/gtqspiljiu.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.0kj1m.cn/gtodwzdemu.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.xuanzx.com/gtgvavyvhr.html

TS:   constructor(public name: string) {}
来源：http://hz.wangshuangyany.cn/gtoypwbuoz.html

Java: User(String name) { this.name = name; }
来源：http://hz.sweek.top/gtnpqtfxph.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.xuetiantiany.cn/gtuswwsyby.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.ydzc1.top/gtjinonlhs.html

C#:   public User(string name) { Name = name; }
来源：http://hz.havefunace.top/gtnsecqedl.html

[G03] 实例属性
来源：http://hz.yangfankeji.com/gtoqvlfmpa.html

Py:   self.name = "x"
来源：http://hz.dashuyun.cn/gtbzonkdjg.html

PHP:  public string $name = "x";
来源：http://hz.svipenyu.cn/gtaohemtjo.html

JS:   this.name = "x";
来源：http://hz.yongpay.top/gtyaxjdfol.html

TS:   name: string = "x";
来源：http://hz.zhixingplan.top/gtlozygyui.html

Java: private String name;
来源：http://hz.smart0.xyz/gtiozqgxas.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.feifeiyinyue.top/gtsmfccprn.html

Ruby: @name = "x"
来源：http://hz.jiagoushi.top/gtknaiybqf.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jlsjyb.cn/gtnchgwdml.html

[G04] 定义方法
来源：http://hz.ywan-chungtsiang.top/gtmnxghttt.html

Py:   def greet(self): return self.name
来源：http://hz.tanke756.top/gtohndxtod.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.tanke756.top/gtkhfmwfmi.html

JS:   greet() { return this.name; }
来源：http://hz.redwolf501.top/gtfsbsfxke.html

TS:   greet(): string { return this.name; }
来源：http://hz.xuanzx.com/gtcthrleei.html

Java: String greet() { return name; }
来源：http://hz.ehwqpu.com/gtpbpqlagq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.iojbl.cn/gttmamzrjh.html

Ruby: def greet; @name; end
来源：http://hz.xinyue.icu/gtnnffffnq.html

C#:   public string Greet() => Name;
来源：http://hz.fengsongda.top/gthqntpfxn.html

[G05] 继承
来源：http://hz.xylfe.cn/gtlyqtkyja.html

Py:   class Admin(User): pass
来源：http://hz.havefunace.top/gtcmipferg.html

PHP:  class Admin extends User {}
来源：http://hz.yueranfly.top/gtagvneaen.html

JS:   class Admin extends User {}
来源：http://hz.daxiang520.top/gtcirjisyz.html

TS:   class Admin extends User {}
来源：http://hz.aizwys.cn/gtbzlfzzvk.html

Java: class Admin extends User {}
来源：http://hz.aibaodan.cn/gtnenygryl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.ehwqpu.com/gtyxwqmimh.html

Ruby: class Admin < User; end
来源：http://hz.jlsjyb.cn/gtrvsfzcnr.html

C#:   class Admin : User {}
来源：http://hz.ehwqpu.com/gtxqrmjsxh.html

[G06] 重写方法
来源：http://hz.zhiwuduotai.top/gtycwlxpjm.html

Py:   def greet(self): return "admin"
来源：http://hz.c1oappe.top/gtetvdjtxw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.zhongyouzk.top/gtgtpnncap.html

JS:   greet() { return "admin"; }
来源：http://hz.dianchejie.cn/gtjzrzbxvn.html

TS:   greet(): string { return "admin"; }
来源：http://hz.ivvv.top/gtykqmgnch.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.sysykeji.top/gtzbpeylfq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.vqdsnc.cn/gtatiffnuw.html

Ruby: def greet; "admin"; end
来源：http://hz.tian-w.cn/gtdbbweywu.html

C#:   public override string Greet() => "admin";
来源：http://hz.haohaochexian.top/gtcvpfxorp.html

[G07] 调用父类方法
来源：http://hz.ywan-chungtsiang.top/gtwlkkiucv.html

Py:   super().greet()
来源：http://hz.mhx1999.top/gtcjisebhy.html

PHP:  parent::greet();
来源：http://hz.guowangkeji.top/gtnwczvhjc.html

JS:   super.greet();
来源：http://hz.sxryk.cn/gttetwcpnd.html

TS:   super.greet();
来源：http://hz.ybcxt.top/gtvnltqgip.html

Java: super.greet();
来源：http://hz.zhaomingkeji.xyz/gtanhlpoee.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.cucudq.cn/gtopwhfubi.html

Ruby: super
来源：http://hz.jqgufenzy.top/gtimtfuykh.html

C#:   base.Greet();
来源：http://hz.bjfxy.top/gtytonnzbf.html

[G08] 静态方法与属性
来源：http://hz.jlsjyb.cn/gtusvmpdtx.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.gotoacloud.top/gtymjvfbho.html

PHP:  public static function f() {}
来源：http://hz.zhaomingkeji.xyz/gtvzllkhzs.html

JS:   static f() {}
来源：http://hz.xuetiantiany.cn/gtanstpioe.html

TS:   static f(): void {}
来源：http://hz.316326.xyz/gtjoepgvgs.html

Java: static void f() {}
来源：http://hz.fengsongda.top/gtxctrsgpz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.cdnleiting.top/gtecklymnj.html

Ruby: def self.f; end
来源：http://hz.cucudq.cn/gtfkzfkcbn.html

C#:   public static void F() {}
来源：http://hz.feifeiyinyue.top/gtkmtypzbr.html

[G09] 接口 / 抽象类
来源：http://hz.zhengqikj.top/gtfdarllgs.html


<!-- 参考信息 -->