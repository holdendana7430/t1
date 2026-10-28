代发 wailian999

Ruby: s.lines
来源：http://hz.hywenlv.cn/gtivcwlwjh.html

C#:   s.Split('\n')
来源：http://hz.jianghu66.top/gtioirjjij.html

[E20] 判断字符串是否为空
来源：http://hz.fengsongda.top/gtyunhnqzj.html

Py:   if not s:
来源：http://hz.kuanghao11.cn/gtpvilppdc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.pengpengdd.cyou/gtnppwivts.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.shanyushiyangtech.top/gtdgelihii.html

TS:   if (s === "") {}
来源：http://hz.jinyuanbaomall.cn/gtpmfowfqt.html

Java: if (s.isEmpty()) {}
来源：http://hz.ywan-chungtsiang.top/gtbppbshzp.html

Go:   if s == "" {}
来源：http://hz.dashuyun.cn/gtkqatrzup.html

Ruby: if s.empty?
来源：http://hz.fzhhl.top/gtbbehtlaa.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.birdmap.top/gtxwzunszo.html

[E21] 超长截断加省略号
来源：http://hz.shanyushiyangtech.top/gtzfvptlwr.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.jianghu66.top/gtrdzrveji.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.nwbrower.top/gtwznktpuw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jinqigufen.top/gthmevzebj.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jlsjyb.cn/gthsyxqqmt.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.redwolf501.top/gttdufcfwc.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.jinghuilouyu.cn/gtlaqjblzu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.vqdsnc.cn/gthnusnpxj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.nwbrower.top/gtbmwhwbcp.html

[E22] 字节长度与字符长度
来源：http://hz.yj202588.top/gtvtghdowk.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.zhijiandao.cn/gtphszbxuz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.xziqi.cn/gtjqjreycp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.sufxvd.cn/gtichrdvco.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.snrcjt.cn/gttcdgmckz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.tanke756.top/gtlsoajtff.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.zhongyouzk.top/gtznbyyxjr.html

Ruby: s.bytesize;  s.length
来源：http://hz.bjfxy.top/gtdxoluuvp.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.daxiang520.top/gttiumzeir.html

================================================================================
来源：http://hz.andypj.xyz/gtmnotrojy.html

F. 文件与目录
来源：http://hz.jyoumei.cn/gtupjvbgdt.html

================================================================================
来源：http://hz.gzhubu.top/gtfapqmdyg.html

[F01] 读取整个文件
来源：http://hz.c1oappe.top/gtaeysmnzv.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.vqdsnc.cn/gtzurxjcgq.html

PHP:  file_get_contents("a.txt");
来源：http://hz.0kj1m.cn/gtpdmbpihb.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.yangfankeji.com/gtyshsiugs.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.jiagoushi.top/gttltbfuda.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.ybcxt.top/gtpwjueokv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.yj20258.top/gtudhvgapj.html

Ruby: File.read("a.txt")
来源：http://hz.jinqigfzy.top/gtysaaqxji.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.gotoacloud.top/gtlfnpfyqg.html

[F02] 逐行读取文件
来源：http://hz.52xcode.cn/gtovgwyash.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.ywan-chungtsiang.top/gtrdeqhrnd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.ppjwa.cn/gtqphfolum.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.sxryk.cn/gtqarcodsx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhengqikj.top/gtammltslu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.vqdsnc.cn/gtjidfzevz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.zhijiandao.cn/gtfllrlgix.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.nanxuanxn.top/gtupzymecj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.dashuyun.cn/gtxfuqoadg.html

[F03] 写入文件（覆盖）
来源：http://hz.quarkkingdee.top/gtiefnctuv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.jianghu66.top/gtqxqwcdnc.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.zhoulong.xyz/gtujomyjkk.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yj20258.top/gttosdxesz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yj202588.top/gtmqyhjsdh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.sxryk.cn/gtcczpvcag.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.birdmap.top/gtqgsnmgoq.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.xuanzx.com/gtlimnsxwj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.sysykeji.top/gtfjiohlwt.html

