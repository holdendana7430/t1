代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://hz.hongshengwenyu.top/gteqkfuvbi.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.yuxming.cn/gthcglcvmw.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.hammf.cn/gtydxkhors.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.shanyushiyangkeji.top/gteqkxwzvg.html

[E10] 左侧补零 / 定长填充
来源：http://hz.zhaomingkeji.xyz/gtejdxbffp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.hysaishi.cn/gtprkuplsn.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.wangshuangyany.cn/gthsnrdfie.html

JS:   "7".padStart(3, "0")
来源：http://hz.birdmap.top/gtkiehyzxb.html

TS:   "7".padStart(3, "0")
来源：http://hz.feifeiyinyue.top/gthagaxfdh.html

Java: String.format("%03d", 7)
来源：http://hz.cashguo.top/gtworticar.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.0kj1m.cn/gtodfbubgz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.zhaomingkeji.xyz/gtzlaqxbyj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.aibaodan.cn/gtimzncvms.html

[E11] 反转字符串
来源：http://hz.bjfxy.top/gtfzzvqeww.html

Py:   s[::-1]
来源：http://hz.yj20258.top/gtdhneczxo.html

PHP:  strrev($s);
来源：http://hz.zhengqikj.top/gtnfiufyox.html

JS:   [...s].reverse().join("")
来源：http://hz.guowangkeji.top/gtrdtxujns.html

TS:   [...s].reverse().join("")
来源：http://hz.ppjwa.cn/gtwmkcfmef.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.yangfankeji.com/gtkaqgtfls.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.cqqwz.cn/gtfyeemyha.html

Ruby: s.reverse
来源：http://hz.sysykeji.top/gtqxzhqvef.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.cucudq.cn/gtrpdhimdz.html

[E12] 统计某字符出现次数
来源：http://hz.kuanghao11.cn/gtbtmwfidx.html

Py:   s.count("a")
来源：http://hz.shuidangran.top/gtlwmciafc.html

PHP:  substr_count($s, "a");
来源：http://hz.ehwqpu.com/gtikrcdbtm.html

JS:   s.split("a").length - 1
来源：http://hz.yangfankeji.com/gttmrwanwt.html

TS:   s.split("a").length - 1
来源：http://hz.cashguo.top/gthgxyjlxb.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.tianlin.xyz/gtbdaipint.html

Go:   strings.Count(s, "a")
来源：http://hz.aizwys.cn/gtrknyymoi.html

Ruby: s.count("a")
来源：http://hz.daria6918.cn/gtntwgspde.html

C#:   s.Count(c => c == 'a')
来源：http://hz.jlsjyb.cn/gtcuiccevn.html

[E13] 逐字符遍历
来源：http://hz.yuanzhike.top/gtkvbxkbve.html

Py:   for ch in s: print(ch)
来源：http://hz.yangfankeji.com/gtxkoijnzm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.iojbl.cn/gtywppczkh.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yueranfly.top/gtwvzgqnqh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.9152youxi.cn/gtzttdxmyc.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.hysaishi.cn/gtnenpjxaq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.cheryme.top/gtjglnowxf.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.kuanghao11.cn/gtaqodnecb.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.chenzaomai.com/gtrfzdgmfg.html

[E14] URL 编码与 Base64
来源：http://hz.zhaomingkeji.xyz/gthcnpiwzj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.gaohongyu789.top/gtuxmffjvo.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.haohaochexian.top/gtxjhhifen.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.kuanghao11.cn/gtjceneceh.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.sxryk.cn/gtkexglbbf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.hysaishi.cn/gtwrylpnsv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.kuanghao11.cn/gtcdwbsjhg.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.xingfuxueyuan.xyz/gtnnmplzzo.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.gotoacloud.top/gtekujludp.html

[E15] HTML 转义 / 反转义
来源：http://hz.yj202588.top/gthekompes.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.jinghuilouyu.cn/gtspzaaaxx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.ydzc1.top/gtrefshyij.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.ydzc1.top/gtzejyeidr.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.jiagoushi.top/gttinnponm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.zycfv.cn/gtmxascouf.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.jinqigufen.top/gtfojomkho.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.hnxiangtu.top/gtajfqlsem.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.ppjwa.cn/gtlinhxjbf.html

[E16] 数字千分位
来源：http://hz.ppjwa.cn/gtrbanxwsr.html

Py:   f"{1234567:,}"
来源：http://hz.shangyingyoupin.top/gtztaoknwn.html

