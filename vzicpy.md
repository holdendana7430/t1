代发 wailian999

PHP:  number_format(1234567);
来源：http://hz.52xcode.cn/gtplxgxnev.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.iojbl.cn/gtlpaulvxk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.mhx1999.top/gtypnqagby.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.tianlin.xyz/gtlgqlpykd.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.sysykeji.top/gtclzfqcga.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.birdmap.top/gtxfzhjmvk.html

C#:   1234567.ToString("N0")
来源：http://hz.ydjk.org.cn/gtbetvsfwm.html

[E17] 首字母大写
来源：http://hz.sysykeji.top/gtwlttngkw.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.zhiwuduotai.top/gtizduncol.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.zhoulong.xyz/gtzepnsycl.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhengqikj.top/gtnyarfqou.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.iojbl.cn/gtyxburthk.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.zycfv.cn/gtymxaafdp.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.zhongyouzk.top/gtmfhzebfq.html

Ruby: s.capitalize
来源：http://hz.yanxiufei.cn/gtpdotokde.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.chenzaomai.com/gtcswaqexc.html

[E18] 模板占位符替换
来源：http://hz.tian-w.cn/gtebmktmce.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.yj20258.top/gtwlilzedh.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.wangdashe.top/gtxhwrbego.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.andypj.xyz/gtzegmxzsi.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.bjfxy.top/gtpymuogfa.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.gzhubu.top/gtrrjfpolb.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.meibo888.top/gtyqkholrw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.hywenlv.cn/gtotkiispy.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.zhongyouzk.top/gtnivoarzs.html

[E19] 多行文本按行拆分
来源：http://hz.wangshuangyany.cn/gttssjbldx.html

Py:   s.splitlines()
来源：http://hz.pengpengdd.cyou/gtqlgqhaml.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.chenjidiqi.icu/gtifvogyhy.html

JS:   s.split(/\r?\n/)
来源：http://hz.feifeiyinyue.top/gtnwibtwdy.html

TS:   s.split(/\r?\n/)
来源：http://hz.vqdsnc.cn/gtttfhyuih.html

Java: s.lines().toList()
来源：http://hz.snrcjt.cn/gtrsgvyiri.html

Go:   strings.Split(s, "\n")
来源：http://hz.jinqigufen.top/gtxzvnpxmm.html

Ruby: s.lines
来源：http://hz.wangdashe.top/gtjbcuktvh.html

C#:   s.Split('\n')
来源：http://hz.aibaodan.cn/gtwdtytxby.html

[E20] 判断字符串是否为空
来源：http://hz.xuetiantiany.cn/gteoypyagv.html

Py:   if not s:
来源：http://hz.cheryme.top/gtchtioiac.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.jqgfzy.top/gtvytnmkvb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.guowangkeji.top/gtmipndrmj.html

TS:   if (s === "") {}
来源：http://hz.ppjwa.cn/gthggpntrq.html

Java: if (s.isEmpty()) {}
来源：http://hz.guowangkeji.top/gtkoyqoggr.html

Go:   if s == "" {}
来源：http://hz.fzhhl.top/gtfbgmutcc.html

Ruby: if s.empty?
来源：http://hz.shangyingyoupin.top/gtvmtjhsfu.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.cqqwz.cn/gtbcqvrxcl.html

[E21] 超长截断加省略号
来源：http://hz.andypj.xyz/gtibsqodso.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.gotoacloud.top/gtwjfuovft.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.kuanghao11.cn/gtdxhbrxvq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jlsjyb.cn/gtvmxvrjmq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.nwbrower.top/gtlwqmsyoi.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.sweek.top/gtjrtdnmkw.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.ivvv.top/gtedvksprg.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.sxryk.cn/gttzetkmje.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.aizwys.cn/gtytjbdovs.html

