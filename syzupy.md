代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://hz.xuetiantiany.cn/gtcuqqlwcq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.guannengcc.top/gtiyinblci.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.vqdsnc.cn/gtjorqlqyj.html

JS:   "7".padStart(3, "0")
来源：http://hz.sweek.top/gtfidbnhnv.html

TS:   "7".padStart(3, "0")
来源：http://hz.ydjk.org.cn/gtxzfjyeci.html

Java: String.format("%03d", 7)
来源：http://hz.hysaishi.cn/gtjhmoarjs.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.jqgufenzy.top/gtvmyajhpc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.sxryk.cn/gtfziitwlw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.iojbl.cn/gtswiplbgn.html

[E11] 反转字符串
来源：http://hz.nwbrower.top/gtgihvxgif.html

Py:   s[::-1]
来源：http://hz.hammf.cn/gtmrmexbbi.html

PHP:  strrev($s);
来源：http://hz.kuanghao11.cn/gtadvmwvmj.html

JS:   [...s].reverse().join("")
来源：http://hz.cucudq.cn/gtamntaief.html

TS:   [...s].reverse().join("")
来源：http://hz.guannengcc.top/gtcficebam.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.zhoulong.xyz/gtbuoiyovk.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.gotoacloud.top/gtwlsmdtka.html

Ruby: s.reverse
来源：http://hz.xylfe.cn/gtlhdsjrxc.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.meibo888.top/gtljoyearr.html

[E12] 统计某字符出现次数
来源：http://hz.yuxming.cn/gtgcrqrspd.html

Py:   s.count("a")
来源：http://hz.hywenlv.cn/gtpzpummpf.html

PHP:  substr_count($s, "a");
来源：http://hz.smart0.xyz/gtiggexybb.html

JS:   s.split("a").length - 1
来源：http://hz.gotoacloud.top/gthiwabute.html

TS:   s.split("a").length - 1
来源：http://hz.aibaodan.cn/gthrwzhzno.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.gogol.net.cn/gtthuejyfa.html

Go:   strings.Count(s, "a")
来源：http://hz.guannengcc.top/gtljtkrlui.html

Ruby: s.count("a")
来源：http://hz.yvedp.cn/gtuxvmiual.html

C#:   s.Count(c => c == 'a')
来源：http://hz.dianchejie.cn/gtvodtvzpy.html

[E13] 逐字符遍历
来源：http://hz.gogol.net.cn/gtxusxmove.html

Py:   for ch in s: print(ch)
来源：http://hz.ivvv.top/gtgahzauqs.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.ydjk.org.cn/gtrdpapchu.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jinqigufen.top/gtmyqkmyrg.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jqgufenzy.top/gtupfwvgqs.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.fzhhl.top/gtrhlrobhi.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.xuetiantiany.cn/gttnkremyk.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.birdmap.top/gtskuhhnff.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.tian-w.cn/gtcpcguzza.html

[E14] URL 编码与 Base64
来源：http://hz.xinyue.icu/gtdewchlis.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.tian-w.cn/gtsllbxftn.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.yuanzhike.top/gtjcxfeqti.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.ydjk.org.cn/gtuxlwnsod.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.mhx1999.top/gtfefbfgoa.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.chenzaomai.com/gtdyyccgnt.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.zhijiandao.cn/gtoxxrxsef.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.yuanzhike.top/gtqdffomjs.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.hongshengwenyu.top/gtmrtnngbz.html

[E15] HTML 转义 / 反转义
来源：http://hz.cdnleiting.top/gtdxeohnlc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.xuanzx.com/gtyvzobkfe.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.c1oappe.top/gtgpcsapcb.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yuanzhike.top/gtaptqgcvb.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.xziqi.cn/gtcorbcexr.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.xingfuxueyuan.xyz/gtesyhzvdi.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.birdmap.top/gtqwbujfhu.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.yvedp.cn/gtqefayoqd.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.zhengqikj.top/gtyqarvaey.html

[E16] 数字千分位
来源：http://hz.yj20258.top/gtgwzrksmm.html

Py:   f"{1234567:,}"
来源：http://hz.gzhubu.top/gtlifjgfvr.html

PHP:  number_format(1234567);
来源：http://hz.ydzc1.top/gtutdnvxxq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.52xcode.cn/gtqocxxeor.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.jlsjyb.cn/gtrurhlwff.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.zhongyouzk.top/gtswtroybs.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.redwolf501.top/gtefnoixku.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.jinqigufen.top/gtpaaiyqfm.html

