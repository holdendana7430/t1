代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.cqqwz.cn/gtectqsjdq.html

[E15] HTML 转义 / 反转义
来源：http://hz.shanyushiyangkeji.top/gtbpfijlsr.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.jianghu66.top/gthoizgpmm.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.zhengqikj.top/gtkcxtbikt.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.cdnleiting.top/gtpbrttrtf.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.hnqzz.top/gtdnymqohb.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.zhixingplan.top/gtxrogwbtr.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.jianghu66.top/gtqsjzwkfi.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.pengpengdd.cyou/gtysnlouss.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.kuanghao11.cn/gtxoizakgg.html

[E16] 数字千分位
来源：http://hz.nwbrower.top/gtrbtcqurk.html

Py:   f"{1234567:,}"
来源：http://hz.hysaishi.cn/gtjrjxmelb.html

PHP:  number_format(1234567);
来源：http://hz.pengpengdd.cyou/gtkxfjlbxf.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.dianchejie.cn/gtkcwwbemo.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.redwolf501.top/gtgbkjtpkt.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.fzhhl.top/gtgyuhwipd.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.shanyushiyangkeji.top/gtxxcrinva.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.yanxiufei.cn/gtzwjmckdk.html

C#:   1234567.ToString("N0")
来源：http://hz.kuanghao11.cn/gtcqifkixw.html

[E17] 首字母大写
来源：http://hz.jiagoushi.top/gtsmxsddvh.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.bjfxy.top/gtmseopaxe.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.wangdashe.top/gtiexrmzlq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.shangyingyoupin.top/gtzmehdebb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.cucudq.cn/gttuscdidw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.ydjk.org.cn/gtxmzublge.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.shzxlz.cn/gteyzrszwr.html

Ruby: s.capitalize
来源：http://hz.gogol.net.cn/gttpokwkps.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.haohaochexian.top/gtcmjzknzj.html

[E18] 模板占位符替换
来源：http://hz.zhixingplan.top/gtmaazjrhx.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.hnqzz.top/gtqinchrea.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.haohaochexian.top/gtxvoztzan.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.jinqigufen.top/gtkbotlcxt.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.hysaishi.cn/gtvcufyrhs.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.52xcode.cn/gtmmeuwgib.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.hnqzz.top/gtolyeisnr.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.guannengcc.top/gthqlzdete.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.tianlin.xyz/gtfbaifncz.html

[E19] 多行文本按行拆分
来源：http://hz.sxryk.cn/gtwswtdpvg.html

Py:   s.splitlines()
来源：http://hz.bjfxy.top/gtjzgrblrq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.9152youxi.cn/gtzfeslvjd.html

JS:   s.split(/\r?\n/)
来源：http://hz.dianchejie.cn/gtxddwygdv.html

TS:   s.split(/\r?\n/)
来源：http://hz.quarkkingdee.top/gtufkggojs.html

Java: s.lines().toList()
来源：http://hz.feifeiyinyue.top/gtgitfdcsh.html

Go:   strings.Split(s, "\n")
来源：http://hz.guowangkeji.top/gtlnzgbxes.html

Ruby: s.lines
来源：http://hz.shanyushiyangtech.top/gtinknbeju.html

C#:   s.Split('\n')
来源：http://hz.snrcjt.cn/gtkouvmpxj.html

[E20] 判断字符串是否为空
来源：http://hz.vqdsnc.cn/gtilthadvx.html

Py:   if not s:
来源：http://hz.chenzaomai.com/gtutynbhwr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.zhixingplan.top/gtwhsdntrx.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.haohaochexian.top/gtngxjatpj.html

TS:   if (s === "") {}
来源：http://hz.shzxlz.cn/gtrrlqyzer.html

Java: if (s.isEmpty()) {}
来源：http://hz.aibaodan.cn/gtsaroxieq.html

Go:   if s == "" {}
来源：http://hz.aizwys.cn/gtnwlewpqu.html