[E22] 字节长度与字符长度
来源：http://hz.svipenyu.cn/gtpzoehwmp.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.cdnleiting.top/gtgqzqggee.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.pycfn.com/gtvdfmptue.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yangfankeji.com/gtklqmfpql.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.sxryk.cn/gtcdiszgnd.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.smart0.xyz/gtyxjdwnsp.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.zycfv.cn/gtmjspqypj.html

Ruby: s.bytesize;  s.length
来源：http://hz.iojbl.cn/gthblyysvc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.jinyuanbaomall.cn/gtknhuqntp.html

================================================================================
来源：http://hz.yj20258.top/gtwxdbpegm.html

F. 文件与目录
来源：http://hz.cqqwz.cn/gtzrjjvibd.html

================================================================================
来源：http://hz.nanxuanxn.top/gtqxylvcas.html

[F01] 读取整个文件
来源：http://hz.zdqjudy.top/gthbtcfsju.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.nanxinkj.top/gtaivrajhr.html

PHP:  file_get_contents("a.txt");
来源：http://hz.zdqjudy.top/gtuelqsdgz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.meibo888.top/gtbgxiuqep.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.316326.xyz/gtrudyeaot.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.dianchejie.cn/gtwhfzfvjo.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.guannengcc.top/gtubhakxkb.html

Ruby: File.read("a.txt")
来源：http://hz.fzhhl.top/gtjioqxxhp.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.dianchejie.cn/gtupctngmk.html

[F02] 逐行读取文件
来源：http://hz.haohaochexian.top/gtazcyvuej.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.gaohongyu789.top/gtiwfzopos.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.xylfe.cn/gtttxlyisv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.snrcjt.cn/gtyxzusyej.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xingfuxueyuan.xyz/gtuoducipw.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.yuanzhike.top/gtwoifwqkx.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.ehwqpu.com/gtyxboxwua.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yueranfly.top/gtgejllset.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.mhx1999.top/gtomftkpvo.html

[F03] 写入文件（覆盖）
来源：http://hz.c1oappe.top/gtgbkcdyoe.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.redwolf501.top/gtizuurxyq.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.xziqi.cn/gtkhhgskgv.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yuxming.cn/gtfdrtytsg.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ydzc1.top/gtcfzxcarx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.ivvv.top/gthjrmjoqj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.svipenyu.cn/gtqzsplxoz.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.ybcxt.top/gtdikyazko.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.sweek.top/gtowhpugil.html

[F04] 追加写入文件
来源：http://hz.kuanghao11.cn/gtphprtlmz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.sysykeji.top/gtyxusbjmx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.yangfankeji.com/gtzrycamtk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.nanxuanxn.top/gtcoybloly.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.svipenyu.cn/gttlddsczq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.shanyushiyangkeji.top/gtqqbegzyj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.vqdsnc.cn/gtavfhayys.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.sysykeji.top/gtjmgwhpqy.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.xinyue.icu/gtobxbjvdp.html

[F05] 判断文件或目录是否存在
来源：http://hz.ivvv.top/gtnxlukoqg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.aibaodan.cn/gtqfhkmcqw.html

PHP:  file_exists("a.txt");
来源：http://hz.dianchejie.cn/gtarfjnpcp.html

JS:   fs.existsSync("a.txt")
来源：http://hz.gaohongyu789.top/gtabrbvhek.html

TS:   fs.existsSync("a.txt")
来源：http://hz.hysaishi.cn/gttmoovuqn.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.andypj.xyz/gtiagqecmc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.wangdashe.top/gtqttjjwgv.html

Ruby: File.exist?("a.txt")
来源：http://hz.jinqigufen.top/gtzlknfbrb.html

C#:   File.Exists("a.txt")
来源：http://hz.sysykeji.top/gtpaugqzje.html

[F06] 删除文件
来源：http://hz.zhixingplan.top/gtbnxudghx.html

Py:   os.remove("a.txt")
来源：http://hz.ppjwa.cn/gtcjrjnqfc.html

