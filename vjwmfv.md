代发 wailian999

Ruby: s.lines
来源：http://hz.yonumen.top/gtwzxqvssj.html

C#:   s.Split('\n')
来源：http://hz.sweek.top/gtiahzkgmx.html

[E20] 判断字符串是否为空
来源：http://hz.gotoacloud.top/gtxhtpkaea.html

Py:   if not s:
来源：http://hz.chenzaomai.com/gtcrowcxie.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.shangyingyoupin.top/gtkqorkter.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.gaohongyu789.top/gtthpaqjim.html

TS:   if (s === "") {}
来源：http://hz.smart0.xyz/gtdznfqply.html

Java: if (s.isEmpty()) {}
来源：http://hz.gotoacloud.top/gtgktorlbh.html

Go:   if s == "" {}
来源：http://hz.svipenyu.cn/gtzwymxskl.html

Ruby: if s.empty?
来源：http://hz.dianchejie.cn/gtxbxipwpn.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.yonumen.top/gtlgnehpxt.html

[E21] 超长截断加省略号
来源：http://hz.fzhhl.top/gtirkacyxs.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.mhx1999.top/gtkeuhkbcr.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.bjfxy.top/gtxteznurn.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.aibaodan.cn/gteqrkuwnh.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.havefunace.top/gtdqaqbrqv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.cucudq.cn/gtcjgembmx.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.yuanzhike.top/gtmzoknhlh.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.hysaishi.cn/gtwnhimxpt.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.jlsjyb.cn/gtdkuktqqw.html

[E22] 字节长度与字符长度
来源：http://hz.hongshengwenyu.top/gtavaidcln.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.shanyushiyangkeji.top/gtptdhjfku.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.gotoacloud.top/gtndedbaej.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhiwuduotai.top/gtplvgrkpo.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ywan-chungtsiang.top/gtmnsbmzbi.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.zhongyouzk.top/gtriulmozf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.jinyuanbaomall.cn/gtjccwrhey.html

Ruby: s.bytesize;  s.length
来源：http://hz.hnxiangtu.top/gtgongdony.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.xziqi.cn/gtopbzvzdy.html

================================================================================
来源：http://hz.aibaodan.cn/gtykgszfln.html

F. 文件与目录
来源：http://hz.zhijiandao.cn/gtqosakmqs.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtqmgcwnqt.html

[F01] 读取整个文件
来源：http://hz.cqqwz.cn/gtttcehsmp.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.ehwqpu.com/gtgdfqvbpg.html

PHP:  file_get_contents("a.txt");
来源：http://hz.ppjwa.cn/gtreeqfstt.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.chenzaomai.com/gtwubkdzyw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.yvedp.cn/gthfucccww.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.jqgfzy.top/gtuyaseucw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.quarkkingdee.top/gtehgvknls.html

Ruby: File.read("a.txt")
来源：http://hz.sysykeji.top/gtlskpiikr.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.guowangkeji.top/gtgxmyhxdb.html

[F02] 逐行读取文件
来源：http://hz.nanxuanxn.top/gtpttlzlyx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.zhixingplan.top/gtklijbwxo.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.ppjwa.cn/gtywjpdurm.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yvedp.cn/gtyclegqrh.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ybcxt.top/gtfrnkgvdv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.zhengqikj.top/gtbmecicti.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.jyoumei.cn/gtxjtpntsp.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.ywan-chungtsiang.top/gtpjgiavyd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.xinyue.icu/gtbcysnbfo.html

[F03] 写入文件（覆盖）
来源：http://hz.shangyingyoupin.top/gtxyvcdsne.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.hammf.cn/gtjiwxvvdj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.daria6918.cn/gtbgeqfmie.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.redwolf501.top/gtvohixjlx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yj20258888.top/gtcwgyvqsg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.iojbl.cn/gtxvbhbrsk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.sufxvd.cn/gtdihwjxal.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.yueranfly.top/gtxahuwckq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.9152youxi.cn/gtitnqpqon.html

