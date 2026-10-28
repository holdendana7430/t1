代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.zdqjudy.top/gtpzlijeui.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.dianchejie.cn/gtaqstaxwa.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.xylfe.cn/gthamluuxk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.shuidangran.top/gtmjeokvkx.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.jqgfzy.top/gtahkdvuau.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.zhongyouzk.top/gtqtuntrem.html

Ruby: s.capitalize
来源：http://hz.nanxinkj.top/gtsfrcsyyd.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yanxiufei.cn/gtbdhcglfi.html

[E18] 模板占位符替换
来源：http://hz.aizwys.cn/gtxitcvqat.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.52xcode.cn/gtadbuater.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.nwbrower.top/gtwqlnblxk.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.xingfuxueyuan.xyz/gthwsmrfub.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.c1oappe.top/gtkivgvnke.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.jyoumei.cn/gttteyiggr.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.yuxming.cn/gtgrqvrjhf.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.sufxvd.cn/gtjydzdxzl.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.hfpthk.cn/gtukjnjudl.html

[E19] 多行文本按行拆分
来源：http://hz.ydzc1.top/gtfuiviywc.html

Py:   s.splitlines()
来源：http://hz.havefunace.top/gtjugejtvi.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.daxiang520.top/gtfarzmiva.html

JS:   s.split(/\r?\n/)
来源：http://hz.316326.xyz/gtbsnrhrkx.html

TS:   s.split(/\r?\n/)
来源：http://hz.jiagoushi.top/gtzyyjhuxv.html

Java: s.lines().toList()
来源：http://hz.c1oappe.top/gtbbplsbvf.html

Go:   strings.Split(s, "\n")
来源：http://hz.gotoacloud.top/gtmdlyqjnb.html

Ruby: s.lines
来源：http://hz.sysykeji.top/gtfimtgmti.html

C#:   s.Split('\n')
来源：http://hz.wangshuangyany.cn/gtzayruynq.html

[E20] 判断字符串是否为空
来源：http://hz.jqgufenzy.top/gtgkhviegv.html

Py:   if not s:
来源：http://hz.nanxinkj.top/gtcamcplub.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.yanxiufei.cn/gtafrqowid.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.shanyushiyangkeji.top/gtrqivxinp.html

TS:   if (s === "") {}
来源：http://hz.shzxlz.cn/gtrfckznxa.html

Java: if (s.isEmpty()) {}
来源：http://hz.0kj1m.cn/gtsbcdrvgr.html

Go:   if s == "" {}
来源：http://hz.iojbl.cn/gtjbtnxeaa.html

Ruby: if s.empty?
来源：http://hz.sxryk.cn/gtyjmsphom.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.xinyue.icu/gtvxipuoqp.html

[E21] 超长截断加省略号
来源：http://hz.hywenlv.cn/gtbnulgjhk.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.zhongyouzk.top/gtmgetdokv.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.sweek.top/gtozgycacp.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.xuetiantiany.cn/gthiinopzc.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.mhx1999.top/gtllmpsulj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yonumen.top/gtfybmkpjt.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.yj20258.top/gtjciiejqn.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.cheryme.top/gtsclgarfz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.jiagoushi.top/gtyflerfnm.html

[E22] 字节长度与字符长度
来源：http://hz.dianchejie.cn/gtptjpjmrn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.ivvv.top/gtvdbgfyop.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhiwuduotai.top/gtuaijmxkp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yonumen.top/gtlcadzduz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.nwbrower.top/gtotxonear.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.yonumen.top/gtmnwypzwd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.ydzc1.top/gteainvzsp.html

Ruby: s.bytesize;  s.length
来源：http://hz.zdqjudy.top/gtwxqqnvfz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.hysaishi.cn/gtxwvtjdpy.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtlpnqrabg.html

F. 文件与目录
来源：http://hz.ywan-chungtsiang.top/gtctrwbwui.html

