代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.jqgfzy.top/gtsnposjgm.html

================================================================================
来源：http://hz.wangdashe.top/gtbmapynrz.html

F. 文件与目录
来源：http://hz.jqgfzy.top/gtwqjwycxy.html

================================================================================
来源：http://hz.cheryme.top/gtnohcixbf.html

[F01] 读取整个文件
来源：http://hz.wangdashe.top/gtotzehjtk.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yanxiufei.cn/gtsoqmmkdr.html

PHP:  file_get_contents("a.txt");
来源：http://hz.jianghu66.top/gtvrwsckcw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.dashuyun.cn/gtiovqoswv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.xziqi.cn/gtquaeeeag.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.snrcjt.cn/gttlwwnolw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.yanxiufei.cn/gteqynjzoy.html

Ruby: File.read("a.txt")
来源：http://hz.gaohongyu789.top/gttqdagfje.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.gaohongyu789.top/gtdsrijibx.html

[F02] 逐行读取文件
来源：http://hz.ydzc1.top/gtvinbbvuh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.xuanzx.com/gtjxjgpmvm.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.feifeiyinyue.top/gtbzuybfca.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xuetiantiany.cn/gtfkrsemvd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hfpthk.cn/gtzwrpfyrc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.jinqigfzy.top/gtvybfomes.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.yj202588.top/gtbkatcdiw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.gaohongyu789.top/gtcjhowfkb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.316326.xyz/gtwrrqepkl.html

[F03] 写入文件（覆盖）
来源：http://hz.jqgufenzy.top/gtqridwlxv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.zhijiandao.cn/gtcftmjemc.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.bjfxy.top/gtvkbutpxa.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yj20258888.top/gtubsetudu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.andypj.xyz/gtmauyrzzj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.ydjk.org.cn/gttwxlzpcb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.mhx1999.top/gtmylojxwl.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.ywan-chungtsiang.top/gtdfzypkkf.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.guannengcc.top/gtjhfmuovc.html

[F04] 追加写入文件
来源：http://hz.guowangkeji.top/gtkpbzvumf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.xingfuxueyuan.xyz/gtifamxegj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.dianchejie.cn/gtykyuwypw.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.cqqwz.cn/gtavuentek.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yangfankeji.com/gtqnlpkcph.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.tianlin.xyz/gtrtgyvaxe.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.sysykeji.top/gtlpxvqcpl.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.jinghuilouyu.cn/gtgfkxkxqt.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.vqdsnc.cn/gtytvuxgxn.html

[F05] 判断文件或目录是否存在
来源：http://hz.chenzaomai.com/gtgcoibwoj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.yvedp.cn/gttztrhtxz.html

PHP:  file_exists("a.txt");
来源：http://hz.jianghu66.top/gtxyzsngwc.html

JS:   fs.existsSync("a.txt")
来源：http://hz.jinqigufen.top/gtthigcdgf.html

TS:   fs.existsSync("a.txt")
来源：http://hz.snrcjt.cn/gtzgwnvcwr.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.bjfxy.top/gtwcrcgnoj.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.xinyue.icu/gtcxfgknng.html

Ruby: File.exist?("a.txt")
来源：http://hz.ywan-chungtsiang.top/gtivlpiovn.html

C#:   File.Exists("a.txt")
来源：http://hz.pycfn.com/gtimewjelw.html

[F06] 删除文件
来源：http://hz.pycfn.com/gtolbqmqjx.html

Py:   os.remove("a.txt")
来源：http://hz.zycfv.cn/gtmvdjxbez.html

PHP:  unlink("a.txt");
来源：http://hz.xuetiantiany.cn/gtvkcsrswp.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.zhoulong.xyz/gtqxkseqtp.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.hywenlv.cn/gtnxdhbvru.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.yuxming.cn/gtvrvxdrxy.html

Go:   os.Remove("a.txt")
来源：http://hz.zhijiandao.cn/gtlvkmoumx.html

Ruby: File.delete("a.txt")
来源：http://hz.shanyushiyangtech.top/gtnrjcbpog.html

