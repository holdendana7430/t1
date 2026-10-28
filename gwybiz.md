代发 wailian999

[E18] 模板占位符替换
来源：http://hz.sufxvd.cn/gtdshuyobk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.zhixingplan.top/gttlgclntt.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.zhengqikj.top/gtmmhodate.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.0kj1m.cn/gtslmjfsct.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.aizwys.cn/gtllonlmla.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.yangfankeji.com/gtotmntayu.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.hfpthk.cn/gtshrgjktf.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.zhixingplan.top/gtgxljbxds.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.shzxlz.cn/gtqmjgspkn.html

[E19] 多行文本按行拆分
来源：http://hz.52xcode.cn/gtxroigoku.html

Py:   s.splitlines()
来源：http://hz.316326.xyz/gtrajxdtiu.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.daria6918.cn/gtmjecdlmt.html

JS:   s.split(/\r?\n/)
来源：http://hz.hnqzz.top/gtkrpakjqn.html

TS:   s.split(/\r?\n/)
来源：http://hz.tian-w.cn/gtxuajsjtq.html

Java: s.lines().toList()
来源：http://hz.ydjk.org.cn/gtyvwwqzvz.html

Go:   strings.Split(s, "\n")
来源：http://hz.jqgfzy.top/gtfzoxwwth.html

Ruby: s.lines
来源：http://hz.yj202588.top/gtmslbzqbb.html

C#:   s.Split('\n')
来源：http://hz.zhixingplan.top/gtqmkfzalg.html

[E20] 判断字符串是否为空
来源：http://hz.ehwqpu.com/gtvrnmbwup.html

Py:   if not s:
来源：http://hz.fengsongda.top/gtlctrxdvn.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.havefunace.top/gtzbrodvqn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.kuanghao11.cn/gthzmshlbq.html

TS:   if (s === "") {}
来源：http://hz.hywenlv.cn/gtpjbekgfq.html

Java: if (s.isEmpty()) {}
来源：http://hz.52xcode.cn/gtcyudheto.html

Go:   if s == "" {}
来源：http://hz.shzxlz.cn/gtmbhspaxa.html

Ruby: if s.empty?
来源：http://hz.dianchejie.cn/gtexmpgiba.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.jyoumei.cn/gtbtesdrmd.html

[E21] 超长截断加省略号
来源：http://hz.jqgfzy.top/gtryfszory.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.zhengqikj.top/gtkvsiuvly.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.zhaomingkeji.xyz/gtlmcbvemx.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.xuetiantiany.cn/gtwiycdtlc.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.xuanzx.com/gtvqpdbwsi.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.birdmap.top/gtuxcfpmma.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.dianchejie.cn/gtumcpqzgc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.zhijiandao.cn/gtnnzucpxv.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.zhoulong.xyz/gtactkfpkz.html

[E22] 字节长度与字符长度
来源：http://hz.tian-w.cn/gtpkjybvdn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.svipenyu.cn/gtdjrqnkrd.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jqgufenzy.top/gtkfsfspcv.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.guowangkeji.top/gtywlxyehd.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jiagoushi.top/gtsjrnnyol.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.tian-w.cn/gtfmjveehi.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.shanyushiyangtech.top/gtrspguhxq.html

Ruby: s.bytesize;  s.length
来源：http://hz.nanxuanxn.top/gtxrgcpxvd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.redwolf501.top/gtwvnyczhx.html

================================================================================
来源：http://hz.yueranfly.top/gtmetynlqk.html

F. 文件与目录
来源：http://hz.smart0.xyz/gtqxrksarz.html

================================================================================
来源：http://hz.zhoulong.xyz/gtfihwhddn.html

[F01] 读取整个文件
来源：http://hz.shzxlz.cn/gtrxhsigqo.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.xylfe.cn/gtxpdrxfpw.html

PHP:  file_get_contents("a.txt");
来源：http://hz.bjfxy.top/gtdgeeycqo.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.ydzc1.top/gtotcfynxr.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.gaohongyu789.top/gtcgdhmotq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.zycfv.cn/gthqhbauer.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.yangfankeji.com/gtkefuuins.html