PHP:  unlink("a.txt");
来源：http://hz.daria6918.cn/gtsqbhekkb.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.xziqi.cn/gtsijlbwxo.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.ybcxt.top/gtyrwhwais.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.zdqjudy.top/gtllychwjr.html

Go:   os.Remove("a.txt")
来源：http://hz.yj202588.top/gtnllnrsuv.html

Ruby: File.delete("a.txt")
来源：http://hz.ywan-chungtsiang.top/gtxbveyvlp.html

C#:   File.Delete("a.txt");
来源：http://hz.redwolf501.top/gthfqttimd.html

[F07] 创建目录（含多级）
来源：http://hz.aibaodan.cn/gtblmrfylj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.xuetiantiany.cn/gtvzfmrbic.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.sysykeji.top/gtpckkytio.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.shanyushiyangtech.top/gtnfnaqzou.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhongyouzk.top/gtccjasuva.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.shzxlz.cn/gtvbedwgus.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.quarkkingdee.top/gtvmprcoht.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.ywan-chungtsiang.top/gtencyowxl.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.xziqi.cn/gtrtlaeqyo.html

[F08] 遍历目录
来源：http://hz.jinqigfzy.top/gtqinwxsiy.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.shanyushiyangkeji.top/gtycaqgimq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.yuanzhike.top/gtmrydwgjo.html

JS:   fs.readdirSync("dir")
来源：http://hz.yj20258.top/gtxtvcpvfl.html

TS:   fs.readdirSync("dir")
来源：http://hz.hysaishi.cn/gtkepjmslg.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.fzhhl.top/gtzheklhbk.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.shanyushiyangkeji.top/gtlmpzxlcj.html

Ruby: Dir.children("dir")
来源：http://hz.9152youxi.cn/gtsbsrgyuu.html

C#:   Directory.GetFiles("dir")
来源：http://hz.gogol.net.cn/gtghzdvfmp.html

[F09] 获取文件大小
来源：http://hz.ehwqpu.com/gtzekgvyzt.html

Py:   os.path.getsize("a.txt")
来源：http://hz.guowangkeji.top/gttlrpryai.html

PHP:  filesize("a.txt");
来源：http://hz.snrcjt.cn/gtiydujqmi.html

JS:   fs.statSync("a.txt").size
来源：http://hz.yuxming.cn/gtnschwqrx.html

TS:   fs.statSync("a.txt").size
来源：http://hz.bjfxy.top/gtvaxpftui.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jyoumei.cn/gtzlbohgzd.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.cucudq.cn/gtavqtnhuo.html

Ruby: File.size("a.txt")
来源：http://hz.zycfv.cn/gtyusexvhq.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yuanzhike.top/gtktnxyggn.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.andypj.xyz/gtbtogrrxu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.zhengqikj.top/gtyigeiwzc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.dashuyun.cn/gtndcdijcy.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.9152youxi.cn/gtyyeyvewt.html

TS:   path.extname("a.txt")
来源：http://hz.jianghu66.top/gtbnwubtjh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.aibaodan.cn/gtsnkdvijx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.guowangkeji.top/gtpswphpkt.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.daria6918.cn/gtiivivofh.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.zhiwuduotai.top/gtjaynpzlw.html

[F11] 复制与移动文件
来源：http://hz.cqqwz.cn/gtdgxfqlyc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.cqqwz.cn/gtfdlhculi.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.zhongyouzk.top/gtpguwgxac.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.iojbl.cn/gtwjivfnly.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hfpthk.cn/gtncaucfzy.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.jinqigufen.top/gtrjhzghws.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.daria6918.cn/gtruuxmexr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.shuidangran.top/gtmrhddutt.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.chenlongwang.top/gtzjrefvjn.html

[F12] CSV 读写
来源：http://hz.yuanzhike.top/gtuunlvkoz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.shangyingyoupin.top/gtharwqkfa.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.yuanzhike.top/gtytkbuijn.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.pengpengdd.cyou/gtxtpiqhic.html

