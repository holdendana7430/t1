代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.zhijiandao.cn/gttkqepvcu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.zhaomingkeji.xyz/gtnkrcylsm.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.ivvv.top/gtzhpwnooy.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.xingfuxueyuan.xyz/gtnznoujqc.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.tanke756.top/gtljbrazgq.html

[E19] 多行文本按行拆分
来源：http://hz.yuanzhike.top/gtufshecmv.html

Py:   s.splitlines()
来源：http://hz.jinghuilouyu.cn/gtpupaproo.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.hnxiangtu.top/gturqmuulb.html

JS:   s.split(/\r?\n/)
来源：http://hz.cheryme.top/gtowvhfitt.html

TS:   s.split(/\r?\n/)
来源：http://hz.yj20258888.top/gtvqkazkfo.html

Java: s.lines().toList()
来源：http://hz.yanxiufei.cn/gtbotxjrib.html

Go:   strings.Split(s, "\n")
来源：http://hz.shuidangran.top/gtnrlaowhu.html

Ruby: s.lines
来源：http://hz.zhengqikj.top/gtbzezhzpk.html

C#:   s.Split('\n')
来源：http://hz.zhiwuduotai.top/gtvyhklxdk.html

[E20] 判断字符串是否为空
来源：http://hz.c1oappe.top/gtxqsdxiah.html

Py:   if not s:
来源：http://hz.shzxlz.cn/gttpwwfaix.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.yangfankeji.com/gtjusqmpwo.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.52xcode.cn/gtenwknouc.html

TS:   if (s === "") {}
来源：http://hz.shangyingyoupin.top/gtmcppgelu.html

Java: if (s.isEmpty()) {}
来源：http://hz.yuanzhike.top/gtelgettdu.html

Go:   if s == "" {}
来源：http://hz.guannengcc.top/gtzrnerlrv.html

Ruby: if s.empty?
来源：http://hz.gaohongyu789.top/gtaktmohfu.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.cashguo.top/gtnriwxuux.html

[E21] 超长截断加省略号
来源：http://hz.snrcjt.cn/gtslrgudef.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.tanke756.top/gtbnevhhnh.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.wangshuangyany.cn/gtfqffpzmj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.fzhhl.top/gtlsiwloiy.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.kuanghao11.cn/gtrumjbild.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.jqgufenzy.top/gtohajimjk.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.tian-w.cn/gtvzfmqrsl.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.yanxiufei.cn/gtesrpijsp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.jinyuanbaomall.cn/gttgogfvuj.html

[E22] 字节长度与字符长度
来源：http://hz.jinghuilouyu.cn/gtxxieawxq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.mhx1999.top/gtnpinqekk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yuxming.cn/gtxkbqjcji.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yj20258.top/gtutxlawap.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jinyuanbaomall.cn/gtexnmtnqg.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.yj20258.top/gthyxekeqn.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.jinqigufen.top/gtjuzoutbs.html

Ruby: s.bytesize;  s.length
来源：http://hz.redwolf501.top/gtswuzbjnn.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.shanyushiyangtech.top/gtgyjtmapb.html

================================================================================
来源：http://hz.fzhhl.top/gtdexojmyu.html

F. 文件与目录
来源：http://hz.cqqwz.cn/gtdjhymrxu.html

================================================================================
来源：http://hz.cdnleiting.top/gtcxcwzcyb.html

[F01] 读取整个文件
来源：http://hz.yueranfly.top/gtcmedjgvs.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.ehwqpu.com/gtkcpqwkzm.html

PHP:  file_get_contents("a.txt");
来源：http://hz.xuetiantiany.cn/gtkahgqqmw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.yangfankeji.com/gtbpxwebdd.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.cashguo.top/gtahwvsegg.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.mhx1999.top/gtofnuqkla.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.sysykeji.top/gtzeoipgnt.html

Ruby: File.read("a.txt")
来源：http://hz.fzhhl.top/gtublkvpqw.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.chenlongwang.top/gtewzahcsm.html

