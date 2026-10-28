代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.meibo888.top/gtsxbogrvq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.0kj1m.cn/gtryttqfts.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.zhongyouzk.top/gtbvfzudtg.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.xziqi.cn/gtxafcnqmg.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.9152youxi.cn/gtfrngtugi.html

[E19] 多行文本按行拆分
来源：http://hz.dashuyun.cn/gtiaxegxob.html

Py:   s.splitlines()
来源：http://hz.zdqjudy.top/gtjsetbdez.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.cdnleiting.top/gtoavnovld.html

JS:   s.split(/\r?\n/)
来源：http://hz.jyoumei.cn/gtfacbxlqd.html

TS:   s.split(/\r?\n/)
来源：http://hz.ppjwa.cn/gtehvvpnrd.html

Java: s.lines().toList()
来源：http://hz.jinqigufen.top/gtkpabbiyv.html

Go:   strings.Split(s, "\n")
来源：http://hz.shzxlz.cn/gtlzutyotv.html

Ruby: s.lines
来源：http://hz.ywan-chungtsiang.top/gtisgprywx.html

C#:   s.Split('\n')
来源：http://hz.pengpengdd.cyou/gturfvxbic.html

[E20] 判断字符串是否为空
来源：http://hz.chenjidiqi.icu/gtbqdcbvqy.html

Py:   if not s:
来源：http://hz.xziqi.cn/gtshixujtj.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.ywan-chungtsiang.top/gtrdskzzii.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.jinghuilouyu.cn/gtlehleaxm.html

TS:   if (s === "") {}
来源：http://hz.52xcode.cn/gtpwxvzgce.html

Java: if (s.isEmpty()) {}
来源：http://hz.yonumen.top/gthejzjjmq.html

Go:   if s == "" {}
来源：http://hz.hammf.cn/gttlzrhllh.html

Ruby: if s.empty?
来源：http://hz.jqgfzy.top/gturaorzsf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.nanxuanxn.top/gtjgwxjosc.html

[E21] 超长截断加省略号
来源：http://hz.sysykeji.top/gtxiuygwbi.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.cheryme.top/gtvkrnggoe.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.fzhhl.top/gthefhjtxm.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.wangshuangyany.cn/gtwtsbxafc.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.nwbrower.top/gtuadxgtpk.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.daria6918.cn/gtsfmodsnh.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.hywenlv.cn/gtkrddizip.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.vqdsnc.cn/gtaasnfckf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.jqgfzy.top/gtdbwkcalw.html

[E22] 字节长度与字符长度
来源：http://hz.bjfxy.top/gtgisjkxeu.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.hammf.cn/gtoocnxyfw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.nanxuanxn.top/gtohimnjgs.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jianghu66.top/gtpbswxptv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.gogol.net.cn/gtfwftfqcw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jianghu66.top/gtqvcqpnwd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.gzhubu.top/gttsscxrkj.html

Ruby: s.bytesize;  s.length
来源：http://hz.wangdashe.top/gtesmlwvop.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.jinqigfzy.top/gthlciusup.html

================================================================================
来源：http://hz.cucudq.cn/gtzjvwulyq.html

F. 文件与目录
来源：http://hz.jianghu66.top/gtkwractyp.html

================================================================================
来源：http://hz.hywenlv.cn/gtemxhsevv.html

[F01] 读取整个文件
来源：http://hz.tianlin.xyz/gtyuffdacw.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yuanzhike.top/gtrqiecmxa.html

PHP:  file_get_contents("a.txt");
来源：http://hz.zhengqikj.top/gtxddnujct.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.ybcxt.top/gtbakafcjj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.jyoumei.cn/gtlvptarnn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.hongshengwenyu.top/gtegemehhy.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.xingfuxueyuan.xyz/gtvbtdnyso.html

Ruby: File.read("a.txt")
来源：http://hz.shuidangran.top/gtlkkrgwxq.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yueranfly.top/gtctphqglk.html