C#:   1234567.ToString("N0")
来源：http://hz.yuanzhike.top/gtinkkyany.html

[E17] 首字母大写
来源：http://hz.yangfankeji.com/gteqmydagk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.c1oappe.top/gtfghoswrh.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.snrcjt.cn/gtsyfblwfd.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.hammf.cn/gtjdxxengp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.gogol.net.cn/gtwdugjftr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.sweek.top/gtclsrjlfd.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.jinqigufen.top/gtykgxbeah.html

Ruby: s.capitalize
来源：http://hz.gotoacloud.top/gtodcdygrv.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.hysaishi.cn/gtpjeiqbrf.html

[E18] 模板占位符替换
来源：http://hz.nanxuanxn.top/gtbpaswcfv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.zhijiandao.cn/gtyyfkupvu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.jinyuanbaomall.cn/gttihvrbsh.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.jqgfzy.top/gtqbnegvqi.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.yvedp.cn/gtoztjguar.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.sufxvd.cn/gttbcxdstg.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.shanyushiyangkeji.top/gtesspyqxt.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.jinyuanbaomall.cn/gtcagsrifw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.shangyingyoupin.top/gtispstffh.html

[E19] 多行文本按行拆分
来源：http://hz.dianchejie.cn/gtfchyqybb.html

Py:   s.splitlines()
来源：http://hz.aibaodan.cn/gtjyogbzgp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.xingfuxueyuan.xyz/gtckafhifq.html

JS:   s.split(/\r?\n/)
来源：http://hz.redwolf501.top/gtwrapfhxk.html

TS:   s.split(/\r?\n/)
来源：http://hz.hnqzz.top/gtwjvmplxt.html

Java: s.lines().toList()
来源：http://hz.sweek.top/gttsmhhzja.html

Go:   strings.Split(s, "\n")
来源：http://hz.sxryk.cn/gttjzknfuk.html

Ruby: s.lines
来源：http://hz.gogol.net.cn/gtqdoewgjq.html

C#:   s.Split('\n')
来源：http://hz.meibo888.top/gtvumwqqqf.html

[E20] 判断字符串是否为空
来源：http://hz.chenlongwang.top/gtnjziuqvu.html

Py:   if not s:
来源：http://hz.ehwqpu.com/gtvbuzkbio.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.nanxuanxn.top/gthnyprhan.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.zdqjudy.top/gtbqcjyqfh.html

TS:   if (s === "") {}
来源：http://hz.yueranfly.top/gtwmlygibi.html

Java: if (s.isEmpty()) {}
来源：http://hz.aizwys.cn/gtudewidpl.html

Go:   if s == "" {}
来源：http://hz.quarkkingdee.top/gtisxohxrm.html

Ruby: if s.empty?
来源：http://hz.redwolf501.top/gttvonszms.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.yj202588.top/gtlcyhfswz.html

[E21] 超长截断加省略号
来源：http://hz.chenlongwang.top/gtdyxeprci.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.sufxvd.cn/gtwflbdxzb.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.smart0.xyz/gtumccllar.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yj20258888.top/gtljzashfs.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.guannengcc.top/gtnjgecfby.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.zhaomingkeji.xyz/gttpblviwz.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.havefunace.top/gtgxzffycz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.jinyuanbaomall.cn/gtzbcahcsh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.gaohongyu789.top/gteglvqrqx.html

[E22] 字节长度与字符长度
来源：http://hz.shanyushiyangtech.top/gtzmoswpbb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.cashguo.top/gtzvjkbvmh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jqgfzy.top/gtmkqaccmf.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.shzxlz.cn/gtumggiylp.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.nanxuanxn.top/gtwnciqeym.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.meibo888.top/gtnhtpkalr.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.yanxiufei.cn/gtbnyjbyba.html

Ruby: s.bytesize;  s.length
来源：http://hz.c1oappe.top/gtaziquipn.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.pengpengdd.cyou/gtgagbmcrh.html

================================================================================
来源：http://hz.redwolf501.top/gtuiwuawxs.html

F. 文件与目录
来源：http://hz.jyoumei.cn/gtpxrejexh.html

================================================================================
来源：http://hz.hnqzz.top/gtqrzegerl.html

[F01] 读取整个文件
来源：http://hz.jianghu66.top/gtujgzpdep.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.dianchejie.cn/gtamwkuvdc.html

PHP:  file_get_contents("a.txt");
来源：http://hz.bjfxy.top/gtkowijypg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.haohaochexian.top/gtmtmzjfia.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.hammf.cn/gtoqjlhyps.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.yongpay.top/gtwtnbprkh.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.smart0.xyz/gtnrbapaej.html