[F02] 逐行读取文件
来源：http://hz.xziqi.cn/gtwabkccxn.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.hnxiangtu.top/gtzmygwlij.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.shangyingyoupin.top/gtoythyxqx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jianghu66.top/gtrkznhyti.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.cdnleiting.top/gtecgybuvq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.jinghuilouyu.cn/gtxsocicrr.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.nanxinkj.top/gtabrpdzni.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.nanxinkj.top/gtwuxjoxwj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.chenlongwang.top/gtniumwtii.html

[F03] 写入文件（覆盖）
来源：http://hz.ivvv.top/gtqdhukdoy.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.xuetiantiany.cn/gtqicutadq.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.snrcjt.cn/gtosgmgrkw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yueranfly.top/gtvoowdtgl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.cucudq.cn/gttejjgtyr.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.yonumen.top/gtskupnyqc.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.andypj.xyz/gtsnyedcon.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.chenzaomai.com/gtgsiuduex.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.hywenlv.cn/gthbhduhxy.html

[F04] 追加写入文件
来源：http://hz.sweek.top/gtpqpotvgl.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.vqdsnc.cn/gttiudiqbw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.redwolf501.top/gtkvbywvck.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jianghu66.top/gtuhuoqazx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.tian-w.cn/gtivvgkusf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.hysaishi.cn/gturdtpesi.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.yanxiufei.cn/gtdiccnpwp.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.aibaodan.cn/gtavhbcype.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.havefunace.top/gtqzcoxtdf.html

[F05] 判断文件或目录是否存在
来源：http://hz.ywan-chungtsiang.top/gttgrzoyax.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.kuanghao11.cn/gtypchgtcz.html

PHP:  file_exists("a.txt");
来源：http://hz.zhongyouzk.top/gtezgklbce.html

JS:   fs.existsSync("a.txt")
来源：http://hz.cucudq.cn/gtxnoeblhv.html

TS:   fs.existsSync("a.txt")
来源：http://hz.hnxiangtu.top/gtmgflxept.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.gotoacloud.top/gtexsyaufm.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.shzxlz.cn/gtgcspyooo.html

Ruby: File.exist?("a.txt")
来源：http://hz.ivvv.top/gtuarszqln.html

C#:   File.Exists("a.txt")
来源：http://hz.yuanzhike.top/gtgcjunpnm.html

[F06] 删除文件
来源：http://hz.yj20258888.top/gthoodinme.html

Py:   os.remove("a.txt")
来源：http://hz.zdqjudy.top/gtikvrqizh.html

PHP:  unlink("a.txt");
来源：http://hz.cheryme.top/gtuowesgyr.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.gaohongyu789.top/gtaxhvubjt.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.xuetiantiany.cn/gtklullqgk.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.yj20258.top/gtvrzgyqtf.html

Go:   os.Remove("a.txt")
来源：http://hz.xziqi.cn/gtlhwcarta.html

Ruby: File.delete("a.txt")
来源：http://hz.jiagoushi.top/gthwynnqlb.html

C#:   File.Delete("a.txt");
来源：http://hz.shzxlz.cn/gtjiglthjz.html

[F07] 创建目录（含多级）
来源：http://hz.jinqigufen.top/gtafgyucla.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.svipenyu.cn/gtlnedcxyn.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.shangyingyoupin.top/gtbdveqpba.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.316326.xyz/gtqborzlhu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhaomingkeji.xyz/gtvzyrksvv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.xylfe.cn/gtajvpyafv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.wangshuangyany.cn/gtuqhzgmix.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.zhongyouzk.top/gtymoghuzk.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.chenlongwang.top/gtrucikboa.html

[F08] 遍历目录
来源：http://hz.nwbrower.top/gteimhdeiz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.redwolf501.top/gtqohzorpe.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.wangshuangyany.cn/gtkjutkhrm.html

JS:   fs.readdirSync("dir")
来源：http://hz.yuanzhike.top/gtrsqxrxey.html

