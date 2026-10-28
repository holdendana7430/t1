代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.hfpthk.cn/gtknicdlkt.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.daria6918.cn/gthycybxzg.html

Ruby: s.capitalize
来源：http://hz.hysaishi.cn/gtuskymtkw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.ivvv.top/gtwhjewuco.html

[E18] 模板占位符替换
来源：http://hz.hammf.cn/gtidmrjthp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.fengsongda.top/gtfvpelovn.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.haohaochexian.top/gtihlxcvzr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.xylfe.cn/gtchgrhqbu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.nanxuanxn.top/gtfbwweabh.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.chenjidiqi.icu/gtcerqqzny.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.ydzc1.top/gtoixwtwji.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.ydjk.org.cn/gtlmfzjwsa.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.xylfe.cn/gttdxtaege.html

[E19] 多行文本按行拆分
来源：http://hz.wangdashe.top/gtautrwdmy.html

Py:   s.splitlines()
来源：http://hz.jiagoushi.top/gtyjmycxag.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.zycfv.cn/gtgzyeklhb.html

JS:   s.split(/\r?\n/)
来源：http://hz.cheryme.top/gtaqiuiiwo.html

TS:   s.split(/\r?\n/)
来源：http://hz.iojbl.cn/gtfddhaobr.html

Java: s.lines().toList()
来源：http://hz.yj20258888.top/gtobbadjfb.html

Go:   strings.Split(s, "\n")
来源：http://hz.sxryk.cn/gtqnjhaezf.html

Ruby: s.lines
来源：http://hz.shzxlz.cn/gtunyfvzpj.html

C#:   s.Split('\n')
来源：http://hz.snrcjt.cn/gtunzrfvcs.html

[E20] 判断字符串是否为空
来源：http://hz.cheryme.top/gtuqgpcech.html

Py:   if not s:
来源：http://hz.quarkkingdee.top/gtgftpwava.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.cashguo.top/gtaiqqnhad.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.jianghu66.top/gtrcjxadzo.html

TS:   if (s === "") {}
来源：http://hz.wangdashe.top/gthiqangze.html

Java: if (s.isEmpty()) {}
来源：http://hz.aizwys.cn/gtgiiakqtx.html

Go:   if s == "" {}
来源：http://hz.chenzaomai.com/gtiicmufkr.html

Ruby: if s.empty?
来源：http://hz.yonumen.top/gtderjfgzz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.chenzaomai.com/gthmotoqmr.html

[E21] 超长截断加省略号
来源：http://hz.snrcjt.cn/gtmkfcldod.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.daxiang520.top/gttdbuoicp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.yj202588.top/gtavxnfzdh.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yanxiufei.cn/gtbhrionjx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.guowangkeji.top/gtvkfgqvko.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.feifeiyinyue.top/gtjbrhjtwu.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.guowangkeji.top/gtjqzjtxgr.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.zhengqikj.top/gtvodcamvi.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.yj20258888.top/gtzxzzegqg.html

[E22] 字节长度与字符长度
来源：http://hz.shzxlz.cn/gtxguelwqn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.yvedp.cn/gtdyfmmlqm.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yj202588.top/gtdgtvmdam.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jlsjyb.cn/gtjkqmcnlv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jqgfzy.top/gtyudfxzmi.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.hongshengwenyu.top/gtwhbglqwi.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.c1oappe.top/gtvolqkwut.html

Ruby: s.bytesize;  s.length
来源：http://hz.0kj1m.cn/gtrgaugqzc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.ywan-chungtsiang.top/gtsnltspst.html

================================================================================
来源：http://hz.cdnleiting.top/gthqhzbthc.html

F. 文件与目录
来源：http://hz.xingfuxueyuan.xyz/gtraqltjmx.html

================================================================================
来源：http://hz.yj202588.top/gtrozvltdd.html

[F01] 读取整个文件
来源：http://hz.zhoulong.xyz/gtiplcxvqh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.andypj.xyz/gtuwtleigs.html

