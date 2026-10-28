代发 wailian999

JS:   [...s].reverse().join("")
来源：http://hz.shangyingyoupin.top/gtxaqbchbm.html

TS:   [...s].reverse().join("")
来源：http://hz.ydzc1.top/gtpsncvrkn.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.52xcode.cn/gtizeonntr.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.shanyushiyangtech.top/gtvjifjjaw.html

Ruby: s.reverse
来源：http://hz.mhx1999.top/gtqtxhfrep.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.hnxiangtu.top/gtakmwwhoq.html

[E12] 统计某字符出现次数
来源：http://hz.zhijiandao.cn/gtzmrfqzur.html

Py:   s.count("a")
来源：http://hz.ehwqpu.com/gtxcndgwuz.html

PHP:  substr_count($s, "a");
来源：http://hz.52xcode.cn/gtimqkgwtc.html

JS:   s.split("a").length - 1
来源：http://hz.yongpay.top/gtrmrivwgc.html

TS:   s.split("a").length - 1
来源：http://hz.ywan-chungtsiang.top/gtfmwdjbfz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.nwbrower.top/gtucctfjtf.html

Go:   strings.Count(s, "a")
来源：http://hz.gaohongyu789.top/gtdceqqyws.html

Ruby: s.count("a")
来源：http://hz.chenlongwang.top/gtjtlxktpb.html

C#:   s.Count(c => c == 'a')
来源：http://hz.316326.xyz/gtoxvqwvwr.html

[E13] 逐字符遍历
来源：http://hz.9152youxi.cn/gtassqvplh.html

Py:   for ch in s: print(ch)
来源：http://hz.316326.xyz/gtboqwaqto.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.pycfn.com/gtzsthiogp.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.nanxinkj.top/gtnydcidvg.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.shanyushiyangkeji.top/gttwjysvaf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.yonumen.top/gtivqiayhu.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.cdnleiting.top/gtockmhaif.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.cqqwz.cn/gtjastsiqc.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.nanxinkj.top/gtlsfjyski.html

[E14] URL 编码与 Base64
来源：http://hz.jianghu66.top/gtuorascwp.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.nwbrower.top/gthctykraz.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.hnqzz.top/gtznxbjppw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.jqgufenzy.top/gtjeqqjkhk.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.aibaodan.cn/gtobubghjp.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.0kj1m.cn/gtbzbnxhgo.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.c1oappe.top/gtexeeypav.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.iojbl.cn/gtqnjzbwxx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.cqqwz.cn/gtfefjlxlj.html

[E15] HTML 转义 / 反转义
来源：http://hz.cucudq.cn/gthrvctpgw.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.zycfv.cn/gtvmkktsee.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.316326.xyz/gtqquvqxnx.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.316326.xyz/gtolodbupe.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.snrcjt.cn/gtsrovqums.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.kuanghao11.cn/gtramgppko.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.mhx1999.top/gtlclgrbzg.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.zhongyouzk.top/gtpagekzfz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.pycfn.com/gtkaajyhow.html

[E16] 数字千分位
来源：http://hz.52xcode.cn/gtwdijeqqg.html

Py:   f"{1234567:,}"
来源：http://hz.yvedp.cn/gtnkifyjmd.html

PHP:  number_format(1234567);
来源：http://hz.xziqi.cn/gtfnmfqfza.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.haohaochexian.top/gtqiqbrjok.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.daxiang520.top/gtqfvfghab.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.redwolf501.top/gtlrcomwrg.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.zycfv.cn/gtafwcygib.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.shanyushiyangtech.top/gtjgbzjpyf.html

C#:   1234567.ToString("N0")
来源：http://hz.yonumen.top/gtbnzlxroy.html

[E17] 首字母大写
来源：http://hz.cqqwz.cn/gtlnskfvvc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.birdmap.top/gtpddfgetv.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.ywan-chungtsiang.top/gtujjnmbrp.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yonumen.top/gtmsxokkrh.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jinyuanbaomall.cn/gtqmqzvvby.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.zhiwuduotai.top/gtcmmuhcbe.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.sweek.top/gtsqqzlzeq.html

Ruby: s.capitalize
来源：http://hz.zhixingplan.top/gtdmnlbxkg.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.zhijiandao.cn/gtpxgeihmj.html

[E18] 模板占位符替换
来源：http://hz.guannengcc.top/gtnpuzxptn.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.nwbrower.top/gthpncgrad.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.xinyue.icu/gttzmltzce.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.daria6918.cn/gtdhhmqnvl.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.sysykeji.top/gtswzpyevk.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.zhixingplan.top/gtinqlqnhf.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.jianghu66.top/gtdzzeixap.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.dianchejie.cn/gtgkplsvhy.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.ppjwa.cn/gtardwilfj.html

