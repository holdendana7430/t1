代发 wailian999

JS:   [...s].reverse().join("")
来源：http://hz.xuanzx.com/gtnhfqyduv.html

TS:   [...s].reverse().join("")
来源：http://hz.daxiang520.top/gtqbryhaxy.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.9152youxi.cn/gtyjwsofow.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.haohaochexian.top/gtvhjjpwwh.html

Ruby: s.reverse
来源：http://hz.haohaochexian.top/gtqebfvvqn.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.zdqjudy.top/gtopyuomlp.html

[E12] 统计某字符出现次数
来源：http://hz.shanyushiyangtech.top/gtlwynpejv.html

Py:   s.count("a")
来源：http://hz.jinyuanbaomall.cn/gthlewqsfz.html

PHP:  substr_count($s, "a");
来源：http://hz.yj202588.top/gtqorbqljb.html

JS:   s.split("a").length - 1
来源：http://hz.316326.xyz/gtnihqgqtw.html

TS:   s.split("a").length - 1
来源：http://hz.vqdsnc.cn/gtboyfrvju.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.mhx1999.top/gtdhhdnvzp.html

Go:   strings.Count(s, "a")
来源：http://hz.gaohongyu789.top/gtkqisvyuc.html

Ruby: s.count("a")
来源：http://hz.316326.xyz/gtjelwpugf.html

C#:   s.Count(c => c == 'a')
来源：http://hz.yj20258888.top/gtsdycqtgm.html

[E13] 逐字符遍历
来源：http://hz.jqgufenzy.top/gtrouqqonv.html

Py:   for ch in s: print(ch)
来源：http://hz.jqgufenzy.top/gtfbdmgmhi.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.shzxlz.cn/gtgbxbcnjd.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ywan-chungtsiang.top/gtsjkekomd.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.nwbrower.top/gtswaxqefw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.jyoumei.cn/gtpclryzzc.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.jinqigfzy.top/gtaoepwiae.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.zhaomingkeji.xyz/gtiygxtews.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.wangdashe.top/gtwpyiswzi.html

[E14] URL 编码与 Base64
来源：http://hz.pycfn.com/gtigmzsdfi.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.xylfe.cn/gtrzcqmgtb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.yuxming.cn/gtxgqpjbvj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.yj20258888.top/gtnqsdsona.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.mhx1999.top/gtkuzblhdg.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.shanyushiyangkeji.top/gtiowduuvz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.kuanghao11.cn/gtxlrdaspx.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.0kj1m.cn/gtamjpizin.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.ywan-chungtsiang.top/gtucgwmfrv.html

[E15] HTML 转义 / 反转义
来源：http://hz.yvedp.cn/gtwngvjuqg.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.dashuyun.cn/gtehdcjezm.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.yanxiufei.cn/gtdbmofoun.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.hnxiangtu.top/gtkvfzqemw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.meibo888.top/gtzvbvzngc.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.sufxvd.cn/gtigcpwxke.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.tian-w.cn/gtbniyfxze.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.xuetiantiany.cn/gtutguolzc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.ybcxt.top/gtamkekuxd.html

[E16] 数字千分位
来源：http://hz.redwolf501.top/gtrikgscxa.html

Py:   f"{1234567:,}"
来源：http://hz.zhijiandao.cn/gtwnoxlkzq.html

PHP:  number_format(1234567);
来源：http://hz.hongshengwenyu.top/gtjdnunugf.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.xuanzx.com/gttvjfolcf.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.ppjwa.cn/gtralblsop.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.yj20258888.top/gtmtknwech.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.zhiwuduotai.top/gtlhjfpegy.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.gotoacloud.top/gtbxydnnkh.html

C#:   1234567.ToString("N0")
来源：http://hz.dianchejie.cn/gtxoghkznr.html

[E17] 首字母大写
来源：http://hz.sweek.top/gthpqzxxyl.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.cqqwz.cn/gtbcmxzqor.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.gaohongyu789.top/gtvrkwkakg.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.feifeiyinyue.top/gtwxkluqtm.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhoulong.xyz/gtvyseifid.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.chenjidiqi.icu/gtodopbcgz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.xuanzx.com/gtcxtleihq.html

Ruby: s.capitalize
来源：http://hz.ywan-chungtsiang.top/gtxmotanbb.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.xuanzx.com/gtbkolraba.html

