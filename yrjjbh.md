代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://hz.hnxiangtu.top/gtitwxxtrp.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.aizwys.cn/gttpeohjtu.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.ivvv.top/gtzejxwpza.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.shangyingyoupin.top/gtibglgolr.html

[E10] 左侧补零 / 定长填充
来源：http://hz.feifeiyinyue.top/gtidzduwtx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.tanke756.top/gtjadqgukq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.c1oappe.top/gtdlzmboof.html

JS:   "7".padStart(3, "0")
来源：http://hz.xziqi.cn/gtqiysosxk.html

TS:   "7".padStart(3, "0")
来源：http://hz.gzhubu.top/gtwsyqxxha.html

Java: String.format("%03d", 7)
来源：http://hz.52xcode.cn/gtolqscxgz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.yonumen.top/gtfrntniyv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.aizwys.cn/gtskmfneqp.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.jinyuanbaomall.cn/gtdgwpqtoa.html

[E11] 反转字符串
来源：http://hz.jqgufenzy.top/gtxioukwyq.html

Py:   s[::-1]
来源：http://hz.ydzc1.top/gtbcjvtoji.html

PHP:  strrev($s);
来源：http://hz.vqdsnc.cn/gtviaufjec.html

JS:   [...s].reverse().join("")
来源：http://hz.aibaodan.cn/gtvztfpmqi.html

TS:   [...s].reverse().join("")
来源：http://hz.jinghuilouyu.cn/gttpvitpby.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.gzhubu.top/gtfcerdfoz.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.hfpthk.cn/gtpozuzppv.html

Ruby: s.reverse
来源：http://hz.nanxinkj.top/gtipzdfvsy.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.hnxiangtu.top/gttibslnop.html

[E12] 统计某字符出现次数
来源：http://hz.guannengcc.top/gtbkczwkqn.html

Py:   s.count("a")
来源：http://hz.wangdashe.top/gtltjuvadn.html

PHP:  substr_count($s, "a");
来源：http://hz.yonumen.top/gteidgsonp.html

JS:   s.split("a").length - 1
来源：http://hz.sufxvd.cn/gtfxyzvyfb.html

TS:   s.split("a").length - 1
来源：http://hz.bjfxy.top/gtkusgzmgd.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.xuetiantiany.cn/gtxldbflgr.html

Go:   strings.Count(s, "a")
来源：http://hz.jinqigfzy.top/gtiwugfsgi.html

Ruby: s.count("a")
来源：http://hz.zhixingplan.top/gtxiknbdne.html

C#:   s.Count(c => c == 'a')
来源：http://hz.ydzc1.top/gtywvdqpwd.html

[E13] 逐字符遍历
来源：http://hz.yuxming.cn/gtitqnxcli.html

Py:   for ch in s: print(ch)
来源：http://hz.meibo888.top/gturoagzzf.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.yvedp.cn/gttjlceqqa.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zhengqikj.top/gtslqxclfr.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jianghu66.top/gtdtzajftv.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.wangshuangyany.cn/gtgrgeohwf.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.guowangkeji.top/gtgeghgzbs.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.haohaochexian.top/gtcdnmpfao.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.tanke756.top/gtgflgqcqp.html

[E14] URL 编码与 Base64
来源：http://hz.zhengqikj.top/gtojtuyhyr.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.hnxiangtu.top/gtqzxzfcvm.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.pengpengdd.cyou/gthhcphgpy.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.fzhhl.top/gtpwizceqd.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.yueranfly.top/gtiwmtuzjp.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.shangyingyoupin.top/gtzbgfvcbj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.ydzc1.top/gtptsqreds.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.haohaochexian.top/gtskygchph.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.guannengcc.top/gtqmpygnix.html

[E15] HTML 转义 / 反转义
来源：http://hz.hnqzz.top/gtpmlocsku.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.sxryk.cn/gtqjbkdvbk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.hfpthk.cn/gtwavqfieu.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.zdqjudy.top/gtdjkbqoag.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.yuxming.cn/gtakiswmry.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.zhoulong.xyz/gtwwatosbd.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.ivvv.top/gttcqqtjbl.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.gotoacloud.top/gtghygfugb.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.zhixingplan.top/gttcbuprbo.html

[E16] 数字千分位
来源：http://hz.kuanghao11.cn/gtjvexfhtz.html

Py:   f"{1234567:,}"
来源：http://hz.shangyingyoupin.top/gtvgfxsuuj.html

