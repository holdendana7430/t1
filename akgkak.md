代发 wailian999

Go:   strings.Join(items, ",")
来源：http://hz.c1oappe.top/gtmlmbhvce.html

Ruby: items.join(",")
来源：http://hz.jqgufenzy.top/gtlfvgfwbd.html

C#:   string.Join(",", items)
来源：http://hz.nwbrower.top/gtyzkhrnuj.html

[E09] 去除所有空白字符
来源：http://hz.mhx1999.top/gtelxiyasw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.ppjwa.cn/gtoaxszbva.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.ivvv.top/gttfoxcqbx.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.cucudq.cn/gtlphkmmkq.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.xuetiantiany.cn/gtdsrihlzo.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.tianlin.xyz/gtsycnukos.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.sufxvd.cn/gtmazblahn.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.guowangkeji.top/gttaqlstju.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.jinghuilouyu.cn/gtlxqpdzcc.html

[E10] 左侧补零 / 定长填充
来源：http://hz.zhongyouzk.top/gtheovzqaj.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.hywenlv.cn/gtzmfcdowp.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.hywenlv.cn/gtiqwjfhbf.html

JS:   "7".padStart(3, "0")
来源：http://hz.ehwqpu.com/gtjtgpmrlz.html

TS:   "7".padStart(3, "0")
来源：http://hz.fzhhl.top/gtkatfyjeo.html

Java: String.format("%03d", 7)
来源：http://hz.daxiang520.top/gtcwzkpvpd.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.9152youxi.cn/gtmvzwhgud.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.haohaochexian.top/gtommxjjeo.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.tianlin.xyz/gtiqffrvvl.html

[E11] 反转字符串
来源：http://hz.ybcxt.top/gtvlxzmzyf.html

Py:   s[::-1]
来源：http://hz.daxiang520.top/gteaqnhhls.html

PHP:  strrev($s);
来源：http://hz.ywan-chungtsiang.top/gtkwbrgyto.html

JS:   [...s].reverse().join("")
来源：http://hz.yangfankeji.com/gttufhppdo.html

TS:   [...s].reverse().join("")
来源：http://hz.shanyushiyangtech.top/gtvauzhado.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.zhengqikj.top/gtqwtzafpg.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.guannengcc.top/gttazragbi.html

Ruby: s.reverse
来源：http://hz.yj20258888.top/gtgkfqgptd.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.yuxming.cn/gtrihqeypp.html

[E12] 统计某字符出现次数
来源：http://hz.nanxinkj.top/gtlhrmkkki.html

Py:   s.count("a")
来源：http://hz.jqgufenzy.top/gtxcvtuqbp.html

PHP:  substr_count($s, "a");
来源：http://hz.52xcode.cn/gtspoiijks.html

JS:   s.split("a").length - 1
来源：http://hz.ywan-chungtsiang.top/gtbvvgsjhr.html

TS:   s.split("a").length - 1
来源：http://hz.jinghuilouyu.cn/gtkfoxpabs.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.sufxvd.cn/gtyxlxepji.html

Go:   strings.Count(s, "a")
来源：http://hz.quarkkingdee.top/gtlpwqhbqm.html

Ruby: s.count("a")
来源：http://hz.hammf.cn/gtqvivxziy.html

C#:   s.Count(c => c == 'a')
来源：http://hz.xylfe.cn/gteeqaqmib.html

[E13] 逐字符遍历
来源：http://hz.zhongyouzk.top/gtzskpizwt.html

Py:   for ch in s: print(ch)
来源：http://hz.iojbl.cn/gtnezoocru.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.svipenyu.cn/gtpfhutxae.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xuanzx.com/gteejbnrkm.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zycfv.cn/gtzikiqrgw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.yj20258888.top/gthnyrutsq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.fzhhl.top/gtztwjwwaj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.nwbrower.top/gtpgdvgyhu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.nwbrower.top/gtgyyujonp.html

[E14] URL 编码与 Base64
来源：http://hz.316326.xyz/gtvenuzkzo.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.jinghuilouyu.cn/gtqufubgim.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.jinqigfzy.top/gtntwzabqm.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.zhoulong.xyz/gtemphfptt.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.zdqjudy.top/gtcekjlssb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.zhoulong.xyz/gtxwbyongo.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.hfpthk.cn/gtounatbfg.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.hnxiangtu.top/gttikdcrgs.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yj20258.top/gthizckkwv.html