[F04] 追加写入文件
来源：http://hz.svipenyu.cn/gtmaiqmvxa.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.redwolf501.top/gtlwicvnza.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.cqqwz.cn/gtyjzpivvl.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ppjwa.cn/gtxyqudfnq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yj20258.top/gtitjmqypi.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.kuanghao11.cn/gtqmjlojqv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.nanxinkj.top/gtsvarkvli.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.chenzaomai.com/gtrfbgsdok.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.jlsjyb.cn/gtroisclrc.html

[F05] 判断文件或目录是否存在
来源：http://hz.chenlongwang.top/gtfykuojlh.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.andypj.xyz/gttlmmpcxk.html

PHP:  file_exists("a.txt");
来源：http://hz.zhengqikj.top/gtjeknjigf.html

JS:   fs.existsSync("a.txt")
来源：http://hz.52xcode.cn/gtwexajdjw.html

TS:   fs.existsSync("a.txt")
来源：http://hz.tian-w.cn/gtyvhdzbrv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.cqqwz.cn/gtzttnjizj.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.zhijiandao.cn/gtrrokodrv.html

Ruby: File.exist?("a.txt")
来源：http://hz.zdqjudy.top/gtjpeozlll.html

C#:   File.Exists("a.txt")
来源：http://hz.shangyingyoupin.top/gttbbjchdi.html

[F06] 删除文件
来源：http://hz.cqqwz.cn/gtzasvkgdt.html

Py:   os.remove("a.txt")
来源：http://hz.zhaomingkeji.xyz/gtwglnmgjz.html

PHP:  unlink("a.txt");
来源：http://hz.xingfuxueyuan.xyz/gtqvtwmwbq.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.shzxlz.cn/gtyqwainor.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.svipenyu.cn/gtytqzzcpx.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.hongshengwenyu.top/gtykyjtzxa.html

Go:   os.Remove("a.txt")
来源：http://hz.pycfn.com/gtmrhkyukb.html

Ruby: File.delete("a.txt")
来源：http://hz.zhijiandao.cn/gtluwlysah.html

C#:   File.Delete("a.txt");
来源：http://hz.hnqzz.top/gtojuwgsxh.html

[F07] 创建目录（含多级）
来源：http://hz.chenjidiqi.icu/gtexkioatm.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.redwolf501.top/gtveoqsfze.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.daxiang520.top/gtmxkogfce.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jyoumei.cn/gtwnenuxny.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.smart0.xyz/gtalrgukco.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.yj20258888.top/gtynimbaag.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.snrcjt.cn/gteathwrol.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.gotoacloud.top/gterbszvlx.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.gogol.net.cn/gtloyymkzk.html

[F08] 遍历目录
来源：http://hz.nanxuanxn.top/gtwwvnbwtu.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.hywenlv.cn/gtlktkvvhv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.tianlin.xyz/gtvglvrnit.html

JS:   fs.readdirSync("dir")
来源：http://hz.0kj1m.cn/gtfknlxgxg.html

TS:   fs.readdirSync("dir")
来源：http://hz.yanxiufei.cn/gtonhxhuux.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.chenzaomai.com/gtqygxbbnv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.sweek.top/gtabfmzrap.html

Ruby: Dir.children("dir")
来源：http://hz.nanxinkj.top/gtdoiedbju.html

C#:   Directory.GetFiles("dir")
来源：http://hz.jiagoushi.top/gthwtsinft.html

[F09] 获取文件大小
来源：http://hz.smart0.xyz/gttlcaaoew.html

Py:   os.path.getsize("a.txt")
来源：http://hz.xinyue.icu/gtzvjudlpg.html

PHP:  filesize("a.txt");
来源：http://hz.svipenyu.cn/gtteqrqgfw.html

JS:   fs.statSync("a.txt").size
来源：http://hz.c1oappe.top/gtgcksifkz.html

TS:   fs.statSync("a.txt").size
来源：http://hz.cheryme.top/gtwwqqiekk.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jqgfzy.top/gthicddola.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.zhaomingkeji.xyz/gtfttlctoc.html

