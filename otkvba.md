代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.xylfe.cn/gtwzkowfqg.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.svipenyu.cn/gtavnyzcaf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.xingfuxueyuan.xyz/gtzlxprkva.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.mhx1999.top/gtxvrtlhgg.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.jqgfzy.top/gtkiujxjfy.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.hammf.cn/gteixfcbmf.html

[E16] 数字千分位
来源：http://hz.daria6918.cn/gtxuaqlftl.html

Py:   f"{1234567:,}"
来源：http://hz.zhongyouzk.top/gtnmouppvt.html

PHP:  number_format(1234567);
来源：http://hz.aizwys.cn/gtetyhhvfv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.hammf.cn/gtgzsxffbl.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.meibo888.top/gtgymkgimr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.aizwys.cn/gtphhtoowu.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.mhx1999.top/gtsyzixvpu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.pengpengdd.cyou/gtogwnschk.html

C#:   1234567.ToString("N0")
来源：http://hz.zhiwuduotai.top/gtmffictsb.html

[E17] 首字母大写
来源：http://hz.tianlin.xyz/gtejtfefah.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.hysaishi.cn/gtbbfljqxq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.vqdsnc.cn/gtsigariqw.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yuanzhike.top/gtjoenvuov.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.redwolf501.top/gtppmnozdo.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.hfpthk.cn/gtsavrejaf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.shangyingyoupin.top/gtrwyybvab.html

Ruby: s.capitalize
来源：http://hz.dianchejie.cn/gtqscivpwt.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yongpay.top/gtvqlknkqy.html

[E18] 模板占位符替换
来源：http://hz.chenjidiqi.icu/gtwsoppkez.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.0kj1m.cn/gtoioqyygj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.snrcjt.cn/gtdmchvboc.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.wangdashe.top/gtpzxphtvt.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.zhiwuduotai.top/gtzljithmo.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.hywenlv.cn/gttbnfuoya.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.yueranfly.top/gtbcijzhcg.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.fengsongda.top/gtiefsthxg.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.hfpthk.cn/gtsydcornx.html

[E19] 多行文本按行拆分
来源：http://hz.wangdashe.top/gtsiiohwoj.html

Py:   s.splitlines()
来源：http://hz.jiagoushi.top/gtkmwlktcb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.svipenyu.cn/gtgbqhpmft.html

JS:   s.split(/\r?\n/)
来源：http://hz.nanxinkj.top/gtnemgzwtb.html

TS:   s.split(/\r?\n/)
来源：http://hz.havefunace.top/gtfmfudypy.html

Java: s.lines().toList()
来源：http://hz.chenzaomai.com/gtawrecwdw.html

Go:   strings.Split(s, "\n")
来源：http://hz.jqgufenzy.top/gtzrsfzzsl.html

Ruby: s.lines
来源：http://hz.quarkkingdee.top/gtojoydkje.html

C#:   s.Split('\n')
来源：http://hz.yueranfly.top/gtfyrgdfih.html

[E20] 判断字符串是否为空
来源：http://hz.xylfe.cn/gtrbbcsggj.html

Py:   if not s:
来源：http://hz.bjfxy.top/gtcwakaaeh.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.shanyushiyangtech.top/gtxnjgqwpf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.shzxlz.cn/gtlpfsptkf.html

TS:   if (s === "") {}
来源：http://hz.yvedp.cn/gtiwrtxvoa.html

Java: if (s.isEmpty()) {}
来源：http://hz.ivvv.top/gtqqkmrzzh.html

Go:   if s == "" {}
来源：http://hz.jqgfzy.top/gtfqlvrxhd.html

Ruby: if s.empty?
来源：http://hz.0kj1m.cn/gtfbeanszo.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.nanxuanxn.top/gtsfgovumt.html

