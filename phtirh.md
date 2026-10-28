代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.kuanghao11.cn/gtldvcsthj.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.cdnleiting.top/gtljbqddtj.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.guowangkeji.top/gtcnsxyhwh.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.hnqzz.top/gtncjvdgrk.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.yj20258888.top/gtvdxenuoy.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.xuetiantiany.cn/gtfmlgxvna.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.shangyingyoupin.top/gthcdrocsu.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.ivvv.top/gtcllkrhux.html

[E10] 左侧补零 / 定长填充
来源：http://hz.quarkkingdee.top/gtrotalxrr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.hnqzz.top/gtgdiwvjge.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.yanxiufei.cn/gtbvtcsklj.html

JS:   "7".padStart(3, "0")
来源：http://hz.yj20258888.top/gtdrllrwot.html

TS:   "7".padStart(3, "0")
来源：http://hz.zhongyouzk.top/gturagpvkt.html

Java: String.format("%03d", 7)
来源：http://hz.0kj1m.cn/gtonunmkxs.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.gaohongyu789.top/gtxmpwthgf.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.jlsjyb.cn/gthmsbwgvf.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.zhijiandao.cn/gthllzzkpv.html

[E11] 反转字符串
来源：http://hz.nwbrower.top/gtgvirtlvr.html

Py:   s[::-1]
来源：http://hz.gzhubu.top/gtnigmdlaz.html

PHP:  strrev($s);
来源：http://hz.ywan-chungtsiang.top/gtgcpcgggs.html

JS:   [...s].reverse().join("")
来源：http://hz.svipenyu.cn/gtcnyutnsk.html

TS:   [...s].reverse().join("")
来源：http://hz.zhiwuduotai.top/gtekvdgkuj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.meibo888.top/gttdvqynpn.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.xuanzx.com/gtopbaqdec.html

Ruby: s.reverse
来源：http://hz.316326.xyz/gtnlxybwjd.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.jyoumei.cn/gtgvbyoido.html

[E12] 统计某字符出现次数
来源：http://hz.zhengqikj.top/gtdzeltlli.html

Py:   s.count("a")
来源：http://hz.ywan-chungtsiang.top/gtbpmgsyhd.html

PHP:  substr_count($s, "a");
来源：http://hz.fengsongda.top/gtzpmnmupa.html

JS:   s.split("a").length - 1
来源：http://hz.jinghuilouyu.cn/gtruipegnk.html

TS:   s.split("a").length - 1
来源：http://hz.zycfv.cn/gtflhklgxc.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.ydjk.org.cn/gtjjsauhqq.html

Go:   strings.Count(s, "a")
来源：http://hz.xinyue.icu/gtznryzyqc.html

Ruby: s.count("a")
来源：http://hz.yueranfly.top/gtymjlorkp.html

C#:   s.Count(c => c == 'a')
来源：http://hz.zhengqikj.top/gtgvdvnzyl.html

[E13] 逐字符遍历
来源：http://hz.feifeiyinyue.top/gtgemwokco.html

Py:   for ch in s: print(ch)
来源：http://hz.svipenyu.cn/gtxcdexnkp.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.yj20258888.top/gtlduiagtu.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.smart0.xyz/gtvldvjbbz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.hammf.cn/gtffgawpis.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.jiagoushi.top/gtihlpivfu.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.cdnleiting.top/gtcdhxthwd.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.jyoumei.cn/gtfhhlthaw.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.havefunace.top/gtdeaicgfy.html

[E14] URL 编码与 Base64
来源：http://hz.kuanghao11.cn/gtfmycbilk.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.cdnleiting.top/gtrweuoxuv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.zhiwuduotai.top/gthzaffvcj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.yj20258888.top/gtpxsnuofh.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.zhiwuduotai.top/gtjqscssbs.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.birdmap.top/gtelhtrkqn.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.zhijiandao.cn/gtbqgbcgxd.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.yj20258.top/gtpfeidecn.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.fzhhl.top/gttjwmtrbg.html

[E15] HTML 转义 / 反转义
来源：http://hz.nanxinkj.top/gtffegpici.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.c1oappe.top/gtggpvnprv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.gzhubu.top/gtjesfnynn.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.xylfe.cn/gtwezvrdhp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.zhijiandao.cn/gtupdjljou.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.hywenlv.cn/gtkvlzkaog.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.cucudq.cn/gtpkxvrukw.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.smart0.xyz/gtlmpvypyn.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.hnxiangtu.top/gtumjzsxiu.html