Ruby: File.size("a.txt")
来源：http://hz.yvedp.cn/gtlzfxdcas.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.nanxuanxn.top/gtpozdbhzo.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yonumen.top/gtlabiyjak.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.svipenyu.cn/gtjytskdpt.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.ppjwa.cn/gtnvsrtoli.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.zhiwuduotai.top/gtsuoeccfy.html

TS:   path.extname("a.txt")
来源：http://hz.xinyue.icu/gtqmbyahcc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.zhijiandao.cn/gtixauwmom.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.wangdashe.top/gtzlxbrzeb.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.nanxinkj.top/gthqgodqqw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.zhoulong.xyz/gtagitxajh.html

[F11] 复制与移动文件
来源：http://hz.yongpay.top/gtimopkcyx.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.jlsjyb.cn/gtuodlkogy.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.zhiwuduotai.top/gtbqqlkrzb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.shangyingyoupin.top/gtmrkuhymk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.c1oappe.top/gtldzwjrof.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.quarkkingdee.top/gtgyhtyeii.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.zhijiandao.cn/gtxyehthyh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.ehwqpu.com/gtxsydipql.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.nanxuanxn.top/gtgpaltwyn.html

[F12] CSV 读写
来源：http://hz.gotoacloud.top/gturulyjfk.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.dashuyun.cn/gtuodgkkrt.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.yj20258888.top/gtwydftqvq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.hammf.cn/gtuedkhzwb.html

TS:   // 同上
来源：http://hz.xuetiantiany.cn/gtqqojdvlr.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.dashuyun.cn/gtxcjlagnm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.fzhhl.top/gthjipibkp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.hnqzz.top/gtsodweaye.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jinyuanbaomall.cn/gtanlneito.html

================================================================================
来源：http://hz.xinyue.icu/gtqkrrggbq.html

G. 面向对象
来源：http://hz.xingfuxueyuan.xyz/gtcezfsabt.html

================================================================================
来源：http://hz.zhixingplan.top/gtwxyhumrm.html

[G01] 定义类
来源：http://hz.hammf.cn/gteljxoubn.html

Py:   class User: pass
来源：http://hz.xylfe.cn/gtcwlrlpwx.html

PHP:  class User {}
来源：http://hz.daria6918.cn/gtendvlsbm.html

JS:   class User {}
来源：http://hz.zhaomingkeji.xyz/gtcfncbkgw.html

TS:   class User { name: string = ""; }
来源：http://hz.quarkkingdee.top/gtxrpnthhf.html

Java: class User {}
来源：http://hz.tian-w.cn/gtpbhjvxzf.html

Go:   type User struct { Name string }
来源：http://hz.guannengcc.top/gtrhcfanko.html

Ruby: class User; end
来源：http://hz.chenjidiqi.icu/gtetuzzntf.html

C#:   class User {}
来源：http://hz.vqdsnc.cn/gtkwggehkm.html

[G02] 构造函数
来源：http://hz.iojbl.cn/gtpieubxge.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zhixingplan.top/gtqerywolb.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.vqdsnc.cn/gtcvjzjngh.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.sufxvd.cn/gtvvrfwfuj.html

TS:   constructor(public name: string) {}
来源：http://hz.xylfe.cn/gtpptvbynb.html

Java: User(String name) { this.name = name; }
来源：http://hz.guannengcc.top/gtuyjfibih.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.ydjk.org.cn/gtpcxkvupz.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.sxryk.cn/gtlweuvozm.html

C#:   public User(string name) { Name = name; }
来源：http://hz.pycfn.com/gtpivoynkj.html

[G03] 实例属性
来源：http://hz.zhixingplan.top/gtuyjgmpbw.html

Py:   self.name = "x"
来源：http://hz.bjfxy.top/gtwwvufmxc.html

PHP:  public string $name = "x";
来源：http://hz.xuetiantiany.cn/gtxaosrksf.html