TS:   fs.readdirSync("dir")
来源：http://hz.yangfankeji.com/gtdobxgntr.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.yanxiufei.cn/gtvpsjhpjg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.dianchejie.cn/gtyiidhbhn.html

Ruby: Dir.children("dir")
来源：http://hz.ybcxt.top/gtfgaouled.html

C#:   Directory.GetFiles("dir")
来源：http://hz.cdnleiting.top/gtopwqkjep.html

[F09] 获取文件大小
来源：http://hz.iojbl.cn/gtwlqykwet.html

Py:   os.path.getsize("a.txt")
来源：http://hz.hammf.cn/gthxgwejxj.html

PHP:  filesize("a.txt");
来源：http://hz.gaohongyu789.top/gtesiezzny.html

JS:   fs.statSync("a.txt").size
来源：http://hz.yuanzhike.top/gtiwnnlglu.html

TS:   fs.statSync("a.txt").size
来源：http://hz.mhx1999.top/gtbusizqnx.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.cashguo.top/gtndiasfxi.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.birdmap.top/gtmixweglu.html

Ruby: File.size("a.txt")
来源：http://hz.ydjk.org.cn/gtutpqzmjs.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yvedp.cn/gtfqgxmqyb.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.guannengcc.top/gtiemwzltb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jinqigfzy.top/gtqnazoqqt.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.yj20258888.top/gtzvqzukls.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.shangyingyoupin.top/gtygivljnq.html

TS:   path.extname("a.txt")
来源：http://hz.nanxuanxn.top/gtolvsxurp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.jinyuanbaomall.cn/gtmgtyrkry.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yuxming.cn/gtjlytllsm.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.xuanzx.com/gtnpnhtlsq.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.zhiwuduotai.top/gtukihmsqx.html

[F11] 复制与移动文件
来源：http://hz.shzxlz.cn/gtmeetvtgp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.ehwqpu.com/gttobvqewm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.dianchejie.cn/gtcivhtdvo.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zdqjudy.top/gttuqvisvv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xuetiantiany.cn/gtsbawtbja.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.aibaodan.cn/gtrpvcosdf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.sufxvd.cn/gtavgxdrpz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.meibo888.top/gtwpsyazya.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.gogol.net.cn/gtvyrawcnl.html

[F12] CSV 读写
来源：http://hz.tanke756.top/gtmwddxgtp.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.xingfuxueyuan.xyz/gtdfpyklts.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.guowangkeji.top/gttpejycov.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yangfankeji.com/gtemagqlqp.html

TS:   // 同上
来源：http://hz.hywenlv.cn/gtnsgguolz.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.hfpthk.cn/gtixcrckxb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.redwolf501.top/gtdmiagorv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.hnqzz.top/gteeaifsjd.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jqgufenzy.top/gthiarynnj.html

================================================================================
来源：http://hz.ehwqpu.com/gtvbybvxqa.html

G. 面向对象
来源：http://hz.zhongyouzk.top/gtpjyyilck.html

================================================================================
来源：http://hz.sysykeji.top/gtgdcfvgff.html

[G01] 定义类
来源：http://hz.chenjidiqi.icu/gtfljlummg.html

Py:   class User: pass
来源：http://hz.c1oappe.top/gtwqmtqwpe.html

PHP:  class User {}
来源：http://hz.ydzc1.top/gtybvxylgp.html

JS:   class User {}
来源：http://hz.daria6918.cn/gtgwbwjurb.html

TS:   class User { name: string = ""; }
来源：http://hz.tanke756.top/gtburqzdxw.html

Java: class User {}
来源：http://hz.cashguo.top/gthiqhbeya.html

Go:   type User struct { Name string }
来源：http://hz.birdmap.top/gtluceerso.html

Ruby: class User; end
来源：http://hz.hfpthk.cn/gtqaphlame.html

C#:   class User {}
来源：http://hz.smart0.xyz/gtwggxovtj.html