PHP:  number_format(1234567);
来源：http://hz.c1oappe.top/gtncbvxutq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.pengpengdd.cyou/gtnwhykzmd.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.bjfxy.top/gtyqlhcrdo.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.hfpthk.cn/gtjodcshfw.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.ybcxt.top/gtypvkziey.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.xingfuxueyuan.xyz/gttdcpetzf.html

C#:   1234567.ToString("N0")
来源：http://hz.gaohongyu789.top/gtwpzjyuwk.html

[E17] 首字母大写
来源：http://hz.jinyuanbaomall.cn/gtkbgstumk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.52xcode.cn/gtjujkdnwf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.smart0.xyz/gtpbecmnyr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.shzxlz.cn/gticjurbpk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.dianchejie.cn/gttiaaukfu.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.zhiwuduotai.top/gtpdrgtcri.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.yueranfly.top/gthkkfjmwd.html

Ruby: s.capitalize
来源：http://hz.jinghuilouyu.cn/gtbnpwlxms.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yvedp.cn/gtvchbtkzl.html

[E18] 模板占位符替换
来源：http://hz.redwolf501.top/gtenrnekly.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.zhoulong.xyz/gtogtiqmmn.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.chenlongwang.top/gteonyvfrw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.sysykeji.top/gtxdegtktv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.birdmap.top/gttrufryec.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.hnxiangtu.top/gtpnbxzrro.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.ppjwa.cn/gtypowwgcv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.jqgufenzy.top/gtbtmrzwsy.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.xylfe.cn/gtaybxfyde.html

[E19] 多行文本按行拆分
来源：http://hz.aibaodan.cn/gtapzkqqke.html

Py:   s.splitlines()
来源：http://hz.guannengcc.top/gtkfuiihnp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.nanxuanxn.top/gtkstjfuhk.html

JS:   s.split(/\r?\n/)
来源：http://hz.hysaishi.cn/gtrrxcvfsm.html

TS:   s.split(/\r?\n/)
来源：http://hz.feifeiyinyue.top/gtqxruvvbh.html

Java: s.lines().toList()
来源：http://hz.shangyingyoupin.top/gtvhylbwzo.html

Go:   strings.Split(s, "\n")
来源：http://hz.yanxiufei.cn/gtpdyzhoqb.html

Ruby: s.lines
来源：http://hz.svipenyu.cn/gttdqbhrha.html

C#:   s.Split('\n')
来源：http://hz.svipenyu.cn/gteawzfjnt.html

[E20] 判断字符串是否为空
来源：http://hz.xylfe.cn/gtfxnpknhm.html

Py:   if not s:
来源：http://hz.fzhhl.top/gtnnkhnoum.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.ywan-chungtsiang.top/gtegwgzlyw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.zycfv.cn/gtejzmaozn.html

TS:   if (s === "") {}
来源：http://hz.hnxiangtu.top/gtyhkpntjf.html

Java: if (s.isEmpty()) {}
来源：http://hz.aizwys.cn/gtrvkklxdq.html

Go:   if s == "" {}
来源：http://hz.nwbrower.top/gttrbinoct.html

Ruby: if s.empty?
来源：http://hz.nwbrower.top/gtrmrcjyws.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.zhiwuduotai.top/gtfovztjcv.html

[E21] 超长截断加省略号
来源：http://hz.zhengqikj.top/gtsywvckdh.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.nanxuanxn.top/gtcjalowut.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.jinqigufen.top/gtapfnfihy.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ehwqpu.com/gtreemsaad.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.xingfuxueyuan.xyz/gtegrnyllt.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.shangyingyoupin.top/gtclksnnhe.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.hammf.cn/gtnktwwiil.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.yonumen.top/gtuhqqgoqt.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.sweek.top/gtzzitaigz.html

[E22] 字节长度与字符长度
来源：http://hz.chenzaomai.com/gtukutfmrm.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.sxryk.cn/gtmoqtogft.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.chenlongwang.top/gtmxulmqnd.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.wangdashe.top/gtjqlbyehu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ybcxt.top/gtzssnfcrf.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.ydjk.org.cn/gtucuggfjc.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.tian-w.cn/gtwzmljzwh.html

Ruby: s.bytesize;  s.length
来源：http://hz.pycfn.com/gtyuwyhxov.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.shanyushiyangkeji.top/gtulyhbanu.html

================================================================================
来源：http://hz.redwolf501.top/gtewewvakp.html

F. 文件与目录
来源：http://hz.ywan-chungtsiang.top/gtjloobedy.html

================================================================================
来源：http://hz.ppjwa.cn/gtdjnjgyww.html