[E16] 数字千分位
来源：http://hz.hnxiangtu.top/gtpdjsqihi.html

Py:   f"{1234567:,}"
来源：http://hz.hongshengwenyu.top/gthyujdawg.html

PHP:  number_format(1234567);
来源：http://hz.chenzaomai.com/gtrjtkaxgv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.gotoacloud.top/gtashacpmh.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.guowangkeji.top/gtzckuyoth.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.ivvv.top/gteawlhkhr.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.zhiwuduotai.top/gtrngvhkug.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.dianchejie.cn/gtqjlvexsi.html

C#:   1234567.ToString("N0")
来源：http://hz.dashuyun.cn/gtilgwhiaa.html

[E17] 首字母大写
来源：http://hz.zhoulong.xyz/gtyvlohzak.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.guannengcc.top/gtkywuqndn.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.hammf.cn/gttozdfeef.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.nwbrower.top/gtaxaqevbk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.daria6918.cn/gtlphgrpsw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.zdqjudy.top/gtcppzfoai.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.cashguo.top/gtwbagltsa.html

Ruby: s.capitalize
来源：http://hz.chenlongwang.top/gtepaxjhgv.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.birdmap.top/gtownkhgeu.html

[E18] 模板占位符替换
来源：http://hz.smart0.xyz/gtftdjfjeg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.iojbl.cn/gtgrmyxywk.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.sysykeji.top/gtgxsssgag.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.jyoumei.cn/gtmuxnolnv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.yangfankeji.com/gtygwozslj.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.haohaochexian.top/gtvihyaofl.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.zhengqikj.top/gtpwcsviol.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.nanxinkj.top/gtvmxpmvep.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.ydzc1.top/gtwlhatghy.html

[E19] 多行文本按行拆分
来源：http://hz.havefunace.top/gtzkzjztjz.html

Py:   s.splitlines()
来源：http://hz.gogol.net.cn/gtxhmynmtf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.ppjwa.cn/gtfwtemrog.html

JS:   s.split(/\r?\n/)
来源：http://hz.birdmap.top/gtnhoczcue.html

TS:   s.split(/\r?\n/)
来源：http://hz.yueranfly.top/gtjcyfjbtw.html

Java: s.lines().toList()
来源：http://hz.pengpengdd.cyou/gtctahpnwt.html

Go:   strings.Split(s, "\n")
来源：http://hz.jlsjyb.cn/gtwyivrjcg.html

Ruby: s.lines
来源：http://hz.guowangkeji.top/gtvjbwvnpx.html

C#:   s.Split('\n')
来源：http://hz.quarkkingdee.top/gthpgjcgxa.html

[E20] 判断字符串是否为空
来源：http://hz.shzxlz.cn/gtnujjaqko.html

Py:   if not s:
来源：http://hz.ehwqpu.com/gtogeajkcy.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.jiagoushi.top/gtsevhtidn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.meibo888.top/gtedrqqngq.html

TS:   if (s === "") {}
来源：http://hz.jlsjyb.cn/gthtlghewu.html

Java: if (s.isEmpty()) {}
来源：http://hz.ppjwa.cn/gtyztrcrqa.html

Go:   if s == "" {}
来源：http://hz.svipenyu.cn/gtfkavqhtg.html

Ruby: if s.empty?
来源：http://hz.ydjk.org.cn/gthkdlvgpo.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.jiagoushi.top/gtxwggkeoq.html

[E21] 超长截断加省略号
来源：http://hz.yangfankeji.com/gtmshhradh.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.aibaodan.cn/gtynpymazo.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.ehwqpu.com/gtkuiysvre.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.smart0.xyz/gtftpwwkyw.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhengqikj.top/gtdoxwuupz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.jqgfzy.top/gtfbgdiglv.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.guowangkeji.top/gtyropqjdp.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.cucudq.cn/gtqwhczryg.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.aizwys.cn/gtnhaybzli.html

[E22] 字节长度与字符长度
来源：http://hz.cashguo.top/gtjsmmbcne.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.hnqzz.top/gttrfdcbot.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ivvv.top/gtgcnwuaoh.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhengqikj.top/gtdbqnuzli.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.tianlin.xyz/gtoqczevfb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.xuetiantiany.cn/gtmnrwuuck.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.sysykeji.top/gtbouxhdok.html

Ruby: s.bytesize;  s.length
来源：http://hz.havefunace.top/gtmhyyjnte.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.yuanzhike.top/gtsngmfyau.html

