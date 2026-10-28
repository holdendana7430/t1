代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.shangyingyoupin.top/gtwevowbdl.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.ivvv.top/gtvbueaeey.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.ivvv.top/gtmhhkkzvh.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.wangshuangyany.cn/gtakkaewnb.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.cucudq.cn/gtjcppeaba.html

[E15] HTML 转义 / 反转义
来源：http://hz.xziqi.cn/gtvhjjbcpn.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.ppjwa.cn/gtnygccvyt.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.guannengcc.top/gttdmhekkm.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.quarkkingdee.top/gtaxkfssjy.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.jinyuanbaomall.cn/gtzivuweou.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.shuidangran.top/gthwqbqsyi.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.yonumen.top/gtzlrnfzms.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.0kj1m.cn/gtckbnpake.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.nwbrower.top/gttlmxtron.html

[E16] 数字千分位
来源：http://hz.wangdashe.top/gtefrraujw.html

Py:   f"{1234567:,}"
来源：http://hz.svipenyu.cn/gtaxiwqiyz.html

PHP:  number_format(1234567);
来源：http://hz.ppjwa.cn/gtrxqxbldl.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.aibaodan.cn/gtpcoqbeag.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.hywenlv.cn/gtvpeuyhuv.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.hongshengwenyu.top/gttvzlamyh.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.yangfankeji.com/gtwvmuatbx.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.pycfn.com/gtzvlpzzjg.html

C#:   1234567.ToString("N0")
来源：http://hz.vqdsnc.cn/gtoxpqjqvj.html

[E17] 首字母大写
来源：http://hz.shzxlz.cn/gtvuxxdjwd.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.svipenyu.cn/gtkqllwcmf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.andypj.xyz/gtxmmipvpj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jianghu66.top/gtvnffuaph.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.wangshuangyany.cn/gtjyfpfczi.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.316326.xyz/gtuntwbjnt.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.ehwqpu.com/gtatvuckhj.html

Ruby: s.capitalize
来源：http://hz.fengsongda.top/gthbpwagnp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.gotoacloud.top/gtvialiuaj.html

[E18] 模板占位符替换
来源：http://hz.sxryk.cn/gtqgowxmba.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.zdqjudy.top/gtfpzywjst.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.zdqjudy.top/gtalmbgmrd.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.zhaomingkeji.xyz/gthgikgoxc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.daxiang520.top/gtywqtvtmq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.wangdashe.top/gtivwlwhzc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.zhengqikj.top/gthoyakojk.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.vqdsnc.cn/gtktbixqpm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.feifeiyinyue.top/gtvgprkbfe.html

[E19] 多行文本按行拆分
来源：http://hz.xingfuxueyuan.xyz/gtfyeryrrz.html

Py:   s.splitlines()
来源：http://hz.yuanzhike.top/gtrakvievv.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.tian-w.cn/gtjvrjwrbf.html

JS:   s.split(/\r?\n/)
来源：http://hz.jinqigufen.top/gtvtpeyiye.html

TS:   s.split(/\r?\n/)
来源：http://hz.guannengcc.top/gttxhufebx.html

Java: s.lines().toList()
来源：http://hz.svipenyu.cn/gtixvalnhn.html

Go:   strings.Split(s, "\n")
来源：http://hz.xuetiantiany.cn/gtzeqepcia.html

Ruby: s.lines
来源：http://hz.jyoumei.cn/gtplpxqzxc.html

C#:   s.Split('\n')
来源：http://hz.ydjk.org.cn/gtmjgnptxd.html

[E20] 判断字符串是否为空
来源：http://hz.ywan-chungtsiang.top/gtdxugujur.html

Py:   if not s:
来源：http://hz.316326.xyz/gtcqwmxsrs.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.shzxlz.cn/gtjqcyjitn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.meibo888.top/gtdlxvunlm.html

TS:   if (s === "") {}
来源：http://hz.shanyushiyangkeji.top/gtpnhffube.html

Java: if (s.isEmpty()) {}
来源：http://hz.xylfe.cn/gttygugaxn.html

Go:   if s == "" {}
来源：http://hz.nanxuanxn.top/gtdpepzynj.html

Ruby: if s.empty?
来源：http://hz.gzhubu.top/gtiuiyohgr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.ehwqpu.com/gtjzpqtota.html

[E21] 超长截断加省略号
来源：http://hz.aizwys.cn/gthuphvrrh.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.quarkkingdee.top/gtilsgwkqh.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.zhoulong.xyz/gtlcygpsik.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yj20258888.top/gtqijcscde.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.shangyingyoupin.top/gtjayfwodz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.jiagoushi.top/gtllltdabv.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.pengpengdd.cyou/gtmzfkapqa.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.shanyushiyangkeji.top/gtryrhovno.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.sxryk.cn/gtsgfdsiqd.html