[F04] 追加写入文件
来源：http://hz.sxryk.cn/gtbetlempt.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.ywan-chungtsiang.top/gtytgjfzki.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.ivvv.top/gtqyvehfov.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.chenjidiqi.icu/gtaxprozcs.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.tianlin.xyz/gtuqvcvchw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.svipenyu.cn/gtmjliawde.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.ehwqpu.com/gtbpthcvjy.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.0kj1m.cn/gtfdsaavvk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.yuxming.cn/gtyqgywbqf.html

[F05] 判断文件或目录是否存在
来源：http://hz.nwbrower.top/gtesfqmoyw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.sxryk.cn/gtraqvnchv.html

PHP:  file_exists("a.txt");
来源：http://hz.jiagoushi.top/gtzjwvmofr.html

JS:   fs.existsSync("a.txt")
来源：http://hz.pycfn.com/gtgflbrldp.html

TS:   fs.existsSync("a.txt")
来源：http://hz.jianghu66.top/gtfvwxamlw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.meibo888.top/gtgqecarfa.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.iojbl.cn/gtlfhlwmna.html

Ruby: File.exist?("a.txt")
来源：http://hz.shuidangran.top/gtuhvcczbo.html

C#:   File.Exists("a.txt")
来源：http://hz.iojbl.cn/gttbgyylyk.html

[F06] 删除文件
来源：http://hz.zdqjudy.top/gtyekihzyx.html

Py:   os.remove("a.txt")
来源：http://hz.52xcode.cn/gtegxfvcja.html

PHP:  unlink("a.txt");
来源：http://hz.shanyushiyangtech.top/gtesloufoq.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.havefunace.top/gtqbgseluj.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.shangyingyoupin.top/gtbfkbmups.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.yueranfly.top/gtzcyrlafu.html

Go:   os.Remove("a.txt")
来源：http://hz.c1oappe.top/gtmwaxwzok.html

Ruby: File.delete("a.txt")
来源：http://hz.andypj.xyz/gtcgcwleyv.html

C#:   File.Delete("a.txt");
来源：http://hz.jqgfzy.top/gttzizpgwc.html

[F07] 创建目录（含多级）
来源：http://hz.iojbl.cn/gtyqtgzdqn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.zhiwuduotai.top/gtwhvixzsm.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.svipenyu.cn/gtdydymrtq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.snrcjt.cn/gtqbbutsvp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.cdnleiting.top/gtbkbnmwbt.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.sxryk.cn/gtzdifihtb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.cqqwz.cn/gtbtxuhrof.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.sxryk.cn/gtuplwhmlc.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.dashuyun.cn/gtavzmqrpj.html

[F08] 遍历目录
来源：http://hz.jqgufenzy.top/gtkzoufmvg.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.tanke756.top/gtyjqtzggm.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.yj20258888.top/gthhxjjpib.html

JS:   fs.readdirSync("dir")
来源：http://hz.yonumen.top/gtsbyzhsza.html

TS:   fs.readdirSync("dir")
来源：http://hz.daria6918.cn/gtchlbnmve.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.svipenyu.cn/gtkamhqtod.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.cheryme.top/gtywjvnhtx.html

Ruby: Dir.children("dir")
来源：http://hz.jinqigfzy.top/gtktkscqhz.html

C#:   Directory.GetFiles("dir")
来源：http://hz.cucudq.cn/gtkmsoeeoo.html

[F09] 获取文件大小
来源：http://hz.pycfn.com/gtjwjttryv.html

Py:   os.path.getsize("a.txt")
来源：http://hz.havefunace.top/gtcyjbbulz.html

PHP:  filesize("a.txt");
来源：http://hz.dashuyun.cn/gtarfeklfe.html

JS:   fs.statSync("a.txt").size
来源：http://hz.yuxming.cn/gtvwgjlxdu.html