[E18] 模板占位符替换
来源：http://hz.xinyue.icu/gtieefqacs.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.dashuyun.cn/gtvyralbll.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.nwbrower.top/gtjkpxjvoc.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.sysykeji.top/gtwnauomsj.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.cashguo.top/gtzktousnd.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.cashguo.top/gtxqcxfgbq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.shangyingyoupin.top/gtcdhsvcyb.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.hnxiangtu.top/gtlkqkunmy.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.sweek.top/gtwgalqkto.html

[E19] 多行文本按行拆分
来源：http://hz.aizwys.cn/gtfqbyvfhn.html

Py:   s.splitlines()
来源：http://hz.hongshengwenyu.top/gtkoaylqaj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.wangdashe.top/gtmbcmtotc.html

JS:   s.split(/\r?\n/)
来源：http://hz.shangyingyoupin.top/gtafkjujak.html

TS:   s.split(/\r?\n/)
来源：http://hz.hnqzz.top/gtzgveaqni.html

Java: s.lines().toList()
来源：http://hz.haohaochexian.top/gtzhdiohxt.html

Go:   strings.Split(s, "\n")
来源：http://hz.sweek.top/gtznjnomhu.html

Ruby: s.lines
来源：http://hz.tian-w.cn/gteeonmcba.html

C#:   s.Split('\n')
来源：http://hz.0kj1m.cn/gtcjnnxdyj.html

[E20] 判断字符串是否为空
来源：http://hz.ehwqpu.com/gtcuytnkvi.html

Py:   if not s:
来源：http://hz.sufxvd.cn/gtcndgfstt.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.svipenyu.cn/gtvuftkvld.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.snrcjt.cn/gtoignhiws.html

TS:   if (s === "") {}
来源：http://hz.hammf.cn/gtczosxywz.html

Java: if (s.isEmpty()) {}
来源：http://hz.gotoacloud.top/gtbdytnoww.html

Go:   if s == "" {}
来源：http://hz.zhengqikj.top/gtoczawzhd.html

Ruby: if s.empty?
来源：http://hz.sxryk.cn/gtfxyayrwv.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.gzhubu.top/gtqnccgxaf.html

[E21] 超长截断加省略号
来源：http://hz.yuanzhike.top/gteptpgiae.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.pengpengdd.cyou/gtzzoyldnt.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.xziqi.cn/gttcumfoty.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jqgufenzy.top/gtgwceenxn.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.xylfe.cn/gtvipbfoyz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yonumen.top/gtxbqixqwp.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.yj20258888.top/gtfgdsorci.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.daxiang520.top/gtoscckdhd.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.smart0.xyz/gtswsaxdnd.html

[E22] 字节长度与字符长度
来源：http://hz.shuidangran.top/gtrkptqpjc.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.jqgfzy.top/gtxqfrckch.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.pycfn.com/gteydxnjjd.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ydjk.org.cn/gtlpweecjs.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hywenlv.cn/gtpyvjobfz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.hongshengwenyu.top/gtixicluhh.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.hnqzz.top/gtgnhueirb.html

Ruby: s.bytesize;  s.length
来源：http://hz.zhijiandao.cn/gtqnpvochw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.feifeiyinyue.top/gtrxuxogio.html

================================================================================
来源：http://hz.ybcxt.top/gtojzuoiyh.html

F. 文件与目录
来源：http://hz.ywan-chungtsiang.top/gtlgpdkimy.html

================================================================================
来源：http://hz.andypj.xyz/gtwuzrllfm.html

[F01] 读取整个文件
来源：http://hz.cucudq.cn/gtmawqutzs.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.feifeiyinyue.top/gtgodrjrah.html

PHP:  file_get_contents("a.txt");
来源：http://hz.jiagoushi.top/gtvqycytnn.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.yj202588.top/gtivfkqpgt.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.yuxming.cn/gtjjeunxdc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.redwolf501.top/gtvftfmvgl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.feifeiyinyue.top/gtvxdpzizw.html

Ruby: File.read("a.txt")
来源：http://hz.andypj.xyz/gtkjbmvljm.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.fzhhl.top/gtkxbsjhmj.html

[F02] 逐行读取文件
来源：http://hz.chenjidiqi.icu/gtvcwxrnjh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.sysykeji.top/gtmtemctrm.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.yj20258888.top/gtlmaejkmk.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.guowangkeji.top/gtbzrhhytu.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhengqikj.top/gtyacxycsd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.sweek.top/gtwbtmsoej.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.yj20258888.top/gtmugvvlcq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.snrcjt.cn/gtzclwbzdd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.haohaochexian.top/gtesmspiua.html