[E22] 字节长度与字符长度
来源：http://hz.hywenlv.cn/gthpypvvvt.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.jinghuilouyu.cn/gtawowanvo.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yonumen.top/gtqnocmyks.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.xingfuxueyuan.xyz/gtmpuwrtgk.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.0kj1m.cn/gtbqkpfxpy.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.316326.xyz/gtyxumycog.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.gotoacloud.top/gttqhivmim.html

Ruby: s.bytesize;  s.length
来源：http://hz.xuanzx.com/gtryvvcpgr.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.yuanzhike.top/gtfxjrtonj.html

================================================================================
来源：http://hz.sysykeji.top/gtmlwtokhg.html

F. 文件与目录
来源：http://hz.yonumen.top/gtgdffvlqg.html

================================================================================
来源：http://hz.jinqigufen.top/gtilcmdqxf.html

[F01] 读取整个文件
来源：http://hz.jinqigfzy.top/gtjlxuqugm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.fengsongda.top/gtnimfedyr.html

PHP:  file_get_contents("a.txt");
来源：http://hz.sweek.top/gtnxctoreg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.bjfxy.top/gtydlmanjs.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.tianlin.xyz/gtuyoniejg.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.hammf.cn/gtnffketka.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.9152youxi.cn/gtfvejbgos.html

Ruby: File.read("a.txt")
来源：http://hz.hammf.cn/gtrtwecwik.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.sweek.top/gtyqraikms.html

[F02] 逐行读取文件
来源：http://hz.hnqzz.top/gtgdfmeejc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.smart0.xyz/gtmleokhju.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.wangdashe.top/gtbhtxyybk.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.tanke756.top/gtlmawurcq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.redwolf501.top/gtbsvqljou.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.andypj.xyz/gtufxabven.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.cashguo.top/gtmmsycqjn.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.andypj.xyz/gthkradanr.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.yvedp.cn/gtoenxdxlc.html

[F03] 写入文件（覆盖）
来源：http://hz.gotoacloud.top/gtramhglhc.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.dianchejie.cn/gtkijrnzaf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.zhixingplan.top/gtxtlwuxbb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yuxming.cn/gtbxazhkzt.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hnxiangtu.top/gtwtngxpde.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.zhixingplan.top/gtgbtxjozk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.tanke756.top/gtkvmryvpp.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.feifeiyinyue.top/gttkjfrfak.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.sweek.top/gtpqzlbybf.html

[F04] 追加写入文件
来源：http://hz.ivvv.top/gtnfbzawrn.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.dianchejie.cn/gtmrmwjylm.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.ydjk.org.cn/gtzwakcexz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhijiandao.cn/gtdcfaofao.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ppjwa.cn/gtmmuifppp.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.ivvv.top/gtfbfkwkyu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.yangfankeji.com/gtywhapwai.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.ehwqpu.com/gtpwqcityx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.daria6918.cn/gtcfloroee.html

[F05] 判断文件或目录是否存在
来源：http://hz.zhengqikj.top/gthfqctmsu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.daria6918.cn/gtukfpsdmq.html

PHP:  file_exists("a.txt");
来源：http://hz.hammf.cn/gttcaqhrvp.html

JS:   fs.existsSync("a.txt")
来源：http://hz.316326.xyz/gtexeyoxgy.html

TS:   fs.existsSync("a.txt")
来源：http://hz.ydjk.org.cn/gtebuavqtm.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.shangyingyoupin.top/gtmxwbmgba.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.pengpengdd.cyou/gtczpvxlcd.html

Ruby: File.exist?("a.txt")
来源：http://hz.svipenyu.cn/gtxdvkjawy.html

C#:   File.Exists("a.txt")
来源：http://hz.jiagoushi.top/gtsbzluels.html

[F06] 删除文件
来源：http://hz.52xcode.cn/gthmhtjnhy.html

Py:   os.remove("a.txt")
来源：http://hz.52xcode.cn/gtyxgsekwl.html

PHP:  unlink("a.txt");
来源：http://hz.cdnleiting.top/gtsozrlkhl.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.dianchejie.cn/gtknoydpix.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.zdqjudy.top/gtoklgpdym.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.iojbl.cn/gthyigrzsr.html

Go:   os.Remove("a.txt")
来源：http://hz.cucudq.cn/gtnhscseci.html

Ruby: File.delete("a.txt")
来源：http://hz.hnqzz.top/gtrpcxlpmw.html