PHP:  number_format(1234567);
来源：http://hz.guannengcc.top/gtbysxfqnd.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhijiandao.cn/gtaqhswnwx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.jlsjyb.cn/gtkqpxofus.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.bjfxy.top/gtpsovfnji.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.jqgfzy.top/gtxsebwuem.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.zhaomingkeji.xyz/gtastjorgs.html

C#:   1234567.ToString("N0")
来源：http://hz.cdnleiting.top/gtjtqhfrxc.html

[E17] 首字母大写
来源：http://hz.hnxiangtu.top/gtybxnzovk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.fzhhl.top/gtbczpgsku.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.hnxiangtu.top/gtttyybipv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jianghu66.top/gtqjrtdjpj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ppjwa.cn/gtvbcdphau.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.tanke756.top/gtdtdiwrqm.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.hnxiangtu.top/gttskbvpuu.html

Ruby: s.capitalize
来源：http://hz.tian-w.cn/gtjissdqll.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.chenjidiqi.icu/gtucmwgkpy.html

[E18] 模板占位符替换
来源：http://hz.zhiwuduotai.top/gtfdmxhpyh.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.ppjwa.cn/gtsdevbkto.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.shangyingyoupin.top/gtyrovzevo.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.feifeiyinyue.top/gtotlyuwya.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.gogol.net.cn/gtzmwaqctp.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.yueranfly.top/gtctyiypiz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.sxryk.cn/gtdtznosla.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.sufxvd.cn/gtaglbnvxv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.daria6918.cn/gtqknemfqe.html

[E19] 多行文本按行拆分
来源：http://hz.ehwqpu.com/gtoxtrnifx.html

Py:   s.splitlines()
来源：http://hz.daxiang520.top/gtdlzlxlvu.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.zhixingplan.top/gtafnjvypm.html

JS:   s.split(/\r?\n/)
来源：http://hz.chenjidiqi.icu/gtrllnnllc.html

TS:   s.split(/\r?\n/)
来源：http://hz.tian-w.cn/gtrraagefk.html

Java: s.lines().toList()
来源：http://hz.cheryme.top/gtvqfhhmuo.html

Go:   strings.Split(s, "\n")
来源：http://hz.svipenyu.cn/gttvzlsgbh.html

Ruby: s.lines
来源：http://hz.yj202588.top/gtrqhhnhwj.html

C#:   s.Split('\n')
来源：http://hz.yuanzhike.top/gtckkdtukg.html

[E20] 判断字符串是否为空
来源：http://hz.hnqzz.top/gtrvxnevwb.html

Py:   if not s:
来源：http://hz.shzxlz.cn/gttdpbzgcn.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.ydjk.org.cn/gttionmyjb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.cashguo.top/gtgfsepojo.html

TS:   if (s === "") {}
来源：http://hz.daxiang520.top/gtljtkltdx.html

Java: if (s.isEmpty()) {}
来源：http://hz.birdmap.top/gthgmrdkhr.html

Go:   if s == "" {}
来源：http://hz.daxiang520.top/gtioxvhhwb.html

Ruby: if s.empty?
来源：http://hz.fengsongda.top/gtmmqwrgdn.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.hfpthk.cn/gtrbshkcyj.html

[E21] 超长截断加省略号
来源：http://hz.ybcxt.top/gtephbuvmt.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.gzhubu.top/gtqiskmvat.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.jqgufenzy.top/gtanlvafpy.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.mhx1999.top/gtuxslksjd.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.aizwys.cn/gtxrzlwwyx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.xziqi.cn/gtilkhqkzr.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.jqgufenzy.top/gtstmmemwu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.jinyuanbaomall.cn/gtewcmzxjh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.xziqi.cn/gtxlqkenxx.html

[E22] 字节长度与字符长度
来源：http://hz.jiagoushi.top/gthicimrtj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.yj20258.top/gthifmqnuw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ybcxt.top/gtlznqtnyw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.dianchejie.cn/gtqvxagvhv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.shanyushiyangkeji.top/gtgsjbgafv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.xylfe.cn/gtgvrgnooq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.jinghuilouyu.cn/gttkwtsvpb.html

Ruby: s.bytesize;  s.length
来源：http://hz.zhengqikj.top/gtnnrupzqq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.xylfe.cn/gtmzdykskd.html

================================================================================
来源：http://hz.hnxiangtu.top/gtihyksmqz.html

F. 文件与目录
来源：http://hz.jyoumei.cn/gtvygjvmiw.html

================================================================================
来源：http://hz.guannengcc.top/gtqogfjndd.html