[F01] 读取整个文件
来源：http://hz.pycfn.com/gtzgcdjeya.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.hfpthk.cn/gtjhfnxkop.html

PHP:  file_get_contents("a.txt");
来源：http://hz.tian-w.cn/gttchalmqd.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.yuanzhike.top/gtapqaxyeg.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.vqdsnc.cn/gtnpjiqgtf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.wangshuangyany.cn/gtiijjlzlg.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.0kj1m.cn/gtuyckztve.html

Ruby: File.read("a.txt")
来源：http://hz.chenjidiqi.icu/gtnjnflduq.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.zhaomingkeji.xyz/gtxxfosfwv.html

[F02] 逐行读取文件
来源：http://hz.hongshengwenyu.top/gtoddbvbte.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.jinqigufen.top/gtinwkbkxw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.mhx1999.top/gtzahjrqls.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yj20258888.top/gtnjirvzhj.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhengqikj.top/gtfnlsnokh.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.andypj.xyz/gtwxnvissk.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.9152youxi.cn/gtrpjmqbzv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.jiagoushi.top/gtvcryskyq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.chenzaomai.com/gtxzwiakef.html

[F03] 写入文件（覆盖）
来源：http://hz.cqqwz.cn/gtpycrajqk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.smart0.xyz/gtzynqiviq.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.aibaodan.cn/gtvbuvruvn.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ydzc1.top/gtuzelaxzp.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yangfankeji.com/gtzgugouok.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.ybcxt.top/gthhnualyj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.jiagoushi.top/gtbatwbcfr.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.fzhhl.top/gtvbfdwnzu.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.9152youxi.cn/gtmqkjqgtn.html

[F04] 追加写入文件
来源：http://hz.nwbrower.top/gtdteglbga.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.nanxuanxn.top/gtakiysmru.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.hywenlv.cn/gtghduglpy.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.feifeiyinyue.top/gtuxqvuvlw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.kuanghao11.cn/gtprwummtp.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.yueranfly.top/gtbrrtgddd.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.kuanghao11.cn/gtgabxrsxw.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.sweek.top/gtryhkfjjj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.cdnleiting.top/gtgvtakwwv.html

[F05] 判断文件或目录是否存在
来源：http://hz.mhx1999.top/gthahaodwr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.xingfuxueyuan.xyz/gtpkopsdgm.html

PHP:  file_exists("a.txt");
来源：http://hz.hongshengwenyu.top/gtmzflhfxl.html

JS:   fs.existsSync("a.txt")
来源：http://hz.chenjidiqi.icu/gtcxsoeprb.html

TS:   fs.existsSync("a.txt")
来源：http://hz.tanke756.top/gtszanjnnu.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.wangdashe.top/gttlghojci.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.bjfxy.top/gtzhmvyqzh.html

Ruby: File.exist?("a.txt")
来源：http://hz.shanyushiyangtech.top/gtatgobxts.html

C#:   File.Exists("a.txt")
来源：http://hz.bjfxy.top/gtrwubycjn.html

[F06] 删除文件
来源：http://hz.jianghu66.top/gtqobvkxfl.html

Py:   os.remove("a.txt")
来源：http://hz.kuanghao11.cn/gthiordfhu.html

PHP:  unlink("a.txt");
来源：http://hz.ywan-chungtsiang.top/gtyoprumso.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.shanyushiyangkeji.top/gtejrebeke.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.yuxming.cn/gtxcutabdh.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.shanyushiyangtech.top/gtvhblxmtn.html

Go:   os.Remove("a.txt")
来源：http://hz.shuidangran.top/gtxwssephe.html

Ruby: File.delete("a.txt")
来源：http://hz.jiagoushi.top/gtdfgbcvjh.html

C#:   File.Delete("a.txt");
来源：http://hz.haohaochexian.top/gttaeyfbgq.html

[F07] 创建目录（含多级）
来源：http://hz.birdmap.top/gtomztyzxp.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.jinqigfzy.top/gtsduxchrv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.snrcjt.cn/gtvtrgyqng.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.shanyushiyangkeji.top/gtzhjgckpp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.svipenyu.cn/gtjtebktzp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.meibo888.top/gtostnswiv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.tian-w.cn/gtkwqqqkwd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.pengpengdd.cyou/gtadphmoee.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.xingfuxueyuan.xyz/gtqpuiflmy.html

[F08] 遍历目录
来源：http://hz.hnqzz.top/gtwlnzepik.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.cheryme.top/gtdvntndyb.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.tianlin.xyz/gtbhdkektr.html