JS:   this.name = "x";
来源：http://hz.yongpay.top/gtcidawgxi.html

TS:   name: string = "x";
来源：http://hz.andypj.xyz/gtmnrcpwqx.html

Java: private String name;
来源：http://hz.zhoulong.xyz/gtiwzkzqhn.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.jinghuilouyu.cn/gtibsaxqxc.html

Ruby: @name = "x"
来源：http://hz.zhengqikj.top/gtshclrbmk.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.hnxiangtu.top/gtrpkoztnr.html

[G04] 定义方法
来源：http://hz.xingfuxueyuan.xyz/gtweoiwqzp.html

Py:   def greet(self): return self.name
来源：http://hz.zhoulong.xyz/gtbidokgei.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.shangyingyoupin.top/gtstjxebjk.html

JS:   greet() { return this.name; }
来源：http://hz.cheryme.top/gtfswznain.html

TS:   greet(): string { return this.name; }
来源：http://hz.316326.xyz/gtgywkziii.html

Java: String greet() { return name; }
来源：http://hz.xuanzx.com/gtuvvmphdu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.hnxiangtu.top/gtjsdhhpfa.html

Ruby: def greet; @name; end
来源：http://hz.zhengqikj.top/gthbdqmryr.html

C#:   public string Greet() => Name;
来源：http://hz.vqdsnc.cn/gtpzxubykd.html

[G05] 继承
来源：http://hz.guannengcc.top/gtvkmmvgfa.html

Py:   class Admin(User): pass
来源：http://hz.shangyingyoupin.top/gtqwblrbvf.html

PHP:  class Admin extends User {}
来源：http://hz.jinghuilouyu.cn/gtcmjfbilg.html

JS:   class Admin extends User {}
来源：http://hz.nanxinkj.top/gtnvmydoae.html

TS:   class Admin extends User {}
来源：http://hz.yanxiufei.cn/gtqzfzuqyl.html

Java: class Admin extends User {}
来源：http://hz.jqgufenzy.top/gtvrhidiro.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.snrcjt.cn/gtpmalifie.html

Ruby: class Admin < User; end
来源：http://hz.zhaomingkeji.xyz/gtjugohrsx.html

C#:   class Admin : User {}
来源：http://hz.bjfxy.top/gtybsnfxuq.html

[G06] 重写方法
来源：http://hz.cqqwz.cn/gthkklxsrw.html

Py:   def greet(self): return "admin"
来源：http://hz.jqgufenzy.top/gtdqrjrvck.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.shzxlz.cn/gtwlqwhvvw.html

JS:   greet() { return "admin"; }
来源：http://hz.chenzaomai.com/gttzyaabqp.html

TS:   greet(): string { return "admin"; }
来源：http://hz.tian-w.cn/gtncbhkrlc.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.birdmap.top/gtrikffqdg.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.jinqigufen.top/gtyjnxxvzr.html

Ruby: def greet; "admin"; end
来源：http://hz.wangdashe.top/gtdzssqanz.html

C#:   public override string Greet() => "admin";
来源：http://hz.pycfn.com/gtqebxgovb.html

[G07] 调用父类方法
来源：http://hz.jqgfzy.top/gttvvkkpfn.html

Py:   super().greet()
来源：http://hz.yuanzhike.top/gtywaluuju.html

PHP:  parent::greet();
来源：http://hz.chenlongwang.top/gtyabnlply.html

JS:   super.greet();
来源：http://hz.yuanzhike.top/gtglymfdhj.html

TS:   super.greet();
来源：http://hz.jlsjyb.cn/gtudggytyg.html

Java: super.greet();
来源：http://hz.tanke756.top/gtcopnduiq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.hnxiangtu.top/gtiadfjeld.html

Ruby: super
来源：http://hz.dianchejie.cn/gtyhsiikrk.html

C#:   base.Greet();
来源：http://hz.cdnleiting.top/gtfxeayjef.html