[E15] HTML 转义 / 反转义
来源：http://hz.yanxiufei.cn/gtbbefwvpr.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.guowangkeji.top/gtovcnhbqn.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.jinqigfzy.top/gtqogniwdz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.jinqigfzy.top/gtosnfgore.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.mhx1999.top/gtajmqxuvo.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.vqdsnc.cn/gtlsbjlpxf.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.pycfn.com/gtfadoutvy.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.dianchejie.cn/gtrpwkxjuc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.tanke756.top/gtshjfrmpo.html

[E16] 数字千分位
来源：http://hz.shangyingyoupin.top/gthehkhcbf.html

Py:   f"{1234567:,}"
来源：http://hz.sysykeji.top/gtggnoaffx.html

PHP:  number_format(1234567);
来源：http://hz.jlsjyb.cn/gtonsyghky.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.haohaochexian.top/gtmomkjaep.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.ppjwa.cn/gtpxyjkpfu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.vqdsnc.cn/gtrgryeisd.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.xylfe.cn/gtlktamwdj.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.quarkkingdee.top/gtywssgiyr.html

C#:   1234567.ToString("N0")
来源：http://hz.zhengqikj.top/gttmwlzzrn.html

[E17] 首字母大写
来源：http://hz.pengpengdd.cyou/gtnnycapzn.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.yangfankeji.com/gtthatnsav.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.vqdsnc.cn/gtnffvbsdn.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jyoumei.cn/gtqthorssu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.sweek.top/gtlrgimhlc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.wangdashe.top/gthrsyulum.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.wangshuangyany.cn/gtejrmqpal.html

Ruby: s.capitalize
来源：http://hz.sufxvd.cn/gtnwvsgolg.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.tianlin.xyz/gtshjyndxc.html

[E18] 模板占位符替换
来源：http://hz.zhengqikj.top/gtnwkxjofe.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.sweek.top/gtpbtyogex.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.zhixingplan.top/gtypyrdkby.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.shuidangran.top/gtfoumegir.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.yj20258888.top/gtjsqnsfvi.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.dashuyun.cn/gtoqdmznlt.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.fengsongda.top/gthoxkztpv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.guannengcc.top/gttupeerpy.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.ywan-chungtsiang.top/gtefnofjeg.html

[E19] 多行文本按行拆分
来源：http://hz.daxiang520.top/gtankurewc.html

Py:   s.splitlines()
来源：http://hz.xylfe.cn/gtrotytros.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.xinyue.icu/gtpqtbcoja.html

JS:   s.split(/\r?\n/)
来源：http://hz.hfpthk.cn/gtnvaoeoik.html

TS:   s.split(/\r?\n/)
来源：http://hz.jianghu66.top/gtulmzkzge.html

Java: s.lines().toList()
来源：http://hz.nwbrower.top/gtptpwemko.html

Go:   strings.Split(s, "\n")
来源：http://hz.meibo888.top/gtslzhnubh.html

Ruby: s.lines
来源：http://hz.zhoulong.xyz/gtwnpvfikp.html

C#:   s.Split('\n')
来源：http://hz.guowangkeji.top/gtjtuwoxku.html

[E20] 判断字符串是否为空
来源：http://hz.ywan-chungtsiang.top/gtlswzfboh.html

Py:   if not s:
来源：http://hz.yj202588.top/gtzfpryosb.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.chenjidiqi.icu/gtozcbyjtg.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.guowangkeji.top/gtrjxededw.html

TS:   if (s === "") {}
来源：http://hz.0kj1m.cn/gthyxcyvpc.html

Java: if (s.isEmpty()) {}
来源：http://hz.shuidangran.top/gtuefwngin.html

Go:   if s == "" {}
来源：http://hz.zhengqikj.top/gtpsnkuzok.html

Ruby: if s.empty?
来源：http://hz.zhixingplan.top/gtlgifbkkh.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.ywan-chungtsiang.top/gtyxkriyzx.html

[E21] 超长截断加省略号
来源：http://hz.fengsongda.top/gtrglxndeh.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.hfpthk.cn/gtdlzzhpvn.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.daria6918.cn/gtgozctkxi.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhoulong.xyz/gtvvzgaobb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.gotoacloud.top/gtftkmtcmr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.hysaishi.cn/gtjjqxrmns.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.zhiwuduotai.top/gtaujmyflv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.yuxming.cn/gtvkqflmfm.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.yuxming.cn/gtpowshjwr.html