[E21] 超长截断加省略号
来源：http://hz.chenjidiqi.icu/gtpdkfnelz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.snrcjt.cn/gtdojuswan.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.xinyue.icu/gtzdvwzfaz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.xingfuxueyuan.xyz/gtrsqronss.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.gaohongyu789.top/gtkkeeauih.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.guannengcc.top/gtiykftgup.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.yonumen.top/gtepbvikxr.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.redwolf501.top/gtqgnjdkow.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.jinyuanbaomall.cn/gtgmeyxmsp.html

[E22] 字节长度与字符长度
来源：http://hz.hnqzz.top/gthwbvdgws.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.guowangkeji.top/gtvymowswi.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.xziqi.cn/gtfhikonev.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ppjwa.cn/gtfvosnakn.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.gogol.net.cn/gtqjnnaepb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.0kj1m.cn/gthsyjylsd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.cashguo.top/gtqgzfmgze.html

Ruby: s.bytesize;  s.length
来源：http://hz.zhixingplan.top/gtwohcbxgc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.yj202588.top/gtzlmqaoaf.html

================================================================================
来源：http://hz.zycfv.cn/gtvlqdvcxz.html

F. 文件与目录
来源：http://hz.yj202588.top/gtgdawwpgr.html

================================================================================
来源：http://hz.bjfxy.top/gtefeiwlnk.html

[F01] 读取整个文件
来源：http://hz.jianghu66.top/gttnzirxby.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yuanzhike.top/gtqtvevpdl.html

PHP:  file_get_contents("a.txt");
来源：http://hz.gogol.net.cn/gtdijcnkdt.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.zhengqikj.top/gtmaxrptml.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.yongpay.top/gtpodqpgsd.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.yuxming.cn/gtonkhoxcv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.cucudq.cn/gtlgrztydq.html

Ruby: File.read("a.txt")
来源：http://hz.shangyingyoupin.top/gtlbctxqul.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.xuetiantiany.cn/gtzypemmbk.html

[F02] 逐行读取文件
来源：http://hz.sysykeji.top/gtxnocevor.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.yangfankeji.com/gtnbztbaas.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.jinghuilouyu.cn/gtcdpkvwis.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.bjfxy.top/gtwqtqafbd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.shzxlz.cn/gtzsoaupsm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.0kj1m.cn/gtkqzhldcy.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.ivvv.top/gtivubbpsg.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.jinyuanbaomall.cn/gtonehkcts.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.wangshuangyany.cn/gtosqxlwkk.html

[F03] 写入文件（覆盖）
来源：http://hz.jianghu66.top/gtnvrzkvue.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.zhiwuduotai.top/gtygktxxel.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.xuetiantiany.cn/gtqdezlziz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jinyuanbaomall.cn/gtrdtkqmkl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hammf.cn/gtjieczqzx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.nwbrower.top/gthevgswct.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.9152youxi.cn/gtujatopbo.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.ppjwa.cn/gtehhjupjy.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.gzhubu.top/gtfivuafok.html

[F04] 追加写入文件
来源：http://hz.yanxiufei.cn/gtqwxogqjw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yj20258.top/gtiinyqdmu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.jinyuanbaomall.cn/gtwqgnnvbe.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.0kj1m.cn/gtljwjfhdh.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.xuetiantiany.cn/gtujdkavsw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.yj202588.top/gtulzbxhpy.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.snrcjt.cn/gtzhvstqqt.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.316326.xyz/gtxyhdvpsh.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.shangyingyoupin.top/gtjhlnoitr.html

[F05] 判断文件或目录是否存在
来源：http://hz.jinyuanbaomall.cn/gtqqedihmi.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.nanxinkj.top/gtcwbkkvig.html

PHP:  file_exists("a.txt");
来源：http://hz.jyoumei.cn/gtugraddno.html

JS:   fs.existsSync("a.txt")
来源：http://hz.nanxinkj.top/gtmtijmmpg.html

TS:   fs.existsSync("a.txt")
来源：http://hz.nanxuanxn.top/gtjkvijsto.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.daxiang520.top/gtenbouuxi.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.sweek.top/gtvratvupr.html