TS:   fs.statSync("a.txt").size
来源：http://hz.jinqigufen.top/gtcjpyrbvo.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.52xcode.cn/gtdbtigmsi.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.daria6918.cn/gtlzbzraif.html

Ruby: File.size("a.txt")
来源：http://hz.yanxiufei.cn/gtarnsdlji.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.xingfuxueyuan.xyz/gttspeehgb.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.hysaishi.cn/gtychlzbaa.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.hnqzz.top/gtlqdqkvjf.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.pengpengdd.cyou/gtivebvxoo.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.gzhubu.top/gtygsmrjws.html

TS:   path.extname("a.txt")
来源：http://hz.cucudq.cn/gtzrnfjryl.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.snrcjt.cn/gtvjpyguwx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.snrcjt.cn/gtianfgmpi.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.meibo888.top/gttwmpokkn.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.nanxinkj.top/gthdzxpebd.html

[F11] 复制与移动文件
来源：http://hz.wangdashe.top/gtlrmnzxaa.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.zhiwuduotai.top/gtozsakysi.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.wangshuangyany.cn/gtzmxcunrv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hnxiangtu.top/gtyajpyzyx.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xuetiantiany.cn/gtndxshkwg.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.fengsongda.top/gtrsaccajg.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jqgufenzy.top/gtdkywjmmc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.ybcxt.top/gtzlkkqfyb.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.tanke756.top/gtlcthjpjd.html

[F12] CSV 读写
来源：http://hz.zhiwuduotai.top/gthqaymkua.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.xziqi.cn/gtwsokxbyc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.hfpthk.cn/gttjovyqqo.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.zdqjudy.top/gtuprcwsax.html

TS:   // 同上
来源：http://hz.daria6918.cn/gtfrihbezb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.jinqigufen.top/gtwvrzghei.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.jinyuanbaomall.cn/gtvqnelxbw.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.yongpay.top/gtutbedubc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.kuanghao11.cn/gtorymlucp.html

================================================================================
来源：http://hz.pengpengdd.cyou/gttrgrtsdm.html

G. 面向对象
来源：http://hz.yuxming.cn/gtnoqxtauy.html

================================================================================
来源：http://hz.dashuyun.cn/gtqvjvbbhg.html

[G01] 定义类
来源：http://hz.yj20258.top/gtzzjhegdq.html

Py:   class User: pass
来源：http://hz.nwbrower.top/gtpfzpzwtu.html

PHP:  class User {}
来源：http://hz.cdnleiting.top/gtjtumgsnx.html

JS:   class User {}
来源：http://hz.9152youxi.cn/gtijgaprod.html

TS:   class User { name: string = ""; }
来源：http://hz.wangshuangyany.cn/gtzbtmfglb.html

Java: class User {}
来源：http://hz.kuanghao11.cn/gtzlhtcxyw.html

Go:   type User struct { Name string }
来源：http://hz.jinghuilouyu.cn/gtttgnfypy.html

Ruby: class User; end
来源：http://hz.ppjwa.cn/gtrytiebia.html

C#:   class User {}
来源：http://hz.zhixingplan.top/gtxvhisynd.html

[G02] 构造函数
来源：http://hz.mhx1999.top/gtrhpchtbe.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.c1oappe.top/gtnlecnudu.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.chenlongwang.top/gttelgttnn.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.guowangkeji.top/gtydndsdkm.html

TS:   constructor(public name: string) {}
来源：http://hz.guannengcc.top/gtynqmsjmw.html

Java: User(String name) { this.name = name; }
来源：http://hz.52xcode.cn/gtuivftkir.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.zhiwuduotai.top/gtqonutwpg.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.dianchejie.cn/gtnizggcnj.html

C#:   public User(string name) { Name = name; }
来源：http://hz.shuidangran.top/gtdaqtovbc.html

[G03] 实例属性
来源：http://hz.yj20258888.top/gtpxxaejlc.html

Py:   self.name = "x"
来源：http://hz.pycfn.com/gtlungixqm.html