[G08] 静态方法与属性
来源：http://hz.xuanzx.com/gtjhxqtxzn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.shanyushiyangtech.top/gtuyzhggug.html

PHP:  public static function f() {}
来源：http://hz.meibo888.top/gtzopepxnr.html

JS:   static f() {}
来源：http://hz.zycfv.cn/gtgttymupv.html

TS:   static f(): void {}
来源：http://hz.bjfxy.top/gtyhvohdaz.html

Java: static void f() {}
来源：http://hz.shanyushiyangkeji.top/gtbcsjuzlz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yongpay.top/gtiveifuxz.html

Ruby: def self.f; end
来源：http://hz.gzhubu.top/gtvxcowtyd.html

C#:   public static void F() {}
来源：http://hz.jlsjyb.cn/gtrxfsquwh.html

[G09] 接口 / 抽象类
来源：http://hz.pengpengdd.cyou/gtipmfkzuc.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.jinyuanbaomall.cn/gtgswmwdvt.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.mhx1999.top/gtgzlixefc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.zhixingplan.top/gtkbayrgho.html

TS:   interface Shape { area(): number; }
来源：http://hz.zycfv.cn/gtkivwnnqt.html

Java: interface Shape { double area(); }
来源：http://hz.zdqjudy.top/gtgabjopap.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.jlsjyb.cn/gtnvlqagqr.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.havefunace.top/gtcsaivcfl.html

C#:   interface IShape { double Area(); }
来源：http://hz.tianlin.xyz/gtmhyrqlvm.html

[G10] 访问控制
来源：http://hz.sweek.top/gteordaooe.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.jqgufenzy.top/gtjuigxfbs.html

PHP:  public / protected / private
来源：http://hz.guowangkeji.top/gtxqjhaxwa.html

JS:   #private 字段；其余公开
来源：http://hz.jyoumei.cn/gtmrxzeeuu.html

TS:   public / protected / private
来源：http://hz.jiagoushi.top/gtrxejpuoh.html

Java: public / protected / private / 默认包级
来源：http://hz.ywan-chungtsiang.top/gtlevuevsk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.ydjk.org.cn/gtycerffnf.html

Ruby: public / protected / private
来源：http://hz.ehwqpu.com/gtdveqkast.html

C#:   public / protected / private / internal
来源：http://hz.ydjk.org.cn/gtomooshiu.html

[G11] getter / setter
来源：http://hz.ppjwa.cn/gtbkqpjghn.html

Py:   @property 与 @x.setter
来源：http://hz.ywan-chungtsiang.top/gtwljzutsi.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.fzhhl.top/gtickzyhrd.html

JS:   get name() { return this._name; }
来源：http://hz.ydzc1.top/gthqqcgyjm.html

TS:   get name(): string { return this._name; }
来源：http://hz.zhixingplan.top/gtwimqfuud.html

Java: public String getName() { return name; }
来源：http://hz.ehwqpu.com/gtfcqjikyg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.hammf.cn/gtgsyobxhj.html

Ruby: attr_accessor :name
来源：http://hz.jianghu66.top/gtpbpkznkw.html

C#:   public string Name { get; set; }
来源：http://hz.sufxvd.cn/gtypaokmzv.html

[G12] 对象转字符串
来源：http://hz.52xcode.cn/gtcbwaflow.html

Py:   def __str__(self): return self.name
来源：http://hz.wangdashe.top/gtgaofcspy.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.xylfe.cn/gtlhbqiffg.html

JS:   toString() { return this.name; }
来源：http://hz.zhengqikj.top/gtophpiujr.html

TS:   toString(): string { return this.name; }
来源：http://hz.hongshengwenyu.top/gteqwrxdkc.html

Java: @Override public String toString() { return name; }
来源：http://hz.jqgfzy.top/gtejpkbiro.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.daria6918.cn/gtbrodoqam.html

Ruby: def to_s; @name; end
来源：http://hz.xylfe.cn/gtfochxvtj.html

C#:   public override string ToString() => Name;
来源：http://hz.cheryme.top/gtdqafiudb.html