[G02] 构造函数
来源：http://hz.dashuyun.cn/gtyzqsatpq.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yvedp.cn/gtarubkalu.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.jinyuanbaomall.cn/gtyndlxgny.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.gzhubu.top/gtcnokqkpj.html

TS:   constructor(public name: string) {}
来源：http://hz.yj20258888.top/gtselnbbjp.html

Java: User(String name) { this.name = name; }
来源：http://hz.sufxvd.cn/gtjyqiczff.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.hywenlv.cn/gtkganbkbe.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yj20258888.top/gtmcaoferc.html

C#:   public User(string name) { Name = name; }
来源：http://hz.jqgufenzy.top/gtlgpqozya.html

[G03] 实例属性
来源：http://hz.fzhhl.top/gtgizdaclj.html

Py:   self.name = "x"
来源：http://hz.svipenyu.cn/gtdrgkfkav.html

PHP:  public string $name = "x";
来源：http://hz.zhaomingkeji.xyz/gtcpnjqhez.html

JS:   this.name = "x";
来源：http://hz.fengsongda.top/gtlkvayphx.html

TS:   name: string = "x";
来源：http://hz.jinyuanbaomall.cn/gtqtlzhrim.html

Java: private String name;
来源：http://hz.zycfv.cn/gtazantkfb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.ywan-chungtsiang.top/gtfmdmdgzx.html

Ruby: @name = "x"
来源：http://hz.ivvv.top/gtugjbutpc.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.zhiwuduotai.top/gtohclmqhb.html

[G04] 定义方法
来源：http://hz.tian-w.cn/gthqmzduvx.html

Py:   def greet(self): return self.name
来源：http://hz.gogol.net.cn/gtqwyxlqal.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.jianghu66.top/gttuzemhcx.html

JS:   greet() { return this.name; }
来源：http://hz.zhoulong.xyz/gtcmufinuy.html

TS:   greet(): string { return this.name; }
来源：http://hz.hammf.cn/gtbmpjnxks.html

Java: String greet() { return name; }
来源：http://hz.cqqwz.cn/gtjzmcsfaa.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.hfpthk.cn/gtfjwhrazi.html

Ruby: def greet; @name; end
来源：http://hz.0kj1m.cn/gtzxhrxlle.html

C#:   public string Greet() => Name;
来源：http://hz.cucudq.cn/gtgdosljxy.html

[G05] 继承
来源：http://hz.jinyuanbaomall.cn/gtyexjogpv.html

Py:   class Admin(User): pass
来源：http://hz.bjfxy.top/gtcxdwrtxg.html

PHP:  class Admin extends User {}
来源：http://hz.aibaodan.cn/gthdghccyw.html

JS:   class Admin extends User {}
来源：http://hz.mhx1999.top/gttjzbatvh.html

TS:   class Admin extends User {}
来源：http://hz.yueranfly.top/gtfafzwthq.html

Java: class Admin extends User {}
来源：http://hz.shuidangran.top/gtttketrjm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.c1oappe.top/gtowatxbdq.html

Ruby: class Admin < User; end
来源：http://hz.zhijiandao.cn/gtuttsigez.html

C#:   class Admin : User {}
来源：http://hz.wangdashe.top/gtntwldxdw.html

[G06] 重写方法
来源：http://hz.yvedp.cn/gtyzfgmqvc.html

Py:   def greet(self): return "admin"
来源：http://hz.tian-w.cn/gtoyhuidrf.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.zhijiandao.cn/gtdxqcwfre.html

JS:   greet() { return "admin"; }
来源：http://hz.chenlongwang.top/gtpbhhpozd.html

TS:   greet(): string { return "admin"; }
来源：http://hz.fzhhl.top/gtpfweizws.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.tianlin.xyz/gtunqqfumx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.yuxming.cn/gtnriizofa.html

Ruby: def greet; "admin"; end
来源：http://hz.zhongyouzk.top/gtrsbwmaih.html

C#:   public override string Greet() => "admin";
来源：http://hz.tian-w.cn/gtouvrvnif.html