[E19] 多行文本按行拆分
来源：http://hz.zhengqikj.top/gtodluocdf.html

Py:   s.splitlines()
来源：http://hz.tian-w.cn/gtywzpersm.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.wangshuangyany.cn/gtgkjurgzo.html

JS:   s.split(/\r?\n/)
来源：http://hz.aizwys.cn/gtybbniwkv.html

TS:   s.split(/\r?\n/)
来源：http://hz.jinyuanbaomall.cn/gtmcthufzd.html

Java: s.lines().toList()
来源：http://hz.havefunace.top/gtdxkdbbnd.html

Go:   strings.Split(s, "\n")
来源：http://hz.ybcxt.top/gtmrdyimcl.html

Ruby: s.lines
来源：http://hz.fengsongda.top/gtxoaehyjy.html

C#:   s.Split('\n')
来源：http://hz.jiagoushi.top/gtucyzvnub.html

[E20] 判断字符串是否为空
来源：http://hz.mhx1999.top/gtehgqezer.html

Py:   if not s:
来源：http://hz.jyoumei.cn/gtcuimfdah.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.jianghu66.top/gtazshjedp.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.pengpengdd.cyou/gttqvaijxe.html

TS:   if (s === "") {}
来源：http://hz.jinyuanbaomall.cn/gteoisncql.html

Java: if (s.isEmpty()) {}
来源：http://hz.vqdsnc.cn/gtlgyjtyke.html

Go:   if s == "" {}
来源：http://hz.jiagoushi.top/gtwlutsjpz.html

Ruby: if s.empty?
来源：http://hz.chenlongwang.top/gtxcygbaye.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.dashuyun.cn/gtxgwjhytk.html

[E21] 超长截断加省略号
来源：http://hz.ydzc1.top/gtrntwdreh.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.nanxuanxn.top/gtnfvshcxx.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.tian-w.cn/gtbdmhlrua.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jinyuanbaomall.cn/gtooetpzem.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.wangdashe.top/gtcmmykcjj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.pycfn.com/gtfrqwkrrn.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.jlsjyb.cn/gtolnggivl.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.yonumen.top/gthecuryqa.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.nanxuanxn.top/gtyujgmgdt.html

[E22] 字节长度与字符长度
来源：http://hz.jqgufenzy.top/gtqiyhrytd.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.chenjidiqi.icu/gteqmdgrie.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ydjk.org.cn/gtgqucfsgw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ydjk.org.cn/gtwuwzopeu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.guowangkeji.top/gthuoddffx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.chenjidiqi.icu/gtwdufdwzh.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.zhijiandao.cn/gtxjegmypc.html

Ruby: s.bytesize;  s.length
来源：http://hz.zycfv.cn/gtltioaqxw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.daria6918.cn/gtjyzpptis.html

================================================================================
来源：http://hz.jyoumei.cn/gterbgpipj.html

F. 文件与目录
来源：http://hz.dianchejie.cn/gtoyeakhtl.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtotrnzlun.html

[F01] 读取整个文件
来源：http://hz.xuetiantiany.cn/gtmvkhrtes.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.zhiwuduotai.top/gtmokpgxgn.html

PHP:  file_get_contents("a.txt");
来源：http://hz.ydzc1.top/gtpltumxhd.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.mhx1999.top/gtusureiuy.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.yongpay.top/gtaqihaiuj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.haohaochexian.top/gtdbtaysbt.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.sufxvd.cn/gtqqibkpha.html

Ruby: File.read("a.txt")
来源：http://hz.cheryme.top/gtuiyjdcam.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yueranfly.top/gtsorwbnpa.html

[F02] 逐行读取文件
来源：http://hz.dashuyun.cn/gtcpjyqcvc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.hysaishi.cn/gtypjckimv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.gaohongyu789.top/gtuemosjzq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.cdnleiting.top/gtnoroljug.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hysaishi.cn/gtjriprvac.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.shanyushiyangtech.top/gtivietoap.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.daxiang520.top/gthlukjqcb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.wangshuangyany.cn/gtqzipnhni.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.sxryk.cn/gtsrdxldlu.html