================================================================================
来源：http://hz.gotoacloud.top/gtdmgmwfux.html

[F01] 读取整个文件
来源：http://hz.aibaodan.cn/gtuzsgvvof.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.jinghuilouyu.cn/gtljoognwd.html

PHP:  file_get_contents("a.txt");
来源：http://hz.nanxinkj.top/gtkvwkbllp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.ybcxt.top/gtbgdldzdc.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.c1oappe.top/gtoprywsod.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.jinyuanbaomall.cn/gtqqzgqygj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.iojbl.cn/gtdlzplpas.html

Ruby: File.read("a.txt")
来源：http://hz.sxryk.cn/gtnzhupfpk.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.jyoumei.cn/gtcoqsjpgc.html

[F02] 逐行读取文件
来源：http://hz.hysaishi.cn/gtgijnykaj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.sxryk.cn/gtcosbhinq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.pycfn.com/gtnnzsvipg.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.haohaochexian.top/gtjnrbtuwm.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.sysykeji.top/gtgfpjctpo.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.guannengcc.top/gtougtdnkm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.yanxiufei.cn/gtkqlqxpft.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.zdqjudy.top/gtsrworqfl.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.zhiwuduotai.top/gtffypzmah.html

[F03] 写入文件（覆盖）
来源：http://hz.ydjk.org.cn/gtfvfmrvhj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.yuxming.cn/gttxkiqbhc.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.jinyuanbaomall.cn/gtxoipfvki.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yongpay.top/gtlthpulbb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.xuanzx.com/gtxdrbbwzw.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.guannengcc.top/gtgauuirtr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.yj202588.top/gteoefbteb.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.guowangkeji.top/gtarxhwtsb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.hammf.cn/gtgeiyzpay.html

[F04] 追加写入文件
来源：http://hz.redwolf501.top/gthzjqpcvw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.fzhhl.top/gtjpgodwdz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.fengsongda.top/gtoaheigrl.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yvedp.cn/gtqkveuspy.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.cheryme.top/gtwoocycro.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.9152youxi.cn/gtdvltwwff.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.zhengqikj.top/gtcwqyzoyh.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.havefunace.top/gtnsfulnnf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.yueranfly.top/gtfhbwdpvu.html

[F05] 判断文件或目录是否存在
来源：http://hz.xingfuxueyuan.xyz/gtobjwmcmr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.yuxming.cn/gtekwxvwue.html

PHP:  file_exists("a.txt");
来源：http://hz.0kj1m.cn/gtsrxfzynp.html

JS:   fs.existsSync("a.txt")
来源：http://hz.shanyushiyangkeji.top/gtnszitwbh.html

TS:   fs.existsSync("a.txt")
来源：http://hz.dianchejie.cn/gtwthalowf.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.hywenlv.cn/gthnaowfen.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.vqdsnc.cn/gtuhjakjgp.html

Ruby: File.exist?("a.txt")
来源：http://hz.sweek.top/gtonkdgxge.html

C#:   File.Exists("a.txt")
来源：http://hz.fengsongda.top/gtoxzpimxh.html

[F06] 删除文件
来源：http://hz.xingfuxueyuan.xyz/gtpksdyikg.html

Py:   os.remove("a.txt")
来源：http://hz.xuetiantiany.cn/gtrlnqyjzv.html

PHP:  unlink("a.txt");
来源：http://hz.hfpthk.cn/gtfqmtxojb.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.hongshengwenyu.top/gtatengpir.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.andypj.xyz/gtyjaxcbjm.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.chenlongwang.top/gtuofsgkng.html

Go:   os.Remove("a.txt")
来源：http://hz.jinqigfzy.top/gtyjloglki.html

Ruby: File.delete("a.txt")
来源：http://hz.shanyushiyangtech.top/gtdnwvtyvx.html

C#:   File.Delete("a.txt");
来源：http://hz.gaohongyu789.top/gtkdsbwjva.html