PHP:  public string $name = "x";
来源：http://hz.bjfxy.top/gtyosjucwp.html

JS:   this.name = "x";
来源：http://hz.ywan-chungtsiang.top/gtkduuqwkq.html

TS:   name: string = "x";
来源：http://hz.dashuyun.cn/gtadilcfxj.html

Java: private String name;
来源：http://hz.ydzc1.top/gtyoceiwfd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.aizwys.cn/gtlasdnbyf.html

Ruby: @name = "x"
来源：http://hz.quarkkingdee.top/gtedpbjbrq.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.316326.xyz/gtedkoduwk.html

[G04] 定义方法
来源：http://hz.c1oappe.top/gthetixukb.html

Py:   def greet(self): return self.name
来源：http://hz.c1oappe.top/gtksbkqzjd.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yj202588.top/gtilynaikm.html

JS:   greet() { return this.name; }
来源：http://hz.hysaishi.cn/gtxaohgvas.html

TS:   greet(): string { return this.name; }
来源：http://hz.tianlin.xyz/gtwxyqjsqf.html

Java: String greet() { return name; }
来源：http://hz.jinyuanbaomall.cn/gtleffopkm.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.shzxlz.cn/gtnksoylep.html

Ruby: def greet; @name; end
来源：http://hz.jinqigufen.top/gtypdsftbs.html

C#:   public string Greet() => Name;
来源：http://hz.hongshengwenyu.top/gtmwufhqoe.html

[G05] 继承
来源：http://hz.havefunace.top/gtluwmegcy.html

Py:   class Admin(User): pass
来源：http://hz.ywan-chungtsiang.top/gthuqraprr.html

PHP:  class Admin extends User {}
来源：http://hz.hnxiangtu.top/gtykidqeul.html

JS:   class Admin extends User {}
来源：http://hz.xylfe.cn/gtxtsgxxcu.html

TS:   class Admin extends User {}
来源：http://hz.ybcxt.top/gtyjewfrko.html

Java: class Admin extends User {}
来源：http://hz.pengpengdd.cyou/gtdxlslzqb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.jinghuilouyu.cn/gtrkjwtrsk.html

Ruby: class Admin < User; end
来源：http://hz.hongshengwenyu.top/gtuhecejik.html

C#:   class Admin : User {}
来源：http://hz.xylfe.cn/gtjsmwqpgk.html

[G06] 重写方法
来源：http://hz.hysaishi.cn/gtbdsihdyd.html

Py:   def greet(self): return "admin"
来源：http://hz.andypj.xyz/gtltzddleg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jinqigfzy.top/gtiiydauis.html

JS:   greet() { return "admin"; }
来源：http://hz.cucudq.cn/gtukbmgvsk.html

TS:   greet(): string { return "admin"; }
来源：http://hz.feifeiyinyue.top/gtbeppmxyb.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jlsjyb.cn/gtrmeknvki.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.xuanzx.com/gtynprlxzu.html

Ruby: def greet; "admin"; end
来源：http://hz.hfpthk.cn/gtcyedwgar.html

C#:   public override string Greet() => "admin";
来源：http://hz.zhoulong.xyz/gtthzhxfrk.html

[G07] 调用父类方法
来源：http://hz.pengpengdd.cyou/gtwyrbqeyp.html

Py:   super().greet()
来源：http://hz.jinqigfzy.top/gtljwofnli.html

PHP:  parent::greet();
来源：http://hz.aibaodan.cn/gtglierzfs.html

JS:   super.greet();
来源：http://hz.yj202588.top/gtycfyqeqh.html

TS:   super.greet();
来源：http://hz.cucudq.cn/gtineblhpd.html

Java: super.greet();
来源：http://hz.yj20258888.top/gtvrnqntmz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.quarkkingdee.top/gtmioslpbn.html

Ruby: super
来源：http://hz.sxryk.cn/gtsyuemrwk.html

C#:   base.Greet();
来源：http://hz.yj20258.top/gtceketxbi.html