TS:   // 同上
来源：http://hz.chenzaomai.com/gtbmurmmpw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.xylfe.cn/gtmzckrbrl.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.nwbrower.top/gtidgqswyq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.vqdsnc.cn/gtozfcncxf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.zhaomingkeji.xyz/gtazpsdnzd.html

================================================================================
来源：http://hz.xinyue.icu/gtrkhkckwc.html

G. 面向对象
来源：http://hz.hongshengwenyu.top/gtfgxnpeee.html

================================================================================
来源：http://hz.yonumen.top/gtwxybtjaf.html

[G01] 定义类
来源：http://hz.yuanzhike.top/gtadkjeoto.html

Py:   class User: pass
来源：http://hz.aibaodan.cn/gtngwfgaho.html

PHP:  class User {}
来源：http://hz.ydzc1.top/gtrniqnyfp.html

JS:   class User {}
来源：http://hz.svipenyu.cn/gtpvwuqoub.html

TS:   class User { name: string = ""; }
来源：http://hz.vqdsnc.cn/gtquyiewma.html

Java: class User {}
来源：http://hz.cashguo.top/gtcehfgsii.html

Go:   type User struct { Name string }
来源：http://hz.fzhhl.top/gtrfvfozbs.html

Ruby: class User; end
来源：http://hz.haohaochexian.top/gtcghdstzx.html

C#:   class User {}
来源：http://hz.dianchejie.cn/gtpvcesfrb.html

[G02] 构造函数
来源：http://hz.xinyue.icu/gtshdjgsod.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yanxiufei.cn/gtwwskpvws.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yongpay.top/gteodbbzkn.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.hnxiangtu.top/gtjsvnscyt.html

TS:   constructor(public name: string) {}
来源：http://hz.nanxinkj.top/gtbcgrzosk.html

Java: User(String name) { this.name = name; }
来源：http://hz.pycfn.com/gtyafvxwdy.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.hongshengwenyu.top/gtecnwzdte.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.gogol.net.cn/gtlwuajgko.html

C#:   public User(string name) { Name = name; }
来源：http://hz.zycfv.cn/gthpvotxvk.html

[G03] 实例属性
来源：http://hz.hnxiangtu.top/gtscfrbsbr.html

Py:   self.name = "x"
来源：http://hz.jinyuanbaomall.cn/gtipdwjcsg.html

PHP:  public string $name = "x";
来源：http://hz.xylfe.cn/gtnpkwpqkx.html

JS:   this.name = "x";
来源：http://hz.feifeiyinyue.top/gtblmsuyxb.html

TS:   name: string = "x";
来源：http://hz.jinqigfzy.top/gtqviixkmf.html

Java: private String name;
来源：http://hz.nanxuanxn.top/gtndljmavs.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.shzxlz.cn/gtgiaauozb.html

Ruby: @name = "x"
来源：http://hz.jlsjyb.cn/gtnocymnmi.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.ywan-chungtsiang.top/gthrqxacbw.html

[G04] 定义方法
来源：http://hz.ywan-chungtsiang.top/gtiedgiyye.html

Py:   def greet(self): return self.name
来源：http://hz.havefunace.top/gtwhrcmzhl.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.cqqwz.cn/gtpcnwgbkm.html

JS:   greet() { return this.name; }
来源：http://hz.yj202588.top/gtegxwshru.html

TS:   greet(): string { return this.name; }
来源：http://hz.iojbl.cn/gtypduuddc.html

Java: String greet() { return name; }
来源：http://hz.aizwys.cn/gtuqammaaz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.guannengcc.top/gtijdazheg.html

Ruby: def greet; @name; end
来源：http://hz.redwolf501.top/gtohdxbnki.html

C#:   public string Greet() => Name;
来源：http://hz.gzhubu.top/gtncpswqmm.html

[G05] 继承
来源：http://hz.jianghu66.top/gtrufihgdk.html

Py:   class Admin(User): pass
来源：http://hz.tianlin.xyz/gtbnsnrolz.html