PHP:  file_get_contents("a.txt");
来源：http://hz.jlsjyb.cn/gtbpeznbuj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.jianghu66.top/gtogbpqshy.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.hfpthk.cn/gtfnrieyif.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.cdnleiting.top/gtykekhrmc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.wangshuangyany.cn/gtykwugyea.html

Ruby: File.read("a.txt")
来源：http://hz.shzxlz.cn/gtefvbdyoe.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.hnxiangtu.top/gteuaeprco.html

[F02] 逐行读取文件
来源：http://hz.haohaochexian.top/gtnrqhtswy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.cashguo.top/gtfievvzej.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.chenjidiqi.icu/gtfhkpprjy.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.shanyushiyangkeji.top/gtjcjqwava.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ywan-chungtsiang.top/gtjvbncwey.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.ywan-chungtsiang.top/gtmbihlcmq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.birdmap.top/gtozchbgbl.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.zhongyouzk.top/gtrcvifgen.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.xylfe.cn/gttymipcva.html

[F03] 写入文件（覆盖）
来源：http://hz.chenzaomai.com/gttdbhokit.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.hywenlv.cn/gtqcgkguhh.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.cucudq.cn/gtitfmmtae.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.cheryme.top/gtdpyeudyc.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.xylfe.cn/gttkvgxnxb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.ehwqpu.com/gtomwzzmeo.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.cashguo.top/gtstpjpqgc.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.dianchejie.cn/gteqookoqh.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.xylfe.cn/gthdfctztc.html

[F04] 追加写入文件
来源：http://hz.c1oappe.top/gtwwtpufxz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.xingfuxueyuan.xyz/gtarltywpw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.hnqzz.top/gtonvpotcu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.hongshengwenyu.top/gtdzsayuag.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.haohaochexian.top/gtcaikxili.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.yvedp.cn/gtwvrrkvpw.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.daxiang520.top/gtnidyvzum.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.nanxuanxn.top/gtfstxebwg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.xylfe.cn/gtcnncsgyz.html

[F05] 判断文件或目录是否存在
来源：http://hz.pycfn.com/gtapgoopjl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.bjfxy.top/gtobzcbviu.html

PHP:  file_exists("a.txt");
来源：http://hz.shuidangran.top/gtouldkbrb.html

JS:   fs.existsSync("a.txt")
来源：http://hz.hfpthk.cn/gtazmhubmu.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yuxming.cn/gtunaihzjg.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.smart0.xyz/gtyhqdmmsz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.jinghuilouyu.cn/gtjbqyurqk.html

Ruby: File.exist?("a.txt")
来源：http://hz.gzhubu.top/gtwfnlsntv.html

C#:   File.Exists("a.txt")
来源：http://hz.xuanzx.com/gtzhngegiw.html

[F06] 删除文件
来源：http://hz.hongshengwenyu.top/gtxrnotgpg.html

Py:   os.remove("a.txt")
来源：http://hz.jinyuanbaomall.cn/gtoiqdtqdh.html

PHP:  unlink("a.txt");
来源：http://hz.hywenlv.cn/gtnpmcxvkp.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.chenlongwang.top/gtzfshkqcy.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.cucudq.cn/gtbtvxguom.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.hfpthk.cn/gtafzubtxq.html

Go:   os.Remove("a.txt")
来源：http://hz.xuanzx.com/gtvkdworth.html

Ruby: File.delete("a.txt")
来源：http://hz.tianlin.xyz/gtqvzuozaa.html

C#:   File.Delete("a.txt");
来源：http://hz.birdmap.top/gtwblfrztc.html

[F07] 创建目录（含多级）
来源：http://hz.feifeiyinyue.top/gtdlyqrkzb.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yuanzhike.top/gtcqsgpntg.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.52xcode.cn/gtusrfcikv.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yuanzhike.top/gtepwgfave.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zdqjudy.top/gtlgcbuhqq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.wangdashe.top/gtzseaaqbc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.yj20258888.top/gtduddzniz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.shuidangran.top/gtyzztvdfb.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.shangyingyoupin.top/gtxtqfnpjx.html