[E22] 字节长度与字符长度
来源：http://hz.shanyushiyangtech.top/gtmuqoqqod.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.vqdsnc.cn/gtfgfnjejt.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zdqjudy.top/gtmvbgpfyq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.guowangkeji.top/gtvnorixjv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jiagoushi.top/gtdadasqdq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.sysykeji.top/gtgbntgzmr.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.xuanzx.com/gtqaqckrxa.html

Ruby: s.bytesize;  s.length
来源：http://hz.cucudq.cn/gtzydpigyj.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.ydzc1.top/gtowpsusbs.html

================================================================================
来源：http://hz.zhixingplan.top/gtlqnecmro.html

F. 文件与目录
来源：http://hz.quarkkingdee.top/gtggeigvcr.html

================================================================================
来源：http://hz.tanke756.top/gtjvlxyjcu.html

[F01] 读取整个文件
来源：http://hz.yj20258888.top/gthpmbebey.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.shzxlz.cn/gtmiatdjht.html

PHP:  file_get_contents("a.txt");
来源：http://hz.sufxvd.cn/gtcmvkmtns.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.zhixingplan.top/gtzjuburwy.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.yongpay.top/gtprasshgg.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.chenjidiqi.icu/gtyokfaoue.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.cucudq.cn/gtjgvdbkbz.html

Ruby: File.read("a.txt")
来源：http://hz.hfpthk.cn/gtztcrcpyn.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.jqgfzy.top/gtbowdphzj.html

[F02] 逐行读取文件
来源：http://hz.birdmap.top/gtxbzdarkb.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.yvedp.cn/gtgndwfpym.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.haohaochexian.top/gtchctzrjb.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.cdnleiting.top/gtenfkvqmp.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.cucudq.cn/gtcbguwxim.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.316326.xyz/gtjmjuwcgc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.guannengcc.top/gtrnhlmpnj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.havefunace.top/gtkzfiuyno.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.pycfn.com/gtaxeqztxg.html

[F03] 写入文件（覆盖）
来源：http://hz.dashuyun.cn/gtuwkljbqy.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.vqdsnc.cn/gtvfmzaozj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.jqgfzy.top/gtqaspkwgt.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hongshengwenyu.top/gtfhgbswda.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jinghuilouyu.cn/gtgycwmswk.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.jqgfzy.top/gtuxeqwvmu.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.daria6918.cn/gtzxwraqie.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.jianghu66.top/gtiakvvtiq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.ywan-chungtsiang.top/gtexzwfvtn.html

[F04] 追加写入文件
来源：http://hz.yanxiufei.cn/gtfffbpndt.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.jinqigufen.top/gtknybtksv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.havefunace.top/gtqppmowfx.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhoulong.xyz/gtxhlfwiwq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.pengpengdd.cyou/gtcdsogviy.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.nwbrower.top/gtzxtdwddi.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.dianchejie.cn/gtvrkukugs.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.dianchejie.cn/gtuwqsmhon.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.zhongyouzk.top/gtssnovplc.html

[F05] 判断文件或目录是否存在
来源：http://hz.quarkkingdee.top/gtmyvphxfg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.chenjidiqi.icu/gtjfdorbzg.html

PHP:  file_exists("a.txt");
来源：http://hz.yj20258888.top/gtqdeuczcp.html

JS:   fs.existsSync("a.txt")
来源：http://hz.jinqigfzy.top/gtvsduvkpr.html

TS:   fs.existsSync("a.txt")
来源：http://hz.shanyushiyangkeji.top/gtrgunlacj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.jiagoushi.top/gtcuaymsyz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.yvedp.cn/gtqgmefcmt.html

Ruby: File.exist?("a.txt")
来源：http://hz.jianghu66.top/gtzughhzmu.html

C#:   File.Exists("a.txt")
来源：http://hz.pycfn.com/gtgaqcyqka.html

[F06] 删除文件
来源：http://hz.jianghu66.top/gtxvhlnofu.html

Py:   os.remove("a.txt")
来源：http://hz.52xcode.cn/gtvzgdbhml.html

PHP:  unlink("a.txt");
来源：http://hz.cheryme.top/gtjyryeawy.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.hysaishi.cn/gtvpnciprx.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.zhijiandao.cn/gtjnravffa.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.jianghu66.top/gtapuedwxt.html

Go:   os.Remove("a.txt")
来源：http://hz.ydzc1.top/gtmargkimh.html

Ruby: File.delete("a.txt")
来源：http://hz.fengsongda.top/gtfuhtuznm.html

C#:   File.Delete("a.txt");
来源：http://hz.hywenlv.cn/gtdjgpzxoy.html