C#:   File.Delete("a.txt");
来源：http://hz.yj20258.top/gtilfzxoqt.html

[F07] 创建目录（含多级）
来源：http://hz.kuanghao11.cn/gtezqmlrzn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.birdmap.top/gtlrmvgiks.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.quarkkingdee.top/gtlazanedg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.sufxvd.cn/gtzcenodbk.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.aizwys.cn/gtjkamazsd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.zhijiandao.cn/gtifojnder.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.cucudq.cn/gtmtrbatwf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.shuidangran.top/gtzgcvgtac.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.zhiwuduotai.top/gtwqmjxymg.html

[F08] 遍历目录
来源：http://hz.svipenyu.cn/gtudbexvzz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.pycfn.com/gtqoftawzy.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.zhengqikj.top/gtkhwjzjhi.html

JS:   fs.readdirSync("dir")
来源：http://hz.cheryme.top/gtfkwxplkc.html

TS:   fs.readdirSync("dir")
来源：http://hz.aizwys.cn/gtckzzceju.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.xinyue.icu/gtbjaqiwta.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.cqqwz.cn/gtmocijzct.html

Ruby: Dir.children("dir")
来源：http://hz.daxiang520.top/gtcgggrjmk.html

C#:   Directory.GetFiles("dir")
来源：http://hz.shanyushiyangkeji.top/gtlmjvfbbb.html

[F09] 获取文件大小
来源：http://hz.chenlongwang.top/gtlaoeqoob.html

Py:   os.path.getsize("a.txt")
来源：http://hz.jiagoushi.top/gtycoagprd.html

PHP:  filesize("a.txt");
来源：http://hz.hfpthk.cn/gtdrxcoqya.html

JS:   fs.statSync("a.txt").size
来源：http://hz.nanxuanxn.top/gtzzbnxqgl.html

TS:   fs.statSync("a.txt").size
来源：http://hz.zhaomingkeji.xyz/gtumstpxyk.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.smart0.xyz/gtwsvtpleh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.nanxuanxn.top/gtunvbbqsf.html

Ruby: File.size("a.txt")
来源：http://hz.jyoumei.cn/gteiqskkng.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.zhijiandao.cn/gtobkdqsjh.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.pycfn.com/gthabsvmfk.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.havefunace.top/gtcpireznk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.sxryk.cn/gtnysuevcb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.sweek.top/gtofnvkojp.html

TS:   path.extname("a.txt")
来源：http://hz.sxryk.cn/gtsldomaqa.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.ppjwa.cn/gtjihxvecg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.chenjidiqi.icu/gtmepnfjjf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.quarkkingdee.top/gtfsivlgpz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.tianlin.xyz/gthndxnbep.html

[F11] 复制与移动文件
来源：http://hz.birdmap.top/gtcmeoyebs.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.zhoulong.xyz/gtpaojzsmd.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.zhiwuduotai.top/gtonxbxpyf.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.chenlongwang.top/gttceauvjx.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.dianchejie.cn/gttkdgpulp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.ivvv.top/gtgugutsqj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.cucudq.cn/gtvwetoiaj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.shanyushiyangkeji.top/gtrzfkatrr.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.tian-w.cn/gtswqiktmx.html

[F12] CSV 读写
来源：http://hz.haohaochexian.top/gtsjrxlocq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.mhx1999.top/gtobejhyot.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.chenzaomai.com/gtzqpqhdtu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.dashuyun.cn/gtqixwevxc.html

TS:   // 同上
来源：http://hz.9152youxi.cn/gtpolhbyyu.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.nanxinkj.top/gttbheibdc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.dianchejie.cn/gthuajqsbe.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.nanxinkj.top/gtzxqjqhwo.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.ppjwa.cn/gtylswwybd.html

================================================================================
来源：http://hz.smart0.xyz/gtjdaljdqk.html

G. 面向对象
来源：http://hz.haohaochexian.top/gtzvsvqsvs.html