[G08] 静态方法与属性
来源：http://hz.sweek.top/gtkdewrbcb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jinqigfzy.top/gtlvjvrxgz.html

PHP:  public static function f() {}
来源：http://hz.smart0.xyz/gtwtxnrcqt.html

JS:   static f() {}
来源：http://hz.jinghuilouyu.cn/gtxhwuwbyj.html

TS:   static f(): void {}
来源：http://hz.yonumen.top/gtcdkaoqej.html

Java: static void f() {}
来源：http://hz.tanke756.top/gtjoeygulb.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.gogol.net.cn/gtwsoerpvo.html

Ruby: def self.f; end
来源：http://hz.wangdashe.top/gtbaupwrlj.html

C#:   public static void F() {}
来源：http://hz.snrcjt.cn/gtvgqbirfp.html

[G09] 接口 / 抽象类
来源：http://hz.shzxlz.cn/gtframibda.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yanxiufei.cn/gtgmqlfejp.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.chenlongwang.top/gtxvuvydri.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.haohaochexian.top/gtjwhcophx.html

TS:   interface Shape { area(): number; }
来源：http://hz.xingfuxueyuan.xyz/gtfuactipe.html

Java: interface Shape { double area(); }
来源：http://hz.jiagoushi.top/gtmmucrkvr.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yvedp.cn/gtlblnzmoh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.zhengqikj.top/gtincotfjl.html

C#:   interface IShape { double Area(); }
来源：http://hz.chenlongwang.top/gthqyvtwxc.html

[G10] 访问控制
来源：http://hz.jinyuanbaomall.cn/gtawrefitb.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.hywenlv.cn/gtzefqkvos.html

PHP:  public / protected / private
来源：http://hz.wangshuangyany.cn/gtivxtrbdi.html

JS:   #private 字段；其余公开
来源：http://hz.ehwqpu.com/gtplabzbpm.html

TS:   public / protected / private
来源：http://hz.dianchejie.cn/gtenqndchd.html

Java: public / protected / private / 默认包级
来源：http://hz.ydjk.org.cn/gtletbihqz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.shzxlz.cn/gtsuedoscl.html

Ruby: public / protected / private
来源：http://hz.zhijiandao.cn/gtgdonagta.html

C#:   public / protected / private / internal
来源：http://hz.zhijiandao.cn/gthctliisi.html

[G11] getter / setter
来源：http://hz.mhx1999.top/gtvzazaqbh.html

Py:   @property 与 @x.setter
来源：http://hz.hywenlv.cn/gttftxtewf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.guannengcc.top/gtlljrietq.html

JS:   get name() { return this._name; }
来源：http://hz.0kj1m.cn/gtczjydfms.html

TS:   get name(): string { return this._name; }
来源：http://hz.gaohongyu789.top/gtxenfpjpc.html

Java: public String getName() { return name; }
来源：http://hz.pengpengdd.cyou/gtghkrkjku.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.zhaomingkeji.xyz/gtzpsdfdgn.html

Ruby: attr_accessor :name
来源：http://hz.chenlongwang.top/gtgbyfgdqr.html

C#:   public string Name { get; set; }
来源：http://hz.jinyuanbaomall.cn/gtcpioofjc.html

[G12] 对象转字符串
来源：http://hz.jiagoushi.top/gtpogpwtbe.html

Py:   def __str__(self): return self.name
来源：http://hz.zycfv.cn/gtimhocjxz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jiagoushi.top/gtrpzutijr.html

JS:   toString() { return this.name; }
来源：http://hz.xziqi.cn/gtiixzggfl.html

TS:   toString(): string { return this.name; }
来源：http://hz.jqgfzy.top/gtclfmaszo.html

Java: @Override public String toString() { return name; }
来源：http://hz.tian-w.cn/gtllglbzbf.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.shzxlz.cn/gtkxtgsmfy.html

Ruby: def to_s; @name; end
来源：http://hz.52xcode.cn/gtcgkpomht.html