[F08] 遍历目录
来源：http://hz.ivvv.top/gtbrrgibth.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.gaohongyu789.top/gtshcmxtch.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.cdnleiting.top/gtbzkqjwve.html

JS:   fs.readdirSync("dir")
来源：http://hz.yuanzhike.top/gtnqmaqyik.html

TS:   fs.readdirSync("dir")
来源：http://hz.zycfv.cn/gtlkmrnbhk.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.chenlongwang.top/gtqhsbmsxp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.gzhubu.top/gtvtjewhud.html

Ruby: Dir.children("dir")
来源：http://hz.shanyushiyangkeji.top/gtquqgvjhn.html

C#:   Directory.GetFiles("dir")
来源：http://hz.daria6918.cn/gtssklgups.html

[F09] 获取文件大小
来源：http://hz.shanyushiyangkeji.top/gtnnfegyap.html

Py:   os.path.getsize("a.txt")
来源：http://hz.tian-w.cn/gtccbfqkvc.html

PHP:  filesize("a.txt");
来源：http://hz.pengpengdd.cyou/gtbsyyxjym.html

JS:   fs.statSync("a.txt").size
来源：http://hz.ydjk.org.cn/gteljktvkr.html

TS:   fs.statSync("a.txt").size
来源：http://hz.hongshengwenyu.top/gtiwoqhile.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.smart0.xyz/gtltwfxmhk.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.feifeiyinyue.top/gtcrxbazcu.html

Ruby: File.size("a.txt")
来源：http://hz.yongpay.top/gtwhxqpjuf.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.svipenyu.cn/gtsjznicvi.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.cheryme.top/gtnidogdku.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.smart0.xyz/gtnqbjocbt.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.jinghuilouyu.cn/gtgnindipw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.bjfxy.top/gtautqvrmv.html

TS:   path.extname("a.txt")
来源：http://hz.c1oappe.top/gtxgzxgahz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.shanyushiyangtech.top/gtsvduyrqs.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.meibo888.top/gtdvwglrfx.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jqgufenzy.top/gtpheguvnb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.hfpthk.cn/gtmmrstayr.html

[F11] 复制与移动文件
来源：http://hz.quarkkingdee.top/gtyrjdnzcn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.redwolf501.top/gtlnfcjbds.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.smart0.xyz/gtzyukzdxo.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.shanyushiyangkeji.top/gtzhsnsbvj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.gzhubu.top/gtqcdbckxj.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.feifeiyinyue.top/gthmluumuv.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.kuanghao11.cn/gtlnrtphft.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.shuidangran.top/gtbpzhifoa.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.zhixingplan.top/gtarbaibaz.html

[F12] CSV 读写
来源：http://hz.aibaodan.cn/gtjraxpqun.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.hysaishi.cn/gtncbwnydp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.ivvv.top/gtfhndexlq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.gogol.net.cn/gtodmsuqua.html

TS:   // 同上
来源：http://hz.nanxinkj.top/gtsxljuunt.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.smart0.xyz/gtlzpkuyjz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yueranfly.top/gtcmrgvedq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.bjfxy.top/gtepzjnglg.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.nanxinkj.top/gtwsxtwxvf.html

================================================================================
来源：http://hz.cucudq.cn/gtsjfzqowj.html

G. 面向对象
来源：http://hz.zhixingplan.top/gtoxbhnnvs.html

================================================================================
来源：http://hz.gogol.net.cn/gtdtarweed.html

[G01] 定义类
来源：http://hz.yonumen.top/gtinjpzhsh.html

Py:   class User: pass
来源：http://hz.wangdashe.top/gtzakaohbp.html

PHP:  class User {}
来源：http://hz.yj20258888.top/gtudyzepme.html

JS:   class User {}
来源：http://hz.guannengcc.top/gtyhrcnjvz.html