PHP:  class Admin extends User {}
来源：http://hz.9152youxi.cn/gtpxttcaeo.html

JS:   class Admin extends User {}
来源：http://hz.nanxinkj.top/gtrrkcvrjw.html

TS:   class Admin extends User {}
来源：http://hz.yvedp.cn/gthvhwmpgi.html

Java: class Admin extends User {}
来源：http://hz.shangyingyoupin.top/gtwuhmcjfd.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.shangyingyoupin.top/gtlsnyaxrx.html

Ruby: class Admin < User; end
来源：http://hz.yj20258.top/gtbtaswfvy.html

C#:   class Admin : User {}
来源：http://hz.jqgfzy.top/gtukxreovd.html

[G06] 重写方法
来源：http://hz.hammf.cn/gtagvhuajh.html

Py:   def greet(self): return "admin"
来源：http://hz.feifeiyinyue.top/gtxkaxiqrx.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.cucudq.cn/gtdhhteaeh.html

JS:   greet() { return "admin"; }
来源：http://hz.yueranfly.top/gtklvdirfo.html

TS:   greet(): string { return "admin"; }
来源：http://hz.nanxuanxn.top/gtsfactnln.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.guannengcc.top/gtbcbdcgir.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.tianlin.xyz/gtwzilzuzn.html

Ruby: def greet; "admin"; end
来源：http://hz.quarkkingdee.top/gtfbgclguy.html

C#:   public override string Greet() => "admin";
来源：http://hz.zhiwuduotai.top/gtytrjcrhb.html

[G07] 调用父类方法
来源：http://hz.yj20258888.top/gtxoztnuqe.html

Py:   super().greet()
来源：http://hz.ybcxt.top/gtmarpeesh.html

PHP:  parent::greet();
来源：http://hz.zhengqikj.top/gtuwjekebr.html

JS:   super.greet();
来源：http://hz.gaohongyu789.top/gtryogaffj.html

TS:   super.greet();
来源：http://hz.zhoulong.xyz/gtnsoinjjn.html

Java: super.greet();
来源：http://hz.jqgfzy.top/gtnwsrovjd.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jlsjyb.cn/gthtvoeghd.html

Ruby: super
来源：http://hz.ywan-chungtsiang.top/gtdplielue.html

C#:   base.Greet();
来源：http://hz.xylfe.cn/gtwjyzxqqh.html

[G08] 静态方法与属性
来源：http://hz.hammf.cn/gtrgrmqrvt.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jlsjyb.cn/gtvnqddlfh.html

PHP:  public static function f() {}
来源：http://hz.tianlin.xyz/gtxfvukqis.html

JS:   static f() {}
来源：http://hz.daria6918.cn/gtpbawpfmh.html

TS:   static f(): void {}
来源：http://hz.zycfv.cn/gthwtuteuu.html

Java: static void f() {}
来源：http://hz.hywenlv.cn/gtonxxtgci.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.chenzaomai.com/gtllxnpzwr.html

Ruby: def self.f; end
来源：http://hz.meibo888.top/gtgqevfxbv.html

C#:   public static void F() {}
来源：http://hz.chenjidiqi.icu/gtmyldufht.html

[G09] 接口 / 抽象类
来源：http://hz.yvedp.cn/gthblbmlvd.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.mhx1999.top/gtwponqucm.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jinqigufen.top/gthfotqmed.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.jinqigufen.top/gtsfepgzuc.html

TS:   interface Shape { area(): number; }
来源：http://hz.nwbrower.top/gttntuknhl.html

Java: interface Shape { double area(); }
来源：http://hz.yuanzhike.top/gtylygnshl.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.sweek.top/gtlwjidnnz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.52xcode.cn/gtxmtpwxaz.html

C#:   interface IShape { double Area(); }
来源：http://hz.smart0.xyz/gtpgzysnay.html

[G10] 访问控制
来源：http://hz.jinyuanbaomall.cn/gtsqslrljw.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.snrcjt.cn/gtkhyegdjv.html