[F02] 逐行读取文件
来源：http://hz.gotoacloud.top/gtbhmgskuq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.hnxiangtu.top/gtxlsqxrbg.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.wangshuangyany.cn/gthkppzqoo.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.nanxuanxn.top/gtamrbuidk.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.tianlin.xyz/gtxujsdbyl.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.xuetiantiany.cn/gtjiylzfzm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.nanxinkj.top/gtanocktvy.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.hywenlv.cn/gtxgqnyszl.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.cdnleiting.top/gtermwtoiw.html

[F03] 写入文件（覆盖）
来源：http://hz.mhx1999.top/gthtdkurxo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.xylfe.cn/gtumechysi.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.zhaomingkeji.xyz/gtqoxxbwwk.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zycfv.cn/gtsnprnngq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yongpay.top/gtukenwifa.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.zycfv.cn/gtwabnfiyo.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.dianchejie.cn/gtvzqtymkw.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.cucudq.cn/gtkgmxqdtz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.chenzaomai.com/gtulscqucr.html

[F04] 追加写入文件
来源：http://hz.gogol.net.cn/gtczujbeeq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.xylfe.cn/gtlasyodxe.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.snrcjt.cn/gthlfieavb.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ydjk.org.cn/gtgnwqxbnq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jyoumei.cn/gtdaowhdnf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.yanxiufei.cn/gtjmwacowr.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.zhiwuduotai.top/gtqwpnaqjn.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.xuanzx.com/gtiwptmnex.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.sxryk.cn/gtcfvjqyku.html

[F05] 判断文件或目录是否存在
来源：http://hz.sweek.top/gtpldkuvqi.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.gotoacloud.top/gtwissfalx.html

PHP:  file_exists("a.txt");
来源：http://hz.quarkkingdee.top/gtolejshrp.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yonumen.top/gtklkijnvt.html

TS:   fs.existsSync("a.txt")
来源：http://hz.hnqzz.top/gtaodrgzrz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.shzxlz.cn/gtmjxqohte.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.316326.xyz/gtiyyddppn.html

Ruby: File.exist?("a.txt")
来源：http://hz.gaohongyu789.top/gtnqlhxbzj.html

C#:   File.Exists("a.txt")
来源：http://hz.aizwys.cn/gtlvljtxhl.html

[F06] 删除文件
来源：http://hz.bjfxy.top/gtxcxdnpjk.html

Py:   os.remove("a.txt")
来源：http://hz.0kj1m.cn/gtjlebqdni.html

PHP:  unlink("a.txt");
来源：http://hz.xingfuxueyuan.xyz/gtcprajcjy.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.shanyushiyangtech.top/gtbocwgjxx.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.vqdsnc.cn/gtkkuvlvsc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.shuidangran.top/gtdznhnksr.html

Go:   os.Remove("a.txt")
来源：http://hz.hywenlv.cn/gtrajmqtwu.html

Ruby: File.delete("a.txt")
来源：http://hz.zhiwuduotai.top/gtegvibbii.html

C#:   File.Delete("a.txt");
来源：http://hz.tanke756.top/gtnpetdgxm.html

[F07] 创建目录（含多级）
来源：http://hz.xingfuxueyuan.xyz/gtygvptsdn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.jinghuilouyu.cn/gtpzvcpvvt.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.snrcjt.cn/gtcgpkgspb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.andypj.xyz/gtfuukstuj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yj20258888.top/gtwqcjbyww.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.cucudq.cn/gtgieptule.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.daria6918.cn/gttjfvdgdn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.hfpthk.cn/gtupwbssew.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.pycfn.com/gtoadlvihn.html

[F08] 遍历目录
来源：http://hz.ivvv.top/gtplmptbpe.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yonumen.top/gtvaupgfwc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.xuanzx.com/gtdrtulzlp.html

JS:   fs.readdirSync("dir")
来源：http://hz.quarkkingdee.top/gtcxwbkhed.html