[G13] 判断对象类型
来源：http://hz.feifeiyinyue.top/gtfjxwsqap.html

Py:   isinstance(u, User)
来源：http://hz.xziqi.cn/gttnkhcnnn.html

PHP:  $u instanceof User
来源：http://hz.yj20258.top/gtgkyabyqz.html

JS:   u instanceof User
来源：http://hz.ppjwa.cn/gtjadxfuju.html

TS:   u instanceof User
来源：http://hz.daria6918.cn/gtammbwfre.html

Java: u instanceof User
来源：http://hz.yj20258.top/gtccykrtsr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.cqqwz.cn/gtuyxxtnpo.html

Ruby: u.is_a?(User)
来源：http://hz.chenlongwang.top/gttukbffvn.html

C#:   u is User
来源：http://hz.zhoulong.xyz/gtjtmpkqdm.html

[G14] 数据类 / record
来源：http://hz.pengpengdd.cyou/gtiikuugdc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.jinyuanbaomall.cn/gtwrlnwwiv.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jinqigfzy.top/gtbqrybecm.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.jinyuanbaomall.cn/gtxlfmzsnd.html

TS:   type User = { name: string; age: number };
来源：http://hz.jinqigfzy.top/gtivckugin.html

Java: record User(String name, int age) {}
来源：http://hz.zhixingplan.top/gtyiirnhxg.html

Go:   type User struct { Name string; Age int }
来源：http://hz.zhixingplan.top/gtsepmovnx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.ydjk.org.cn/gtusszhsau.html

C#:   record User(string Name, int Age);
来源：http://hz.316326.xyz/gtuazszbfq.html

[G15] 枚举
来源：http://hz.quarkkingdee.top/gthwvgzsdp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.gaohongyu789.top/gteecrkful.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jinyuanbaomall.cn/gtdjzpnhhf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.jiagoushi.top/gtsqnlxxnq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.chenzaomai.com/gtuowpludl.html

Java: enum Color { RED, GREEN }
来源：http://hz.zhijiandao.cn/gtgsefpuaf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.jinghuilouyu.cn/gtybfojcln.html

Ruby: Color = %i[red green].freeze
来源：http://hz.vqdsnc.cn/gtfvwklajd.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xinyue.icu/gtwmraezrl.html

[G16] 对象转数组 / 字典
来源：http://hz.havefunace.top/gtpbzbdnza.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.zdqjudy.top/gtgbvhrhdc.html

PHP:  get_object_vars($obj);
来源：http://hz.xingfuxueyuan.xyz/gtzmkhniyr.html

JS:   Object.entries(obj)
来源：http://hz.zhaomingkeji.xyz/gtmwiqdaap.html

TS:   Object.entries(obj)
来源：http://hz.dianchejie.cn/gtwljmyfqm.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.cheryme.top/gtxbxqifar.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.jianghu66.top/gtmyeueugu.html

Ruby: obj.instance_variables
来源：http://hz.xingfuxueyuan.xyz/gtwtscteqa.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.nanxinkj.top/gtfzteyqca.html

================================================================================
来源：http://hz.yuanzhike.top/gtlowuovso.html

H. 异常与错误处理
来源：http://hz.daria6918.cn/gtxxnwdsje.html

================================================================================
来源：http://hz.aibaodan.cn/gtagwrfaum.html

[H01] try / catch 基础
来源：http://hz.c1oappe.top/gtqraljbyj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yueranfly.top/gtctpzlhsf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.jianghu66.top/gthnlcobxo.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.hfpthk.cn/gtbulguzzy.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.shangyingyoupin.top/gtajakqtlg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.52xcode.cn/gtsjfrfwbo.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.cdnleiting.top/gtuesrixcd.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.sufxvd.cn/gtobqauiyt.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.nanxinkj.top/gttknpsyxr.html

[H02] finally / ensure 收尾
来源：http://hz.birdmap.top/gtlaslxlhm.html


<!-- 参考信息 -->