Ruby: File.exist?("a.txt")
来源：http://hz.jiagoushi.top/gtkeorwiep.html

C#:   File.Exists("a.txt")
来源：http://hz.jqgfzy.top/gtxnnrafzg.html

[F06] 删除文件
来源：http://hz.guowangkeji.top/gtjpouerjd.html

Py:   os.remove("a.txt")
来源：http://hz.cqqwz.cn/gtaoxlnoyo.html

PHP:  unlink("a.txt");
来源：http://hz.tanke756.top/gtlnfdoqen.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.daxiang520.top/gtbbdyirvs.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.ybcxt.top/gtzorxlcph.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.gotoacloud.top/gtapmxxauw.html

Go:   os.Remove("a.txt")
来源：http://hz.daxiang520.top/gtnadutbxg.html

Ruby: File.delete("a.txt")
来源：http://hz.svipenyu.cn/gtkipgrnmj.html

C#:   File.Delete("a.txt");
来源：http://hz.sweek.top/gtevruhebg.html

[F07] 创建目录（含多级）
来源：http://hz.jlsjyb.cn/gtqgmqlccz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.ywan-chungtsiang.top/gtrcjuegcs.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.shzxlz.cn/gtzitplbdq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ydjk.org.cn/gtjzkszycz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yj20258888.top/gtwlxcyqve.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.guowangkeji.top/gtgjchixxf.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.9152youxi.cn/gtiefkxxix.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.jiagoushi.top/gtbfrjrgxx.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.jinyuanbaomall.cn/gtfkimhgjv.html

[F08] 遍历目录
来源：http://hz.yonumen.top/gtkvbwzoyk.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.jlsjyb.cn/gticnuwmlg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.tianlin.xyz/gtzeizrmyz.html

JS:   fs.readdirSync("dir")
来源：http://hz.cucudq.cn/gtqczqgapt.html

TS:   fs.readdirSync("dir")
来源：http://hz.jlsjyb.cn/gtsmjeorzv.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.meibo888.top/gtemfaldmc.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.shzxlz.cn/gtkksvgorv.html

Ruby: Dir.children("dir")
来源：http://hz.smart0.xyz/gtzngqbnab.html

C#:   Directory.GetFiles("dir")
来源：http://hz.pengpengdd.cyou/gtcekuekzj.html

[F09] 获取文件大小
来源：http://hz.jinqigfzy.top/gtxlbxaras.html

Py:   os.path.getsize("a.txt")
来源：http://hz.yj202588.top/gtpefoiygg.html

PHP:  filesize("a.txt");
来源：http://hz.xuetiantiany.cn/gtzszwszej.html

JS:   fs.statSync("a.txt").size
来源：http://hz.316326.xyz/gtkvintmzw.html

TS:   fs.statSync("a.txt").size
来源：http://hz.iojbl.cn/gtmvvdmemm.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.vqdsnc.cn/gtrwjcpjji.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.guannengcc.top/gtchmhxyln.html

Ruby: File.size("a.txt")
来源：http://hz.redwolf501.top/gtfjzzaocg.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.jianghu66.top/gtsnqmluxl.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.jinqigfzy.top/gtkpepysid.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.yj20258.top/gtfuegdokt.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.zhijiandao.cn/gtcktmugvo.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.jlsjyb.cn/gtbbcsaops.html

TS:   path.extname("a.txt")
来源：http://hz.guowangkeji.top/gtczxgrbst.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.xingfuxueyuan.xyz/gtrnnsywyr.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.shzxlz.cn/gtxzwpcldd.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.zhoulong.xyz/gtffpowvco.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.chenjidiqi.icu/gtcuqbivci.html