Ruby: if s.empty?
来源：http://hz.zhaomingkeji.xyz/gtztcfvtly.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.feifeiyinyue.top/gtkhlxgkmh.html

[E21] 超长截断加省略号
来源：http://hz.jyoumei.cn/gtwvluyorz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.andypj.xyz/gtskahisqm.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.ivvv.top/gttjingkxj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yongpay.top/gtaoqctkmv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.andypj.xyz/gtpanmjaam.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.pycfn.com/gtwisfbafi.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.ydzc1.top/gtsbpxgehd.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.ivvv.top/gtbpwxmyap.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.daria6918.cn/gtipjrutrn.html

[E22] 字节长度与字符长度
来源：http://hz.yonumen.top/gtcnnlzule.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.yj202588.top/gtpjzkfyxy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.bjfxy.top/gtjijepjii.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.wangshuangyany.cn/gtjreqqact.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.fengsongda.top/gtdwotyaql.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.tanke756.top/gtewhsbjtw.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.ybcxt.top/gtffxvsnqb.html

Ruby: s.bytesize;  s.length
来源：http://hz.kuanghao11.cn/gtvrkuqvgl.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.wangshuangyany.cn/gtibykrsjt.html

================================================================================
来源：http://hz.gotoacloud.top/gthsmsnagl.html

F. 文件与目录
来源：http://hz.316326.xyz/gtijxakxhw.html

================================================================================
来源：http://hz.yj20258.top/gtzemllobb.html

[F01] 读取整个文件
来源：http://hz.snrcjt.cn/gteoovedkc.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.cdnleiting.top/gtgbfqsnlq.html

PHP:  file_get_contents("a.txt");
来源：http://hz.birdmap.top/gtkjzbztve.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.jqgufenzy.top/gtilprpmbu.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.cheryme.top/gtaolmafpq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.hfpthk.cn/gthfefzimv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.9152youxi.cn/gtzqtkwtiy.html

Ruby: File.read("a.txt")
来源：http://hz.yuxming.cn/gtvxyvremu.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.316326.xyz/gtvqyuqapr.html

[F02] 逐行读取文件
来源：http://hz.guannengcc.top/gthfggyicf.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.zhijiandao.cn/gtthwhxcxb.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.snrcjt.cn/gtqmedlexg.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.52xcode.cn/gtrppuraby.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.c1oappe.top/gtfhtubeab.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.xylfe.cn/gtbzqucqnx.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.hysaishi.cn/gtcfdumzab.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.fengsongda.top/gtfxmofhre.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.zhoulong.xyz/gtzcihlnds.html

[F03] 写入文件（覆盖）
来源：http://hz.chenzaomai.com/gtizoeogek.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.zhaomingkeji.xyz/gthnsoltqq.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.haohaochexian.top/gtpwpvxbuh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.haohaochexian.top/gtpqeqedlx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.shzxlz.cn/gtrffbzgne.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.cashguo.top/gtvgkoyzds.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.ehwqpu.com/gtmiozjyiy.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.xziqi.cn/gtvhkhtman.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.jinqigufen.top/gtxssfvubp.html

[F04] 追加写入文件
来源：http://hz.aibaodan.cn/gtcanixpbs.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.hysaishi.cn/gthsreovty.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.andypj.xyz/gtlhvbealz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.iojbl.cn/gtbojbiycx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.hnxiangtu.top/gthsenkrgm.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.sysykeji.top/gtgndtgfqn.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.ybcxt.top/gtxvetewkt.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.ywan-chungtsiang.top/gtbdudralk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.cdnleiting.top/gtwwxptjsw.html

[F05] 判断文件或目录是否存在
来源：http://hz.aibaodan.cn/gtevlmshrw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.hongshengwenyu.top/gtdlhpvhhi.html

PHP:  file_exists("a.txt");
来源：http://hz.mhx1999.top/gtsvmnjmyu.html