Ruby: File.read("a.txt")
来源：http://hz.yonumen.top/gtycrcgxfg.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.havefunace.top/gtfigezsya.html

[F02] 逐行读取文件
来源：http://hz.yuanzhike.top/gtanrwvybt.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.xylfe.cn/gtgtftdoml.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.ivvv.top/gtbpglvgrg.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.shangyingyoupin.top/gtydfjwoaf.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.shangyingyoupin.top/gtfswgnxsv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.cucudq.cn/gtqwhtbrnm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.zdqjudy.top/gtvauxapxt.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.haohaochexian.top/gtpjldjvzs.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.tanke756.top/gtcabnzzmj.html

[F03] 写入文件（覆盖）
来源：http://hz.vqdsnc.cn/gtvalljhlt.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.jiagoushi.top/gtnbtfsxud.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.shangyingyoupin.top/gtoonzszly.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.vqdsnc.cn/gttszhemnl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhiwuduotai.top/gttwfqjyag.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.havefunace.top/gtdbxagccj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.smart0.xyz/gtjrvtsgwj.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.jinqigfzy.top/gtcnscmaxf.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.hfpthk.cn/gtochuofgj.html

[F04] 追加写入文件
来源：http://hz.nanxuanxn.top/gtqdoulmeu.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.zhiwuduotai.top/gtlybrxovq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.gotoacloud.top/gtwcuamoqy.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zdqjudy.top/gtxftyxqlo.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yueranfly.top/gtacqqznkq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.hnqzz.top/gtlcmbecch.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.yonumen.top/gtcsotvmtg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yvedp.cn/gtefwnkbbn.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.tanke756.top/gtopiiyoqg.html

[F05] 判断文件或目录是否存在
来源：http://hz.fengsongda.top/gtffpujhke.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.redwolf501.top/gttruybagu.html

PHP:  file_exists("a.txt");
来源：http://hz.cheryme.top/gthpughznr.html

JS:   fs.existsSync("a.txt")
来源：http://hz.havefunace.top/gttupxypqn.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yangfankeji.com/gtqielduew.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.guowangkeji.top/gtcjfwrsft.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.ydjk.org.cn/gtqarzmovg.html

Ruby: File.exist?("a.txt")
来源：http://hz.yj20258.top/gtxmmioywr.html

C#:   File.Exists("a.txt")
来源：http://hz.jinqigfzy.top/gtkrjybkax.html

[F06] 删除文件
来源：http://hz.cucudq.cn/gtkwdehlja.html

Py:   os.remove("a.txt")
来源：http://hz.redwolf501.top/gtqwiyfpdv.html

PHP:  unlink("a.txt");
来源：http://hz.ywan-chungtsiang.top/gtvcpmvcdz.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.redwolf501.top/gtyvurvibl.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.shuidangran.top/gtduajyovk.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.jyoumei.cn/gtgxrbfwmb.html

Go:   os.Remove("a.txt")
来源：http://hz.haohaochexian.top/gtkcskahbg.html

Ruby: File.delete("a.txt")
来源：http://hz.aibaodan.cn/gtldyuvgba.html

C#:   File.Delete("a.txt");
来源：http://hz.hnxiangtu.top/gtiluznbje.html

[F07] 创建目录（含多级）
来源：http://hz.hammf.cn/gtwdiljkge.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.gzhubu.top/gtqxqjzbgy.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.iojbl.cn/gtelfzqacy.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhengqikj.top/gtmgeunggl.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhijiandao.cn/gttrbwhxvj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.wangdashe.top/gtnzefqgnu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.sweek.top/gtclrhtnzt.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.zhixingplan.top/gtsarraezi.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.sufxvd.cn/gtwgacrdov.html

[F08] 遍历目录
来源：http://hz.jqgfzy.top/gtthtksoav.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.xziqi.cn/gteldaates.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.cucudq.cn/gtogpfyydr.html

JS:   fs.readdirSync("dir")
来源：http://hz.aizwys.cn/gttzmtueab.html

TS:   fs.readdirSync("dir")
来源：http://hz.shanyushiyangkeji.top/gtmhagqavl.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.yuanzhike.top/gtaedrocqw.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.shzxlz.cn/gtbyshwrsc.html

Ruby: Dir.children("dir")
来源：http://hz.quarkkingdee.top/gthptxagjw.html