[F01] 读取整个文件
来源：http://hz.hysaishi.cn/gtqfyicify.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.dashuyun.cn/gtyruxzyvl.html

PHP:  file_get_contents("a.txt");
来源：http://hz.yuxming.cn/gtyhsupjqh.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.aibaodan.cn/gtzgskturr.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.316326.xyz/gtjjoulyur.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.jinyuanbaomall.cn/gtsfwzzvxv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.cheryme.top/gtzezbhktu.html

Ruby: File.read("a.txt")
来源：http://hz.yuanzhike.top/gtjyvtulze.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.jinqigfzy.top/gtrbvhzdog.html

[F02] 逐行读取文件
来源：http://hz.andypj.xyz/gtjfdkgfiz.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.jqgfzy.top/gtufqnrkjy.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.ehwqpu.com/gtnxhhwxey.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.quarkkingdee.top/gtnjfgzpun.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jinqigufen.top/gtrryizlyc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.xinyue.icu/gtvxwoseve.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.hnxiangtu.top/gtazfdtrbv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.pycfn.com/gthdhpngjy.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.cdnleiting.top/gtfwmiblkn.html

[F03] 写入文件（覆盖）
来源：http://hz.yueranfly.top/gtyuzuhxnj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.gotoacloud.top/gtsthlsczs.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.ydzc1.top/gtqjigqbwz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.316326.xyz/gtxvyukniy.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.gaohongyu789.top/gtuqqkuwiu.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.cashguo.top/gtlwsbnlfl.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.dianchejie.cn/gteuodzwkt.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.gaohongyu789.top/gtikpbrdcx.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.316326.xyz/gtsswkrgeu.html

[F04] 追加写入文件
来源：http://hz.ehwqpu.com/gtzuxkqydl.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.chenjidiqi.icu/gtcuuwsnej.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.wangdashe.top/gtqhyzxplr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhoulong.xyz/gtvptxqlde.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.cdnleiting.top/gtapyyonvt.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.ppjwa.cn/gtydakpnpa.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.mhx1999.top/gtwxrfgjwk.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.zhengqikj.top/gtdjqctruv.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.guannengcc.top/gtliupvpzf.html

[F05] 判断文件或目录是否存在
来源：http://hz.aibaodan.cn/gthssypxog.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.cucudq.cn/gtekdzqnhm.html

PHP:  file_exists("a.txt");
来源：http://hz.zhongyouzk.top/gtkfvuzsey.html

JS:   fs.existsSync("a.txt")
来源：http://hz.svipenyu.cn/gtdkuhhcso.html

TS:   fs.existsSync("a.txt")
来源：http://hz.ydzc1.top/gthxudobwc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.tian-w.cn/gtwjyersng.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.nanxuanxn.top/gtmifovahq.html

Ruby: File.exist?("a.txt")
来源：http://hz.yj20258.top/gtpijngqer.html

C#:   File.Exists("a.txt")
来源：http://hz.cqqwz.cn/gtyijcvbtl.html

[F06] 删除文件
来源：http://hz.yvedp.cn/gtiryjhwef.html

Py:   os.remove("a.txt")
来源：http://hz.yj20258.top/gtcmabzkrs.html

PHP:  unlink("a.txt");
来源：http://hz.yuxming.cn/gtxsekhdzo.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.svipenyu.cn/gtwbggureg.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.svipenyu.cn/gtgmrfuxro.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.fengsongda.top/gtdeotudii.html

Go:   os.Remove("a.txt")
来源：http://hz.wangdashe.top/gtkymruleg.html

Ruby: File.delete("a.txt")
来源：http://hz.chenjidiqi.icu/gtaeczwsny.html

C#:   File.Delete("a.txt");
来源：http://hz.cqqwz.cn/gtsncsxryl.html

[F07] 创建目录（含多级）
来源：http://hz.ywan-chungtsiang.top/gtqdlmyczg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.hysaishi.cn/gtikgreuzj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.tanke756.top/gtnxbsopon.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.mhx1999.top/gtqvnakzhb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.gaohongyu789.top/gtcdgnijcm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.pengpengdd.cyou/gtkxduhhts.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.vqdsnc.cn/gtmwjkjsrd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.andypj.xyz/gtoepxkogu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.jqgufenzy.top/gtctvedtqs.html

[F08] 遍历目录
来源：http://hz.zycfv.cn/gtteivmuff.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.ivvv.top/gtxqnanhlg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.xylfe.cn/gtsnnanuci.html

JS:   fs.readdirSync("dir")
来源：http://hz.kuanghao11.cn/gtpjzkwifa.html