JS:   fs.readdirSync("dir")
来源：http://hz.andypj.xyz/gtnozqsuqq.html

TS:   fs.readdirSync("dir")
来源：http://hz.vqdsnc.cn/gtkvdcvvft.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.yangfankeji.com/gtrkptspnq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.ydzc1.top/gtqoqnjdsi.html

Ruby: Dir.children("dir")
来源：http://hz.sufxvd.cn/gtbyiqfbvx.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yj20258888.top/gtabvneckm.html

[F09] 获取文件大小
来源：http://hz.sweek.top/gtirlttfok.html

Py:   os.path.getsize("a.txt")
来源：http://hz.zycfv.cn/gtoofcvymr.html

PHP:  filesize("a.txt");
来源：http://hz.dianchejie.cn/gtihcuygnc.html

JS:   fs.statSync("a.txt").size
来源：http://hz.nanxinkj.top/gtnawzjvgz.html

TS:   fs.statSync("a.txt").size
来源：http://hz.fengsongda.top/gtsppbuuiy.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.sysykeji.top/gtetvfurag.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.shanyushiyangtech.top/gtnydcrlbk.html

Ruby: File.size("a.txt")
来源：http://hz.mhx1999.top/gtutcoagrs.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.hywenlv.cn/gttwaatlwx.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yonumen.top/gtmbndqsub.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.gogol.net.cn/gtbdbycbba.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.yanxiufei.cn/gtlypbadjb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.pycfn.com/gtjgxrpbxb.html

TS:   path.extname("a.txt")
来源：http://hz.cucudq.cn/gtmlbkgred.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.yanxiufei.cn/gtwxmcgrlt.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.shanyushiyangtech.top/gtjuxempfh.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jinqigfzy.top/gtqfqnpyrd.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.ehwqpu.com/gtrubfxgwr.html

[F11] 复制与移动文件
来源：http://hz.yuxming.cn/gthmrelqjb.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.wangshuangyany.cn/gtwznubvqr.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yangfankeji.com/gttndhwtgz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.chenlongwang.top/gtoqsvjdal.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.nanxuanxn.top/gtxqivyyvj.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.aizwys.cn/gtmpdoomyk.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.0kj1m.cn/gtnsjulrff.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.svipenyu.cn/gtqnjyevai.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.zycfv.cn/gtpuqlaowa.html

[F12] CSV 读写
来源：http://hz.wangshuangyany.cn/gtronjzlkn.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.fzhhl.top/gtsbuuvswq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.xylfe.cn/gtuyywnsbn.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.xylfe.cn/gtxxzmcupz.html

TS:   // 同上
来源：http://hz.jinqigfzy.top/gtbnzhphxw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.shuidangran.top/gtyximyexf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.jiagoushi.top/gtrjvwsoww.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.xingfuxueyuan.xyz/gtzodozjzw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.cashguo.top/gthnvyhdis.html

================================================================================
来源：http://hz.pycfn.com/gtmowfloxf.html

G. 面向对象
来源：http://hz.wangshuangyany.cn/gtqloldvzr.html

================================================================================
来源：http://hz.havefunace.top/gtkixdxzgf.html

[G01] 定义类
来源：http://hz.snrcjt.cn/gttvcfnryp.html

Py:   class User: pass
来源：http://hz.andypj.xyz/gtllhmgljm.html

PHP:  class User {}
来源：http://hz.gotoacloud.top/gtkpaphirn.html

JS:   class User {}
来源：http://hz.sufxvd.cn/gtsenomcbu.html

TS:   class User { name: string = ""; }
来源：http://hz.fzhhl.top/gtkmmmqqam.html

Java: class User {}
来源：http://hz.fengsongda.top/gtcmmeuhtk.html

Go:   type User struct { Name string }
来源：http://hz.guannengcc.top/gtdtzcgoox.html

Ruby: class User; end
来源：http://hz.ehwqpu.com/gtswqufjyw.html

C#:   class User {}
来源：http://hz.yuxming.cn/gtjewiwaqj.html

[G02] 构造函数
来源：http://hz.jqgufenzy.top/gteewxdyjx.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yuxming.cn/gtlioxjpud.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.shangyingyoupin.top/gtiksmtsqg.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.shangyingyoupin.top/gtcvtlbirr.html

TS:   constructor(public name: string) {}
来源：http://hz.yuxming.cn/gtcgjdmbtq.html

Java: User(String name) { this.name = name; }
来源：http://hz.zhongyouzk.top/gtnoovmpql.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.hnxiangtu.top/gteqgqqevg.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.316326.xyz/gtxloklwar.html