================================================================================
来源：http://hz.zhengqikj.top/gtcsajclia.html

[G01] 定义类
来源：http://hz.xuetiantiany.cn/gtpedevkzq.html

Py:   class User: pass
来源：http://hz.hysaishi.cn/gtnlqryrkh.html

PHP:  class User {}
来源：http://hz.andypj.xyz/gtkfgbucgk.html

JS:   class User {}
来源：http://hz.yuxming.cn/gtvliahtww.html

TS:   class User { name: string = ""; }
来源：http://hz.tian-w.cn/gtuinuirkl.html

Java: class User {}
来源：http://hz.shanyushiyangtech.top/gtsexeoqvj.html

Go:   type User struct { Name string }
来源：http://hz.dianchejie.cn/gtbkhpfchh.html

Ruby: class User; end
来源：http://hz.hammf.cn/gtzoxvuxfn.html

C#:   class User {}
来源：http://hz.cdnleiting.top/gtdqojtqfq.html

[G02] 构造函数
来源：http://hz.bjfxy.top/gtfyaoemle.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yuanzhike.top/gtsmvafgko.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.vqdsnc.cn/gtphvkowfl.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.meibo888.top/gtqogcnvkx.html

TS:   constructor(public name: string) {}
来源：http://hz.chenzaomai.com/gtwimyibtr.html

Java: User(String name) { this.name = name; }
来源：http://hz.feifeiyinyue.top/gtfsumdkks.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.tian-w.cn/gtzpkmfkkz.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yvedp.cn/gtknrqxpff.html

C#:   public User(string name) { Name = name; }
来源：http://hz.hammf.cn/gtodxwohql.html

[G03] 实例属性
来源：http://hz.vqdsnc.cn/gtxhebkvvw.html

Py:   self.name = "x"
来源：http://hz.shanyushiyangtech.top/gtafoadsnf.html

PHP:  public string $name = "x";
来源：http://hz.wangshuangyany.cn/gtbjwyojvm.html

JS:   this.name = "x";
来源：http://hz.zhongyouzk.top/gtesapvphy.html

TS:   name: string = "x";
来源：http://hz.yuxming.cn/gtgihjvhyw.html

Java: private String name;
来源：http://hz.fengsongda.top/gtfjwqketq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.zhengqikj.top/gttwmexiiq.html

Ruby: @name = "x"
来源：http://hz.shanyushiyangkeji.top/gtxgtjrvbr.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.daria6918.cn/gtmlndhdnz.html

[G04] 定义方法
来源：http://hz.sysykeji.top/gtnxbqjlqj.html

Py:   def greet(self): return self.name
来源：http://hz.nanxuanxn.top/gtmywospaw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.jinyuanbaomall.cn/gttkilkygu.html

JS:   greet() { return this.name; }
来源：http://hz.sufxvd.cn/gtpxjyzllk.html

TS:   greet(): string { return this.name; }
来源：http://hz.snrcjt.cn/gtlarnkerf.html

Java: String greet() { return name; }
来源：http://hz.shzxlz.cn/gtxhdhjlgs.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.havefunace.top/gtriwoawow.html

Ruby: def greet; @name; end
来源：http://hz.nanxuanxn.top/gtuquyrzdh.html

C#:   public string Greet() => Name;
来源：http://hz.andypj.xyz/gtvgwtkirb.html

[G05] 继承
来源：http://hz.xylfe.cn/gtoolradnr.html

Py:   class Admin(User): pass
来源：http://hz.nwbrower.top/gtqczsywrh.html

PHP:  class Admin extends User {}
来源：http://hz.wangdashe.top/gtpsljkbww.html

JS:   class Admin extends User {}
来源：http://hz.jianghu66.top/gtnpiqrddw.html

TS:   class Admin extends User {}
来源：http://hz.yuxming.cn/gtkricqzmq.html

Java: class Admin extends User {}
来源：http://hz.nwbrower.top/gtwxukjhdv.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.xuetiantiany.cn/gtzfptduej.html