================================================================================
来源：http://hz.yongpay.top/gtxsfcjjmh.html

F. 文件与目录
来源：http://hz.hysaishi.cn/gtkuftcepr.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtcdiwyqdi.html

[F01] 读取整个文件
来源：http://hz.tian-w.cn/gtrtkihsox.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yuxming.cn/gtuauigixg.html

PHP:  file_get_contents("a.txt");
来源：http://hz.dianchejie.cn/gtectllajg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.svipenyu.cn/gtazkgsfev.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.yangfankeji.com/gtgzqjhohu.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.birdmap.top/gttnkgfywv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.daxiang520.top/gtcryfwmiu.html

Ruby: File.read("a.txt")
来源：http://hz.hfpthk.cn/gtaipgvkph.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yj20258888.top/gtepukvfwf.html

[F02] 逐行读取文件
来源：http://hz.quarkkingdee.top/gtxcbsemdq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.jqgfzy.top/gtrzvahhwl.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.jinqigufen.top/gtvaijyitj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xinyue.icu/gtdrtcribh.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.gotoacloud.top/gthxxtauqs.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.yj20258888.top/gtdixoscsm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.sufxvd.cn/gtzfmsbmoe.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.smart0.xyz/gtyygaadmr.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.zhixingplan.top/gtdeikgznw.html

[F03] 写入文件（覆盖）
来源：http://hz.hnxiangtu.top/gtdcvnwjyv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.shanyushiyangtech.top/gtycmjhmox.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.316326.xyz/gtsoskhstb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jinqigfzy.top/gtfhflwycf.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jiagoushi.top/gtkhsvvmgz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.jianghu66.top/gtnvdcqenj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.cdnleiting.top/gtkexcgnhu.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.0kj1m.cn/gtllwxciip.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.0kj1m.cn/gtolqswimf.html

[F04] 追加写入文件
来源：http://hz.ehwqpu.com/gtwctpamuz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yj20258.top/gtbgphbzea.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.yj20258888.top/gtsbexhsxd.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.gotoacloud.top/gtgeufklml.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.tian-w.cn/gtbvdpkgoz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.hywenlv.cn/gtwahptprq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.sxryk.cn/gtdcsgyamm.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.jqgufenzy.top/gtmaabfwow.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.zhoulong.xyz/gtziwefuhf.html

[F05] 判断文件或目录是否存在
来源：http://hz.xingfuxueyuan.xyz/gtorgsyjxl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.gzhubu.top/gtcncxtzzv.html

PHP:  file_exists("a.txt");
来源：http://hz.sufxvd.cn/gtbyjonltt.html

JS:   fs.existsSync("a.txt")
来源：http://hz.hnxiangtu.top/gtrnxiupfi.html

TS:   fs.existsSync("a.txt")
来源：http://hz.jinghuilouyu.cn/gtdjshtike.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.ybcxt.top/gtiptbuhyp.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.dianchejie.cn/gtfcfzypwg.html

Ruby: File.exist?("a.txt")
来源：http://hz.aibaodan.cn/gtgtduzdot.html

C#:   File.Exists("a.txt")
来源：http://hz.ppjwa.cn/gtxlcwwcga.html

[F06] 删除文件
来源：http://hz.sufxvd.cn/gtvwjxyopg.html

Py:   os.remove("a.txt")
来源：http://hz.0kj1m.cn/gtwgrlmexy.html

PHP:  unlink("a.txt");
来源：http://hz.jianghu66.top/gtzsnezdbp.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.haohaochexian.top/gtrhwokkmc.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.nwbrower.top/gteupvpaua.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.pycfn.com/gtgjinhaad.html

Go:   os.Remove("a.txt")
来源：http://hz.birdmap.top/gtypdqferz.html

Ruby: File.delete("a.txt")
来源：http://hz.cucudq.cn/gtcobrimdw.html

C#:   File.Delete("a.txt");
来源：http://hz.pycfn.com/gtdamhgrnz.html

[F07] 创建目录（含多级）
来源：http://hz.shanyushiyangkeji.top/gtftwpagxk.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.cashguo.top/gtzkyjrvmq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.jyoumei.cn/gthodhxhrs.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jyoumei.cn/gtsnkfflyi.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhengqikj.top/gtnyfmgzut.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.wangdashe.top/gtrtyqbmzj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.c1oappe.top/gtjmhrqols.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.wangshuangyany.cn/gtmluuaacc.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.jiagoushi.top/gthgaoqewr.html