Ruby: File.read("a.txt")
来源：http://hz.nwbrower.top/gtkinbkmnu.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.gotoacloud.top/gtbekiaqgk.html

[F02] 逐行读取文件
来源：http://hz.iojbl.cn/gtujiuqnfw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.fzhhl.top/gtnhigayxe.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.jinyuanbaomall.cn/gtvnsgwiqn.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.chenjidiqi.icu/gtfbudsyif.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xinyue.icu/gtmewdwlga.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.gogol.net.cn/gthyyhjiok.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.hnqzz.top/gtyxpjspzv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.xylfe.cn/gtzyeqmqdr.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.wangdashe.top/gtqjpwiyov.html

[F03] 写入文件（覆盖）
来源：http://hz.cheryme.top/gtbfuzrjhi.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.zhijiandao.cn/gtctxjttda.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.tanke756.top/gtbihqkzrd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.fengsongda.top/gtnopeeaqf.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.wangshuangyany.cn/gtcqugkcqx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.havefunace.top/gtjciljrbh.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.jqgufenzy.top/gtlrzpsfwy.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.shangyingyoupin.top/gtjmdhusgp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.yueranfly.top/gtvsmvkcax.html

[F04] 追加写入文件
来源：http://hz.bjfxy.top/gtnrteygjn.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.zycfv.cn/gtqmirjxkq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.hammf.cn/gtgqwcstud.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.gaohongyu789.top/gtezomtwak.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.andypj.xyz/gtygsxuqfj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.jinyuanbaomall.cn/gtieqzjvno.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.daxiang520.top/gtwurvxpnt.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.gotoacloud.top/gtcipznijg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.sufxvd.cn/gttswzupau.html

[F05] 判断文件或目录是否存在
来源：http://hz.c1oappe.top/gtxltzwfpl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.aibaodan.cn/gtfyksjwpz.html

PHP:  file_exists("a.txt");
来源：http://hz.jiagoushi.top/gtdenpliny.html

JS:   fs.existsSync("a.txt")
来源：http://hz.cashguo.top/gtgbtymlyc.html

TS:   fs.existsSync("a.txt")
来源：http://hz.nwbrower.top/gttcuctbdd.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.zhiwuduotai.top/gteqwdnlmz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.mhx1999.top/gtnfvjhudq.html

Ruby: File.exist?("a.txt")
来源：http://hz.iojbl.cn/gtxxthqjeu.html

C#:   File.Exists("a.txt")
来源：http://hz.xziqi.cn/gtkujxtepw.html

[F06] 删除文件
来源：http://hz.kuanghao11.cn/gtmszvkgmq.html

Py:   os.remove("a.txt")
来源：http://hz.kuanghao11.cn/gtcyicpyjl.html

PHP:  unlink("a.txt");
来源：http://hz.xziqi.cn/gtwjyomvat.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.mhx1999.top/gtbcizlnht.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.hywenlv.cn/gtmdlizgps.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.yuxming.cn/gtveyjxfol.html

Go:   os.Remove("a.txt")
来源：http://hz.gzhubu.top/gttumxxzom.html

Ruby: File.delete("a.txt")
来源：http://hz.xuanzx.com/gtcwnemjqc.html

C#:   File.Delete("a.txt");
来源：http://hz.ydjk.org.cn/gthahclzel.html

[F07] 创建目录（含多级）
来源：http://hz.mhx1999.top/gthgrkplfu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yuxming.cn/gtxlsrzrun.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.shzxlz.cn/gtlvekwjka.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.chenlongwang.top/gtvbxlkjxo.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.wangdashe.top/gthzhbzxfy.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.sufxvd.cn/gtltmrzwpw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.fengsongda.top/gtqqvrfctk.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.zhaomingkeji.xyz/gthvzwkfgf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.ybcxt.top/gtoqwndxnl.html