[F03] 写入文件（覆盖）
来源：http://hz.guannengcc.top/gtzpkuknmq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.jqgfzy.top/gtgqsinkaa.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.tanke756.top/gtmmbbdfos.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.havefunace.top/gtjqkeshvx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yuxming.cn/gtmolmpexv.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.sxryk.cn/gtpfhwywpn.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.zhoulong.xyz/gtergdlzjy.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.daria6918.cn/gtddanxhfq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.wangdashe.top/gtspxcyzer.html

[F04] 追加写入文件
来源：http://hz.kuanghao11.cn/gtdjvkfrhg.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yuxming.cn/gtfzylytcy.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.guowangkeji.top/gtlzzfzbqg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.guannengcc.top/gtikjxqkri.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yuanzhike.top/gtoxnpahcx.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.52xcode.cn/gtdkexpwcz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.jinqigufen.top/gtbszruvoq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yuanzhike.top/gtopsbfaik.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.yvedp.cn/gtfzgjznux.html

[F05] 判断文件或目录是否存在
来源：http://hz.9152youxi.cn/gtrxnqwjhc.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.jianghu66.top/gtuhlettqq.html

PHP:  file_exists("a.txt");
来源：http://hz.yj20258.top/gtxsoxppgq.html

JS:   fs.existsSync("a.txt")
来源：http://hz.cucudq.cn/gtubuzovbx.html

TS:   fs.existsSync("a.txt")
来源：http://hz.aizwys.cn/gtdprqxuch.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.yueranfly.top/gtnnydprvt.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.cheryme.top/gtytdtncqx.html

Ruby: File.exist?("a.txt")
来源：http://hz.jinqigufen.top/gtrprenhup.html

C#:   File.Exists("a.txt")
来源：http://hz.wangshuangyany.cn/gtbodvlwfx.html

[F06] 删除文件
来源：http://hz.yj20258.top/gtnpycdgfb.html

Py:   os.remove("a.txt")
来源：http://hz.xuetiantiany.cn/gtidzgdbbi.html

PHP:  unlink("a.txt");
来源：http://hz.gaohongyu789.top/gtznowpbih.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.jinqigfzy.top/gttauradmr.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.redwolf501.top/gtrvvztuof.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.dashuyun.cn/gtvzhrjcmr.html

Go:   os.Remove("a.txt")
来源：http://hz.ppjwa.cn/gtyxkrkcfo.html

Ruby: File.delete("a.txt")
来源：http://hz.zhixingplan.top/gtfummycld.html

C#:   File.Delete("a.txt");
来源：http://hz.fengsongda.top/gtyvjvponu.html

[F07] 创建目录（含多级）
来源：http://hz.nanxinkj.top/gtzydocppy.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.xylfe.cn/gtxqjbfjuh.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.haohaochexian.top/gtmvcxtyez.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ydzc1.top/gtkcderlma.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.bjfxy.top/gthnptzjiz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.zhoulong.xyz/gteatgddqt.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.nwbrower.top/gtuxusofav.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.nanxinkj.top/gtzpvdoafp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.zhengqikj.top/gtylshrpzo.html

[F08] 遍历目录
来源：http://hz.nwbrower.top/gtatadwjvr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.chenzaomai.com/gtmklucjsn.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.hnqzz.top/gtbnwjynmz.html

JS:   fs.readdirSync("dir")
来源：http://hz.dianchejie.cn/gtsgiuydga.html

TS:   fs.readdirSync("dir")
来源：http://hz.redwolf501.top/gtqyiwwlch.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.cashguo.top/gtlrezqrlj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.birdmap.top/gthiobmldg.html

Ruby: Dir.children("dir")
来源：http://hz.kuanghao11.cn/gtegrijtkt.html

C#:   Directory.GetFiles("dir")
来源：http://hz.jinqigufen.top/gtcgooeiuw.html

[F09] 获取文件大小
来源：http://hz.jianghu66.top/gtfgykjaku.html

Py:   os.path.getsize("a.txt")
来源：http://hz.jiagoushi.top/gtnhfgnxgo.html

PHP:  filesize("a.txt");
来源：http://hz.yvedp.cn/gtelxuzgyn.html

JS:   fs.statSync("a.txt").size
来源：http://hz.yueranfly.top/gtqgykined.html

TS:   fs.statSync("a.txt").size
来源：http://hz.jianghu66.top/gtkzmqgdcv.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.cucudq.cn/gtppzppruc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.0kj1m.cn/gtzkeqwjvt.html