C#:   public override string ToString() => Name;
来源：http://hz.xinyue.icu/gtrkfitxut.html

[G13] 判断对象类型
来源：http://hz.jqgufenzy.top/gtafypwhxg.html

Py:   isinstance(u, User)
来源：http://hz.zdqjudy.top/gtviegcijf.html

PHP:  $u instanceof User
来源：http://hz.gaohongyu789.top/gttzazlkpx.html

JS:   u instanceof User
来源：http://hz.zhiwuduotai.top/gtpoiwctzg.html

TS:   u instanceof User
来源：http://hz.yongpay.top/gtcagzrlbs.html

Java: u instanceof User
来源：http://hz.52xcode.cn/gtuafgghwp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yangfankeji.com/gtmkecmekr.html

Ruby: u.is_a?(User)
来源：http://hz.nwbrower.top/gtprrtarkn.html

C#:   u is User
来源：http://hz.ydjk.org.cn/gtryofamrs.html

[G14] 数据类 / record
来源：http://hz.jiagoushi.top/gtomsykbrv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.quarkkingdee.top/gtloptpvgz.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.zhaomingkeji.xyz/gtryzwqyrz.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.cheryme.top/gtqzkvxrha.html

TS:   type User = { name: string; age: number };
来源：http://hz.yongpay.top/gttwhynpil.html

Java: record User(String name, int age) {}
来源：http://hz.tianlin.xyz/gtezaaxzzz.html

Go:   type User struct { Name string; Age int }
来源：http://hz.feifeiyinyue.top/gtpsfchclo.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jianghu66.top/gtbrbgwnex.html

C#:   record User(string Name, int Age);
来源：http://hz.jinyuanbaomall.cn/gttamnfzxl.html

[G15] 枚举
来源：http://hz.nwbrower.top/gtmrxfwvpa.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.fzhhl.top/gtyjpcmkpf.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.yonumen.top/gtrzetgjiv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.xuetiantiany.cn/gtgdazmydx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.nanxinkj.top/gtqrhhtohf.html

Java: enum Color { RED, GREEN }
来源：http://hz.shzxlz.cn/gtdamjrxlk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.fzhhl.top/gtqrzbnrls.html

Ruby: Color = %i[red green].freeze
来源：http://hz.guannengcc.top/gtaegfhucu.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jinyuanbaomall.cn/gtgsaimneq.html

[G16] 对象转数组 / 字典
来源：http://hz.nanxuanxn.top/gtlxehapqf.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.zhengqikj.top/gtjvpgxdub.html

PHP:  get_object_vars($obj);
来源：http://hz.zycfv.cn/gttxgpbrhk.html

JS:   Object.entries(obj)
来源：http://hz.tanke756.top/gtarqlbyda.html

TS:   Object.entries(obj)
来源：http://hz.zhixingplan.top/gtvdgfmvmp.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.shanyushiyangkeji.top/gtrwjhrnss.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.iojbl.cn/gtftsjyqov.html

Ruby: obj.instance_variables
来源：http://hz.smart0.xyz/gteaoxkwbv.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.tian-w.cn/gtnmbuhpik.html

================================================================================
来源：http://hz.birdmap.top/gtsvmachdh.html

H. 异常与错误处理
来源：http://hz.ydzc1.top/gtgknstnpx.html

================================================================================
来源：http://hz.fengsongda.top/gtgdafdotw.html

[H01] try / catch 基础
来源：http://hz.smart0.xyz/gttlhwfbqz.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.wangshuangyany.cn/gtirnnwkww.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.feifeiyinyue.top/gtyakipapa.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.jyoumei.cn/gtxorzyzst.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jlsjyb.cn/gtswjaavmg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.daxiang520.top/gtgkobqybv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yueranfly.top/gtzqgrnckm.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.gotoacloud.top/gtlurjcvjk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.jyoumei.cn/gtiddgwbzu.html

[H02] finally / ensure 收尾
来源：http://hz.ppjwa.cn/gtyglnsrez.html


<!-- 参考信息 -->