JS:   fs.existsSync("a.txt")
来源：http://hz.xziqi.cn/gtbdqkvhmu.html

TS:   fs.existsSync("a.txt")
来源：http://hz.gaohongyu789.top/gtpxpgvnpw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.yuxming.cn/gtciyicyyw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.jianghu66.top/gtqavovhrz.html

Ruby: File.exist?("a.txt")
来源：http://hz.jqgufenzy.top/gtxmvhalhw.html

C#:   File.Exists("a.txt")
来源：http://hz.andypj.xyz/gtoxsokiwt.html

[F06] 删除文件
来源：http://hz.hnqzz.top/gtvfgbboxx.html

Py:   os.remove("a.txt")
来源：http://hz.zycfv.cn/gtxmdvdjne.html

PHP:  unlink("a.txt");
来源：http://hz.ybcxt.top/gtyqcmdzoo.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yueranfly.top/gtlswxwxcf.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.cashguo.top/gtcprzqscp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.yuanzhike.top/gtndyfhyef.html

Go:   os.Remove("a.txt")
来源：http://hz.jinqigufen.top/gtdexxhjyq.html

Ruby: File.delete("a.txt")
来源：http://hz.sxryk.cn/gtpwxrvpaz.html

C#:   File.Delete("a.txt");
来源：http://hz.wangdashe.top/gtmfrjgmng.html

[F07] 创建目录（含多级）
来源：http://hz.jlsjyb.cn/gtbbcfippp.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yangfankeji.com/gtcqwhnfhl.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.yanxiufei.cn/gtctghhlfb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yj202588.top/gtlghdvphm.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.tian-w.cn/gtznobngrd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.sweek.top/gtalmaysvj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.ybcxt.top/gtrdmzudxq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.svipenyu.cn/gtbfgktsmj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.sufxvd.cn/gtfkacnydc.html

[F08] 遍历目录
来源：http://hz.jiagoushi.top/gtnhujnhqj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.tanke756.top/gtlbiqozov.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.zhengqikj.top/gthnjxwnrw.html

JS:   fs.readdirSync("dir")
来源：http://hz.redwolf501.top/gtewiriwom.html

TS:   fs.readdirSync("dir")
来源：http://hz.chenzaomai.com/gtjdvtdkzj.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.fengsongda.top/gtyukatsio.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yongpay.top/gtfxquxqoq.html

Ruby: Dir.children("dir")
来源：http://hz.cashguo.top/gtxeojszwd.html

C#:   Directory.GetFiles("dir")
来源：http://hz.aibaodan.cn/gtuvsyvxma.html

[F09] 获取文件大小
来源：http://hz.jinghuilouyu.cn/gtebxytmvy.html

Py:   os.path.getsize("a.txt")
来源：http://hz.jqgfzy.top/gtpbjbqsbh.html

PHP:  filesize("a.txt");
来源：http://hz.haohaochexian.top/gtmzlgpzxm.html

JS:   fs.statSync("a.txt").size
来源：http://hz.jqgfzy.top/gttmxeckyp.html

TS:   fs.statSync("a.txt").size
来源：http://hz.jqgufenzy.top/gtvrbamiau.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.ywan-chungtsiang.top/gtqmeiufup.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.redwolf501.top/gtkperwolt.html

Ruby: File.size("a.txt")
来源：http://hz.zhongyouzk.top/gtbgxycjmf.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.xuanzx.com/gthajyplqo.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.cucudq.cn/gtceuqpaej.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.redwolf501.top/gtstvnbkrn.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.ivvv.top/gtwafmhrss.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.pycfn.com/gtlyukilzp.html

TS:   path.extname("a.txt")
来源：http://hz.guowangkeji.top/gtghgdqmhz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.kuanghao11.cn/gtjonojnmh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.316326.xyz/gtcxufxsxh.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.nanxuanxn.top/gtxcamcvsh.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.chenlongwang.top/gtjhwmueqn.html