TS:   fs.readdirSync("dir")
来源：http://hz.iojbl.cn/gtjiejisvd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.zhiwuduotai.top/gtkncjpjwj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.jinyuanbaomall.cn/gtvbcqkitv.html

Ruby: Dir.children("dir")
来源：http://hz.sysykeji.top/gtxsiwmgdy.html

C#:   Directory.GetFiles("dir")
来源：http://hz.shangyingyoupin.top/gttvdtsnfu.html

[F09] 获取文件大小
来源：http://hz.jyoumei.cn/gtmkfpvrdv.html

Py:   os.path.getsize("a.txt")
来源：http://hz.zhixingplan.top/gtdrqmgxzo.html

PHP:  filesize("a.txt");
来源：http://hz.svipenyu.cn/gtrkssxahs.html

JS:   fs.statSync("a.txt").size
来源：http://hz.0kj1m.cn/gtcgeugnhb.html

TS:   fs.statSync("a.txt").size
来源：http://hz.bjfxy.top/gtnycwsuun.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.nanxuanxn.top/gtpmlyujyw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.jinqigfzy.top/gtjrnqwmrd.html

Ruby: File.size("a.txt")
来源：http://hz.shanyushiyangtech.top/gtqhakvdoo.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.52xcode.cn/gtocanweje.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.hfpthk.cn/gttnsbqmpa.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.52xcode.cn/gtobfmwdrx.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.sufxvd.cn/gtfngyyqkf.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.xuanzx.com/gtvsbfdshc.html

TS:   path.extname("a.txt")
来源：http://hz.xylfe.cn/gtatgzrrej.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.ehwqpu.com/gtnuwysgtb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.aibaodan.cn/gtwkwjqjnr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.ybcxt.top/gtqtkuffsf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.jinghuilouyu.cn/gtfwujsyaw.html

[F11] 复制与移动文件
来源：http://hz.shanyushiyangkeji.top/gtdjwjplmt.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.mhx1999.top/gttwuesqln.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.jlsjyb.cn/gtosofodvo.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.cqqwz.cn/gtwtzcjcku.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.birdmap.top/gtxnstajyh.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.fengsongda.top/gtdhhkdzde.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.fzhhl.top/gtsjikdrob.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.zhaomingkeji.xyz/gtkkrhzqzg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.haohaochexian.top/gtwhpuopwi.html

[F12] CSV 读写
来源：http://hz.kuanghao11.cn/gtwxjsxyph.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.yj20258.top/gtcjapoyzd.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.wangshuangyany.cn/gtjmqwkweg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.gzhubu.top/gtxlvncwdn.html

TS:   // 同上
来源：http://hz.jinyuanbaomall.cn/gtywloimzy.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.redwolf501.top/gtbmhceizl.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.zhixingplan.top/gtumyidvqm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.tian-w.cn/gtmdsrwozg.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jinqigfzy.top/gtvgpdbhci.html

================================================================================
来源：http://hz.daxiang520.top/gtliptoefp.html

G. 面向对象
来源：http://hz.316326.xyz/gtxczkayno.html

================================================================================
来源：http://hz.hnxiangtu.top/gtirdpvamd.html

[G01] 定义类
来源：http://hz.birdmap.top/gtncucstdm.html

Py:   class User: pass
来源：http://hz.ydjk.org.cn/gtumgdwhab.html

PHP:  class User {}
来源：http://hz.jianghu66.top/gtbazionxf.html

JS:   class User {}
来源：http://hz.chenlongwang.top/gtdsidcycu.html

TS:   class User { name: string = ""; }
来源：http://hz.wangdashe.top/gtvybstfjl.html

Java: class User {}
来源：http://hz.shanyushiyangtech.top/gtjpiuljtu.html

Go:   type User struct { Name string }
来源：http://hz.iojbl.cn/gtvbegyvst.html

Ruby: class User; end
来源：http://hz.yanxiufei.cn/gtzaxaattu.html

C#:   class User {}
来源：http://hz.mhx1999.top/gtaqwqdyln.html

[G02] 构造函数
来源：http://hz.hnqzz.top/gtayknqhoy.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.ywan-chungtsiang.top/gthwguyuec.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.ywan-chungtsiang.top/gtruqsutpe.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.zhongyouzk.top/gtqlurqnsg.html

TS:   constructor(public name: string) {}
来源：http://hz.jiagoushi.top/gtdgdlhkqz.html

Java: User(String name) { this.name = name; }
来源：http://hz.tianlin.xyz/gtyevblkus.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.nanxuanxn.top/gtpjbqhpwo.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yvedp.cn/gtzkkncvna.html