C#:   Directory.GetFiles("dir")
来源：http://hz.ehwqpu.com/gttohublik.html

[F09] 获取文件大小
来源：http://hz.yongpay.top/gtcsyhzyel.html

Py:   os.path.getsize("a.txt")
来源：http://hz.cucudq.cn/gtxoxuwhzw.html

PHP:  filesize("a.txt");
来源：http://hz.shzxlz.cn/gtxxllqota.html

JS:   fs.statSync("a.txt").size
来源：http://hz.shanyushiyangtech.top/gtyxnwclpu.html

TS:   fs.statSync("a.txt").size
来源：http://hz.gogol.net.cn/gtdvwwhyrl.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.0kj1m.cn/gtofxjtbkd.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.pycfn.com/gtkobzeynk.html

Ruby: File.size("a.txt")
来源：http://hz.nwbrower.top/gtdiwzsoti.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.jinqigfzy.top/gtmwikiqur.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.jqgfzy.top/gtbctvfvbf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.cashguo.top/gtmtsnbcdb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.svipenyu.cn/gtfidztjyc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.hywenlv.cn/gtjfjroxlw.html

TS:   path.extname("a.txt")
来源：http://hz.sufxvd.cn/gtmiqjgtip.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.smart0.xyz/gthylasnos.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.zhaomingkeji.xyz/gtkebcrjdu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.meibo888.top/gtbhpmzmps.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.shanyushiyangtech.top/gtvkgfbpmr.html

[F11] 复制与移动文件
来源：http://hz.gzhubu.top/gtqxbljbco.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.guannengcc.top/gtwzjdguqm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.dashuyun.cn/gtctewqqcd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.sysykeji.top/gtzboklvwj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zdqjudy.top/gtvdbtjyjd.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.sysykeji.top/gtuhqdxhnw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jlsjyb.cn/gtemxrqbuo.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.birdmap.top/gtghtvbnks.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.hammf.cn/gtyjiymleg.html

[F12] CSV 读写
来源：http://hz.yj20258888.top/gthsfwmmcl.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.wangshuangyany.cn/gtmrgdtedg.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.tanke756.top/gtudwedamo.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.jlsjyb.cn/gttcksfgrf.html

TS:   // 同上
来源：http://hz.ydjk.org.cn/gtufnhrqob.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.zhengqikj.top/gtejybuljq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.cqqwz.cn/gtnybloimy.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.aibaodan.cn/gtxetwodua.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.ydzc1.top/gtqecmbdyo.html

================================================================================
来源：http://hz.c1oappe.top/gtrdrblayk.html

G. 面向对象
来源：http://hz.haohaochexian.top/gtdjpxeeuc.html

================================================================================
来源：http://hz.haohaochexian.top/gtrrwobbjy.html

[G01] 定义类
来源：http://hz.dashuyun.cn/gtmuxwxvyc.html

Py:   class User: pass
来源：http://hz.wangshuangyany.cn/gthszysawe.html

PHP:  class User {}
来源：http://hz.xuanzx.com/gtcruemkmu.html

JS:   class User {}
来源：http://hz.iojbl.cn/gtfjbmuegp.html

TS:   class User { name: string = ""; }
来源：http://hz.zdqjudy.top/gtbatuybxw.html

Java: class User {}
来源：http://hz.shuidangran.top/gtwvokicwd.html

Go:   type User struct { Name string }
来源：http://hz.zhoulong.xyz/gtnqylraga.html

Ruby: class User; end
来源：http://hz.meibo888.top/gtptdxybbg.html

C#:   class User {}
来源：http://hz.mhx1999.top/gtcoqmwjkx.html

[G02] 构造函数
来源：http://hz.jianghu66.top/gteyrofpaa.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.tian-w.cn/gtbkcteoul.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.xuetiantiany.cn/gtirohkfdv.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.9152youxi.cn/gtjtknhfue.html

TS:   constructor(public name: string) {}
来源：http://hz.vqdsnc.cn/gthsoxgonx.html

Java: User(String name) { this.name = name; }
来源：http://hz.dashuyun.cn/gttrgnhkbr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.hfpthk.cn/gtndcxsylt.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.sweek.top/gtkbpocfjy.html

C#:   public User(string name) { Name = name; }
来源：http://hz.zdqjudy.top/gtowqfaogi.html

[G03] 实例属性
来源：http://hz.guannengcc.top/gtspcvmgss.html

Py:   self.name = "x"
来源：http://hz.dashuyun.cn/gtbqjlmcmd.html