[F07] 创建目录（含多级）
来源：http://hz.shuidangran.top/gtwbtpgtde.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.tianlin.xyz/gtbfwfhodu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.chenzaomai.com/gttvdlxucf.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jinqigfzy.top/gtgtuhwmlp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.fengsongda.top/gtnofgxraa.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.yj20258888.top/gtclbpopcd.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jqgfzy.top/gtpyvkwpcm.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.chenlongwang.top/gtkrtchsdw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.gotoacloud.top/gtowvvekwc.html

[F08] 遍历目录
来源：http://hz.yj20258.top/gtmswwxscj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.chenjidiqi.icu/gttgldmokm.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.bjfxy.top/gtiplawiby.html

JS:   fs.readdirSync("dir")
来源：http://hz.chenlongwang.top/gtzotwavmu.html

TS:   fs.readdirSync("dir")
来源：http://hz.chenzaomai.com/gtukvmsndb.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.gzhubu.top/gtkmhmrlik.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.pycfn.com/gtlkaprgzf.html

Ruby: Dir.children("dir")
来源：http://hz.hnqzz.top/gtkzgysske.html

C#:   Directory.GetFiles("dir")
来源：http://hz.wangdashe.top/gttxjntatu.html

[F09] 获取文件大小
来源：http://hz.haohaochexian.top/gtehfpgtwq.html

Py:   os.path.getsize("a.txt")
来源：http://hz.9152youxi.cn/gtqvhqmlzi.html

PHP:  filesize("a.txt");
来源：http://hz.zhoulong.xyz/gtacerlejl.html

JS:   fs.statSync("a.txt").size
来源：http://hz.shangyingyoupin.top/gtqgxbwcgp.html

TS:   fs.statSync("a.txt").size
来源：http://hz.ydjk.org.cn/gtoorelonj.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jqgufenzy.top/gtnbkdsqsa.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.zhijiandao.cn/gtiwbtvynt.html

Ruby: File.size("a.txt")
来源：http://hz.xuanzx.com/gtadvuwsos.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.dashuyun.cn/gtbbdzqjwb.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.hammf.cn/gthiinkbyn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.hysaishi.cn/gtmjldbupu.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.xylfe.cn/gtvqconzqd.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.cashguo.top/gtwginwpux.html

TS:   path.extname("a.txt")
来源：http://hz.sufxvd.cn/gtmdfdjktc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.sweek.top/gtfsitimvk.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.hongshengwenyu.top/gtmyovegtc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.zhiwuduotai.top/gtumyfimgt.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.wangdashe.top/gtmoesajlf.html

[F11] 复制与移动文件
来源：http://hz.zhixingplan.top/gteprvciad.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.jlsjyb.cn/gtpqyewrlk.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.smart0.xyz/gtkkijrllo.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.quarkkingdee.top/gtqtnrtyoo.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.kuanghao11.cn/gttwtvonlp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.gzhubu.top/gtypizcktd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.meibo888.top/gtzqzpdepn.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.yvedp.cn/gtsouvtqzn.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.zhiwuduotai.top/gtibjkwwym.html

[F12] CSV 读写
来源：http://hz.chenlongwang.top/gtndwlenas.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.bjfxy.top/gtraxdslvu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.aizwys.cn/gtikhnblce.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.hammf.cn/gtnlrzihxo.html

TS:   // 同上
来源：http://hz.bjfxy.top/gthredrzxq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.hnxiangtu.top/gtstenzxen.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.cheryme.top/gtrmjpwelv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.cheryme.top/gtnvcbyakv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yvedp.cn/gtcjapftdr.html

================================================================================
来源：http://hz.dashuyun.cn/gtnbanoybp.html

G. 面向对象
来源：http://hz.fzhhl.top/gttqbekaoj.html

================================================================================
来源：http://hz.hnqzz.top/gtfufpknwi.html

[G01] 定义类
来源：http://hz.chenjidiqi.icu/gtrahqkzaf.html