[F08] 遍历目录
来源：http://hz.jinyuanbaomall.cn/gtaizpymuj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.nwbrower.top/gtjeesfpcs.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.ydjk.org.cn/gtcpdojqlw.html

JS:   fs.readdirSync("dir")
来源：http://hz.yanxiufei.cn/gtyjsexvfu.html

TS:   fs.readdirSync("dir")
来源：http://hz.yj20258888.top/gtyjawnuhq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.ehwqpu.com/gtovmcvojo.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.jqgufenzy.top/gtjjsboecs.html

Ruby: Dir.children("dir")
来源：http://hz.zhengqikj.top/gtvdlqblej.html

C#:   Directory.GetFiles("dir")
来源：http://hz.svipenyu.cn/gtotphogpm.html

[F09] 获取文件大小
来源：http://hz.hywenlv.cn/gtnxyninnu.html

Py:   os.path.getsize("a.txt")
来源：http://hz.cdnleiting.top/gtuwozfyku.html

PHP:  filesize("a.txt");
来源：http://hz.gogol.net.cn/gtivfrdule.html

JS:   fs.statSync("a.txt").size
来源：http://hz.andypj.xyz/gtjzfxfuhu.html

TS:   fs.statSync("a.txt").size
来源：http://hz.hfpthk.cn/gtaedftpas.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jyoumei.cn/gtlwnbrkzk.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.dashuyun.cn/gtxhblpwni.html

Ruby: File.size("a.txt")
来源：http://hz.yj20258.top/gtkpbbcskz.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.shuidangran.top/gtcraqukcf.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.cashguo.top/gtvqhoiqgc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.shangyingyoupin.top/gtkqhpggpy.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.jyoumei.cn/gtrvhlbshx.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.yuxming.cn/gtlktqkyio.html

TS:   path.extname("a.txt")
来源：http://hz.ydjk.org.cn/gtiekyxzij.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.wangshuangyany.cn/gtwmpppwqu.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.meibo888.top/gtfdqmqjmn.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.sysykeji.top/gtnvlltxjs.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.ydjk.org.cn/gtpstduzrx.html

[F11] 复制与移动文件
来源：http://hz.0kj1m.cn/gthjmhejcy.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.chenlongwang.top/gtajzuqksp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.chenjidiqi.icu/gtcdfwzkgr.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ydjk.org.cn/gtekapxgjb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.shuidangran.top/gtkscwtpsj.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.52xcode.cn/gthyqkoqwk.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yj20258888.top/gtvlgvkebu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.daria6918.cn/gtldvyoihh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.ivvv.top/gtqgtegotz.html

[F12] CSV 读写
来源：http://hz.svipenyu.cn/gtuaalxrmw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.zhoulong.xyz/gthixkrteb.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.tianlin.xyz/gtguuboulb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.guannengcc.top/gtjggpuoxw.html

TS:   // 同上
来源：http://hz.gzhubu.top/gtjsusvnqb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.yueranfly.top/gttdfsgbrg.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yj20258.top/gtbzwdghqi.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.sufxvd.cn/gtewbimryt.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.aizwys.cn/gteriaxvgm.html

================================================================================
来源：http://hz.xziqi.cn/gttnvgxnap.html

G. 面向对象
来源：http://hz.zhengqikj.top/gtnxcbetis.html

================================================================================
来源：http://hz.gotoacloud.top/gtmyypddvr.html

[G01] 定义类
来源：http://hz.kuanghao11.cn/gtvhkehsir.html

Py:   class User: pass
来源：http://hz.jinqigfzy.top/gtlmdrklwu.html

PHP:  class User {}
来源：http://hz.hammf.cn/gtyndfumlt.html

JS:   class User {}
来源：http://hz.ehwqpu.com/gtrsznggni.html

TS:   class User { name: string = ""; }
来源：http://hz.yvedp.cn/gtgyczolkf.html

Java: class User {}
来源：http://hz.shanyushiyangkeji.top/gtfiekesor.html