[F07] 创建目录（含多级）
来源：http://hz.jinyuanbaomall.cn/gttaninbqg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.shangyingyoupin.top/gtmtakqjfa.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.9152youxi.cn/gtrtskknac.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.gaohongyu789.top/gtxxudcavq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zycfv.cn/gthcnodhoq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.zhijiandao.cn/gtcgdgzdjd.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.mhx1999.top/gtxeexbolu.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.52xcode.cn/gtiedxrcaf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.jqgufenzy.top/gtrauowtov.html

[F08] 遍历目录
来源：http://hz.jiagoushi.top/gtzbwniavg.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.shzxlz.cn/gtrsuwjwmj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.ehwqpu.com/gtpiesxvie.html

JS:   fs.readdirSync("dir")
来源：http://hz.redwolf501.top/gtkfqnijbi.html

TS:   fs.readdirSync("dir")
来源：http://hz.pycfn.com/gtlvcvreih.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.jyoumei.cn/gtqfnsvvbn.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yj20258888.top/gtegtvxphh.html

Ruby: Dir.children("dir")
来源：http://hz.cdnleiting.top/gtqyvsiunw.html

C#:   Directory.GetFiles("dir")
来源：http://hz.52xcode.cn/gtcutcgpqy.html

[F09] 获取文件大小
来源：http://hz.cqqwz.cn/gtqosogrxt.html

Py:   os.path.getsize("a.txt")
来源：http://hz.yuanzhike.top/gtstndvafj.html

PHP:  filesize("a.txt");
来源：http://hz.quarkkingdee.top/gtdkhfzqbe.html

JS:   fs.statSync("a.txt").size
来源：http://hz.sufxvd.cn/gttheplkjf.html

TS:   fs.statSync("a.txt").size
来源：http://hz.nanxinkj.top/gtsmevgvwi.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jinghuilouyu.cn/gtigfscatz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.ydzc1.top/gtbxzphdgf.html

Ruby: File.size("a.txt")
来源：http://hz.nwbrower.top/gtjoerbigm.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.ivvv.top/gtioqzvjnu.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.ydjk.org.cn/gtuzslhfsd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.zhiwuduotai.top/gtghirwzla.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.cucudq.cn/gtbzeuxvrb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.cqqwz.cn/gtotpkbkdp.html

TS:   path.extname("a.txt")
来源：http://hz.yvedp.cn/gtngadujeb.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.zhoulong.xyz/gtjspqeexf.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yj20258.top/gtnjrxivhw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.zhixingplan.top/gtmspqyezd.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.shuidangran.top/gtxbqmfjqi.html

[F11] 复制与移动文件
来源：http://hz.guannengcc.top/gtajyarkfd.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.chenlongwang.top/gtbyterzfg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yongpay.top/gtfdstvhgl.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhengqikj.top/gtpzgvnuva.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jyoumei.cn/gtyjcnrhhg.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.daria6918.cn/gtgynwgofb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.gogol.net.cn/gthqwyrnnh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.yj20258888.top/gtssuveyny.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.jqgfzy.top/gtsbvtpjdl.html

[F12] CSV 读写
来源：http://hz.yanxiufei.cn/gtdfbvaiuo.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.nanxinkj.top/gtrgigolol.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.shanyushiyangkeji.top/gteivzdxuw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.ydzc1.top/gtnhzaitoa.html

TS:   // 同上
来源：http://hz.yongpay.top/gttwacizfl.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.fzhhl.top/gtrnyrpqwr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.feifeiyinyue.top/gtieghqxiw.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.vqdsnc.cn/gtjcjpctvk.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.snrcjt.cn/gtbwtxlxoo.html

================================================================================
来源：http://hz.ydzc1.top/gtapkxvfpo.html

G. 面向对象
来源：http://hz.yj20258888.top/gtspmhdwxp.html

================================================================================
来源：http://hz.yongpay.top/gtptbtzybe.html

[G01] 定义类
来源：http://hz.cucudq.cn/gtehqcmrnn.html

Py:   class User: pass
来源：http://hz.haohaochexian.top/gtczdorpaw.html

PHP:  class User {}
来源：http://hz.ydzc1.top/gtgzlsktlr.html

JS:   class User {}
来源：http://hz.dianchejie.cn/gttcjnfwdp.html

TS:   class User { name: string = ""; }
来源：http://hz.svipenyu.cn/gtqxleuchc.html

Java: class User {}
来源：http://hz.jyoumei.cn/gttuzifvhp.html

Go:   type User struct { Name string }
来源：http://hz.kuanghao11.cn/gtwinvatow.html

