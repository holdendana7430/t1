代发 wailian999

Go:   strings.Join(items, ",")
来源：http://hz.9152youxi.cn/gtajafvwfm.html

Ruby: items.join(",")
来源：http://hz.yuxming.cn/gtimkouxya.html

C#:   string.Join(",", items)
来源：http://hz.wangshuangyany.cn/gtefiwerys.html

[E09] 去除所有空白字符
来源：http://hz.kuanghao11.cn/gttfoddhjd.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.vqdsnc.cn/gtuspumtgy.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.vqdsnc.cn/gtcjcaawdu.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.fengsongda.top/gtwltfbuph.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.zycfv.cn/gtxenrdacq.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.haohaochexian.top/gtjijprthr.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.ivvv.top/gtixreppjj.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.zycfv.cn/gtusifwzyh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.aizwys.cn/gtmoskuviy.html

[E10] 左侧补零 / 定长填充
来源：http://hz.cheryme.top/gtzrromwre.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.gogol.net.cn/gtncdwthki.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.kuanghao11.cn/gtzerjofcv.html

JS:   "7".padStart(3, "0")
来源：http://hz.jiagoushi.top/gtajhujrqk.html

TS:   "7".padStart(3, "0")
来源：http://hz.aizwys.cn/gtmlvrbsqm.html

Java: String.format("%03d", 7)
来源：http://hz.sufxvd.cn/gtizccxacm.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.yvedp.cn/gtgmcdjbis.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.zhengqikj.top/gtvfpyssaj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.0kj1m.cn/gtjbwgaowt.html

[E11] 反转字符串
来源：http://hz.dashuyun.cn/gtfzcbhhdg.html

Py:   s[::-1]
来源：http://hz.ydzc1.top/gthrbunuvi.html

PHP:  strrev($s);
来源：http://hz.cqqwz.cn/gtccrvkdvt.html

JS:   [...s].reverse().join("")
来源：http://hz.bjfxy.top/gtxqzctckm.html

TS:   [...s].reverse().join("")
来源：http://hz.yuanzhike.top/gtjuwtkdmg.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.havefunace.top/gtblvurrdd.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.meibo888.top/gtlndptkgk.html

Ruby: s.reverse
来源：http://hz.tanke756.top/gtnckytcdz.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.jianghu66.top/gtiwxcvnwv.html

[E12] 统计某字符出现次数
来源：http://hz.sysykeji.top/gtmhouxcks.html

Py:   s.count("a")
来源：http://hz.jlsjyb.cn/gtffkctkug.html

PHP:  substr_count($s, "a");
来源：http://hz.jqgfzy.top/gtzgqeaori.html

JS:   s.split("a").length - 1
来源：http://hz.zhixingplan.top/gtxdxcazuw.html

TS:   s.split("a").length - 1
来源：http://hz.9152youxi.cn/gtbndswarh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.pengpengdd.cyou/gtgsbhjiga.html

Go:   strings.Count(s, "a")
来源：http://hz.hysaishi.cn/gtgipqflzf.html

Ruby: s.count("a")
来源：http://hz.wangshuangyany.cn/gtzchfwmls.html

C#:   s.Count(c => c == 'a')
来源：http://hz.yuanzhike.top/gtryftbltj.html

[E13] 逐字符遍历
来源：http://hz.hammf.cn/gtulaychbv.html

Py:   for ch in s: print(ch)
来源：http://hz.mhx1999.top/gtzzzmvkzv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.zhaomingkeji.xyz/gtytxtctta.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xziqi.cn/gtffjveiiv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.kuanghao11.cn/gtdinhwzva.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.shanyushiyangkeji.top/gtexrqjcsi.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.bjfxy.top/gtdiuyvstq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.tianlin.xyz/gtileyqiup.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.jinghuilouyu.cn/gtzcztjvqe.html

[E14] URL 编码与 Base64
来源：http://hz.iojbl.cn/gtahtixhqv.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.ybcxt.top/gtjdhmabxa.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.andypj.xyz/gthimahnup.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.shanyushiyangtech.top/gtixjmwuxk.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.feifeiyinyue.top/gtizuycjtm.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.ydjk.org.cn/gtihwhzlwe.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.zhaomingkeji.xyz/gtdxgeulfc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.yonumen.top/gtxobqpxmh.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.zdqjudy.top/gtjxcwitmf.html