[F11] 复制与移动文件
来源：http://hz.aizwys.cn/gtwqqbbfkz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.jlsjyb.cn/gtbdirdhun.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.dianchejie.cn/gtjrqmkxci.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.cashguo.top/gtanoxbfbv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.guannengcc.top/gtjqjfarlv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.wangdashe.top/gtvqvaphpc.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yuanzhike.top/gtlwbjjsni.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.guowangkeji.top/gtxvahvsxd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.tian-w.cn/gtfzgnzbjx.html

[F12] CSV 读写
来源：http://hz.hfpthk.cn/gtxuypjcrx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.shanyushiyangkeji.top/gtmalnayty.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.jinyuanbaomall.cn/gtdvsogsaf.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.jqgufenzy.top/gtempchocj.html

TS:   // 同上
来源：http://hz.gotoacloud.top/gtevplyiyq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.hnxiangtu.top/gttkjwevej.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.ydjk.org.cn/gtamoltcwo.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.yonumen.top/gtlgjitpbo.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jqgfzy.top/gtpjicbbke.html

================================================================================
来源：http://hz.aizwys.cn/gtjhdvllsa.html

G. 面向对象
来源：http://hz.ppjwa.cn/gtoqucewyv.html

================================================================================
来源：http://hz.yongpay.top/gtvcidusns.html

[G01] 定义类
来源：http://hz.jinghuilouyu.cn/gtbkymdjtl.html

Py:   class User: pass
来源：http://hz.c1oappe.top/gtlwrzwhuh.html

PHP:  class User {}
来源：http://hz.daxiang520.top/gtjmifgpya.html

JS:   class User {}
来源：http://hz.smart0.xyz/gtvfabxwfj.html

TS:   class User { name: string = ""; }
来源：http://hz.zhixingplan.top/gtjjdpvviw.html

Java: class User {}
来源：http://hz.mhx1999.top/gtgjjlmvop.html

Go:   type User struct { Name string }
来源：http://hz.yonumen.top/gtghwnrvat.html

Ruby: class User; end
来源：http://hz.hnqzz.top/gtwhuyjghb.html

C#:   class User {}
来源：http://hz.yueranfly.top/gtvxglrjoq.html

[G02] 构造函数
来源：http://hz.fengsongda.top/gtoirsotud.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.xylfe.cn/gtoinesfof.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.zhaomingkeji.xyz/gtsrmwbycp.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yvedp.cn/gtsjpgfqjr.html

TS:   constructor(public name: string) {}
来源：http://hz.yangfankeji.com/gtxaklgaee.html

Java: User(String name) { this.name = name; }
来源：http://hz.snrcjt.cn/gtppuqgufi.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.chenlongwang.top/gtoqylgizv.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.hammf.cn/gtizmbvczr.html

C#:   public User(string name) { Name = name; }
来源：http://hz.zhoulong.xyz/gtzjaalxhs.html

[G03] 实例属性
来源：http://hz.shanyushiyangtech.top/gtmbuuqbem.html

Py:   self.name = "x"
来源：http://hz.xingfuxueyuan.xyz/gtvjziobyt.html

PHP:  public string $name = "x";
来源：http://hz.dashuyun.cn/gtvawlapwc.html

JS:   this.name = "x";
来源：http://hz.gotoacloud.top/gtrgpcdffp.html

TS:   name: string = "x";
来源：http://hz.ivvv.top/gterfupamy.html

Java: private String name;
来源：http://hz.ppjwa.cn/gtvomfuqzp.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.cdnleiting.top/gtucqlslfr.html

Ruby: @name = "x"
来源：http://hz.fengsongda.top/gtxvpvsqnt.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jqgfzy.top/gtzkuyudzs.html

[G04] 定义方法
来源：http://hz.wangdashe.top/gtsepyzbvo.html