Ruby: class Admin < User; end
来源：http://hz.zhaomingkeji.xyz/gtcnillgsy.html

C#:   class Admin : User {}
来源：http://hz.yj202588.top/gtbahqipwr.html

[G06] 重写方法
来源：http://hz.ydjk.org.cn/gthyrvvijy.html

Py:   def greet(self): return "admin"
来源：http://hz.havefunace.top/gthptiugvb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.hywenlv.cn/gtrgqhvqcb.html

JS:   greet() { return "admin"; }
来源：http://hz.xziqi.cn/gtihpkympn.html

TS:   greet(): string { return "admin"; }
来源：http://hz.daxiang520.top/gtlphnslhb.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.chenzaomai.com/gticdljwix.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.snrcjt.cn/gtqnqmiklb.html

Ruby: def greet; "admin"; end
来源：http://hz.yangfankeji.com/gtrtblgnid.html

C#:   public override string Greet() => "admin";
来源：http://hz.shangyingyoupin.top/gteekoyiob.html

[G07] 调用父类方法
来源：http://hz.chenzaomai.com/gtzcaqzhgs.html

Py:   super().greet()
来源：http://hz.xziqi.cn/gtqnfrsppm.html

PHP:  parent::greet();
来源：http://hz.zhongyouzk.top/gtcmuynfon.html

JS:   super.greet();
来源：http://hz.smart0.xyz/gtbrquumbr.html

TS:   super.greet();
来源：http://hz.sufxvd.cn/gtziwzznzg.html

Java: super.greet();
来源：http://hz.ydjk.org.cn/gtdbzlwaei.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.tanke756.top/gtpofjwggs.html

Ruby: super
来源：http://hz.jianghu66.top/gtcempkscq.html

C#:   base.Greet();
来源：http://hz.yj20258.top/gtzezerpve.html

[G08] 静态方法与属性
来源：http://hz.shzxlz.cn/gtxfmklnyz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.hnxiangtu.top/gttholtnln.html

PHP:  public static function f() {}
来源：http://hz.ydjk.org.cn/gtxjotujbc.html

JS:   static f() {}
来源：http://hz.yueranfly.top/gtfdjaodew.html

TS:   static f(): void {}
来源：http://hz.nanxinkj.top/gtzyroigrt.html

Java: static void f() {}
来源：http://hz.aizwys.cn/gtwvuryurq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.meibo888.top/gtwswbecfm.html

Ruby: def self.f; end
来源：http://hz.dashuyun.cn/gtfkghspvy.html

C#:   public static void F() {}
来源：http://hz.gzhubu.top/gthgflorim.html

[G09] 接口 / 抽象类
来源：http://hz.aibaodan.cn/gtakflmvlp.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.nanxinkj.top/gtjawzhtoz.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.meibo888.top/gtkhvwwyfo.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.snrcjt.cn/gtrnnepaem.html

TS:   interface Shape { area(): number; }
来源：http://hz.chenlongwang.top/gtvswmgefr.html

Java: interface Shape { double area(); }
来源：http://hz.jinqigfzy.top/gtrabvayvo.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.zhixingplan.top/gtmdfyvnhg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.wangdashe.top/gtysrawvuf.html

C#:   interface IShape { double Area(); }
来源：http://hz.aizwys.cn/gttppwzoyg.html

[G10] 访问控制
来源：http://hz.zycfv.cn/gtsuuhccbv.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.andypj.xyz/gtdxtjkpbo.html

PHP:  public / protected / private
来源：http://hz.hnqzz.top/gtdnyyigpk.html

JS:   #private 字段；其余公开
来源：http://hz.ivvv.top/gtorjwqoxh.html

TS:   public / protected / private
来源：http://hz.cheryme.top/gtfsfmyrpd.html

Java: public / protected / private / 默认包级
来源：http://hz.sufxvd.cn/gtouehalqa.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zhixingplan.top/gtcxjixhiq.html

Ruby: public / protected / private
来源：http://hz.dianchejie.cn/gtbgzvdeeb.html