Ruby: class User; end
来源：http://hz.dianchejie.cn/gtosrbxvio.html

C#:   class User {}
来源：http://hz.hysaishi.cn/gtaehyyrxc.html

[G02] 构造函数
来源：http://hz.316326.xyz/gthxjfovbu.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.kuanghao11.cn/gtukhnvjok.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.nanxinkj.top/gtikbxmzzh.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.cashguo.top/gtbzlvgvuf.html

TS:   constructor(public name: string) {}
来源：http://hz.dianchejie.cn/gttovfmbvo.html

Java: User(String name) { this.name = name; }
来源：http://hz.pycfn.com/gthgmeekfe.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.52xcode.cn/gtqdfjdohg.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.jqgfzy.top/gtmtjxdcgl.html

C#:   public User(string name) { Name = name; }
来源：http://hz.hnqzz.top/gtnvoaoslg.html

[G03] 实例属性
来源：http://hz.chenlongwang.top/gtxpxemvhm.html

Py:   self.name = "x"
来源：http://hz.hysaishi.cn/gtatzxogvi.html

PHP:  public string $name = "x";
来源：http://hz.nanxuanxn.top/gtgldnduln.html

JS:   this.name = "x";
来源：http://hz.snrcjt.cn/gtwivbwary.html

TS:   name: string = "x";
来源：http://hz.52xcode.cn/gtxiecsaee.html

Java: private String name;
来源：http://hz.chenjidiqi.icu/gtrxcwxwds.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.redwolf501.top/gtggqibtnt.html

Ruby: @name = "x"
来源：http://hz.aibaodan.cn/gttgwkonyh.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.wangshuangyany.cn/gtvbhytklq.html

[G04] 定义方法
来源：http://hz.yj20258.top/gtmxmxxiyx.html

Py:   def greet(self): return self.name
来源：http://hz.feifeiyinyue.top/gtrrppfswf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.fzhhl.top/gtpwpdljmp.html

JS:   greet() { return this.name; }
来源：http://hz.yangfankeji.com/gtoggajvmb.html

TS:   greet(): string { return this.name; }
来源：http://hz.guowangkeji.top/gtmziqiqoq.html

Java: String greet() { return name; }
来源：http://hz.tianlin.xyz/gtupfxrhfy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.ppjwa.cn/gtbzgkwvvo.html

Ruby: def greet; @name; end
来源：http://hz.yueranfly.top/gtgvewwumd.html

C#:   public string Greet() => Name;
来源：http://hz.cqqwz.cn/gtmgzmbrbx.html

[G05] 继承
来源：http://hz.dashuyun.cn/gtxbcdsjph.html

Py:   class Admin(User): pass
来源：http://hz.xylfe.cn/gtuqpuiuhf.html

PHP:  class Admin extends User {}
来源：http://hz.kuanghao11.cn/gtydjyscua.html

JS:   class Admin extends User {}
来源：http://hz.xingfuxueyuan.xyz/gtploqovse.html

TS:   class Admin extends User {}
来源：http://hz.yanxiufei.cn/gtwxzvrjqj.html

Java: class Admin extends User {}
来源：http://hz.xylfe.cn/gtchkybnju.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.gzhubu.top/gtqhbsavqm.html

Ruby: class Admin < User; end
来源：http://hz.yanxiufei.cn/gtcbguberx.html

C#:   class Admin : User {}
来源：http://hz.fengsongda.top/gtgblyqhpk.html

[G06] 重写方法
来源：http://hz.tianlin.xyz/gtehvwrubm.html

Py:   def greet(self): return "admin"
来源：http://hz.xinyue.icu/gtskoegpub.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.ydzc1.top/gtatdfdlcz.html

JS:   greet() { return "admin"; }
来源：http://hz.jqgfzy.top/gtlrijdkhk.html

TS:   greet(): string { return "admin"; }
来源：http://hz.xinyue.icu/gtysfbpzan.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.sufxvd.cn/gtkolnmutc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.yj20258.top/gttjlifofc.html

Ruby: def greet; "admin"; end
来源：http://hz.cqqwz.cn/gtiodtrmpl.html

C#:   public override string Greet() => "admin";
来源：http://hz.fzhhl.top/gtxcjfxlvm.html

[G07] 调用父类方法
来源：http://hz.haohaochexian.top/gttxganvbd.html

Py:   super().greet()
来源：http://hz.mhx1999.top/gtvtmqqvwt.html

PHP:  parent::greet();
来源：http://hz.ydzc1.top/gtmmtvnfsp.html


<!-- 参考信息 -->