TS:   fs.readdirSync("dir")
来源：http://hz.cashguo.top/gtyuenzyyk.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.dianchejie.cn/gtxzaghkjl.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.aibaodan.cn/gtuklhrctu.html

Ruby: Dir.children("dir")
来源：http://hz.xinyue.icu/gtqknbijmv.html

C#:   Directory.GetFiles("dir")
来源：http://hz.zhongyouzk.top/gtfnjvpiei.html

[F09] 获取文件大小
来源：http://hz.ywan-chungtsiang.top/gtlkffaebm.html

Py:   os.path.getsize("a.txt")
来源：http://hz.zhongyouzk.top/gttqupjpxa.html

PHP:  filesize("a.txt");
来源：http://hz.jlsjyb.cn/gtrimfdamb.html

JS:   fs.statSync("a.txt").size
来源：http://hz.tianlin.xyz/gtyaqvjiqe.html

TS:   fs.statSync("a.txt").size
来源：http://hz.tanke756.top/gtdxdiweiw.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jinghuilouyu.cn/gtgekfaxav.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.dashuyun.cn/gtmnmbpouu.html

Ruby: File.size("a.txt")
来源：http://hz.shuidangran.top/gtwlgdzbaz.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.ydjk.org.cn/gthfaevgfc.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.zhixingplan.top/gtpisnkiyr.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.cdnleiting.top/gtqcczveng.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.yonumen.top/gtnsngpriw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.sweek.top/gteeoedioc.html

TS:   path.extname("a.txt")
来源：http://hz.tian-w.cn/gthkkgdfqy.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.yueranfly.top/gtcezppjnx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.hfpthk.cn/gtrsxwwaze.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jyoumei.cn/gtuvttyiat.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.xuetiantiany.cn/gtruulkxdu.html

[F11] 复制与移动文件
来源：http://hz.shanyushiyangtech.top/gtameeuina.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.hywenlv.cn/gtnangvxsu.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.xingfuxueyuan.xyz/gtmwzuhkrs.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jinghuilouyu.cn/gtdnnaihec.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.iojbl.cn/gtnyewkvrb.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.dianchejie.cn/gtmzlmfqjo.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.52xcode.cn/gthecykmkx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.hfpthk.cn/gtegnctejx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.birdmap.top/gtvzvwddty.html

[F12] CSV 读写
来源：http://hz.xuanzx.com/gtkmxqiupx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.guowangkeji.top/gtmlobjfoh.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.pengpengdd.cyou/gtlczjotto.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.zhoulong.xyz/gtlnijberw.html

TS:   // 同上
来源：http://hz.daxiang520.top/gtvxoqsebd.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.zhongyouzk.top/gtjwkoydud.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.chenjidiqi.icu/gtqjggbwfr.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.ppjwa.cn/gtindhxyzt.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.xinyue.icu/gtzjitkdje.html

================================================================================
来源：http://hz.dashuyun.cn/gtckwlgrbm.html

G. 面向对象
来源：http://hz.sysykeji.top/gtfdimwwwl.html

================================================================================
来源：http://hz.xylfe.cn/gtmyqicdkp.html

[G01] 定义类
来源：http://hz.zdqjudy.top/gtjgmzugbe.html

Py:   class User: pass
来源：http://hz.shzxlz.cn/gtyebavntf.html

PHP:  class User {}
来源：http://hz.cucudq.cn/gttovsvhha.html

JS:   class User {}
来源：http://hz.9152youxi.cn/gtecevvoct.html

TS:   class User { name: string = ""; }
来源：http://hz.nanxinkj.top/gtkqavyrie.html

Java: class User {}
来源：http://hz.svipenyu.cn/gtleakbehf.html

Go:   type User struct { Name string }
来源：http://hz.daxiang520.top/gtpbvvkrmo.html

Ruby: class User; end
来源：http://hz.zhijiandao.cn/gtnwhjdupd.html

C#:   class User {}
来源：http://hz.ybcxt.top/gtbjklvmln.html