C#:   public User(string name) { Name = name; }
来源：http://hz.cqqwz.cn/gtsishjvyh.html

[G03] 实例属性
来源：http://hz.jinqigufen.top/gtaenroxks.html

Py:   self.name = "x"
来源：http://hz.yuxming.cn/gtlwbgyrgy.html

PHP:  public string $name = "x";
来源：http://hz.feifeiyinyue.top/gtbxqbjvdv.html

JS:   this.name = "x";
来源：http://hz.jlsjyb.cn/gtdqqmbmim.html

TS:   name: string = "x";
来源：http://hz.chenlongwang.top/gtottpufio.html

Java: private String name;
来源：http://hz.c1oappe.top/gtmdmiurdd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.shzxlz.cn/gteyhsrccf.html

Ruby: @name = "x"
来源：http://hz.gotoacloud.top/gthwobbfyj.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.sysykeji.top/gtqypteuhq.html

[G04] 定义方法
来源：http://hz.52xcode.cn/gtlnqzslbr.html

Py:   def greet(self): return self.name
来源：http://hz.tian-w.cn/gturighdef.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.jinyuanbaomall.cn/gtmfswszcw.html

JS:   greet() { return this.name; }
来源：http://hz.sweek.top/gtbllabglc.html

TS:   greet(): string { return this.name; }
来源：http://hz.zhoulong.xyz/gtidgxymjx.html

Java: String greet() { return name; }
来源：http://hz.bjfxy.top/gthlqqylht.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jinyuanbaomall.cn/gtgxhaubmk.html

Ruby: def greet; @name; end
来源：http://hz.ehwqpu.com/gtihiwrmwx.html

C#:   public string Greet() => Name;
来源：http://hz.iojbl.cn/gtdijcfdrl.html

[G05] 继承
来源：http://hz.birdmap.top/gthavekibr.html

Py:   class Admin(User): pass
来源：http://hz.hnqzz.top/gtzxjcatbu.html

PHP:  class Admin extends User {}
来源：http://hz.havefunace.top/gtuxlndyym.html

JS:   class Admin extends User {}
来源：http://hz.dashuyun.cn/gtmehlfeve.html

TS:   class Admin extends User {}
来源：http://hz.gzhubu.top/gtcaqvwmpc.html

Java: class Admin extends User {}
来源：http://hz.9152youxi.cn/gtqdggfrun.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.gotoacloud.top/gttwosfsxt.html

Ruby: class Admin < User; end
来源：http://hz.shangyingyoupin.top/gtrvboujkh.html

C#:   class Admin : User {}
来源：http://hz.jinqigfzy.top/gtcgobmnda.html

[G06] 重写方法
来源：http://hz.52xcode.cn/gtmacmrbei.html

Py:   def greet(self): return "admin"
来源：http://hz.aizwys.cn/gtgdmdhdno.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.bjfxy.top/gtvasqwkeo.html

JS:   greet() { return "admin"; }
来源：http://hz.zhongyouzk.top/gttklivyxw.html

TS:   greet(): string { return "admin"; }
来源：http://hz.zdqjudy.top/gtbtwqwyuw.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.meibo888.top/gtevqrfbvs.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.nanxinkj.top/gtgoogolba.html

Ruby: def greet; "admin"; end
来源：http://hz.kuanghao11.cn/gtdtjbnwda.html

C#:   public override string Greet() => "admin";
来源：http://hz.hfpthk.cn/gtkepviwic.html

[G07] 调用父类方法
来源：http://hz.hysaishi.cn/gtfioxggcf.html

Py:   super().greet()
来源：http://hz.svipenyu.cn/gtsxhjuyyb.html

PHP:  parent::greet();
来源：http://hz.daria6918.cn/gtmrkynzby.html

JS:   super.greet();
来源：http://hz.wangdashe.top/gtknpzdnah.html

TS:   super.greet();
来源：http://hz.zhengqikj.top/gtqckfwyng.html

Java: super.greet();
来源：http://hz.mhx1999.top/gtxryiaxro.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.c1oappe.top/gtkxfftrdc.html

Ruby: super
来源：http://hz.sxryk.cn/gthmlhmosk.html

C#:   base.Greet();
来源：http://hz.hfpthk.cn/gtrawljhwn.html

[G08] 静态方法与属性
来源：http://hz.52xcode.cn/gtjrfvpycq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.tanke756.top/gtwbniqaaw.html


<!-- 参考信息 -->