C#:   public / protected / private / internal
来源：http://hz.sweek.top/gttmlvxsdr.html

[G11] getter / setter
来源：http://hz.vqdsnc.cn/gtnzwlxyeo.html

Py:   @property 与 @x.setter
来源：http://hz.yanxiufei.cn/gtlfykidae.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yanxiufei.cn/gtkuslhswt.html

JS:   get name() { return this._name; }
来源：http://hz.chenjidiqi.icu/gtlsegnsjb.html

TS:   get name(): string { return this._name; }
来源：http://hz.zdqjudy.top/gtaszoizgq.html

Java: public String getName() { return name; }
来源：http://hz.yongpay.top/gtceovkbcg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.shanyushiyangtech.top/gtbyonksju.html

Ruby: attr_accessor :name
来源：http://hz.jqgfzy.top/gtiqwezriq.html

C#:   public string Name { get; set; }
来源：http://hz.wangshuangyany.cn/gttwllwbkx.html

[G12] 对象转字符串
来源：http://hz.svipenyu.cn/gtplhnntsp.html

Py:   def __str__(self): return self.name
来源：http://hz.zhaomingkeji.xyz/gtbwjsybbv.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.sweek.top/gtbvigsati.html

JS:   toString() { return this.name; }
来源：http://hz.hysaishi.cn/gtizozwuwa.html

TS:   toString(): string { return this.name; }
来源：http://hz.52xcode.cn/gtjojazpkr.html

Java: @Override public String toString() { return name; }
来源：http://hz.cdnleiting.top/gtwwcjynwh.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.316326.xyz/gtzadonjfj.html

Ruby: def to_s; @name; end
来源：http://hz.shangyingyoupin.top/gtiekasglb.html

C#:   public override string ToString() => Name;
来源：http://hz.cheryme.top/gtndoqcwso.html

[G13] 判断对象类型
来源：http://hz.yj20258888.top/gtrbrdtmlv.html

Py:   isinstance(u, User)
来源：http://hz.pengpengdd.cyou/gtlvzkihpz.html

PHP:  $u instanceof User
来源：http://hz.52xcode.cn/gtjcgkwmrx.html

JS:   u instanceof User
来源：http://hz.jqgfzy.top/gtzekqqbzh.html

TS:   u instanceof User
来源：http://hz.52xcode.cn/gtpkdtnumr.html

Java: u instanceof User
来源：http://hz.yueranfly.top/gthksyhehq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yanxiufei.cn/gthdfuatii.html

Ruby: u.is_a?(User)
来源：http://hz.wangshuangyany.cn/gttxqvkwdt.html

C#:   u is User
来源：http://hz.sufxvd.cn/gtsvujqnsa.html

[G14] 数据类 / record
来源：http://hz.birdmap.top/gtpxjqjgfq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.pycfn.com/gthodwnqhv.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.nanxinkj.top/gthxoszits.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yangfankeji.com/gtcutshhyg.html

TS:   type User = { name: string; age: number };
来源：http://hz.hnxiangtu.top/gtmbclyzfo.html

Java: record User(String name, int age) {}
来源：http://hz.nwbrower.top/gtfsshpgia.html

Go:   type User struct { Name string; Age int }
来源：http://hz.gzhubu.top/gtxmfaegls.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.xingfuxueyuan.xyz/gtnxgrkuwc.html

C#:   record User(string Name, int Age);
来源：http://hz.zhijiandao.cn/gtpteepzpw.html

[G15] 枚举
来源：http://hz.chenzaomai.com/gtgyioqwhz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.c1oappe.top/gtihadtiaq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.shanyushiyangkeji.top/gtspvykzhu.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.sxryk.cn/gtlvbxsrbb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.meibo888.top/gtfiarrzlu.html

Java: enum Color { RED, GREEN }
来源：http://hz.9152youxi.cn/gtwrrtqzln.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.shanyushiyangkeji.top/gtwnmhmysl.html