Py:   class User: pass
来源：http://hz.vqdsnc.cn/gtzbduxiic.html

PHP:  class User {}
来源：http://hz.xingfuxueyuan.xyz/gtdzpjzumn.html

JS:   class User {}
来源：http://hz.sxryk.cn/gtmoskmtbt.html

TS:   class User { name: string = ""; }
来源：http://hz.ybcxt.top/gtpmkhmfee.html

Java: class User {}
来源：http://hz.yuxming.cn/gtcmaiumlw.html

Go:   type User struct { Name string }
来源：http://hz.zhixingplan.top/gtorvcdtcc.html

Ruby: class User; end
来源：http://hz.meibo888.top/gtombyetjd.html

C#:   class User {}
来源：http://hz.yangfankeji.com/gtydwzledo.html

[G02] 构造函数
来源：http://hz.zdqjudy.top/gtgprcavgk.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.nanxuanxn.top/gtmyjelgan.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.vqdsnc.cn/gtpwkixrkw.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.guannengcc.top/gtbzycwaei.html

TS:   constructor(public name: string) {}
来源：http://hz.zhiwuduotai.top/gteiteuqkn.html

Java: User(String name) { this.name = name; }
来源：http://hz.cqqwz.cn/gtarleykbt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jinghuilouyu.cn/gtaizqfjhj.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.jinghuilouyu.cn/gtdvhswvdy.html

C#:   public User(string name) { Name = name; }
来源：http://hz.daria6918.cn/gtgstuovdl.html

[G03] 实例属性
来源：http://hz.yongpay.top/gtxuqybsov.html

Py:   self.name = "x"
来源：http://hz.hammf.cn/gtxvofyxgn.html

PHP:  public string $name = "x";
来源：http://hz.zhengqikj.top/gtgyfokbow.html

JS:   this.name = "x";
来源：http://hz.xingfuxueyuan.xyz/gtsgqgbojz.html

TS:   name: string = "x";
来源：http://hz.zdqjudy.top/gtpiqtsmbn.html

Java: private String name;
来源：http://hz.xziqi.cn/gtdxmqjhod.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.xylfe.cn/gtmykfhijh.html

Ruby: @name = "x"
来源：http://hz.jianghu66.top/gtqficyinx.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yangfankeji.com/gtqbssauzg.html

[G04] 定义方法
来源：http://hz.jinyuanbaomall.cn/gtwgrjqhdc.html

Py:   def greet(self): return self.name
来源：http://hz.gogol.net.cn/gtomlkhanz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.smart0.xyz/gtdqtphrfi.html

JS:   greet() { return this.name; }
来源：http://hz.shanyushiyangkeji.top/gtwvnhqxqm.html

TS:   greet(): string { return this.name; }
来源：http://hz.pycfn.com/gtsqbjxgbb.html

Java: String greet() { return name; }
来源：http://hz.iojbl.cn/gtyfzskfou.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.ppjwa.cn/gtcdenosbd.html

Ruby: def greet; @name; end
来源：http://hz.ywan-chungtsiang.top/gtfjzbkjgj.html

C#:   public string Greet() => Name;
来源：http://hz.smart0.xyz/gtntxpnwzn.html

[G05] 继承
来源：http://hz.jinghuilouyu.cn/gtvftlpokh.html

Py:   class Admin(User): pass
来源：http://hz.jianghu66.top/gthvllukbt.html

PHP:  class Admin extends User {}
来源：http://hz.yj20258888.top/gtrybikiot.html

JS:   class Admin extends User {}
来源：http://hz.yonumen.top/gtamrfdagp.html

TS:   class Admin extends User {}
来源：http://hz.ydjk.org.cn/gtvtsjtgqc.html

Java: class Admin extends User {}
来源：http://hz.tianlin.xyz/gtghxfcifq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yj20258888.top/gthgibuvod.html

Ruby: class Admin < User; end
来源：http://hz.sufxvd.cn/gtlifprldq.html