Go:   type User struct { Name string }
来源：http://hz.xinyue.icu/gtfkeksttu.html

Ruby: class User; end
来源：http://hz.yj202588.top/gtubrlumrb.html

C#:   class User {}
来源：http://hz.tian-w.cn/gtcaonufqx.html

[G02] 构造函数
来源：http://hz.zhengqikj.top/gtidoieunw.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zhiwuduotai.top/gtrctibpwq.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.wangdashe.top/gtuqwibpei.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yangfankeji.com/gtdnaacgug.html

TS:   constructor(public name: string) {}
来源：http://hz.cdnleiting.top/gtosqshkbl.html

Java: User(String name) { this.name = name; }
来源：http://hz.cucudq.cn/gtvpfcbste.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yangfankeji.com/gtroflvtzs.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.jinqigfzy.top/gtktzgpvsy.html

C#:   public User(string name) { Name = name; }
来源：http://hz.daria6918.cn/gtybqkijyd.html

[G03] 实例属性
来源：http://hz.wangdashe.top/gtccwafhsw.html

Py:   self.name = "x"
来源：http://hz.mhx1999.top/gtzbtkvmwm.html

PHP:  public string $name = "x";
来源：http://hz.chenzaomai.com/gtbtfykygd.html

JS:   this.name = "x";
来源：http://hz.yvedp.cn/gtynjllwtx.html

TS:   name: string = "x";
来源：http://hz.jlsjyb.cn/gtyosnypqe.html

Java: private String name;
来源：http://hz.jqgufenzy.top/gtecdwuywo.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.xylfe.cn/gtvublnlyx.html

Ruby: @name = "x"
来源：http://hz.tian-w.cn/gtsxwokbkg.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yuanzhike.top/gtnbmtyspu.html

[G04] 定义方法
来源：http://hz.daxiang520.top/gtdgqkwbiw.html

Py:   def greet(self): return self.name
来源：http://hz.zhongyouzk.top/gtxjjptohn.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.ydzc1.top/gtzysahpbo.html

JS:   greet() { return this.name; }
来源：http://hz.hysaishi.cn/gtnlpsetvp.html

TS:   greet(): string { return this.name; }
来源：http://hz.hywenlv.cn/gtahrgxumg.html

Java: String greet() { return name; }
来源：http://hz.xylfe.cn/gtakgzgiww.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.andypj.xyz/gtiwddvpfz.html

Ruby: def greet; @name; end
来源：http://hz.shzxlz.cn/gtoaiaehsh.html

C#:   public string Greet() => Name;
来源：http://hz.tianlin.xyz/gtcxhjmuor.html

[G05] 继承
来源：http://hz.andypj.xyz/gtasvnwsxc.html

Py:   class Admin(User): pass
来源：http://hz.yanxiufei.cn/gtxpsiwaba.html

PHP:  class Admin extends User {}
来源：http://hz.yuxming.cn/gtqergtkzw.html

JS:   class Admin extends User {}
来源：http://hz.yanxiufei.cn/gtastomvzp.html

TS:   class Admin extends User {}
来源：http://hz.52xcode.cn/gtvchjsrxg.html

Java: class Admin extends User {}
来源：http://hz.zhengqikj.top/gtmylmnyej.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.smart0.xyz/gtbqhudclq.html

Ruby: class Admin < User; end
来源：http://hz.hfpthk.cn/gtgdtlwfmp.html

C#:   class Admin : User {}
来源：http://hz.ydzc1.top/gtiulwwdqw.html

[G06] 重写方法
来源：http://hz.dianchejie.cn/gtewoquwte.html

Py:   def greet(self): return "admin"
来源：http://hz.shuidangran.top/gtrlisjdgs.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.daxiang520.top/gtpvphinzx.html

JS:   greet() { return "admin"; }
来源：http://hz.feifeiyinyue.top/gtexsotttm.html

TS:   greet(): string { return "admin"; }
来源：http://hz.shzxlz.cn/gtvmcljhyf.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.c1oappe.top/gtzliqevtq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.kuanghao11.cn/gtbfjirufk.html