Py:   def greet(self): return self.name
来源：http://hz.kuanghao11.cn/gtnkasemri.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.shanyushiyangtech.top/gtidjnrqie.html

JS:   greet() { return this.name; }
来源：http://hz.wangshuangyany.cn/gtphbblwjk.html

TS:   greet(): string { return this.name; }
来源：http://hz.svipenyu.cn/gteeoqnkzd.html

Java: String greet() { return name; }
来源：http://hz.birdmap.top/gtppscssgy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.cucudq.cn/gtpopwgcpd.html

Ruby: def greet; @name; end
来源：http://hz.hywenlv.cn/gtuusvoizb.html

C#:   public string Greet() => Name;
来源：http://hz.gogol.net.cn/gtsnfjahio.html

[G05] 继承
来源：http://hz.shangyingyoupin.top/gtkhfmzrnp.html

Py:   class Admin(User): pass
来源：http://hz.vqdsnc.cn/gtblqqwpmp.html

PHP:  class Admin extends User {}
来源：http://hz.c1oappe.top/gthgwccfbh.html

JS:   class Admin extends User {}
来源：http://hz.xingfuxueyuan.xyz/gthgxaymjp.html

TS:   class Admin extends User {}
来源：http://hz.sufxvd.cn/gtgdcsqlzr.html

Java: class Admin extends User {}
来源：http://hz.yj20258.top/gtedfuqmut.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.zhongyouzk.top/gtltgpwuov.html

Ruby: class Admin < User; end
来源：http://hz.hongshengwenyu.top/gthognjakh.html

C#:   class Admin : User {}
来源：http://hz.shuidangran.top/gtaqexmgza.html

[G06] 重写方法
来源：http://hz.haohaochexian.top/gtrsvnxfki.html

Py:   def greet(self): return "admin"
来源：http://hz.tianlin.xyz/gtjkammyho.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.tian-w.cn/gtetzlumsi.html

JS:   greet() { return "admin"; }
来源：http://hz.chenzaomai.com/gtookfjnyq.html

TS:   greet(): string { return "admin"; }
来源：http://hz.cdnleiting.top/gtikgllqae.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.ehwqpu.com/gteubmyyss.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.hnqzz.top/gtuyrqbbrp.html

Ruby: def greet; "admin"; end
来源：http://hz.jyoumei.cn/gtalgdzdrh.html

C#:   public override string Greet() => "admin";
来源：http://hz.hnqzz.top/gtgdonneux.html

[G07] 调用父类方法
来源：http://hz.ywan-chungtsiang.top/gtvstaurdx.html

Py:   super().greet()
来源：http://hz.jinqigfzy.top/gtjhqcigzi.html

PHP:  parent::greet();
来源：http://hz.gotoacloud.top/gtjrhoyvow.html

JS:   super.greet();
来源：http://hz.zhongyouzk.top/gtnwdiuuij.html

TS:   super.greet();
来源：http://hz.redwolf501.top/gtynurzfos.html

Java: super.greet();
来源：http://hz.cdnleiting.top/gtsxqxzhzv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.zhongyouzk.top/gtrfhzmkqx.html

Ruby: super
来源：http://hz.aizwys.cn/gtgrnxkydk.html

C#:   base.Greet();
来源：http://hz.havefunace.top/gtlptymrey.html

[G08] 静态方法与属性
来源：http://hz.jqgfzy.top/gtoblxefdk.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.cdnleiting.top/gtlokeoyut.html

PHP:  public static function f() {}
来源：http://hz.zhoulong.xyz/gtuaasllue.html

JS:   static f() {}
来源：http://hz.hysaishi.cn/gtuvgynmpb.html

TS:   static f(): void {}
来源：http://hz.xylfe.cn/gtphqkfssn.html

Java: static void f() {}
来源：http://hz.tianlin.xyz/gthsxugagy.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yongpay.top/gtpuxceher.html

Ruby: def self.f; end
来源：http://hz.dianchejie.cn/gtiwcxgcpu.html