C#:   public User(string name) { Name = name; }
来源：http://hz.fzhhl.top/gtofgtqiro.html

[G03] 实例属性
来源：http://hz.tanke756.top/gtzpemgngv.html

Py:   self.name = "x"
来源：http://hz.svipenyu.cn/gtgyyayggn.html

PHP:  public string $name = "x";
来源：http://hz.cashguo.top/gtakiagirw.html

JS:   this.name = "x";
来源：http://hz.wangdashe.top/gtugaflzcw.html

TS:   name: string = "x";
来源：http://hz.birdmap.top/gtkcokhhwq.html

Java: private String name;
来源：http://hz.jqgfzy.top/gtfeazwqfk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.vqdsnc.cn/gtckaqmshx.html

Ruby: @name = "x"
来源：http://hz.jinyuanbaomall.cn/gtfhjcprfi.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.vqdsnc.cn/gtywszklet.html

[G04] 定义方法
来源：http://hz.sweek.top/gtnahekhoy.html

Py:   def greet(self): return self.name
来源：http://hz.jiagoushi.top/gtvjfflbph.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.guowangkeji.top/gtcxdogzft.html

JS:   greet() { return this.name; }
来源：http://hz.ydjk.org.cn/gtukpswhvh.html

TS:   greet(): string { return this.name; }
来源：http://hz.xziqi.cn/gtmiheajse.html

Java: String greet() { return name; }
来源：http://hz.yj20258.top/gtllpaodbi.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.shanyushiyangkeji.top/gtjggtzfrt.html

Ruby: def greet; @name; end
来源：http://hz.yj20258.top/gtptklxbxt.html

C#:   public string Greet() => Name;
来源：http://hz.zdqjudy.top/gtzbgwsxym.html

[G05] 继承
来源：http://hz.gogol.net.cn/gtlyuaxdqd.html

Py:   class Admin(User): pass
来源：http://hz.jqgfzy.top/gtejpouesv.html

PHP:  class Admin extends User {}
来源：http://hz.gogol.net.cn/gtfmzqmhzv.html

JS:   class Admin extends User {}
来源：http://hz.zhijiandao.cn/gtieprpxww.html

TS:   class Admin extends User {}
来源：http://hz.mhx1999.top/gtmfpmsodb.html

Java: class Admin extends User {}
来源：http://hz.yj20258.top/gttfzskspa.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.dashuyun.cn/gtfmuhjfoe.html

Ruby: class Admin < User; end
来源：http://hz.zhaomingkeji.xyz/gtqhsakmzc.html

C#:   class Admin : User {}
来源：http://hz.316326.xyz/gtbamaqcpn.html

[G06] 重写方法
来源：http://hz.yvedp.cn/gthihvkyrt.html

Py:   def greet(self): return "admin"
来源：http://hz.yonumen.top/gtpeuniely.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.sxryk.cn/gtaqgjpbet.html

JS:   greet() { return "admin"; }
来源：http://hz.yj202588.top/gtsvhzdypc.html

TS:   greet(): string { return "admin"; }
来源：http://hz.zdqjudy.top/gtzxdfvwvm.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.sweek.top/gtnhjohajh.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.quarkkingdee.top/gthghdhohr.html

Ruby: def greet; "admin"; end
来源：http://hz.zhoulong.xyz/gtryukdjbg.html

C#:   public override string Greet() => "admin";
来源：http://hz.cucudq.cn/gtvaoymaxt.html

[G07] 调用父类方法
来源：http://hz.shanyushiyangkeji.top/gtsggwpznp.html

Py:   super().greet()
来源：http://hz.bjfxy.top/gtlfqqxrep.html

PHP:  parent::greet();
来源：http://hz.zhongyouzk.top/gtscztbvsb.html

JS:   super.greet();
来源：http://hz.snrcjt.cn/gtuhrqtffo.html

TS:   super.greet();
来源：http://hz.gzhubu.top/gtnkxwtgck.html

Java: super.greet();
来源：http://hz.shangyingyoupin.top/gtpnqtiekg.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.ehwqpu.com/gtcdegkgnu.html

Ruby: super
来源：http://hz.haohaochexian.top/gtpmbngrko.html

C#:   base.Greet();
来源：http://hz.pengpengdd.cyou/gtnudmkbgy.html

[G08] 静态方法与属性
来源：http://hz.c1oappe.top/gtpvueupsr.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.ywan-chungtsiang.top/gtdzmvqqwf.html


<!-- 参考信息 -->