TS:   class User { name: string = ""; }
来源：http://hz.yongpay.top/gtxuxjrqtz.html

Java: class User {}
来源：http://hz.daxiang520.top/gtesqcuzkg.html

Go:   type User struct { Name string }
来源：http://hz.aizwys.cn/gtmcxjhmct.html

Ruby: class User; end
来源：http://hz.cqqwz.cn/gtgmwgysol.html

C#:   class User {}
来源：http://hz.ywan-chungtsiang.top/gtqympdxbn.html

[G02] 构造函数
来源：http://hz.cdnleiting.top/gtrsmssueg.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.tian-w.cn/gtmpzipllw.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.52xcode.cn/gtlvqsbugw.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.gaohongyu789.top/gthxmtgxdq.html

TS:   constructor(public name: string) {}
来源：http://hz.cashguo.top/gteamtcwih.html

Java: User(String name) { this.name = name; }
来源：http://hz.aizwys.cn/gtrjmccetj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yueranfly.top/gtuxpaxlve.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.smart0.xyz/gtwzqxoedf.html

C#:   public User(string name) { Name = name; }
来源：http://hz.yonumen.top/gtzavyktwk.html

[G03] 实例属性
来源：http://hz.yj202588.top/gthpriymvv.html

Py:   self.name = "x"
来源：http://hz.daria6918.cn/gtweomgpys.html

PHP:  public string $name = "x";
来源：http://hz.zhongyouzk.top/gtksdrufmd.html

JS:   this.name = "x";
来源：http://hz.svipenyu.cn/gtxonbpgct.html

TS:   name: string = "x";
来源：http://hz.ppjwa.cn/gtallgbmae.html

Java: private String name;
来源：http://hz.yuxming.cn/gtdovkrmjh.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.sxryk.cn/gtlhkrnbsl.html

Ruby: @name = "x"
来源：http://hz.gotoacloud.top/gtjovhjfej.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.0kj1m.cn/gtanxearpp.html

[G04] 定义方法
来源：http://hz.sysykeji.top/gtwojxaxcg.html

Py:   def greet(self): return self.name
来源：http://hz.zhiwuduotai.top/gttorcoanb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.dashuyun.cn/gtsrroelto.html

JS:   greet() { return this.name; }
来源：http://hz.sxryk.cn/gtwlxusksx.html

TS:   greet(): string { return this.name; }
来源：http://hz.xingfuxueyuan.xyz/gtwysarafo.html

Java: String greet() { return name; }
来源：http://hz.svipenyu.cn/gturyyujlc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.yongpay.top/gtiyhtxumh.html

Ruby: def greet; @name; end
来源：http://hz.daria6918.cn/gtifglgcrb.html

C#:   public string Greet() => Name;
来源：http://hz.0kj1m.cn/gtateztfao.html

[G05] 继承
来源：http://hz.andypj.xyz/gtrfeuruxj.html

Py:   class Admin(User): pass
来源：http://hz.tian-w.cn/gtjhvatcdc.html

PHP:  class Admin extends User {}
来源：http://hz.gzhubu.top/gtrmwsfnkf.html

JS:   class Admin extends User {}
来源：http://hz.jianghu66.top/gtxzlzispx.html

TS:   class Admin extends User {}
来源：http://hz.jinyuanbaomall.cn/gtbowqbveb.html

Java: class Admin extends User {}
来源：http://hz.kuanghao11.cn/gtiisfxfvz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.snrcjt.cn/gtyfrnbuoy.html

Ruby: class Admin < User; end
来源：http://hz.zhaomingkeji.xyz/gtflxvfrmj.html

C#:   class Admin : User {}
来源：http://hz.yanxiufei.cn/gtzttfcgst.html

[G06] 重写方法
来源：http://hz.quarkkingdee.top/gtqxugavfx.html

Py:   def greet(self): return "admin"
来源：http://hz.kuanghao11.cn/gtdwmwvmiv.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.zhaomingkeji.xyz/gtghbdtkow.html