C#:   File.Delete("a.txt");
来源：http://hz.bjfxy.top/gtnswpmunp.html

[F07] 创建目录（含多级）
来源：http://hz.jianghu66.top/gtahigcxwx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.ybcxt.top/gtbbjrxfpx.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.xuetiantiany.cn/gtnzriykag.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ydzc1.top/gtoqeambxz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.mhx1999.top/gtmylhkqma.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.wangdashe.top/gtciemhqwk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.gaohongyu789.top/gtbnoerzvj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.jinqigfzy.top/gtjgcvberl.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.ydjk.org.cn/gttsdzasrt.html

[F08] 遍历目录
来源：http://hz.yanxiufei.cn/gtxlbzkesq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.316326.xyz/gtnihcldew.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.tian-w.cn/gtngzulnhd.html

JS:   fs.readdirSync("dir")
来源：http://hz.chenlongwang.top/gtylmjumcd.html

TS:   fs.readdirSync("dir")
来源：http://hz.52xcode.cn/gtcjvmovjs.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.yueranfly.top/gtxyqvawtu.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yanxiufei.cn/gtngtemayh.html

Ruby: Dir.children("dir")
来源：http://hz.feifeiyinyue.top/gttgpyhtgk.html

C#:   Directory.GetFiles("dir")
来源：http://hz.birdmap.top/gtaprnkvob.html

[F09] 获取文件大小
来源：http://hz.cdnleiting.top/gtmooqlgyo.html

Py:   os.path.getsize("a.txt")
来源：http://hz.shanyushiyangtech.top/gtjlhzxuca.html

PHP:  filesize("a.txt");
来源：http://hz.gogol.net.cn/gtxfrqeksm.html

JS:   fs.statSync("a.txt").size
来源：http://hz.zhijiandao.cn/gtxzqjvjgq.html

TS:   fs.statSync("a.txt").size
来源：http://hz.bjfxy.top/gtkmpcqqpo.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.meibo888.top/gtzhfhtosn.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.ywan-chungtsiang.top/gtudbygekv.html