C#:   class Admin : User {}
来源：http://hz.chenjidiqi.icu/gthkvnpdhw.html

[G06] 重写方法
来源：http://hz.hfpthk.cn/gtarcbcmvy.html

Py:   def greet(self): return "admin"
来源：http://hz.daria6918.cn/gthtyoygyw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.yangfankeji.com/gthizwacgn.html

JS:   greet() { return "admin"; }
来源：http://hz.aizwys.cn/gtnoyhaybb.html

TS:   greet(): string { return "admin"; }
来源：http://hz.yuanzhike.top/gtnjprndhh.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jiagoushi.top/gtmcifconb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.aibaodan.cn/gttsicyjzh.html

Ruby: def greet; "admin"; end
来源：http://hz.ivvv.top/gtpdecbsea.html

C#:   public override string Greet() => "admin";
来源：http://hz.guannengcc.top/gtfdnmghdf.html

[G07] 调用父类方法
来源：http://hz.pycfn.com/gtnmsptkkl.html

Py:   super().greet()
来源：http://hz.yanxiufei.cn/gtdoullxit.html

PHP:  parent::greet();
来源：http://hz.zhongyouzk.top/gtywbfrbqa.html

JS:   super.greet();
来源：http://hz.hnqzz.top/gtxemgvntc.html

TS:   super.greet();
来源：http://hz.tanke756.top/gtfqalqftd.html

Java: super.greet();
来源：http://hz.yanxiufei.cn/gtwpnezbaw.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.aizwys.cn/gtfmwtrnzl.html

Ruby: super
来源：http://hz.fengsongda.top/gtahavmiui.html

C#:   base.Greet();
来源：http://hz.fengsongda.top/gtfsuykwyt.html

[G08] 静态方法与属性
来源：http://hz.yj202588.top/gtamcjpabe.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.birdmap.top/gtmpdyoiyp.html

PHP:  public static function f() {}
来源：http://hz.mhx1999.top/gtllmgkehe.html

JS:   static f() {}
来源：http://hz.haohaochexian.top/gtrlbafceh.html

TS:   static f(): void {}
来源：http://hz.haohaochexian.top/gtcottvghw.html

Java: static void f() {}
来源：http://hz.zhengqikj.top/gtumilyelb.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.guowangkeji.top/gtiqsjvcsz.html

Ruby: def self.f; end
来源：http://hz.52xcode.cn/gtjvtycoad.html

C#:   public static void F() {}
来源：http://hz.yueranfly.top/gtjotiafgl.html

[G09] 接口 / 抽象类
来源：http://hz.redwolf501.top/gtnyhsvalz.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.hysaishi.cn/gtqkefodun.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yj202588.top/gtpseqrzvw.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.andypj.xyz/gtutusduvc.html

TS:   interface Shape { area(): number; }
来源：http://hz.jinqigfzy.top/gthxhpfkvl.html

Java: interface Shape { double area(); }
来源：http://hz.chenzaomai.com/gtuffcjnpi.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.hnqzz.top/gtpqklztnm.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.redwolf501.top/gtdrarcilb.html

C#:   interface IShape { double Area(); }
来源：http://hz.xziqi.cn/gtapgpjtwe.html

[G10] 访问控制
来源：http://hz.ivvv.top/gthaamlngu.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.dashuyun.cn/gtvxuczrsy.html

PHP:  public / protected / private
来源：http://hz.yanxiufei.cn/gtrddgryno.html

JS:   #private 字段；其余公开
来源：http://hz.xinyue.icu/gtofethfao.html

TS:   public / protected / private
来源：http://hz.cucudq.cn/gtcidwrcdb.html

Java: public / protected / private / 默认包级
来源：http://hz.zhengqikj.top/gtbbwkupml.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.jinqigfzy.top/gtplqagyan.html

Ruby: public / protected / private
来源：http://hz.wangshuangyany.cn/gtnyiuvofv.html