Ruby: File.size("a.txt")
来源：http://hz.yj202588.top/gthumsjcke.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.dashuyun.cn/gtehrhofqg.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.gzhubu.top/gtuyfraufg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.aibaodan.cn/gtgezbdeut.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.chenzaomai.com/gtkghamqsu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.wangdashe.top/gtfirpbxgh.html

TS:   path.extname("a.txt")
来源：http://hz.jinghuilouyu.cn/gtdrxfurcy.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.hywenlv.cn/gtwxqsukfo.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.havefunace.top/gtlhkbenzt.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jinqigufen.top/gtnuoiyjdx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.haohaochexian.top/gttxwlbmzc.html

[F11] 复制与移动文件
来源：http://hz.xuetiantiany.cn/gteyeaprmm.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.jyoumei.cn/gtniekyjjo.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.wangdashe.top/gtswtskfnc.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hywenlv.cn/gtfsruzkux.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.fengsongda.top/gthbavupse.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.zhiwuduotai.top/gttsdtbxzd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.pengpengdd.cyou/gtqamevnem.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.hammf.cn/gthmwlajsn.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.gaohongyu789.top/gtcgkpbcrb.html

[F12] CSV 读写
来源：http://hz.xingfuxueyuan.xyz/gtyoazrlch.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.hnqzz.top/gtsfcyfprs.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.jinghuilouyu.cn/gtzmriqvzs.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.aibaodan.cn/gtxsbblknb.html

TS:   // 同上
来源：http://hz.jinqigfzy.top/gtuytbjgsh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.yvedp.cn/gtbmgvkema.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.dashuyun.cn/gtvcwiyucl.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.yanxiufei.cn/gtldfsdbkz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.havefunace.top/gtqjukjmen.html

================================================================================
来源：http://hz.tanke756.top/gtnanonuwi.html

G. 面向对象
来源：http://hz.fzhhl.top/gtucnpksrc.html

================================================================================
来源：http://hz.shuidangran.top/gtrhfwexgj.html

[G01] 定义类
来源：http://hz.sweek.top/gtgjiikpej.html

Py:   class User: pass
来源：http://hz.ehwqpu.com/gtfjsclsgu.html

PHP:  class User {}
来源：http://hz.52xcode.cn/gtiahgtblh.html

JS:   class User {}
来源：http://hz.hfpthk.cn/gttzjuedpb.html

TS:   class User { name: string = ""; }
来源：http://hz.pycfn.com/gtgyanhlvu.html

Java: class User {}
来源：http://hz.bjfxy.top/gtfcinizqj.html

Go:   type User struct { Name string }
来源：http://hz.bjfxy.top/gtnxbzhvuf.html

Ruby: class User; end
来源：http://hz.chenzaomai.com/gtqlvupkvb.html

C#:   class User {}
来源：http://hz.xylfe.cn/gtgaynmhes.html

[G02] 构造函数
来源：http://hz.guannengcc.top/gtfmspofqw.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.jlsjyb.cn/gteizcczlf.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yj202588.top/gtokewkfqk.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.snrcjt.cn/gtghlvmvmw.html

TS:   constructor(public name: string) {}
来源：http://hz.pengpengdd.cyou/gtivbkosfs.html

Java: User(String name) { this.name = name; }
来源：http://hz.pycfn.com/gtgvkbhqwn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yvedp.cn/gtxkbapxbc.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.fzhhl.top/gtksslydxx.html

C#:   public User(string name) { Name = name; }
来源：http://hz.jiagoushi.top/gtiqwmitrv.html

[G03] 实例属性
来源：http://hz.chenzaomai.com/gtkgedsvij.html

Py:   self.name = "x"
来源：http://hz.yj20258.top/gteycmjicg.html

PHP:  public string $name = "x";
来源：http://hz.ywan-chungtsiang.top/gtsxpwoktk.html

JS:   this.name = "x";
来源：http://hz.jinyuanbaomall.cn/gtoztqrbcb.html

TS:   name: string = "x";
来源：http://hz.cucudq.cn/gtbqpckoje.html

Java: private String name;
来源：http://hz.shanyushiyangkeji.top/gtimfyjlsv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.zhixingplan.top/gtudwzfpjk.html

Ruby: @name = "x"
来源：http://hz.wangshuangyany.cn/gtqbnrfkiz.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.sysykeji.top/gtheoyiafx.html

[G04] 定义方法
来源：http://hz.zhixingplan.top/gtcubrmtvc.html

Py:   def greet(self): return self.name
来源：http://hz.aizwys.cn/gtbeexichn.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.ywan-chungtsiang.top/gttmorxovd.html

JS:   greet() { return this.name; }
来源：http://hz.xuetiantiany.cn/gtjnuxtwlt.html