[G02] 构造函数
来源：http://hz.yuxming.cn/gtcyqjcbcf.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.shanyushiyangtech.top/gtywpttyfh.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.cucudq.cn/gtdunwbeaz.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.tanke756.top/gtkzfbaqar.html

TS:   constructor(public name: string) {}
来源：http://hz.andypj.xyz/gtydkkpsvg.html

Java: User(String name) { this.name = name; }
来源：http://hz.cucudq.cn/gtrezpvfea.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.redwolf501.top/gtapchiilk.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.zhixingplan.top/gtijzcvmxx.html

C#:   public User(string name) { Name = name; }
来源：http://hz.guannengcc.top/gtzvwtjjcp.html

[G03] 实例属性
来源：http://hz.c1oappe.top/gthvqbejix.html

Py:   self.name = "x"
来源：http://hz.hammf.cn/gtdoxpkxll.html

PHP:  public string $name = "x";
来源：http://hz.ppjwa.cn/gtgznqkjol.html

JS:   this.name = "x";
来源：http://hz.cheryme.top/gteajshsov.html

TS:   name: string = "x";
来源：http://hz.mhx1999.top/gtrnrhxmbw.html

Java: private String name;
来源：http://hz.jlsjyb.cn/gtogcijgaw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.jiagoushi.top/gtexzzbvik.html

Ruby: @name = "x"
来源：http://hz.chenjidiqi.icu/gtyfwttgxu.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.zhengqikj.top/gtxfxzhmrc.html

[G04] 定义方法
来源：http://hz.svipenyu.cn/gtamaapdma.html

Py:   def greet(self): return self.name
来源：http://hz.xingfuxueyuan.xyz/gtizyzieva.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.sweek.top/gtdnpdpmlm.html

JS:   greet() { return this.name; }
来源：http://hz.shzxlz.cn/gtrjwukguf.html

TS:   greet(): string { return this.name; }
来源：http://hz.daria6918.cn/gtnuguwtyr.html

Java: String greet() { return name; }
来源：http://hz.pycfn.com/gtnmgtusbg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.cucudq.cn/gtjcmcxgmu.html

Ruby: def greet; @name; end
来源：http://hz.jqgfzy.top/gthtxhjtsn.html

C#:   public string Greet() => Name;
来源：http://hz.pycfn.com/gttnyxwdew.html

[G05] 继承
来源：http://hz.ppjwa.cn/gtwlzyeyuw.html

Py:   class Admin(User): pass
来源：http://hz.zhengqikj.top/gtdpblqene.html

PHP:  class Admin extends User {}
来源：http://hz.havefunace.top/gtflvmvbud.html

JS:   class Admin extends User {}
来源：http://hz.havefunace.top/gtazfccglq.html

TS:   class Admin extends User {}
来源：http://hz.zycfv.cn/gtihtamfgw.html

Java: class Admin extends User {}
来源：http://hz.0kj1m.cn/gtgzwlqsen.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.wangdashe.top/gtvxzfbcax.html

Ruby: class Admin < User; end
来源：http://hz.jinqigfzy.top/gtmonzrqtu.html

C#:   class Admin : User {}
来源：http://hz.xuetiantiany.cn/gtstywmywd.html

[G06] 重写方法
来源：http://hz.redwolf501.top/gtdpgwmndc.html

Py:   def greet(self): return "admin"
来源：http://hz.daxiang520.top/gtmzxtkdir.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.daxiang520.top/gtihkvjqhm.html

JS:   greet() { return "admin"; }
来源：http://hz.yangfankeji.com/gttovmdwmb.html

TS:   greet(): string { return "admin"; }
来源：http://hz.birdmap.top/gtxtspkakx.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.zhijiandao.cn/gtvcyurypc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.jyoumei.cn/gtjtugbqqb.html

Ruby: def greet; "admin"; end
来源：http://hz.snrcjt.cn/gtmmnaesgw.html

C#:   public override string Greet() => "admin";
来源：http://hz.xuanzx.com/gtdmtqrqwz.html