[F08] 遍历目录
来源：http://hz.hywenlv.cn/gtqvaahfhq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.sxryk.cn/gtvgefpgjx.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.xziqi.cn/gtwwjyigab.html

JS:   fs.readdirSync("dir")
来源：http://hz.gzhubu.top/gtskonupyy.html

TS:   fs.readdirSync("dir")
来源：http://hz.yueranfly.top/gtlnxoooke.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.ywan-chungtsiang.top/gtqzkyzpma.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.cucudq.cn/gtxvinprmn.html

Ruby: Dir.children("dir")
来源：http://hz.fzhhl.top/gteshihzfj.html

C#:   Directory.GetFiles("dir")
来源：http://hz.pengpengdd.cyou/gtqcxjwxxa.html

[F09] 获取文件大小
来源：http://hz.yangfankeji.com/gtqciuirer.html

Py:   os.path.getsize("a.txt")
来源：http://hz.jinqigfzy.top/gtupqptjcf.html

PHP:  filesize("a.txt");
来源：http://hz.cucudq.cn/gtuoayxzjy.html

JS:   fs.statSync("a.txt").size
来源：http://hz.guannengcc.top/gtyrfktelp.html

TS:   fs.statSync("a.txt").size
来源：http://hz.shanyushiyangtech.top/gtikuyilmv.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.hywenlv.cn/gtjqmeyldy.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.feifeiyinyue.top/gtrvvkfada.html

Ruby: File.size("a.txt")
来源：http://hz.guowangkeji.top/gttmgaxace.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.daria6918.cn/gtydigssid.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.jinqigufen.top/gtmgxhmcjp.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.shanyushiyangtech.top/gtgkmsxwzn.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.zhongyouzk.top/gtnyfxmkox.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.xuanzx.com/gtmclwrcgu.html

TS:   path.extname("a.txt")
来源：http://hz.nanxinkj.top/gtyaswklaz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.ywan-chungtsiang.top/gtcttsrsbd.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.jlsjyb.cn/gtzfgwhsbr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.9152youxi.cn/gtbpzejoti.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.fzhhl.top/gtslhybifw.html

[F11] 复制与移动文件
来源：http://hz.birdmap.top/gtsomybdep.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.chenlongwang.top/gtfttobveo.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.hnqzz.top/gtiplbjsvn.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yongpay.top/gtcgqjqqdd.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jiagoushi.top/gtqngfztem.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.hysaishi.cn/gtujgbkshr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.zhixingplan.top/gtzltgtgbw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.svipenyu.cn/gtuozqrlrq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.jinqigufen.top/gtkauwqumm.html

[F12] CSV 读写
来源：http://hz.sufxvd.cn/gteemfdhkd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.pengpengdd.cyou/gtovddpkfc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.jlsjyb.cn/gthtukfgut.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.chenlongwang.top/gtrkhmnhbu.html

TS:   // 同上
来源：http://hz.mhx1999.top/gtcsobwbol.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.jqgufenzy.top/gtxlyuuoht.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.jyoumei.cn/gteposvkqy.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.hammf.cn/gtroxbirzs.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.cqqwz.cn/gtpmiqzurf.html

================================================================================
来源：http://hz.svipenyu.cn/gtbfeitvtj.html

G. 面向对象
来源：http://hz.gaohongyu789.top/gthuvogaxo.html

================================================================================
来源：http://hz.hfpthk.cn/gtnvnnfyzl.html

[G01] 定义类
来源：http://hz.sweek.top/gtoowzdplr.html

Py:   class User: pass
来源：http://hz.nanxinkj.top/gtkaibkyjf.html

PHP:  class User {}
来源：http://hz.birdmap.top/gtziabaygf.html

JS:   class User {}
来源：http://hz.ydzc1.top/gtigmgqhlt.html

TS:   class User { name: string = ""; }
来源：http://hz.zhijiandao.cn/gtdcahvfzz.html

Java: class User {}
来源：http://hz.tanke756.top/gtopugyeey.html

Go:   type User struct { Name string }
来源：http://hz.wangshuangyany.cn/gtaczcfypn.html

Ruby: class User; end
来源：http://hz.gaohongyu789.top/gtdyhrmfne.html

C#:   class User {}
来源：http://hz.jqgfzy.top/gtclzoysmc.html

[G02] 构造函数
来源：http://hz.316326.xyz/gtztgansqg.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.nanxuanxn.top/gtwrdozgqr.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.jqgfzy.top/gthtdvjblc.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.0kj1m.cn/gtmhwkdtnz.html