PHP:  public / protected / private
来源：http://hz.zhaomingkeji.xyz/gtiktcitnj.html

JS:   #private 字段；其余公开
来源：http://hz.pycfn.com/gtvtifvugf.html

TS:   public / protected / private
来源：http://hz.52xcode.cn/gtllzorzun.html

Java: public / protected / private / 默认包级
来源：http://hz.zycfv.cn/gtzalwrgqg.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.ppjwa.cn/gtzrfbvsbi.html

Ruby: public / protected / private
来源：http://hz.snrcjt.cn/gtlcnzvtjt.html

C#:   public / protected / private / internal
来源：http://hz.sxryk.cn/gtibybfcry.html

[G11] getter / setter
来源：http://hz.ehwqpu.com/gtjkgeycmb.html

Py:   @property 与 @x.setter
来源：http://hz.hnxiangtu.top/gtbzainrvz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.kuanghao11.cn/gtejvlrydj.html

JS:   get name() { return this._name; }
来源：http://hz.redwolf501.top/gtvvtifmzn.html

TS:   get name(): string { return this._name; }
来源：http://hz.sysykeji.top/gtcdqtdreh.html

Java: public String getName() { return name; }
来源：http://hz.wangshuangyany.cn/gtyjnpcvpm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.iojbl.cn/gtljepdovy.html

Ruby: attr_accessor :name
来源：http://hz.jqgufenzy.top/gtvviqwprl.html

C#:   public string Name { get; set; }
来源：http://hz.tian-w.cn/gtziprdkry.html

[G12] 对象转字符串
来源：http://hz.meibo888.top/gtujxzirvy.html

Py:   def __str__(self): return self.name
来源：http://hz.quarkkingdee.top/gthljrinuk.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.mhx1999.top/gtimhxndap.html

JS:   toString() { return this.name; }
来源：http://hz.jinqigufen.top/gtgdigznhu.html

TS:   toString(): string { return this.name; }
来源：http://hz.kuanghao11.cn/gtgrlxfrpk.html

Java: @Override public String toString() { return name; }
来源：http://hz.nanxuanxn.top/gtdtotfdpt.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.gogol.net.cn/gthdpzrruu.html

Ruby: def to_s; @name; end
来源：http://hz.jinyuanbaomall.cn/gtoskfcaii.html

C#:   public override string ToString() => Name;
来源：http://hz.tanke756.top/gtjrbflasj.html

[G13] 判断对象类型
来源：http://hz.fengsongda.top/gtfqebrpiu.html

Py:   isinstance(u, User)
来源：http://hz.haohaochexian.top/gtjvvknpoh.html

PHP:  $u instanceof User
来源：http://hz.ehwqpu.com/gtwnjilzwi.html

JS:   u instanceof User
来源：http://hz.316326.xyz/gtsvyllqpe.html

TS:   u instanceof User
来源：http://hz.smart0.xyz/gtkfawsqjq.html

Java: u instanceof User
来源：http://hz.nwbrower.top/gtlkhjmfvl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.bjfxy.top/gtfktrzovo.html

Ruby: u.is_a?(User)
来源：http://hz.mhx1999.top/gtcslwqycn.html

C#:   u is User
来源：http://hz.ehwqpu.com/gtelodafgx.html

[G14] 数据类 / record
来源：http://hz.chenzaomai.com/gteyjciist.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.jyoumei.cn/gtftdlipes.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.sxryk.cn/gtkkioilgw.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yueranfly.top/gtmtvaybec.html

TS:   type User = { name: string; age: number };
来源：http://hz.gotoacloud.top/gtdpvysqwb.html

Java: record User(String name, int age) {}
来源：http://hz.ivvv.top/gtdxvgdptk.html

Go:   type User struct { Name string; Age int }
来源：http://hz.mhx1999.top/gtissthyet.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.cheryme.top/gtcakhiqlo.html


<!-- 参考信息 -->