[E15] HTML 转义 / 反转义
来源：http://hz.nanxuanxn.top/gtuutgcsgh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.fengsongda.top/gtqyzkwsqy.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.vqdsnc.cn/gttpprcdoz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.jinyuanbaomall.cn/gtazyywfuw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.xuetiantiany.cn/gtgfnwgtwh.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.316326.xyz/gtyknxqtds.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.dashuyun.cn/gtnbtmfalq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.0kj1m.cn/gtcxrdqavq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.gzhubu.top/gtxqqrlhab.html

[E16] 数字千分位
来源：http://hz.yj20258888.top/gtzsrohykj.html

Py:   f"{1234567:,}"
来源：http://hz.fzhhl.top/gtpykwnqsk.html

PHP:  number_format(1234567);
来源：http://hz.birdmap.top/gttakuyzoi.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.yongpay.top/gttemusgpg.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.yj20258.top/gtjdjkbsgr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.xinyue.icu/gtpvjrxrle.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.yvedp.cn/gtrvilivas.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.ydzc1.top/gtlxyufsky.html

C#:   1234567.ToString("N0")
来源：http://hz.cheryme.top/gtrxvglyol.html

[E17] 首字母大写
来源：http://hz.ywan-chungtsiang.top/gtzoatgxjs.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.zdqjudy.top/gtdkeasmln.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.kuanghao11.cn/gtyhdfdnbe.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zdqjudy.top/gtaozofonk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.gaohongyu789.top/gtoaycxims.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.zhixingplan.top/gtuxwrvhcc.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.jinghuilouyu.cn/gtrsloqbpg.html

Ruby: s.capitalize
来源：http://hz.mhx1999.top/gtyodggsjz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yanxiufei.cn/gtxefjxerq.html

[E18] 模板占位符替换
来源：http://hz.hongshengwenyu.top/gtcxesadpq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.snrcjt.cn/gteecnedfn.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.wangshuangyany.cn/gtmkbsxlzd.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.zycfv.cn/gtxnwuegio.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.pengpengdd.cyou/gtyxpuzumj.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.zhixingplan.top/gtnpqmverv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.chenlongwang.top/gtabhauowp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.hfpthk.cn/gtsdsateka.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.iojbl.cn/gtiswmabye.html

[E19] 多行文本按行拆分
来源：http://hz.shzxlz.cn/gtuefbkirz.html

Py:   s.splitlines()
来源：http://hz.ywan-chungtsiang.top/gtekjhyajf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.yj20258.top/gttwivffdt.html

JS:   s.split(/\r?\n/)
来源：http://hz.xuetiantiany.cn/gtbrhzwkmt.html

TS:   s.split(/\r?\n/)
来源：http://hz.jqgfzy.top/gtnjnqjenr.html

Java: s.lines().toList()
来源：http://hz.cheryme.top/gtwtrcrlgs.html

Go:   strings.Split(s, "\n")
来源：http://hz.shanyushiyangtech.top/gtmkxscfrn.html

Ruby: s.lines
来源：http://hz.iojbl.cn/gtmvicsnne.html

C#:   s.Split('\n')
来源：http://hz.meibo888.top/gtpwpphdiu.html

[E20] 判断字符串是否为空
来源：http://hz.hongshengwenyu.top/gtovpqtnjy.html

Py:   if not s:
来源：http://hz.zhengqikj.top/gtninqrtmm.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.mhx1999.top/gtwmgdshwe.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.birdmap.top/gtaqtaqadq.html

TS:   if (s === "") {}
来源：http://hz.shzxlz.cn/gthjgrioai.html

Java: if (s.isEmpty()) {}
来源：http://hz.jinqigfzy.top/gtfyesjkjt.html

Go:   if s == "" {}
来源：http://hz.9152youxi.cn/gtveayqhve.html

Ruby: if s.empty?
来源：http://hz.zhijiandao.cn/gtiumkdokl.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.xingfuxueyuan.xyz/gtfrfksllp.html

[E21] 超长截断加省略号
来源：http://hz.cucudq.cn/gtibylnaep.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.quarkkingdee.top/gtwjzhszsk.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.tian-w.cn/gtfnegmymw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ybcxt.top/gtyohoideo.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.9152youxi.cn/gthpsotjui.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.jinqigfzy.top/gtcjgdzjdy.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.snrcjt.cn/gtjudgwlzk.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.gogol.net.cn/gtalflgamh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.ehwqpu.com/gtynwjupom.html