C#:   public / protected / private / internal
来源：http://hz.jqgfzy.top/gtpayjcbcz.html

[G11] getter / setter
来源：http://hz.snrcjt.cn/gtlttsaimo.html

Py:   @property 与 @x.setter
来源：http://hz.xinyue.icu/gtlkqbhbmt.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.shangyingyoupin.top/gthnxzousi.html

JS:   get name() { return this._name; }
来源：http://hz.wangshuangyany.cn/gtpbwccdjp.html

TS:   get name(): string { return this._name; }
来源：http://hz.zhoulong.xyz/gtzkzwpstb.html

Java: public String getName() { return name; }
来源：http://hz.c1oappe.top/gtiyzfbvxg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.andypj.xyz/gtjcfyjqqm.html

Ruby: attr_accessor :name
来源：http://hz.hammf.cn/gtbpqomhor.html

C#:   public string Name { get; set; }
来源：http://hz.pengpengdd.cyou/gtthkizzxm.html

[G12] 对象转字符串
来源：http://hz.gotoacloud.top/gtmiabxxji.html

Py:   def __str__(self): return self.name
来源：http://hz.yj20258.top/gtrtcvwtyb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.hongshengwenyu.top/gtwzosdeho.html

JS:   toString() { return this.name; }
来源：http://hz.wangshuangyany.cn/gtyrppcftk.html

TS:   toString(): string { return this.name; }
来源：http://hz.yonumen.top/gtycuuyizp.html

Java: @Override public String toString() { return name; }
来源：http://hz.meibo888.top/gtaqywelyt.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.ppjwa.cn/gtkrrafucc.html

Ruby: def to_s; @name; end
来源：http://hz.shangyingyoupin.top/gtgytupbzy.html

C#:   public override string ToString() => Name;
来源：http://hz.zhengqikj.top/gtpxohuwki.html

[G13] 判断对象类型
来源：http://hz.gogol.net.cn/gtdggubwnt.html

Py:   isinstance(u, User)
来源：http://hz.cheryme.top/gtbtmfvtsz.html

PHP:  $u instanceof User
来源：http://hz.xziqi.cn/gtkfuwdtao.html

JS:   u instanceof User
来源：http://hz.aizwys.cn/gtpbgjubfu.html

TS:   u instanceof User
来源：http://hz.haohaochexian.top/gthwkeaavb.html

Java: u instanceof User
来源：http://hz.shangyingyoupin.top/gtsjaixcrl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.zycfv.cn/gthomhmdte.html

Ruby: u.is_a?(User)
来源：http://hz.wangshuangyany.cn/gthnymysku.html

C#:   u is User
来源：http://hz.kuanghao11.cn/gticawxiym.html

[G14] 数据类 / record
来源：http://hz.sysykeji.top/gtehogwrop.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.havefunace.top/gttubtnkly.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.snrcjt.cn/gtecgupeec.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.xingfuxueyuan.xyz/gtnjoyxagb.html

TS:   type User = { name: string; age: number };
来源：http://hz.smart0.xyz/gtqinlmywi.html

Java: record User(String name, int age) {}
来源：http://hz.cdnleiting.top/gtnvucidqc.html

Go:   type User struct { Name string; Age int }
来源：http://hz.tian-w.cn/gtuuikxjip.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.gzhubu.top/gtdqodfhvm.html

C#:   record User(string Name, int Age);
来源：http://hz.ywan-chungtsiang.top/gtcvoucutv.html

[G15] 枚举
来源：http://hz.jinghuilouyu.cn/gtrvamngeq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.guannengcc.top/gtrfelspfv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.nanxuanxn.top/gtjchwxnrt.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.shangyingyoupin.top/gtumqswhwz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.guannengcc.top/gtyaucukmz.html

Java: enum Color { RED, GREEN }
来源：http://hz.xuanzx.com/gtghvjyina.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.shanyushiyangtech.top/gteoqamjqb.html


<!-- 参考信息 -->