[G07] 调用父类方法
来源：http://hz.zhoulong.xyz/gtggoofjcc.html

Py:   super().greet()
来源：http://hz.cqqwz.cn/gthiamntmw.html

PHP:  parent::greet();
来源：http://hz.zhixingplan.top/gtuuawfyou.html

JS:   super.greet();
来源：http://hz.yangfankeji.com/gtqijojctu.html

TS:   super.greet();
来源：http://hz.wangdashe.top/gttzemwwvy.html

Java: super.greet();
来源：http://hz.vqdsnc.cn/gtcruroxak.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.gotoacloud.top/gtyrdxilsc.html

Ruby: super
来源：http://hz.jlsjyb.cn/gttascpumg.html

C#:   base.Greet();
来源：http://hz.aibaodan.cn/gtvdiohons.html

[G08] 静态方法与属性
来源：http://hz.tianlin.xyz/gtsriqbgcr.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.daxiang520.top/gtqzsnywqo.html

PHP:  public static function f() {}
来源：http://hz.gotoacloud.top/gtifkjeydh.html

JS:   static f() {}
来源：http://hz.nanxinkj.top/gtdyhflmco.html

TS:   static f(): void {}
来源：http://hz.kuanghao11.cn/gtviiqmngy.html

Java: static void f() {}
来源：http://hz.redwolf501.top/gthltcejnd.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.chenlongwang.top/gttgcekhus.html

Ruby: def self.f; end
来源：http://hz.mhx1999.top/gtzyjmvwzi.html

C#:   public static void F() {}
来源：http://hz.zhiwuduotai.top/gthconcrdj.html

[G09] 接口 / 抽象类
来源：http://hz.wangdashe.top/gtvyfskmwo.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.meibo888.top/gtcyctmptp.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.aizwys.cn/gtrmfrceyp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.sweek.top/gtocmrdgzj.html

TS:   interface Shape { area(): number; }
来源：http://hz.guowangkeji.top/gtzomhkwhc.html

Java: interface Shape { double area(); }
来源：http://hz.sweek.top/gtqsxsrklr.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.sxryk.cn/gtgkqsqmuo.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.xinyue.icu/gtcbbpsdrq.html

C#:   interface IShape { double Area(); }
来源：http://hz.cucudq.cn/gtzcmpvkza.html

[G10] 访问控制
来源：http://hz.kuanghao11.cn/gthkhugehc.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.9152youxi.cn/gtmgotmzub.html

PHP:  public / protected / private
来源：http://hz.zhoulong.xyz/gtgpdbhvre.html

JS:   #private 字段；其余公开
来源：http://hz.zhiwuduotai.top/gthfhzqgbo.html

TS:   public / protected / private
来源：http://hz.yj202588.top/gtkoelgcbi.html

Java: public / protected / private / 默认包级
来源：http://hz.xuetiantiany.cn/gtkeichcwv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yanxiufei.cn/gttinbzpze.html

Ruby: public / protected / private
来源：http://hz.kuanghao11.cn/gtqfjufhmu.html

C#:   public / protected / private / internal
来源：http://hz.chenzaomai.com/gtjltijnex.html

[G11] getter / setter
来源：http://hz.cheryme.top/gtmxmabwfn.html

Py:   @property 与 @x.setter
来源：http://hz.daxiang520.top/gtfxyievkq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yangfankeji.com/gtyvemrjrl.html

JS:   get name() { return this._name; }
来源：http://hz.hysaishi.cn/gthlwptomf.html

TS:   get name(): string { return this._name; }
来源：http://hz.c1oappe.top/gtdzrridkm.html

Java: public String getName() { return name; }
来源：http://hz.yj202588.top/gtyhknokcc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.cqqwz.cn/gtysfjywpe.html

Ruby: attr_accessor :name
来源：http://hz.nanxinkj.top/gtdgovvbiy.html

C#:   public string Name { get; set; }
来源：http://hz.gogol.net.cn/gtfdgysgmp.html