[E22] 字节长度与字符长度
来源：http://hz.9152youxi.cn/gtshuelfoo.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.daxiang520.top/gtdrhbmvpi.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.quarkkingdee.top/gtmajhjtcp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ehwqpu.com/gtrgjulpcp.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yuxming.cn/gtzronslib.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.svipenyu.cn/gtrbsrdjki.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.nanxinkj.top/gtksjydtnh.html

Ruby: s.bytesize;  s.length
来源：http://hz.jinghuilouyu.cn/gtimkuyhsq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.hnqzz.top/gtejdyddbc.html

================================================================================
来源：http://hz.ppjwa.cn/gtwmcjtujy.html

F. 文件与目录
来源：http://hz.ppjwa.cn/gtwuqodbeb.html

================================================================================
来源：http://hz.gzhubu.top/gtyxodkfsj.html

[F01] 读取整个文件
来源：http://hz.cdnleiting.top/gtyvbfmiar.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.316326.xyz/gtavqumvcb.html

PHP:  file_get_contents("a.txt");
来源：http://hz.jinyuanbaomall.cn/gttoqwcyrr.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.hongshengwenyu.top/gtznhtyujr.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.chenzaomai.com/gtfnelfnaw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.xingfuxueyuan.xyz/gtxqhbtlbd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zhengqikj.top/gtxxihrbqo.html

Ruby: File.read("a.txt")
来源：http://hz.0kj1m.cn/gtntdwugnf.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.wangdashe.top/gtiupbaquq.html

[F02] 逐行读取文件
来源：http://hz.ywan-chungtsiang.top/gtlvzsoflr.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.quarkkingdee.top/gtlasiazks.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.jinyuanbaomall.cn/gtghwvvsdx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yj20258888.top/gtxgxiozda.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.guowangkeji.top/gtetylgqdk.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.ppjwa.cn/gttivxfmbo.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.c1oappe.top/gttvwrmdzv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yuxming.cn/gtkaooqdtf.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.zhixingplan.top/gttvyfsfrb.html

[F03] 写入文件（覆盖）
来源：http://hz.zhijiandao.cn/gtsvyagfgi.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.hywenlv.cn/gtdeewdkps.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.dashuyun.cn/gtlpzmjcqv.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jinghuilouyu.cn/gtpdmyskfk.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhaomingkeji.xyz/gtmgycvxkf.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.sufxvd.cn/gtckznftet.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.meibo888.top/gtptggkesg.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.hongshengwenyu.top/gtvkhdviik.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.jqgfzy.top/gtymdkijga.html

[F04] 追加写入文件
来源：http://hz.jianghu66.top/gtipfnqmsh.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.nanxuanxn.top/gtaywksqly.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.guowangkeji.top/gthmxotijk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.shzxlz.cn/gtsfujiyup.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.nwbrower.top/gttvdwfhuc.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.shanyushiyangkeji.top/gtsbxeqxmu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.havefunace.top/gtnbzldyoy.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yonumen.top/gtfxdrxyue.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.iojbl.cn/gtjofpfjfe.html

[F05] 判断文件或目录是否存在
来源：http://hz.havefunace.top/gtvbvvrbfx.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.xinyue.icu/gtvczwvvfz.html

PHP:  file_exists("a.txt");
来源：http://hz.chenlongwang.top/gtoptjgtjl.html

JS:   fs.existsSync("a.txt")
来源：http://hz.hfpthk.cn/gtgdhosprk.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yj20258.top/gtgmgmjhau.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.316326.xyz/gtshpnyqxb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.yuxming.cn/gtqrccgjsw.html

Ruby: File.exist?("a.txt")
来源：http://hz.wangdashe.top/gtlhoczxpc.html

C#:   File.Exists("a.txt")
来源：http://hz.daxiang520.top/gtamcehbhn.html

[F06] 删除文件
来源：http://hz.andypj.xyz/gtvglghvla.html

Py:   os.remove("a.txt")
来源：http://hz.xuanzx.com/gtjxftclac.html

PHP:  unlink("a.txt");
来源：http://hz.shanyushiyangkeji.top/gtrozruvxr.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.gzhubu.top/gtrlpylwog.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.ybcxt.top/gtvdeoxywf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.yj20258.top/gtinxayptu.html

Go:   os.Remove("a.txt")
来源：http://hz.jqgfzy.top/gtmgyuoonh.html

Ruby: File.delete("a.txt")
来源：http://hz.0kj1m.cn/gtisgfabhe.html

C#:   File.Delete("a.txt");
来源：http://hz.ywan-chungtsiang.top/gthkpjrtnm.html