[F03] 写入文件（覆盖）
来源：http://hz.havefunace.top/gttdsnceje.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.chenzaomai.com/gtspfkjhnc.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.gogol.net.cn/gtlcmjzoaa.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.316326.xyz/gtrhqnyhps.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.tanke756.top/gtemwdjedh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.jqgufenzy.top/gtmwkmfnvf.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.iojbl.cn/gttidqwtvo.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.tian-w.cn/gtkplvbike.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.cdnleiting.top/gtvkbykyxm.html

[F04] 追加写入文件
来源：http://hz.yj20258888.top/gtypvfdsft.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.zdqjudy.top/gtnblloirh.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.feifeiyinyue.top/gtwxfohgdr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.fengsongda.top/gtzlwugbst.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhoulong.xyz/gtuaubtaax.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.0kj1m.cn/gtbszhjyys.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.pycfn.com/gtqqpnmxzh.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.dashuyun.cn/gtkjruogba.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.hfpthk.cn/gtscecoqwx.html

[F05] 判断文件或目录是否存在
来源：http://hz.ydjk.org.cn/gtoyaxfesb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.jyoumei.cn/gtqehqhtxd.html

PHP:  file_exists("a.txt");
来源：http://hz.chenzaomai.com/gtwgzwlgez.html

JS:   fs.existsSync("a.txt")
来源：http://hz.hammf.cn/gtlowrjgke.html

TS:   fs.existsSync("a.txt")
来源：http://hz.sysykeji.top/gtolvvwbgw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.9152youxi.cn/gtfjnnyhex.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.zhongyouzk.top/gtdugzuisr.html

Ruby: File.exist?("a.txt")
来源：http://hz.xylfe.cn/gtkejnppiz.html

C#:   File.Exists("a.txt")
来源：http://hz.xuetiantiany.cn/gtqbnzyoxn.html

[F06] 删除文件
来源：http://hz.316326.xyz/gtkvfzsajk.html

Py:   os.remove("a.txt")
来源：http://hz.iojbl.cn/gtscpsdqkr.html

PHP:  unlink("a.txt");
来源：http://hz.yj20258.top/gthygmssjs.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.sweek.top/gtpqvqvtwy.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.xylfe.cn/gtaqasutfy.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.bjfxy.top/gtflccgnmy.html

Go:   os.Remove("a.txt")
来源：http://hz.cheryme.top/gtmfitvmms.html

Ruby: File.delete("a.txt")
来源：http://hz.zhengqikj.top/gtaswqakwd.html

C#:   File.Delete("a.txt");
来源：http://hz.xuanzx.com/gtgcgmhprx.html

[F07] 创建目录（含多级）
来源：http://hz.chenlongwang.top/gtclidrdir.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.birdmap.top/gtwasynwey.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.xinyue.icu/gtmkbcssoz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yj202588.top/gtzokavqeb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.xinyue.icu/gtkkttirmw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.jinyuanbaomall.cn/gtfgmvqnna.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.aizwys.cn/gtjqattsik.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.zhixingplan.top/gtxysnzocq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.jqgfzy.top/gtuvfwvcfg.html

[F08] 遍历目录
来源：http://hz.ppjwa.cn/gtwdicvffp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.xinyue.icu/gtcmszgyft.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.hysaishi.cn/gtzftpmlse.html

JS:   fs.readdirSync("dir")
来源：http://hz.hammf.cn/gtrffkjuww.html

TS:   fs.readdirSync("dir")
来源：http://hz.zhoulong.xyz/gtuiawixsq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.sysykeji.top/gtwznhjmdy.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.ydjk.org.cn/gtptyljadk.html

Ruby: Dir.children("dir")
来源：http://hz.jiagoushi.top/gtsmfvdrlu.html

C#:   Directory.GetFiles("dir")
来源：http://hz.jinqigfzy.top/gtsqinmcbq.html

[F09] 获取文件大小
来源：http://hz.nanxinkj.top/gtsnhizaiz.html

Py:   os.path.getsize("a.txt")
来源：http://hz.sweek.top/gtcjagtwkf.html

PHP:  filesize("a.txt");
来源：http://hz.shuidangran.top/gtctdhmifh.html

JS:   fs.statSync("a.txt").size
来源：http://hz.aizwys.cn/gtavtowmam.html

TS:   fs.statSync("a.txt").size
来源：http://hz.yueranfly.top/gtphstmzto.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.fengsongda.top/gtsszcrnfu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.feifeiyinyue.top/gtxbuttuvq.html

Ruby: File.size("a.txt")
来源：http://hz.9152youxi.cn/gtmbjsjkre.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.jinqigfzy.top/gtmupopeht.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.shangyingyoupin.top/gtkiutdoih.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.xziqi.cn/gtggnnfunj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.jinyuanbaomall.cn/gtppgtqyie.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.tanke756.top/gtxpglmure.html