Ruby: File.size("a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtliudxbbt.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yonumen.top/gtmlllidka.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.316326.xyz/gtncskqkhu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.dashuyun.cn/gttqjsggln.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.sxryk.cn/gtkylttxne.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.gaohongyu789.top/gtwcyughtw.html

TS:   path.extname("a.txt")
来源：http://hz.wangshuangyany.cn/gtwzujulkc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.guowangkeji.top/gtrcsjrreq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.jinqigufen.top/gtkhwvkfnp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.zhijiandao.cn/gtqbeqrtny.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.nanxuanxn.top/gtvlwtpokn.html

[F11] 复制与移动文件
来源：http://hz.yangfankeji.com/gtckjeupxl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.wangshuangyany.cn/gtnkvcgkcy.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.jlsjyb.cn/gtgfaqcsqk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.redwolf501.top/gttcddhclg.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yonumen.top/gtzqfptarp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.jlsjyb.cn/gtxfzujslo.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.sweek.top/gtxkwueytt.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.mhx1999.top/gtxwgutwfe.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.jinqigfzy.top/gtqealkndj.html

[F12] CSV 读写
来源：http://hz.nanxinkj.top/gtnpzpzhje.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.fengsongda.top/gtttkihyrr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.jyoumei.cn/gtfaadopch.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.iojbl.cn/gtmsvcnvut.html

TS:   // 同上
来源：http://hz.cdnleiting.top/gtjigrgcsi.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.nwbrower.top/gtivntvuwf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.guannengcc.top/gtiuvzmgmh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.ehwqpu.com/gtwxvtbsqs.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yueranfly.top/gtopuhehkt.html

================================================================================
来源：http://hz.haohaochexian.top/gtadmmylrm.html

G. 面向对象
来源：http://hz.feifeiyinyue.top/gtlknycajc.html

================================================================================
来源：http://hz.yuanzhike.top/gtbzyydpws.html

[G01] 定义类
来源：http://hz.meibo888.top/gtkadfpepy.html

Py:   class User: pass
来源：http://hz.dianchejie.cn/gtuaopdrer.html

PHP:  class User {}
来源：http://hz.sweek.top/gtwxlzxngc.html

JS:   class User {}
来源：http://hz.xylfe.cn/gtnfqiovzz.html

TS:   class User { name: string = ""; }
来源：http://hz.birdmap.top/gthmfqyupp.html

Java: class User {}
来源：http://hz.shanyushiyangkeji.top/gtbolpnmry.html

Go:   type User struct { Name string }
来源：http://hz.jyoumei.cn/gttqbzthll.html

Ruby: class User; end
来源：http://hz.wangshuangyany.cn/gtkkuuemkz.html

C#:   class User {}
来源：http://hz.hnqzz.top/gtpxtxwfma.html

[G02] 构造函数
来源：http://hz.shuidangran.top/gtsdsemdib.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yj20258.top/gtelnjtagt.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.hnxiangtu.top/gtzmgsfkkr.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.meibo888.top/gtzjbsvlvr.html

TS:   constructor(public name: string) {}
来源：http://hz.birdmap.top/gtuqcvsgfr.html

Java: User(String name) { this.name = name; }
来源：http://hz.316326.xyz/gtlkpoqnfl.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yuanzhike.top/gtcinhnhlt.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.jinqigufen.top/gtdgayfwqk.html

C#:   public User(string name) { Name = name; }
来源：http://hz.tanke756.top/gtzjlzaxpo.html

[G03] 实例属性
来源：http://hz.tian-w.cn/gthbgkydxh.html

Py:   self.name = "x"
来源：http://hz.cheryme.top/gtrzyljzva.html

PHP:  public string $name = "x";
来源：http://hz.ehwqpu.com/gtfpfjjaaa.html

JS:   this.name = "x";
来源：http://hz.wangdashe.top/gtzckucsjq.html

TS:   name: string = "x";
来源：http://hz.nanxuanxn.top/gtgxkozmsy.html

Java: private String name;
来源：http://hz.hongshengwenyu.top/gtbygyzdzs.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.cqqwz.cn/gtdilufabc.html

Ruby: @name = "x"
来源：http://hz.52xcode.cn/gtqszndhpc.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.ivvv.top/gtpjvgwnyg.html

[G04] 定义方法
来源：http://hz.chenzaomai.com/gtxxuaehxz.html

Py:   def greet(self): return self.name
来源：http://hz.sxryk.cn/gtuztyldep.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.hysaishi.cn/gttzppqimb.html

JS:   greet() { return this.name; }
来源：http://hz.jiagoushi.top/gtioyfjqzz.html

TS:   greet(): string { return this.name; }
来源：http://hz.sxryk.cn/gthfdjuzfk.html

Java: String greet() { return name; }
来源：http://hz.daria6918.cn/gtazpteigu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.shangyingyoupin.top/gtmuhtclql.html

Ruby: def greet; @name; end
来源：http://hz.c1oappe.top/gtoxpjlkhr.html

C#:   public string Greet() => Name;
来源：http://hz.zhiwuduotai.top/gtjchgxnwy.html

[G05] 继承
来源：http://hz.zhaomingkeji.xyz/gttbibvbik.html

Py:   class Admin(User): pass
来源：http://hz.jlsjyb.cn/gtvukssnwb.html

PHP:  class Admin extends User {}
来源：http://hz.sysykeji.top/gtvhwbzpiq.html

JS:   class Admin extends User {}
来源：http://hz.cashguo.top/gtjiqryocr.html

TS:   class Admin extends User {}
来源：http://hz.yvedp.cn/gtswloixhv.html

Java: class Admin extends User {}
来源：http://hz.smart0.xyz/gtonipjdnx.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.gotoacloud.top/gtynsaftla.html

Ruby: class Admin < User; end
来源：http://hz.fengsongda.top/gtxvlhkrsx.html

C#:   class Admin : User {}
来源：http://hz.fzhhl.top/gtgnwiublc.html

[G06] 重写方法
来源：http://hz.birdmap.top/gtqvscvdqq.html

Py:   def greet(self): return "admin"
来源：http://hz.zhixingplan.top/gtkbwbypta.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.xuetiantiany.cn/gtwzpaskcc.html

JS:   greet() { return "admin"; }
来源：http://hz.zdqjudy.top/gtblsicmkw.html

TS:   greet(): string { return "admin"; }
来源：http://hz.cucudq.cn/gtqijeflrg.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.yanxiufei.cn/gtaoymgfax.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.cashguo.top/gtxshsxtdx.html

Ruby: def greet; "admin"; end
来源：http://hz.kuanghao11.cn/gtlyophvtl.html

C#:   public override string Greet() => "admin";
来源：http://hz.yonumen.top/gtnpruxlhp.html

[G07] 调用父类方法
来源：http://hz.shanyushiyangtech.top/gtsepknwhd.html

Py:   super().greet()
来源：http://hz.tanke756.top/gtrazfhuhd.html

PHP:  parent::greet();
来源：http://hz.aizwys.cn/gthbtuhtou.html

JS:   super.greet();
来源：http://hz.redwolf501.top/gtoyzsheap.html

TS:   super.greet();
来源：http://hz.cheryme.top/gtsioklrot.html

Java: super.greet();
来源：http://hz.ywan-chungtsiang.top/gtjzeisckz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jlsjyb.cn/gtazipscxi.html

Ruby: super
来源：http://hz.0kj1m.cn/gtqompjbia.html

C#:   base.Greet();
来源：http://hz.xuetiantiany.cn/gtmjnvbhck.html

[G08] 静态方法与属性
来源：http://hz.tanke756.top/gtxlzeyhpd.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zhiwuduotai.top/gtlkrqtaan.html

PHP:  public static function f() {}
来源：http://hz.cashguo.top/gtorrslfiu.html

JS:   static f() {}
来源：http://hz.shangyingyoupin.top/gtfrkuudtk.html

TS:   static f(): void {}
来源：http://hz.zhoulong.xyz/gtsmxkiifl.html

Java: static void f() {}
来源：http://hz.chenzaomai.com/gtsdryeuug.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yangfankeji.com/gtmczadmck.html

Ruby: def self.f; end
来源：http://hz.ydjk.org.cn/gtxcbcbuop.html

C#:   public static void F() {}
来源：http://hz.hnxiangtu.top/gthtdadmxk.html

[G09] 接口 / 抽象类
来源：http://hz.shzxlz.cn/gtnqmlmfxt.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yuanzhike.top/gtgbmxxlzr.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.nwbrower.top/gtlnvzjkqh.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.andypj.xyz/gtvssmdsrm.html

TS:   interface Shape { area(): number; }
来源：http://hz.xinyue.icu/gtdwnwlzuj.html

Java: interface Shape { double area(); }
来源：http://hz.zhoulong.xyz/gtaqfeiajj.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.chenlongwang.top/gtjacxnnvf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.chenjidiqi.icu/gtuudyfjuh.html

C#:   interface IShape { double Area(); }
来源：http://hz.redwolf501.top/gtgymwikac.html

[G10] 访问控制
来源：http://hz.kuanghao11.cn/gtaphiikda.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.sysykeji.top/gtzooizfxl.html

PHP:  public / protected / private
来源：http://hz.fzhhl.top/gthqfiapvy.html

JS:   #private 字段；其余公开
来源：http://hz.nanxinkj.top/gtgwzfhpee.html

TS:   public / protected / private
来源：http://hz.xylfe.cn/gtpiuqncok.html

Java: public / protected / private / 默认包级
来源：http://hz.dianchejie.cn/gtddabyxke.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.hnxiangtu.top/gtruusacdn.html

Ruby: public / protected / private
来源：http://hz.guannengcc.top/gtscwtdsad.html

C#:   public / protected / private / internal
来源：http://hz.ppjwa.cn/gtitqmqkja.html

[G11] getter / setter
来源：http://hz.hywenlv.cn/gtrbywjssi.html

Py:   @property 与 @x.setter
来源：http://hz.cheryme.top/gtjgpwcfan.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.fzhhl.top/gtqgrtainr.html

JS:   get name() { return this._name; }
来源：http://hz.gotoacloud.top/gtdeadsyjj.html

TS:   get name(): string { return this._name; }
来源：http://hz.jqgfzy.top/gtcafvzzkc.html

Java: public String getName() { return name; }
来源：http://hz.feifeiyinyue.top/gtxlnrfcjf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.gaohongyu789.top/gtbscsiyae.html

Ruby: attr_accessor :name
来源：http://hz.cqqwz.cn/gtrsgdtmmn.html

C#:   public string Name { get; set; }
来源：http://hz.xylfe.cn/gtopymiojm.html

[G12] 对象转字符串
来源：http://hz.sxryk.cn/gtbzjgmqoc.html

Py:   def __str__(self): return self.name
来源：http://hz.yangfankeji.com/gtadhshmoq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.wangdashe.top/gtsdpkqhhk.html

JS:   toString() { return this.name; }
来源：http://hz.aizwys.cn/gtaxhfgfks.html

TS:   toString(): string { return this.name; }
来源：http://hz.chenjidiqi.icu/gtrdkmyqza.html

Java: @Override public String toString() { return name; }
来源：http://hz.shzxlz.cn/gteqlukjws.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yanxiufei.cn/gtpmqhqyvn.html

Ruby: def to_s; @name; end
来源：http://hz.hysaishi.cn/gtlziwsvlj.html

C#:   public override string ToString() => Name;
来源：http://hz.ydzc1.top/gtotcxmpkn.html

[G13] 判断对象类型
来源：http://hz.xuetiantiany.cn/gteqtsooqj.html


<!-- 参考信息 -->