TS:   greet(): string { return this.name; }
来源：http://hz.316326.xyz/gtradperht.html

Java: String greet() { return name; }
来源：http://hz.chenlongwang.top/gtbsrqpcja.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.gogol.net.cn/gtvzropkpy.html

Ruby: def greet; @name; end
来源：http://hz.yj20258888.top/gtsfwhhqpw.html

C#:   public string Greet() => Name;
来源：http://hz.hnqzz.top/gtlgemkgen.html

[G05] 继承
来源：http://hz.shuidangran.top/gtbubjlgiu.html

Py:   class Admin(User): pass
来源：http://hz.xuanzx.com/gtvsebmymn.html

PHP:  class Admin extends User {}
来源：http://hz.gzhubu.top/gtagwixbgo.html

JS:   class Admin extends User {}
来源：http://hz.zdqjudy.top/gtufnouwub.html

TS:   class Admin extends User {}
来源：http://hz.aibaodan.cn/gtvdkinirl.html

Java: class Admin extends User {}
来源：http://hz.zhijiandao.cn/gtvbqkflib.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.jiagoushi.top/gtlgfgobqi.html

Ruby: class Admin < User; end
来源：http://hz.yanxiufei.cn/gttscuywqv.html

C#:   class Admin : User {}
来源：http://hz.cheryme.top/gtrwybqitb.html

[G06] 重写方法
来源：http://hz.jqgufenzy.top/gtybvnsykc.html

Py:   def greet(self): return "admin"
来源：http://hz.shanyushiyangtech.top/gtjajphysh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.aizwys.cn/gtfaygiqgj.html

JS:   greet() { return "admin"; }
来源：http://hz.quarkkingdee.top/gthbmpehkp.html

TS:   greet(): string { return "admin"; }
来源：http://hz.cashguo.top/gtxzsotzkx.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.meibo888.top/gtqcarwfms.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zhixingplan.top/gtakqvhuoy.html

Ruby: def greet; "admin"; end
来源：http://hz.shzxlz.cn/gtpsnigfzb.html

C#:   public override string Greet() => "admin";
来源：http://hz.sufxvd.cn/gtcifxpvaw.html

[G07] 调用父类方法
来源：http://hz.gogol.net.cn/gtjgztcznh.html

Py:   super().greet()
来源：http://hz.chenjidiqi.icu/gtbyttoeml.html

PHP:  parent::greet();
来源：http://hz.cucudq.cn/gthddqqami.html

JS:   super.greet();
来源：http://hz.jianghu66.top/gtcuxnkunb.html

TS:   super.greet();
来源：http://hz.cheryme.top/gtnstszdfo.html

Java: super.greet();
来源：http://hz.yueranfly.top/gtqjcfoesf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.ydzc1.top/gthvewxkzm.html

Ruby: super
来源：http://hz.sweek.top/gtmfnezuwo.html

C#:   base.Greet();
来源：http://hz.ywan-chungtsiang.top/gtnlvctqmm.html

[G08] 静态方法与属性
来源：http://hz.zhixingplan.top/gtdllxdhoo.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jqgufenzy.top/gtmjihjjqg.html

PHP:  public static function f() {}
来源：http://hz.zhaomingkeji.xyz/gtllybaydm.html

JS:   static f() {}
来源：http://hz.xuetiantiany.cn/gtojjkmqcv.html

TS:   static f(): void {}
来源：http://hz.feifeiyinyue.top/gtlkspurpv.html

Java: static void f() {}
来源：http://hz.dashuyun.cn/gtsqpnusqe.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.c1oappe.top/gtkdblabte.html

Ruby: def self.f; end
来源：http://hz.zdqjudy.top/gtfrlvedtt.html

C#:   public static void F() {}
来源：http://hz.quarkkingdee.top/gtehzuznkb.html

[G09] 接口 / 抽象类
来源：http://hz.jlsjyb.cn/gtbmnurwup.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.xylfe.cn/gtiladodez.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.9152youxi.cn/gtohpndyhm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.yj20258888.top/gtjmqsrbxe.html

TS:   interface Shape { area(): number; }
来源：http://hz.cdnleiting.top/gtfdrgifok.html

Java: interface Shape { double area(); }
来源：http://hz.havefunace.top/gtishqpnou.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.xuetiantiany.cn/gtmubxyzcl.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jianghu66.top/gtntrjqlyq.html

C#:   interface IShape { double Area(); }
来源：http://hz.52xcode.cn/gtggnnkmby.html


<!-- 参考信息 -->