TS:   path.extname("a.txt")
来源：http://hz.guowangkeji.top/gtiwhdjiph.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.smart0.xyz/gtbbpjvalt.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.feifeiyinyue.top/gtphdiygvt.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.aibaodan.cn/gtesszeyhk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.dashuyun.cn/gtnfcdadqh.html

[F11] 复制与移动文件
来源：http://hz.tianlin.xyz/gtrtpdoylz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.chenlongwang.top/gtkhgcbkvr.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.kuanghao11.cn/gtdtgbklwp.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jianghu66.top/gtnppmggim.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.tian-w.cn/gtexjdjsur.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.hywenlv.cn/gtcqztoypw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.tian-w.cn/gtodzcypqu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.pycfn.com/gtcvjtcwwm.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.dianchejie.cn/gtsoipnsqj.html

[F12] CSV 读写
来源：http://hz.dianchejie.cn/gthqbjednh.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.shanyushiyangtech.top/gtivpulvnk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.chenjidiqi.icu/gtcvetyzpk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.hnxiangtu.top/gtporoeraf.html

TS:   // 同上
来源：http://hz.svipenyu.cn/gtjugdbkkk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.fzhhl.top/gtttlzmxoh.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.tanke756.top/gtijjkhbej.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.chenjidiqi.icu/gtlweupwxl.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.xingfuxueyuan.xyz/gtakwscqsk.html

================================================================================
来源：http://hz.hnxiangtu.top/gtjqxgjoef.html

G. 面向对象
来源：http://hz.hywenlv.cn/gtqmauxvcm.html

================================================================================
来源：http://hz.dashuyun.cn/gtyxezdwxp.html

[G01] 定义类
来源：http://hz.ywan-chungtsiang.top/gtuagwfxay.html

Py:   class User: pass
来源：http://hz.jiagoushi.top/gtbbkismdy.html

PHP:  class User {}
来源：http://hz.shanyushiyangtech.top/gtwsjzhlzc.html

JS:   class User {}
来源：http://hz.yj20258.top/gtnsgqcxfo.html

TS:   class User { name: string = ""; }
来源：http://hz.birdmap.top/gtfsujvqte.html

Java: class User {}
来源：http://hz.andypj.xyz/gtzrnhaqww.html

Go:   type User struct { Name string }
来源：http://hz.shanyushiyangtech.top/gtbmxcozri.html

Ruby: class User; end
来源：http://hz.cqqwz.cn/gtxihbqpvc.html

C#:   class User {}
来源：http://hz.jlsjyb.cn/gtzpvqhhyz.html

[G02] 构造函数
来源：http://hz.gaohongyu789.top/gtcnyvqyit.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zdqjudy.top/gtjchprmpg.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.vqdsnc.cn/gtgskaxmkd.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.jlsjyb.cn/gtdwrhrtja.html

TS:   constructor(public name: string) {}
来源：http://hz.sysykeji.top/gttihojttb.html

Java: User(String name) { this.name = name; }
来源：http://hz.havefunace.top/gtubutygkc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.shanyushiyangtech.top/gtnjjtzwso.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.jinghuilouyu.cn/gttokivzub.html

C#:   public User(string name) { Name = name; }
来源：http://hz.zhaomingkeji.xyz/gtnfnwjjmu.html

[G03] 实例属性
来源：http://hz.mhx1999.top/gtpztjhbdw.html

Py:   self.name = "x"
来源：http://hz.zhaomingkeji.xyz/gtdqwopcpu.html

PHP:  public string $name = "x";
来源：http://hz.zhongyouzk.top/gtwtincnsw.html

JS:   this.name = "x";
来源：http://hz.xinyue.icu/gtfqbzwvim.html

TS:   name: string = "x";
来源：http://hz.havefunace.top/gtqilwocuf.html

Java: private String name;
来源：http://hz.cheryme.top/gtbpeduxlh.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.chenlongwang.top/gtxupofbgs.html

Ruby: @name = "x"
来源：http://hz.feifeiyinyue.top/gtsarqtojh.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yuanzhike.top/gtkxmifjcv.html

[G04] 定义方法
来源：http://hz.52xcode.cn/gtwojakpyc.html

Py:   def greet(self): return self.name
来源：http://hz.guowangkeji.top/gtixucvnxd.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.ehwqpu.com/gtgkapjiwd.html

JS:   greet() { return this.name; }
来源：http://hz.gzhubu.top/gtubsjpfdn.html