[G07] 调用父类方法
来源：http://hz.hongshengwenyu.top/gtlazuschk.html

Py:   super().greet()
来源：http://hz.guowangkeji.top/gtzwsmkczo.html

PHP:  parent::greet();
来源：http://hz.vqdsnc.cn/gtdauvwrvc.html

JS:   super.greet();
来源：http://hz.jqgfzy.top/gtrxszvbyb.html

TS:   super.greet();
来源：http://hz.316326.xyz/gtqsimhpxn.html

Java: super.greet();
来源：http://hz.gzhubu.top/gtbtaburag.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.feifeiyinyue.top/gtfoxwpobi.html

Ruby: super
来源：http://hz.jyoumei.cn/gtlzeotfky.html

C#:   base.Greet();
来源：http://hz.zhiwuduotai.top/gtsmpshvle.html

[G08] 静态方法与属性
来源：http://hz.tian-w.cn/gtdevvknui.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.cheryme.top/gtcdqvdwjg.html

PHP:  public static function f() {}
来源：http://hz.wangshuangyany.cn/gtiscaxolk.html

JS:   static f() {}
来源：http://hz.yangfankeji.com/gthtluoeyh.html

TS:   static f(): void {}
来源：http://hz.daria6918.cn/gtnitqskut.html

Java: static void f() {}
来源：http://hz.snrcjt.cn/gtozhcoacy.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jlsjyb.cn/gtzokxwwgt.html

Ruby: def self.f; end
来源：http://hz.yongpay.top/gtyaprdksr.html

C#:   public static void F() {}
来源：http://hz.cqqwz.cn/gtvuwimbqh.html

[G09] 接口 / 抽象类
来源：http://hz.sufxvd.cn/gtisiwzvsw.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.iojbl.cn/gttigiomgr.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.quarkkingdee.top/gtqelsipub.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.guowangkeji.top/gtnwmhybcp.html

TS:   interface Shape { area(): number; }
来源：http://hz.cdnleiting.top/gtdlyhkuah.html

Java: interface Shape { double area(); }
来源：http://hz.xinyue.icu/gtsmqitnsi.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.xuanzx.com/gtiyykalbv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.hnxiangtu.top/gtrurvvdqy.html

C#:   interface IShape { double Area(); }
来源：http://hz.yangfankeji.com/gtajjblfst.html

[G10] 访问控制
来源：http://hz.yongpay.top/gtfawfbwwv.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.havefunace.top/gtdpcwvmkm.html

PHP:  public / protected / private
来源：http://hz.quarkkingdee.top/gtaxufzkgi.html

JS:   #private 字段；其余公开
来源：http://hz.bjfxy.top/gtojabntvh.html

TS:   public / protected / private
来源：http://hz.iojbl.cn/gtjvofxldl.html

Java: public / protected / private / 默认包级
来源：http://hz.yongpay.top/gtietxicxf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.xylfe.cn/gtmodfmztf.html

Ruby: public / protected / private
来源：http://hz.wangdashe.top/gtxgvwzkfe.html

C#:   public / protected / private / internal
来源：http://hz.chenlongwang.top/gtozexykgd.html

[G11] getter / setter
来源：http://hz.jlsjyb.cn/gtzqahhozx.html

Py:   @property 与 @x.setter
来源：http://hz.cheryme.top/gtuymqmgiv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.pycfn.com/gtjbemyyml.html

JS:   get name() { return this._name; }
来源：http://hz.xuetiantiany.cn/gtuciavsej.html

TS:   get name(): string { return this._name; }
来源：http://hz.kuanghao11.cn/gtfjmfnkii.html

Java: public String getName() { return name; }
来源：http://hz.jqgufenzy.top/gtatzfizaa.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.sxryk.cn/gtfniecnsn.html

Ruby: attr_accessor :name
来源：http://hz.c1oappe.top/gtjiojtfrk.html

C#:   public string Name { get; set; }
来源：http://hz.yj20258888.top/gtajngyobz.html