TS:   constructor(public name: string) {}
来源：http://hz.wangdashe.top/gtcgzbaoty.html

Java: User(String name) { this.name = name; }
来源：http://hz.vqdsnc.cn/gthjvdsshn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.ydzc1.top/gtuulzuixu.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.zycfv.cn/gtwbqdrzij.html

C#:   public User(string name) { Name = name; }
来源：http://hz.zhongyouzk.top/gtpaqtjvqf.html

[G03] 实例属性
来源：http://hz.0kj1m.cn/gtmmdtuhvg.html

Py:   self.name = "x"
来源：http://hz.kuanghao11.cn/gtzltvnsep.html

PHP:  public string $name = "x";
来源：http://hz.ivvv.top/gtjdpuletn.html

JS:   this.name = "x";
来源：http://hz.hnxiangtu.top/gtegvmbimv.html

TS:   name: string = "x";
来源：http://hz.wangshuangyany.cn/gttjqdnujq.html

Java: private String name;
来源：http://hz.nwbrower.top/gtnpffhpkt.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.zhixingplan.top/gtwtejcsvj.html

Ruby: @name = "x"
来源：http://hz.yangfankeji.com/gtysanmqbq.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.xziqi.cn/gttpxssbyy.html

[G04] 定义方法
来源：http://hz.smart0.xyz/gtastabsqb.html

Py:   def greet(self): return self.name
来源：http://hz.jlsjyb.cn/gtllzazpev.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.chenjidiqi.icu/gtowbthvqf.html

JS:   greet() { return this.name; }
来源：http://hz.wangshuangyany.cn/gtzrpggrgs.html

TS:   greet(): string { return this.name; }
来源：http://hz.sxryk.cn/gtcfxnbprx.html

Java: String greet() { return name; }
来源：http://hz.daria6918.cn/gtczpjsooo.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.hongshengwenyu.top/gtknaghfbm.html

Ruby: def greet; @name; end
来源：http://hz.gaohongyu789.top/gtfajymbom.html

C#:   public string Greet() => Name;
来源：http://hz.hysaishi.cn/gtaqmhcxsc.html

[G05] 继承
来源：http://hz.yuxming.cn/gttlmyhsnu.html

Py:   class Admin(User): pass
来源：http://hz.tianlin.xyz/gtgcjukcnc.html

PHP:  class Admin extends User {}
来源：http://hz.sysykeji.top/gtfitdvqfp.html

JS:   class Admin extends User {}
来源：http://hz.shzxlz.cn/gtnczmjypr.html

TS:   class Admin extends User {}
来源：http://hz.andypj.xyz/gtharmmbns.html

Java: class Admin extends User {}
来源：http://hz.fengsongda.top/gthgyyzcvw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.iojbl.cn/gtqtehgykq.html

Ruby: class Admin < User; end
来源：http://hz.chenlongwang.top/gtfmkocdkp.html

C#:   class Admin : User {}
来源：http://hz.zhiwuduotai.top/gtrezpnzaw.html

[G06] 重写方法
来源：http://hz.aizwys.cn/gtkgawqvzm.html

Py:   def greet(self): return "admin"
来源：http://hz.sweek.top/gtyvzsovjd.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.chenlongwang.top/gtyqlsvtdt.html

JS:   greet() { return "admin"; }
来源：http://hz.c1oappe.top/gtsdhpigpf.html

TS:   greet(): string { return "admin"; }
来源：http://hz.dashuyun.cn/gtyjzubzhp.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.guowangkeji.top/gtlnsipufr.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.aibaodan.cn/gtyhjhukwj.html

Ruby: def greet; "admin"; end
来源：http://hz.zycfv.cn/gtkttkggbr.html

C#:   public override string Greet() => "admin";
来源：http://hz.feifeiyinyue.top/gtmnqtnlyg.html

[G07] 调用父类方法
来源：http://hz.ywan-chungtsiang.top/gtqcsvprnw.html

Py:   super().greet()
来源：http://hz.ydzc1.top/gtainyfzbm.html

PHP:  parent::greet();
来源：http://hz.zhoulong.xyz/gtvhwbjrku.html

JS:   super.greet();
来源：http://hz.nanxinkj.top/gtlxhcxovy.html

TS:   super.greet();
来源：http://hz.xuetiantiany.cn/gtddzoemyg.html

Java: super.greet();
来源：http://hz.xylfe.cn/gtdlcebdxs.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.wangshuangyany.cn/gtkqrtoxwc.html


<!-- 参考信息 -->