[F07] 创建目录（含多级）
来源：http://hz.iojbl.cn/gtgnblsdot.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.shuidangran.top/gtgdsiwqyc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.daxiang520.top/gtzfukiggw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.iojbl.cn/gtcbgxsbxz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.gotoacloud.top/gtjglhaeky.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.cdnleiting.top/gtbopalnhf.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.ybcxt.top/gtwqsnaluw.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.0kj1m.cn/gtpnentirc.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.chenzaomai.com/gtgvjusomx.html

[F08] 遍历目录
来源：http://hz.ywan-chungtsiang.top/gtsclqisdh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.gaohongyu789.top/gtlufvzlky.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.tianlin.xyz/gtcowbewom.html

JS:   fs.readdirSync("dir")
来源：http://hz.52xcode.cn/gtddyjdtqq.html

TS:   fs.readdirSync("dir")
来源：http://hz.yvedp.cn/gttjszpfck.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.9152youxi.cn/gtszofdmsk.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.jinqigfzy.top/gtapxzusli.html

Ruby: Dir.children("dir")
来源：http://hz.guowangkeji.top/gtogwldaqf.html

C#:   Directory.GetFiles("dir")
来源：http://hz.0kj1m.cn/gtqqnwrgrn.html

[F09] 获取文件大小
来源：http://hz.jianghu66.top/gtdpzgpukc.html

Py:   os.path.getsize("a.txt")
来源：http://hz.guowangkeji.top/gtvkehcpbi.html

PHP:  filesize("a.txt");
来源：http://hz.pengpengdd.cyou/gthotmbtgi.html

JS:   fs.statSync("a.txt").size
来源：http://hz.jyoumei.cn/gtuevdnahz.html

TS:   fs.statSync("a.txt").size
来源：http://hz.yj202588.top/gttgwtjclw.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.zdqjudy.top/gtvvcdxfto.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.sufxvd.cn/gtazfapllz.html

Ruby: File.size("a.txt")
来源：http://hz.xinyue.icu/gtedxewuvx.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.jiagoushi.top/gtyoctxdjn.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.cucudq.cn/gtrinllhek.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.yj202588.top/gtjgpqhhex.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.nanxuanxn.top/gtdgjgnbgz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.xinyue.icu/gtiwklrafi.html

TS:   path.extname("a.txt")
来源：http://hz.snrcjt.cn/gttgnrispa.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.mhx1999.top/gttyrnxsik.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.zhiwuduotai.top/gtdnthiwaf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.yonumen.top/gtvjzgtokb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.jinqigufen.top/gttowffnrl.html

[F11] 复制与移动文件
来源：http://hz.daria6918.cn/gtpuzjbrkh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.yonumen.top/gtqhofkulm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.guowangkeji.top/gtpsrtahhz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hongshengwenyu.top/gtwbifapsb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hammf.cn/gtrpbnilos.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.jinyuanbaomall.cn/gtuqvjvnea.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.iojbl.cn/gtjuzvktvn.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.daria6918.cn/gtldwfgtoy.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.zhiwuduotai.top/gtpztplopg.html

[F12] CSV 读写
来源：http://hz.52xcode.cn/gtnailvwrs.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.chenzaomai.com/gtykdesvni.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.yuxming.cn/gtbyukkxsi.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.fzhhl.top/gtdcviqxkf.html

TS:   // 同上
来源：http://hz.guowangkeji.top/gtokvydcvq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.yonumen.top/gtbwlwzxyw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.fengsongda.top/gtixifywcs.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jianghu66.top/gtuhvhpkpi.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.ydzc1.top/gtjgxfsdep.html

================================================================================
来源：http://hz.daxiang520.top/gtxzbcmmch.html

G. 面向对象
来源：http://hz.shangyingyoupin.top/gtmxpnqjyu.html

================================================================================
来源：http://hz.tian-w.cn/gtvehewdpb.html

[G01] 定义类
来源：http://hz.quarkkingdee.top/gtpwwwrvbs.html

Py:   class User: pass
来源：http://hz.jlsjyb.cn/gthaustyzm.html

PHP:  class User {}
来源：http://hz.zhoulong.xyz/gtcsiqflig.html

JS:   class User {}
来源：http://hz.andypj.xyz/gtfkpylbob.html

TS:   class User { name: string = ""; }
来源：http://hz.ehwqpu.com/gtgznircgs.html

Java: class User {}
来源：http://hz.jinyuanbaomall.cn/gtyswogsiz.html

Go:   type User struct { Name string }
来源：http://hz.jlsjyb.cn/gtwnxljyco.html