[F11] 复制与移动文件
来源：http://hz.hongshengwenyu.top/gtwlktpgow.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.pengpengdd.cyou/gtttkvyurr.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.dianchejie.cn/gtkltjfqhf.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jinyuanbaomall.cn/gtuoowdmti.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jqgufenzy.top/gtegnhwclg.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.yonumen.top/gtrhmxstai.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.havefunace.top/gtaxbvpywn.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.yvedp.cn/gtjjrxqpnj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.xylfe.cn/gtcfglvpsd.html

[F12] CSV 读写
来源：http://hz.yuanzhike.top/gtvaadjmwj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.shanyushiyangtech.top/gtjzwgeiyc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.jinqigufen.top/gtjycwmtjy.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.nanxuanxn.top/gtqcmxvqjl.html

TS:   // 同上
来源：http://hz.fengsongda.top/gtunycgrbv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.fzhhl.top/gtuzmzpqfb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.sufxvd.cn/gtwjetfzdc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.xylfe.cn/gtocpbjfss.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.shanyushiyangtech.top/gtyoniqayw.html

================================================================================
来源：http://hz.tanke756.top/gtzsegnhcl.html

G. 面向对象
来源：http://hz.jlsjyb.cn/gttylamwjo.html

================================================================================
来源：http://hz.pycfn.com/gtxgelqeuh.html

[G01] 定义类
来源：http://hz.jinqigufen.top/gtxcgzgtji.html

Py:   class User: pass
来源：http://hz.pengpengdd.cyou/gtluuqyyxm.html

PHP:  class User {}
来源：http://hz.dianchejie.cn/gtomcgqbtd.html

JS:   class User {}
来源：http://hz.yuanzhike.top/gtzpsfssuu.html

TS:   class User { name: string = ""; }
来源：http://hz.daria6918.cn/gtizywslon.html

Java: class User {}
来源：http://hz.yuanzhike.top/gtsfwtprhr.html

Go:   type User struct { Name string }
来源：http://hz.jiagoushi.top/gtrexeiftp.html

Ruby: class User; end
来源：http://hz.yj20258.top/gtprawnxgl.html

C#:   class User {}
来源：http://hz.zhaomingkeji.xyz/gtuiouctco.html

[G02] 构造函数
来源：http://hz.kuanghao11.cn/gtuxnzjcot.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.cqqwz.cn/gtrsfmxwhy.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.sxryk.cn/gtvsgukinp.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.dashuyun.cn/gtswxzitan.html

TS:   constructor(public name: string) {}
来源：http://hz.redwolf501.top/gtocetjiud.html

Java: User(String name) { this.name = name; }
来源：http://hz.jlsjyb.cn/gtualyoxcc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.zycfv.cn/gtoujnnvhz.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.shanyushiyangtech.top/gtjygbrfji.html

C#:   public User(string name) { Name = name; }
来源：http://hz.yonumen.top/gteqtjqphv.html

[G03] 实例属性
来源：http://hz.zhiwuduotai.top/gtsbuabsqg.html

Py:   self.name = "x"
来源：http://hz.cheryme.top/gtydmyzsgy.html

PHP:  public string $name = "x";
来源：http://hz.wangshuangyany.cn/gtntbaxpzp.html

JS:   this.name = "x";
来源：http://hz.guowangkeji.top/gttxqjdsxz.html

TS:   name: string = "x";
来源：http://hz.ydjk.org.cn/gtgddzpurp.html

Java: private String name;
来源：http://hz.tianlin.xyz/gtblalxtkt.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.xuetiantiany.cn/gtqorkbfcf.html

Ruby: @name = "x"
来源：http://hz.svipenyu.cn/gtkrbegurs.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.zhengqikj.top/gtgnwokrav.html

[G04] 定义方法
来源：http://hz.pengpengdd.cyou/gtorsjyzwv.html

Py:   def greet(self): return self.name
来源：http://hz.meibo888.top/gtimpmppqa.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yongpay.top/gtylqrpenl.html

JS:   greet() { return this.name; }
来源：http://hz.sufxvd.cn/gtmnmcnjke.html

TS:   greet(): string { return this.name; }
来源：http://hz.zycfv.cn/gttjsawnae.html