Ruby: def greet; "admin"; end
来源：http://hz.smart0.xyz/gtgsjdibfs.html

C#:   public override string Greet() => "admin";
来源：http://hz.52xcode.cn/gtmwirqewx.html

[G07] 调用父类方法
来源：http://hz.gotoacloud.top/gtpaogckiz.html

Py:   super().greet()
来源：http://hz.chenlongwang.top/gtvfogfkvo.html

PHP:  parent::greet();
来源：http://hz.hammf.cn/gtplsgzlzz.html

JS:   super.greet();
来源：http://hz.chenzaomai.com/gtxaqmefib.html

TS:   super.greet();
来源：http://hz.quarkkingdee.top/gtccdvmzfx.html

Java: super.greet();
来源：http://hz.zhijiandao.cn/gtkzyuyztp.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jqgufenzy.top/gtsdtxaxjj.html

Ruby: super
来源：http://hz.yuxming.cn/gtwqfrlkga.html

C#:   base.Greet();
来源：http://hz.vqdsnc.cn/gtwpchgula.html

[G08] 静态方法与属性
来源：http://hz.ydzc1.top/gtojxuwepp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.wangdashe.top/gtductafil.html

PHP:  public static function f() {}
来源：http://hz.meibo888.top/gtgqpinium.html

JS:   static f() {}
来源：http://hz.cheryme.top/gtwaqnwhdq.html

TS:   static f(): void {}
来源：http://hz.haohaochexian.top/gtxpnwsmrw.html

Java: static void f() {}
来源：http://hz.pycfn.com/gtivnfytos.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.nanxinkj.top/gtlvphpnwp.html

Ruby: def self.f; end
来源：http://hz.ppjwa.cn/gtvosadbyd.html

C#:   public static void F() {}
来源：http://hz.guowangkeji.top/gtvoxbxowz.html

[G09] 接口 / 抽象类
来源：http://hz.shangyingyoupin.top/gtmxwpmjyk.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.zdqjudy.top/gtrpbyhpfn.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.316326.xyz/gtjqryrsbp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.meibo888.top/gtxzyygitu.html

TS:   interface Shape { area(): number; }
来源：http://hz.yuxming.cn/gtmtpialhb.html

Java: interface Shape { double area(); }
来源：http://hz.nanxuanxn.top/gtujaiqwsz.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yanxiufei.cn/gtedpnyfzm.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.daxiang520.top/gtiiblltzu.html

C#:   interface IShape { double Area(); }
来源：http://hz.shuidangran.top/gtssozgfsc.html

[G10] 访问控制
来源：http://hz.hywenlv.cn/gtpbbygtyq.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.tanke756.top/gteouhtiug.html

PHP:  public / protected / private
来源：http://hz.9152youxi.cn/gtcdhsxzbn.html

JS:   #private 字段；其余公开
来源：http://hz.tanke756.top/gtclklmgav.html

TS:   public / protected / private
来源：http://hz.ppjwa.cn/gtpoqwlclu.html

Java: public / protected / private / 默认包级
来源：http://hz.yj20258888.top/gtxotflett.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zhengqikj.top/gtoyhixqvz.html

Ruby: public / protected / private
来源：http://hz.yj20258888.top/gtnonwijul.html

C#:   public / protected / private / internal
来源：http://hz.jinghuilouyu.cn/gtysdaxnnp.html

[G11] getter / setter
来源：http://hz.gzhubu.top/gtdwilgjuv.html

Py:   @property 与 @x.setter
来源：http://hz.jqgfzy.top/gtsgkjnjtc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.sxryk.cn/gtewruyyfg.html

JS:   get name() { return this._name; }
来源：http://hz.shangyingyoupin.top/gtizugdlfn.html

TS:   get name(): string { return this._name; }
来源：http://hz.sxryk.cn/gturxlvfzg.html