[G12] 对象转字符串
来源：http://hz.birdmap.top/gtowjaxobt.html

Py:   def __str__(self): return self.name
来源：http://hz.tianlin.xyz/gtoomxrlnn.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.ppjwa.cn/gtzzvzgdpx.html

JS:   toString() { return this.name; }
来源：http://hz.jianghu66.top/gtbwzfavxj.html

TS:   toString(): string { return this.name; }
来源：http://hz.jinqigfzy.top/gtzsiijssq.html

Java: @Override public String toString() { return name; }
来源：http://hz.shanyushiyangtech.top/gtgtvkkyld.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.ehwqpu.com/gtxpgqxufu.html

Ruby: def to_s; @name; end
来源：http://hz.gotoacloud.top/gtcsmdcama.html

C#:   public override string ToString() => Name;
来源：http://hz.cucudq.cn/gtuzrjeqdw.html

[G13] 判断对象类型
来源：http://hz.yueranfly.top/gtoptpsvdb.html

Py:   isinstance(u, User)
来源：http://hz.haohaochexian.top/gtppmucmmo.html

PHP:  $u instanceof User
来源：http://hz.sweek.top/gtjrzqrpey.html

JS:   u instanceof User
来源：http://hz.vqdsnc.cn/gtillwbsfb.html

TS:   u instanceof User
来源：http://hz.yueranfly.top/gtdjtthokk.html

Java: u instanceof User
来源：http://hz.fzhhl.top/gttranuemn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.nanxuanxn.top/gtfgnpczoh.html

Ruby: u.is_a?(User)
来源：http://hz.zhijiandao.cn/gtcfyuwkef.html

C#:   u is User
来源：http://hz.yonumen.top/gtpofdwipi.html

[G14] 数据类 / record
来源：http://hz.yanxiufei.cn/gtggvgjvqm.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.dashuyun.cn/gtxgspxdoj.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.nwbrower.top/gtkoqrskqz.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.zhengqikj.top/gtbwibgrhm.html

TS:   type User = { name: string; age: number };
来源：http://hz.9152youxi.cn/gtavbpvvmx.html

Java: record User(String name, int age) {}
来源：http://hz.birdmap.top/gtztpdvtal.html

Go:   type User struct { Name string; Age int }
来源：http://hz.zhoulong.xyz/gtpazzlaoa.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.hongshengwenyu.top/gtoowswsax.html

C#:   record User(string Name, int Age);
来源：http://hz.0kj1m.cn/gtqhwgvipz.html

[G15] 枚举
来源：http://hz.shanyushiyangtech.top/gtqxqkhqol.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.kuanghao11.cn/gtqvcsmuyx.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.sxryk.cn/gttdohyvuh.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.tianlin.xyz/gtefyrlrrv.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.guannengcc.top/gtqwsptsdp.html

Java: enum Color { RED, GREEN }
来源：http://hz.daria6918.cn/gtjuvykkep.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.zdqjudy.top/gtruxcucyk.html

Ruby: Color = %i[red green].freeze
来源：http://hz.dianchejie.cn/gthqjteivj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.cqqwz.cn/gtzrmsokyo.html

[G16] 对象转数组 / 字典
来源：http://hz.nanxuanxn.top/gtyxbuazrg.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.cheryme.top/gtnwwfpcdb.html

PHP:  get_object_vars($obj);
来源：http://hz.yj20258888.top/gtukxtugqd.html

JS:   Object.entries(obj)
来源：http://hz.zhixingplan.top/gtqfrthcxu.html

TS:   Object.entries(obj)
来源：http://hz.cashguo.top/gtmyheuhwh.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.aizwys.cn/gtgiwbxdch.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.sufxvd.cn/gtqldyyhjk.html

Ruby: obj.instance_variables
来源：http://hz.nwbrower.top/gtyblgzdgm.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.ehwqpu.com/gtyeikzpyx.html

================================================================================
来源：http://hz.mhx1999.top/gtqlebrlwh.html


<!-- 参考信息 -->