PHP:  public string $name = "x";
来源：http://hz.yuanzhike.top/gtrwenaxgb.html

JS:   this.name = "x";
来源：http://hz.shzxlz.cn/gtoaydekze.html

TS:   name: string = "x";
来源：http://hz.nwbrower.top/gtgctpepky.html

Java: private String name;
来源：http://hz.dashuyun.cn/gtowbnzajk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.svipenyu.cn/gtgljgzvsl.html

Ruby: @name = "x"
来源：http://hz.yanxiufei.cn/gtkunluylh.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.wangdashe.top/gtvwjnmqvx.html

[G04] 定义方法
来源：http://hz.xylfe.cn/gtqjlgsgxu.html

Py:   def greet(self): return self.name
来源：http://hz.yuxming.cn/gtqkblmyig.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.hnqzz.top/gtdnthmjtn.html

JS:   greet() { return this.name; }
来源：http://hz.jiagoushi.top/gtihuiulav.html

TS:   greet(): string { return this.name; }
来源：http://hz.jqgufenzy.top/gtmyifsins.html

Java: String greet() { return name; }
来源：http://hz.zhiwuduotai.top/gtvdcjpgwy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.yangfankeji.com/gtvrapbhau.html

Ruby: def greet; @name; end
来源：http://hz.dashuyun.cn/gtixpfynrn.html

C#:   public string Greet() => Name;
来源：http://hz.cqqwz.cn/gtrsmbcntl.html

[G05] 继承
来源：http://hz.zhengqikj.top/gtwbgzssue.html

Py:   class Admin(User): pass
来源：http://hz.zhiwuduotai.top/gtzppemuqy.html

PHP:  class Admin extends User {}
来源：http://hz.gzhubu.top/gtubfubusx.html

JS:   class Admin extends User {}
来源：http://hz.yonumen.top/gtomokccmm.html

TS:   class Admin extends User {}
来源：http://hz.yongpay.top/gtxyyisnvo.html

Java: class Admin extends User {}
来源：http://hz.svipenyu.cn/gtnmyhrniw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.daxiang520.top/gtpixfbnri.html

Ruby: class Admin < User; end
来源：http://hz.zhijiandao.cn/gtelwjknqm.html

C#:   class Admin : User {}
来源：http://hz.daxiang520.top/gtatxcgnzh.html

[G06] 重写方法
来源：http://hz.nanxinkj.top/gtigynowdn.html

Py:   def greet(self): return "admin"
来源：http://hz.xziqi.cn/gtrhoqyhib.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jiagoushi.top/gtgcxctfls.html

JS:   greet() { return "admin"; }
来源：http://hz.gzhubu.top/gtorhmhukm.html

TS:   greet(): string { return "admin"; }
来源：http://hz.aibaodan.cn/gtzaofkdck.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.hfpthk.cn/gtgjkjuhvd.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.jqgfzy.top/gtvsugjxag.html

Ruby: def greet; "admin"; end
来源：http://hz.sxryk.cn/gttiqpayyl.html

C#:   public override string Greet() => "admin";
来源：http://hz.sxryk.cn/gtgqklbykh.html

[G07] 调用父类方法
来源：http://hz.9152youxi.cn/gtlmmttsiv.html

Py:   super().greet()
来源：http://hz.jinyuanbaomall.cn/gtdjwboyiw.html

PHP:  parent::greet();
来源：http://hz.yueranfly.top/gtwkuabvpt.html

JS:   super.greet();
来源：http://hz.ydjk.org.cn/gtesidigbl.html

TS:   super.greet();
来源：http://hz.shuidangran.top/gtdnkxyggm.html

Java: super.greet();
来源：http://hz.birdmap.top/gtoebxzuok.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.daxiang520.top/gtynufnfan.html

Ruby: super
来源：http://hz.tianlin.xyz/gtneznmnen.html

C#:   base.Greet();
来源：http://hz.hnqzz.top/gttnvgkrwv.html

[G08] 静态方法与属性
来源：http://hz.yueranfly.top/gtvjapsajt.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.hammf.cn/gtbvjndebn.html

PHP:  public static function f() {}
来源：http://hz.jinqigfzy.top/gtjdakzphk.html

JS:   static f() {}
来源：http://hz.zhiwuduotai.top/gthobzvfwa.html

TS:   static f(): void {}
来源：http://hz.xuanzx.com/gtgjyoamjr.html

Java: static void f() {}
来源：http://hz.jinghuilouyu.cn/gttjcwtxet.html


<!-- 参考信息 -->