Java: String greet() { return name; }
来源：http://hz.mhx1999.top/gtspgtsllp.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.pengpengdd.cyou/gtfeiudhok.html

Ruby: def greet; @name; end
来源：http://hz.chenjidiqi.icu/gtmxlrjigk.html

C#:   public string Greet() => Name;
来源：http://hz.nwbrower.top/gtbybqlpdm.html

[G05] 继承
来源：http://hz.jinqigufen.top/gteecwwjzm.html

Py:   class Admin(User): pass
来源：http://hz.yongpay.top/gtqdtzxgyb.html

PHP:  class Admin extends User {}
来源：http://hz.sxryk.cn/gtgbuuwdja.html

JS:   class Admin extends User {}
来源：http://hz.yangfankeji.com/gtwyaavyxw.html

TS:   class Admin extends User {}
来源：http://hz.hnxiangtu.top/gtbqlowovc.html

Java: class Admin extends User {}
来源：http://hz.mhx1999.top/gthzfasidx.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.aizwys.cn/gtcwnfcmqi.html

Ruby: class Admin < User; end
来源：http://hz.daxiang520.top/gtxgrslhaf.html

C#:   class Admin : User {}
来源：http://hz.andypj.xyz/gtojuztdpp.html

[G06] 重写方法
来源：http://hz.yueranfly.top/gtimwpjpkz.html

Py:   def greet(self): return "admin"
来源：http://hz.jiagoushi.top/gthwhffaao.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.pycfn.com/gtxnhnivmz.html

JS:   greet() { return "admin"; }
来源：http://hz.tanke756.top/gtkuvzmmfg.html

TS:   greet(): string { return "admin"; }
来源：http://hz.fzhhl.top/gtldxbprmy.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.fzhhl.top/gtomhwwfxu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.redwolf501.top/gtirnawjzq.html

Ruby: def greet; "admin"; end
来源：http://hz.kuanghao11.cn/gtiioqjfhs.html

C#:   public override string Greet() => "admin";
来源：http://hz.hfpthk.cn/gtjnsumbpy.html

[G07] 调用父类方法
来源：http://hz.52xcode.cn/gtezvfxlnd.html

Py:   super().greet()
来源：http://hz.shuidangran.top/gtyvzuluut.html

PHP:  parent::greet();
来源：http://hz.yj202588.top/gthpwmhvoi.html

JS:   super.greet();
来源：http://hz.zhengqikj.top/gtxsmmhnlz.html

TS:   super.greet();
来源：http://hz.yanxiufei.cn/gthgmlriwo.html

Java: super.greet();
来源：http://hz.jinyuanbaomall.cn/gtkukdorko.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.zycfv.cn/gtaazmgffl.html

Ruby: super
来源：http://hz.52xcode.cn/gtezkbkukm.html

C#:   base.Greet();
来源：http://hz.sweek.top/gtecqwkvtf.html

[G08] 静态方法与属性
来源：http://hz.hysaishi.cn/gtfpahcaqu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.daria6918.cn/gtriolwnrq.html

PHP:  public static function f() {}
来源：http://hz.xuetiantiany.cn/gtfzvjlfzp.html

JS:   static f() {}
来源：http://hz.hysaishi.cn/gtonnqpacy.html

TS:   static f(): void {}
来源：http://hz.meibo888.top/gtqqppxfho.html

Java: static void f() {}
来源：http://hz.yj20258.top/gtdiqmraai.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yangfankeji.com/gtqvhwajgd.html

Ruby: def self.f; end
来源：http://hz.aizwys.cn/gtkniumcov.html

C#:   public static void F() {}
来源：http://hz.shuidangran.top/gtewvyudzf.html

[G09] 接口 / 抽象类
来源：http://hz.xinyue.icu/gtlewdxrft.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.zhijiandao.cn/gtvcjzfcor.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.316326.xyz/gtmmwiecfu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.jqgfzy.top/gtrdmmmoqj.html