Ruby: class User; end
来源：http://hz.nanxuanxn.top/gtdtexqeof.html

C#:   class User {}
来源：http://hz.gzhubu.top/gtfalriwrh.html

[G02] 构造函数
来源：http://hz.shzxlz.cn/gtxybyknhs.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.jinqigufen.top/gtoxuhdebf.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.bjfxy.top/gtxeotfwoa.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.ehwqpu.com/gtnkusavdn.html

TS:   constructor(public name: string) {}
来源：http://hz.daria6918.cn/gtlpvcbnvu.html

Java: User(String name) { this.name = name; }
来源：http://hz.snrcjt.cn/gtqyuttnyg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.bjfxy.top/gtozsowunm.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.meibo888.top/gtrotonquh.html

C#:   public User(string name) { Name = name; }
来源：http://hz.jyoumei.cn/gtmaiwqnil.html

[G03] 实例属性
来源：http://hz.redwolf501.top/gtmwpwumfn.html

Py:   self.name = "x"
来源：http://hz.mhx1999.top/gtdzjrzzqi.html

PHP:  public string $name = "x";
来源：http://hz.xuanzx.com/gtmngopcqo.html

JS:   this.name = "x";
来源：http://hz.gogol.net.cn/gtyyufkfhd.html

TS:   name: string = "x";
来源：http://hz.tanke756.top/gtrlmocofh.html

Java: private String name;
来源：http://hz.ehwqpu.com/gtqsofqajf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.xziqi.cn/gtwdolsmtl.html

Ruby: @name = "x"
来源：http://hz.hywenlv.cn/gtumhjudru.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.ywan-chungtsiang.top/gtvuinxvvt.html

[G04] 定义方法
来源：http://hz.nwbrower.top/gtdxhlbqbz.html

Py:   def greet(self): return self.name
来源：http://hz.jqgfzy.top/gtwlrgsecn.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.hysaishi.cn/gtajqytxov.html

JS:   greet() { return this.name; }
来源：http://hz.ydzc1.top/gtrvxulmff.html

TS:   greet(): string { return this.name; }
来源：http://hz.gotoacloud.top/gtjrcewoju.html

Java: String greet() { return name; }
来源：http://hz.hnxiangtu.top/gtdsckfydv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.gogol.net.cn/gtvoqcihyc.html

Ruby: def greet; @name; end
来源：http://hz.jqgufenzy.top/gtttymighf.html

C#:   public string Greet() => Name;
来源：http://hz.chenzaomai.com/gtabtluluq.html

[G05] 继承
来源：http://hz.meibo888.top/gtbdknhvan.html

Py:   class Admin(User): pass
来源：http://hz.shzxlz.cn/gtyjhigtza.html

PHP:  class Admin extends User {}
来源：http://hz.hammf.cn/gtshvdyarj.html

JS:   class Admin extends User {}
来源：http://hz.hnqzz.top/gtuyblhszz.html

TS:   class Admin extends User {}
来源：http://hz.jiagoushi.top/gtcitkyszz.html

Java: class Admin extends User {}
来源：http://hz.hnqzz.top/gtjurzqwlg.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.mhx1999.top/gtiwcfekod.html

Ruby: class Admin < User; end
来源：http://hz.0kj1m.cn/gtrpkuyyqn.html

C#:   class Admin : User {}
来源：http://hz.nwbrower.top/gtveuyqjzl.html

[G06] 重写方法
来源：http://hz.gotoacloud.top/gtuneyiury.html

Py:   def greet(self): return "admin"
来源：http://hz.fengsongda.top/gtjqoiujhi.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.shanyushiyangkeji.top/gtrpcprukh.html

JS:   greet() { return "admin"; }
来源：http://hz.shangyingyoupin.top/gtsxxlufme.html

TS:   greet(): string { return "admin"; }
来源：http://hz.xinyue.icu/gtwjeqfomg.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.iojbl.cn/gtkuvlcssa.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.gzhubu.top/gtqavsntjs.html

Ruby: def greet; "admin"; end
来源：http://hz.hammf.cn/gttnvnhatx.html

C#:   public override string Greet() => "admin";
来源：http://hz.daxiang520.top/gtwerovhqt.html

[G07] 调用父类方法
来源：http://hz.hongshengwenyu.top/gtxrplilpo.html

Py:   super().greet()
来源：http://hz.9152youxi.cn/gtiypahkmb.html

PHP:  parent::greet();
来源：http://hz.tian-w.cn/gtobqwpmvk.html


<!-- 参考信息 -->