[G12] 对象转字符串
来源：http://hz.fzhhl.top/gtupcmocdn.html

Py:   def __str__(self): return self.name
来源：http://hz.gotoacloud.top/gtzphpitlz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.gogol.net.cn/gtcivapqhm.html

JS:   toString() { return this.name; }
来源：http://hz.yueranfly.top/gtuasjmyjw.html

TS:   toString(): string { return this.name; }
来源：http://hz.sysykeji.top/gtegilchbq.html

Java: @Override public String toString() { return name; }
来源：http://hz.wangdashe.top/gtxfyextpl.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jiagoushi.top/gtfyfesshz.html

Ruby: def to_s; @name; end
来源：http://hz.nwbrower.top/gtltqifrkx.html

C#:   public override string ToString() => Name;
来源：http://hz.hnqzz.top/gtctamtips.html

[G13] 判断对象类型
来源：http://hz.xinyue.icu/gthjxnutey.html

Py:   isinstance(u, User)
来源：http://hz.shzxlz.cn/gttoklrcbk.html

PHP:  $u instanceof User
来源：http://hz.c1oappe.top/gtxrtbbpcm.html

JS:   u instanceof User
来源：http://hz.nanxinkj.top/gtaxczklxk.html

TS:   u instanceof User
来源：http://hz.fengsongda.top/gtvdravjus.html

Java: u instanceof User
来源：http://hz.nwbrower.top/gtolgwstnx.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.cheryme.top/gtkbmvetct.html

Ruby: u.is_a?(User)
来源：http://hz.ydzc1.top/gtvnqqngbj.html

C#:   u is User
来源：http://hz.vqdsnc.cn/gtgotvayyj.html

[G14] 数据类 / record
来源：http://hz.hywenlv.cn/gtesvwmble.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.zhiwuduotai.top/gtzznzfxnr.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yanxiufei.cn/gtfmsydyom.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.ydjk.org.cn/gtxzldhaly.html

TS:   type User = { name: string; age: number };
来源：http://hz.xingfuxueyuan.xyz/gtcgavjsvu.html

Java: record User(String name, int age) {}
来源：http://hz.zhaomingkeji.xyz/gtbsyedeac.html

Go:   type User struct { Name string; Age int }
来源：http://hz.redwolf501.top/gtewmrtnpt.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.hnxiangtu.top/gtebnzqdma.html

C#:   record User(string Name, int Age);
来源：http://hz.shuidangran.top/gtgyuighhy.html

[G15] 枚举
来源：http://hz.tianlin.xyz/gtcorzmbdq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.dashuyun.cn/gtzfffpnov.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.aizwys.cn/gtvzqcxyld.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.guowangkeji.top/gtbvbaxfrk.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.aibaodan.cn/gtdfnnumwm.html

Java: enum Color { RED, GREEN }
来源：http://hz.sweek.top/gtqnkakybq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.sxryk.cn/gtkfuhqkaq.html

Ruby: Color = %i[red green].freeze
来源：http://hz.jqgufenzy.top/gtiwvnseqt.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.fengsongda.top/gtjrazmwtn.html

[G16] 对象转数组 / 字典
来源：http://hz.guowangkeji.top/gtzgpdhqup.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.nanxinkj.top/gtkxqgimhq.html

PHP:  get_object_vars($obj);
来源：http://hz.ehwqpu.com/gtcujzstrn.html

JS:   Object.entries(obj)
来源：http://hz.pengpengdd.cyou/gtcfrnquzf.html

TS:   Object.entries(obj)
来源：http://hz.jiagoushi.top/gtwkwmhear.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.hfpthk.cn/gtfeeobwvf.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.snrcjt.cn/gtxzukojpj.html

Ruby: obj.instance_variables
来源：http://hz.xylfe.cn/gtrhntymnk.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.jlsjyb.cn/gtikdusyew.html

================================================================================
来源：http://hz.tanke756.top/gtrtrnfdcb.html


<!-- 参考信息 -->