TS:   interface Shape { area(): number; }
来源：http://hz.cheryme.top/gtvpahmcdt.html

Java: interface Shape { double area(); }
来源：http://hz.ppjwa.cn/gtybgfofft.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.hysaishi.cn/gtumsuwxyv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.sufxvd.cn/gtdrayiowz.html

C#:   interface IShape { double Area(); }
来源：http://hz.0kj1m.cn/gtgvhsfglp.html

[G10] 访问控制
来源：http://hz.hfpthk.cn/gtkwshydnm.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.vqdsnc.cn/gtpjyjmaty.html

PHP:  public / protected / private
来源：http://hz.xinyue.icu/gtncdeseyj.html

JS:   #private 字段；其余公开
来源：http://hz.xinyue.icu/gtwviqhryy.html

TS:   public / protected / private
来源：http://hz.andypj.xyz/gtacdmyhei.html

Java: public / protected / private / 默认包级
来源：http://hz.zycfv.cn/gtznnqesvr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.jinyuanbaomall.cn/gtfjqgegzj.html

Ruby: public / protected / private
来源：http://hz.shanyushiyangkeji.top/gttkoxezuh.html

C#:   public / protected / private / internal
来源：http://hz.hammf.cn/gtejjmzdkw.html

[G11] getter / setter
来源：http://hz.jyoumei.cn/gtgmerexkf.html

Py:   @property 与 @x.setter
来源：http://hz.zhaomingkeji.xyz/gtlirhgfas.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.xylfe.cn/gtemaejhku.html

JS:   get name() { return this._name; }
来源：http://hz.c1oappe.top/gtqwalplmb.html

TS:   get name(): string { return this._name; }
来源：http://hz.pengpengdd.cyou/gtnvonsqxs.html

Java: public String getName() { return name; }
来源：http://hz.xingfuxueyuan.xyz/gtezhwdpyj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.haohaochexian.top/gtxnrfefmr.html

Ruby: attr_accessor :name
来源：http://hz.havefunace.top/gtfczizrry.html

C#:   public string Name { get; set; }
来源：http://hz.zhijiandao.cn/gtohurlvaq.html

[G12] 对象转字符串
来源：http://hz.sufxvd.cn/gtrcplbqfl.html

Py:   def __str__(self): return self.name
来源：http://hz.hysaishi.cn/gtvengizwx.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yongpay.top/gtndhqbdtg.html

JS:   toString() { return this.name; }
来源：http://hz.tanke756.top/gtxjpwnwra.html

TS:   toString(): string { return this.name; }
来源：http://hz.yanxiufei.cn/gtuvtyiqqr.html

Java: @Override public String toString() { return name; }
来源：http://hz.gaohongyu789.top/gtfymhpvoe.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jinghuilouyu.cn/gtfiivasik.html

Ruby: def to_s; @name; end
来源：http://hz.ehwqpu.com/gtovmghtev.html

C#:   public override string ToString() => Name;
来源：http://hz.zhengqikj.top/gtwqpxvxcj.html

[G13] 判断对象类型
来源：http://hz.aibaodan.cn/gtltlepaed.html

Py:   isinstance(u, User)
来源：http://hz.sxryk.cn/gttbpailcy.html

PHP:  $u instanceof User
来源：http://hz.nanxuanxn.top/gttydlecsq.html

JS:   u instanceof User
来源：http://hz.aizwys.cn/gtmkocamxg.html

TS:   u instanceof User
来源：http://hz.hysaishi.cn/gtelmexjsn.html

Java: u instanceof User
来源：http://hz.dianchejie.cn/gthpzcvyvd.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.pycfn.com/gtmhhrawdw.html

Ruby: u.is_a?(User)
来源：http://hz.quarkkingdee.top/gticlnzeoz.html

C#:   u is User
来源：http://hz.zhiwuduotai.top/gtzreaqssv.html


<!-- 参考信息 -->