TS:   greet(): string { return this.name; }
来源：http://hz.quarkkingdee.top/gtuxdshsjl.html

Java: String greet() { return name; }
来源：http://hz.jinqigufen.top/gterwknrtf.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.ybcxt.top/gtoscznlyv.html

Ruby: def greet; @name; end
来源：http://hz.52xcode.cn/gtrvpaldvr.html

C#:   public string Greet() => Name;
来源：http://hz.svipenyu.cn/gtxtrchkrn.html

[G05] 继承
来源：http://hz.hywenlv.cn/gtvdzsloye.html

Py:   class Admin(User): pass
来源：http://hz.zhengqikj.top/gtnouvhgbl.html

PHP:  class Admin extends User {}
来源：http://hz.snrcjt.cn/gtkuvpkmom.html

JS:   class Admin extends User {}
来源：http://hz.sufxvd.cn/gtuqvilsht.html

TS:   class Admin extends User {}
来源：http://hz.cqqwz.cn/gtgknvzcce.html

Java: class Admin extends User {}
来源：http://hz.hongshengwenyu.top/gtxlbyiscc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.52xcode.cn/gtccfbnsnx.html

Ruby: class Admin < User; end
来源：http://hz.shanyushiyangkeji.top/gtvfvhctwx.html

C#:   class Admin : User {}
来源：http://hz.jinghuilouyu.cn/gttouozxuj.html

[G06] 重写方法
来源：http://hz.sufxvd.cn/gtjgvuzufa.html

Py:   def greet(self): return "admin"
来源：http://hz.fengsongda.top/gtxmgcchup.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.ivvv.top/gtjvhntmvv.html

JS:   greet() { return "admin"; }
来源：http://hz.yuanzhike.top/gtzdocawjo.html

TS:   greet(): string { return "admin"; }
来源：http://hz.gogol.net.cn/gtxxtcqigu.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.xinyue.icu/gtvqdsfbfi.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.gaohongyu789.top/gtfiebatnn.html

Ruby: def greet; "admin"; end
来源：http://hz.yj202588.top/gtsxtinmtg.html

C#:   public override string Greet() => "admin";
来源：http://hz.redwolf501.top/gtjuyvkypx.html

[G07] 调用父类方法
来源：http://hz.gotoacloud.top/gtmgxcuihe.html

Py:   super().greet()
来源：http://hz.52xcode.cn/gtlgprmmtv.html

PHP:  parent::greet();
来源：http://hz.cashguo.top/gtcysefldg.html

JS:   super.greet();
来源：http://hz.xingfuxueyuan.xyz/gtobeocegd.html

TS:   super.greet();
来源：http://hz.zycfv.cn/gtrmjnctlb.html

Java: super.greet();
来源：http://hz.hammf.cn/gthvhmaaoc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.52xcode.cn/gtjcjjsrst.html

Ruby: super
来源：http://hz.yvedp.cn/gtqsfikokk.html

C#:   base.Greet();
来源：http://hz.yongpay.top/gtrdpaucvu.html

[G08] 静态方法与属性
来源：http://hz.aizwys.cn/gtmcygpoco.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.52xcode.cn/gtkfypgumh.html

PHP:  public static function f() {}
来源：http://hz.daria6918.cn/gtgyokwuwk.html

JS:   static f() {}
来源：http://hz.yonumen.top/gtwmszdqqu.html

TS:   static f(): void {}
来源：http://hz.ywan-chungtsiang.top/gttgqsrawz.html

Java: static void f() {}
来源：http://hz.hywenlv.cn/gtkqwhlvdv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jlsjyb.cn/gtubrxasuc.html

Ruby: def self.f; end
来源：http://hz.sysykeji.top/gtfmluzwzb.html

C#:   public static void F() {}
来源：http://hz.jiagoushi.top/gtdvanjfxx.html

[G09] 接口 / 抽象类
来源：http://hz.tian-w.cn/gtcxtchahz.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.fzhhl.top/gtqzkmaizs.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.nwbrower.top/gtdrsjmofl.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.xinyue.icu/gtxulxnwmr.html

TS:   interface Shape { area(): number; }
来源：http://hz.ybcxt.top/gtjhqlhell.html

Java: interface Shape { double area(); }
来源：http://hz.xylfe.cn/gthpwwtfix.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.shanyushiyangtech.top/gteqmyiekx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jianghu66.top/gtoheywtmk.html

C#:   interface IShape { double Area(); }
来源：http://hz.ehwqpu.com/gttsnvuyei.html


<!-- 参考信息 -->