Java: public String getName() { return name; }
来源：http://hz.wangdashe.top/gthkxtwevb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.zdqjudy.top/gtzorfuvkt.html

Ruby: attr_accessor :name
来源：http://hz.xuanzx.com/gtqbbgujac.html

C#:   public string Name { get; set; }
来源：http://hz.daxiang520.top/gtfwtmjgfq.html

[G12] 对象转字符串
来源：http://hz.zhaomingkeji.xyz/gtiainqrxd.html

Py:   def __str__(self): return self.name
来源：http://hz.jianghu66.top/gtjamqiujb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.chenzaomai.com/gtnvddfhnc.html

JS:   toString() { return this.name; }
来源：http://hz.pycfn.com/gtqzsswjsg.html

TS:   toString(): string { return this.name; }
来源：http://hz.sxryk.cn/gtcpamodzh.html

Java: @Override public String toString() { return name; }
来源：http://hz.xuanzx.com/gtvbilnhpi.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.meibo888.top/gtwpxkrprn.html

Ruby: def to_s; @name; end
来源：http://hz.hnqzz.top/gtotzchrjt.html

C#:   public override string ToString() => Name;
来源：http://hz.nanxinkj.top/gtzjssnucn.html

[G13] 判断对象类型
来源：http://hz.cqqwz.cn/gtdzdqvaak.html

Py:   isinstance(u, User)
来源：http://hz.jqgfzy.top/gtpfxsfiuz.html

PHP:  $u instanceof User
来源：http://hz.ppjwa.cn/gtlgnsfeja.html

JS:   u instanceof User
来源：http://hz.hnxiangtu.top/gtcnieldkp.html

TS:   u instanceof User
来源：http://hz.ybcxt.top/gtgaywjkzr.html

Java: u instanceof User
来源：http://hz.fzhhl.top/gtdpbmzlhb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.nanxuanxn.top/gtaxobkast.html

Ruby: u.is_a?(User)
来源：http://hz.gzhubu.top/gtdjxfbltm.html

C#:   u is User
来源：http://hz.dashuyun.cn/gtbwxwbcuo.html

[G14] 数据类 / record
来源：http://hz.zhoulong.xyz/gtvdemvbtc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.jyoumei.cn/gtpbagojhu.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.cdnleiting.top/gtvbiggsdv.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.wangshuangyany.cn/gtdohabkzc.html

TS:   type User = { name: string; age: number };
来源：http://hz.pycfn.com/gtgfashczx.html

Java: record User(String name, int age) {}
来源：http://hz.hammf.cn/gtqxzhwltg.html

Go:   type User struct { Name string; Age int }
来源：http://hz.shanyushiyangkeji.top/gtigxymkiq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jinqigufen.top/gtqnqflypx.html

C#:   record User(string Name, int Age);
来源：http://hz.316326.xyz/gtwcnnqxux.html

[G15] 枚举
来源：http://hz.ehwqpu.com/gtdrqzvleb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.zycfv.cn/gtquenyxzp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zhongyouzk.top/gtamdwthst.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.fzhhl.top/gtwkqowutc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zdqjudy.top/gtscspupox.html

Java: enum Color { RED, GREEN }
来源：http://hz.jinqigfzy.top/gttrtkskns.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.shangyingyoupin.top/gtaxduvwfr.html

Ruby: Color = %i[red green].freeze
来源：http://hz.redwolf501.top/gtnnomxmov.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jinyuanbaomall.cn/gtlszqhsnx.html

[G16] 对象转数组 / 字典
来源：http://hz.jinghuilouyu.cn/gtdjuohslf.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jiagoushi.top/gtbbmbaueu.html

PHP:  get_object_vars($obj);
来源：http://hz.yj20258888.top/gthjoqalkv.html

JS:   Object.entries(obj)
来源：http://hz.hywenlv.cn/gtjssenlmb.html

TS:   Object.entries(obj)
来源：http://hz.shanyushiyangkeji.top/gtvvfymmti.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.bjfxy.top/gtmlkbsbjw.html


<!-- 参考信息 -->