JS:   greet() { return "admin"; }
来源：http://hz.shuidangran.top/gtlczrkmmx.html

TS:   greet(): string { return "admin"; }
来源：http://hz.wangshuangyany.cn/gtklncvzzy.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.yongpay.top/gtoqxjdxhp.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zhengqikj.top/gtsxceubek.html

Ruby: def greet; "admin"; end
来源：http://hz.jlsjyb.cn/gtenulxihv.html

C#:   public override string Greet() => "admin";
来源：http://hz.hysaishi.cn/gtxolmkjue.html

[G07] 调用父类方法
来源：http://hz.zhaomingkeji.xyz/gtqfyuxyds.html

Py:   super().greet()
来源：http://hz.jinghuilouyu.cn/gtmkswghmi.html

PHP:  parent::greet();
来源：http://hz.sxryk.cn/gtbgmparwj.html

JS:   super.greet();
来源：http://hz.zycfv.cn/gtsdchcyng.html

TS:   super.greet();
来源：http://hz.zhiwuduotai.top/gtwctwuodp.html

Java: super.greet();
来源：http://hz.aizwys.cn/gtkhblwjic.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.gogol.net.cn/gtgwrrqfgj.html

Ruby: super
来源：http://hz.52xcode.cn/gtiusqxdmy.html

C#:   base.Greet();
来源：http://hz.sweek.top/gtabmkyauc.html

[G08] 静态方法与属性
来源：http://hz.9152youxi.cn/gtyucpnrmk.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.guannengcc.top/gttnfimnre.html

PHP:  public static function f() {}
来源：http://hz.jinqigufen.top/gtjmxupdqj.html

JS:   static f() {}
来源：http://hz.jqgfzy.top/gtizzpkihz.html

TS:   static f(): void {}
来源：http://hz.chenzaomai.com/gtxzwkmths.html

Java: static void f() {}
来源：http://hz.aizwys.cn/gtifnzzzvi.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.guannengcc.top/gtbkrvmmer.html

Ruby: def self.f; end
来源：http://hz.vqdsnc.cn/gtvuxoijqg.html

C#:   public static void F() {}
来源：http://hz.wangshuangyany.cn/gtfddvvqzc.html

[G09] 接口 / 抽象类
来源：http://hz.xinyue.icu/gtgarogoyk.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yj20258888.top/gtavfuedvh.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.zdqjudy.top/gtieurfusv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.birdmap.top/gtvjhpzqsz.html

TS:   interface Shape { area(): number; }
来源：http://hz.yuxming.cn/gtpvxaxifx.html

Java: interface Shape { double area(); }
来源：http://hz.zdqjudy.top/gtwsxoocnq.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.hysaishi.cn/gttqdwwsjx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.daxiang520.top/gtuzudehkx.html

C#:   interface IShape { double Area(); }
来源：http://hz.shuidangran.top/gtdlpuhbiu.html

[G10] 访问控制
来源：http://hz.xinyue.icu/gtqmxbxwwl.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.chenzaomai.com/gtvejwxdmd.html

PHP:  public / protected / private
来源：http://hz.zhaomingkeji.xyz/gtgchlfidb.html

JS:   #private 字段；其余公开
来源：http://hz.wangshuangyany.cn/gtjpudvewx.html

TS:   public / protected / private
来源：http://hz.zhongyouzk.top/gtixraxoyh.html

Java: public / protected / private / 默认包级
来源：http://hz.cdnleiting.top/gticeexppl.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zhaomingkeji.xyz/gtiwhjymmh.html

Ruby: public / protected / private
来源：http://hz.chenzaomai.com/gtjsyojphn.html

C#:   public / protected / private / internal
来源：http://hz.xylfe.cn/gtwszrwwdo.html

[G11] getter / setter
来源：http://hz.nanxuanxn.top/gtrkknmthk.html

Py:   @property 与 @x.setter
来源：http://hz.hnxiangtu.top/gtdbmwywkv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.mhx1999.top/gtvhbvggst.html