C#:   public static void F() {}
来源：http://hz.xinyue.icu/gtqzarucxv.html

[G09] 接口 / 抽象类
来源：http://hz.jianghu66.top/gtsyijxtsm.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.52xcode.cn/gtqibyixfh.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.aizwys.cn/gttwjypucu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.yj202588.top/gtpfpgkynv.html

TS:   interface Shape { area(): number; }
来源：http://hz.daria6918.cn/gtuahakiik.html

Java: interface Shape { double area(); }
来源：http://hz.snrcjt.cn/gtyxgprrtn.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.cdnleiting.top/gtmrhajvtn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.wangshuangyany.cn/gtwlexsonb.html

C#:   interface IShape { double Area(); }
来源：http://hz.guowangkeji.top/gtisrsvdfk.html

[G10] 访问控制
来源：http://hz.zhaomingkeji.xyz/gtirpenhxd.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.sweek.top/gtuzikcajs.html

PHP:  public / protected / private
来源：http://hz.cheryme.top/gtkuunbgyx.html

JS:   #private 字段；其余公开
来源：http://hz.yj20258888.top/gtupythfcb.html

TS:   public / protected / private
来源：http://hz.feifeiyinyue.top/gtkkupoqrw.html

Java: public / protected / private / 默认包级
来源：http://hz.iojbl.cn/gtteanomzs.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zhijiandao.cn/gtlhpfyshz.html

Ruby: public / protected / private
来源：http://hz.yuxming.cn/gtmnrdbwgg.html

C#:   public / protected / private / internal
来源：http://hz.andypj.xyz/gtbkfchwlu.html

[G11] getter / setter
来源：http://hz.jinqigufen.top/gtuqdvbzuv.html

Py:   @property 与 @x.setter
来源：http://hz.zycfv.cn/gtbgarfdrd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.316326.xyz/gtgqrhoeqi.html

JS:   get name() { return this._name; }
来源：http://hz.mhx1999.top/gtprxwkgby.html

TS:   get name(): string { return this._name; }
来源：http://hz.jlsjyb.cn/gthrjoikzo.html

Java: public String getName() { return name; }
来源：http://hz.haohaochexian.top/gtyqrlwjto.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.wangshuangyany.cn/gttvqqszql.html

Ruby: attr_accessor :name
来源：http://hz.jinghuilouyu.cn/gteretobah.html

C#:   public string Name { get; set; }
来源：http://hz.zhixingplan.top/gtjzzjwvyg.html

[G12] 对象转字符串
来源：http://hz.fengsongda.top/gtgrstawtp.html

Py:   def __str__(self): return self.name
来源：http://hz.zhixingplan.top/gtjytqljtu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.tian-w.cn/gtkackfjor.html

JS:   toString() { return this.name; }
来源：http://hz.zhaomingkeji.xyz/gtcevavjfk.html

TS:   toString(): string { return this.name; }
来源：http://hz.cheryme.top/gtqwthvljx.html

Java: @Override public String toString() { return name; }
来源：http://hz.aibaodan.cn/gtkiivlypt.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.fzhhl.top/gtmcelnrav.html

Ruby: def to_s; @name; end
来源：http://hz.sysykeji.top/gttfxbyrcb.html

C#:   public override string ToString() => Name;
来源：http://hz.jianghu66.top/gtvbnwesyg.html

[G13] 判断对象类型
来源：http://hz.havefunace.top/gttoqucgpg.html

Py:   isinstance(u, User)
来源：http://hz.hnqzz.top/gtnhbwckjl.html

PHP:  $u instanceof User
来源：http://hz.nanxuanxn.top/gtehzqgieo.html

JS:   u instanceof User
来源：http://hz.nwbrower.top/gtrsrviogc.html

TS:   u instanceof User
来源：http://hz.wangdashe.top/gtaipryzoy.html


<!-- 参考信息 -->