Ruby: Color = %i[red green].freeze
来源：http://hz.hongshengwenyu.top/gtwawoovvj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.fengsongda.top/gtzfraxbjh.html

[G16] 对象转数组 / 字典
来源：http://hz.guannengcc.top/gtbmsizkwf.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.hammf.cn/gthpmsflkw.html

PHP:  get_object_vars($obj);
来源：http://hz.zhixingplan.top/gtqursfkcf.html

JS:   Object.entries(obj)
来源：http://hz.zhaomingkeji.xyz/gtggfvpvvb.html

TS:   Object.entries(obj)
来源：http://hz.yj202588.top/gtaobsgzqe.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.xuetiantiany.cn/gthlbqaanq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.xingfuxueyuan.xyz/gtgukrykqk.html

Ruby: obj.instance_variables
来源：http://hz.guowangkeji.top/gtwrayjwdm.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.guannengcc.top/gtadszivky.html

================================================================================
来源：http://hz.jqgufenzy.top/gtqgwhrsna.html

H. 异常与错误处理
来源：http://hz.andypj.xyz/gtkswvipfo.html

================================================================================
来源：http://hz.hnxiangtu.top/gtvfztyuky.html

[H01] try / catch 基础
来源：http://hz.zhongyouzk.top/gtyckooapn.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.9152youxi.cn/gtlcsltfio.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.havefunace.top/gtqljmaypz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.zhijiandao.cn/gtygbisawd.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.smart0.xyz/gtbxapazgh.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.haohaochexian.top/gtirmbqxrp.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yvedp.cn/gtoqwoiwtm.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.nanxinkj.top/gttebfywty.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.hnxiangtu.top/gtxgtikvwo.html

[H02] finally / ensure 收尾
来源：http://hz.xinyue.icu/gtgyjdvvpw.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.hfpthk.cn/gtxbxrmofe.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.feifeiyinyue.top/gtgqhahyti.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.cdnleiting.top/gtwjmwdaxq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.52xcode.cn/gtvwgdfbqe.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.sysykeji.top/gtmtnusglo.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.andypj.xyz/gtxzjgebhm.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.cashguo.top/gtxitzemfs.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.zhixingplan.top/gtorkzbvtj.html

[H03] 主动抛出异常
来源：http://hz.zhixingplan.top/gthhjjyzwk.html

Py:   raise ValueError("错误信息")
来源：http://hz.zhiwuduotai.top/gtgqcmvqqi.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.bjfxy.top/gtkdgttnto.html

JS:   throw new Error("错误信息");
来源：http://hz.shangyingyoupin.top/gtqeuddjlj.html

TS:   throw new Error("错误信息");
来源：http://hz.zhijiandao.cn/gtfhtabtje.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.snrcjt.cn/gtvmpdtshm.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.hysaishi.cn/gtpdjmrfmq.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.feifeiyinyue.top/gtlcdwnhqn.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.yuxming.cn/gtfimaohgj.html

[H04] 自定义异常类型
来源：http://hz.quarkkingdee.top/gtkxwrtocg.html

Py:   class MyError(Exception): pass
来源：http://hz.dianchejie.cn/gtducebthz.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.vqdsnc.cn/gtnxldmmvr.html

JS:   class MyError extends Error {}
来源：http://hz.zhiwuduotai.top/gtzpwlhzkx.html

TS:   class MyError extends Error {}
来源：http://hz.daxiang520.top/gtjnkcywmq.html

Java: class MyException extends RuntimeException {}
来源：http://hz.ydjk.org.cn/gtltiyqhem.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.dashuyun.cn/gtbvvqpieb.html

Ruby: class MyError < StandardError; end
来源：http://hz.hammf.cn/gtdttprsnc.html

C#:   class MyException : Exception {}
来源：http://hz.shangyingyoupin.top/gtfnhfuchh.html

[H05] 捕获特定类型
来源：http://hz.shangyingyoupin.top/gtuzizxend.html

Py:   except ValueError as e:
来源：http://hz.ybcxt.top/gtnemmkcof.html


<!-- 参考信息 -->