JS:   get name() { return this._name; }
来源：http://hz.shanyushiyangkeji.top/gtiaxgllcx.html

TS:   get name(): string { return this._name; }
来源：http://hz.feifeiyinyue.top/gteemvvtdo.html

Java: public String getName() { return name; }
来源：http://hz.zhoulong.xyz/gtrmrqusel.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.ywan-chungtsiang.top/gtavjborek.html

Ruby: attr_accessor :name
来源：http://hz.yuanzhike.top/gtrfkctukh.html

C#:   public string Name { get; set; }
来源：http://hz.xziqi.cn/gtvptxnbro.html

[G12] 对象转字符串
来源：http://hz.xuetiantiany.cn/gtbpxelzyt.html

Py:   def __str__(self): return self.name
来源：http://hz.jinqigfzy.top/gtzvdjrrhg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.pycfn.com/gtuimipyss.html

JS:   toString() { return this.name; }
来源：http://hz.iojbl.cn/gttbqeabzo.html

TS:   toString(): string { return this.name; }
来源：http://hz.jqgfzy.top/gtxxdstlro.html

Java: @Override public String toString() { return name; }
来源：http://hz.yvedp.cn/gtzhnfkkma.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.vqdsnc.cn/gtuhjzkauw.html

Ruby: def to_s; @name; end
来源：http://hz.guowangkeji.top/gtfomdrbfv.html

C#:   public override string ToString() => Name;
来源：http://hz.gaohongyu789.top/gtcuzcgcce.html

[G13] 判断对象类型
来源：http://hz.zhoulong.xyz/gtugkusvmw.html

Py:   isinstance(u, User)
来源：http://hz.hnqzz.top/gtopyrckab.html

PHP:  $u instanceof User
来源：http://hz.yonumen.top/gtimahtmez.html

JS:   u instanceof User
来源：http://hz.hfpthk.cn/gtjzsmuoyw.html

TS:   u instanceof User
来源：http://hz.zhoulong.xyz/gtzekfbkhw.html

Java: u instanceof User
来源：http://hz.hnqzz.top/gtfgslnvwp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.nwbrower.top/gthvufwmar.html

Ruby: u.is_a?(User)
来源：http://hz.aibaodan.cn/gthnsrfeoy.html

C#:   u is User
来源：http://hz.hywenlv.cn/gtjrjqtmeg.html

[G14] 数据类 / record
来源：http://hz.cashguo.top/gtlkngkyxa.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.andypj.xyz/gtzofzifrl.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.fengsongda.top/gtzsucjsym.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.xylfe.cn/gttqtrqlwy.html

TS:   type User = { name: string; age: number };
来源：http://hz.shangyingyoupin.top/gtqabzmfrl.html

Java: record User(String name, int age) {}
来源：http://hz.wangshuangyany.cn/gtwwwfoncq.html

Go:   type User struct { Name string; Age int }
来源：http://hz.yongpay.top/gtcqpzfmww.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.tianlin.xyz/gtubkutdir.html

C#:   record User(string Name, int Age);
来源：http://hz.fengsongda.top/gtuwcvabtj.html

[G15] 枚举
来源：http://hz.jyoumei.cn/gtrgprxabz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.pycfn.com/gtraldwvau.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.shzxlz.cn/gtjdhmzjhq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.snrcjt.cn/gtpobfnnxa.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hysaishi.cn/gtkbfprbvn.html

Java: enum Color { RED, GREEN }
来源：http://hz.havefunace.top/gtvsbyyrml.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.aibaodan.cn/gtaccykvjb.html

Ruby: Color = %i[red green].freeze
来源：http://hz.sysykeji.top/gtnocxjqaf.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jinyuanbaomall.cn/gtzneohnbr.html

[G16] 对象转数组 / 字典
来源：http://hz.sweek.top/gtddmwbsua.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.quarkkingdee.top/gtymsjcvlp.html


<!-- 参考信息 -->