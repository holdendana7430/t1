代发 wailian999

PHP:  number_format(1234567);
来源：http://hz.yanxiufei.cn/gtfmqglyck.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.9152youxi.cn/gtbzgvbort.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.pengpengdd.cyou/gtytmlpywy.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.yj202588.top/gtihrbzsrc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.svipenyu.cn/gtcupmfmro.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.feifeiyinyue.top/gtbrwvewsp.html

C#:   1234567.ToString("N0")
来源：http://hz.tanke756.top/gtbxqzrjpb.html

[E17] 首字母大写
来源：http://hz.mhx1999.top/gtcukhvvyk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.smart0.xyz/gtqyzunlkk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.chenzaomai.com/gteygyglqk.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.bjfxy.top/gtkrcdcrvp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.cheryme.top/gtaedijtff.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.jinyuanbaomall.cn/gtcjumndyb.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.zycfv.cn/gtbolwedbk.html

Ruby: s.capitalize
来源：http://hz.meibo888.top/gtqgpdupmx.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.jinghuilouyu.cn/gtpmsxhfzu.html

[E18] 模板占位符替换
来源：http://hz.fengsongda.top/gtrxdxdpjv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.shuidangran.top/gttjvuffde.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.hnqzz.top/gthkybpnjd.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.ybcxt.top/gtrhpcubiq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.chenlongwang.top/gtaptqxbxg.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.gzhubu.top/gtvupthyeq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.gotoacloud.top/gtgacsycck.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.xuetiantiany.cn/gtllbnxpde.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.tian-w.cn/gthyuifvip.html

[E19] 多行文本按行拆分
来源：http://hz.jqgfzy.top/gtwfjgwglj.html

Py:   s.splitlines()
来源：http://hz.c1oappe.top/gtbwvhkpwz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.bjfxy.top/gthctptxkt.html

JS:   s.split(/\r?\n/)
来源：http://hz.gaohongyu789.top/gtbaxyqavk.html

TS:   s.split(/\r?\n/)
来源：http://hz.hnqzz.top/gtgjekukki.html

Java: s.lines().toList()
来源：http://hz.zhoulong.xyz/gtsodkejja.html

Go:   strings.Split(s, "\n")
来源：http://hz.gogol.net.cn/gtarmkbwtb.html

Ruby: s.lines
来源：http://hz.316326.xyz/gtwpetipmu.html

C#:   s.Split('\n')
来源：http://hz.iojbl.cn/gtkoxqfyel.html

[E20] 判断字符串是否为空
来源：http://hz.shzxlz.cn/gtzpefjjsr.html

Py:   if not s:
来源：http://hz.wangdashe.top/gtgivzgjlk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.iojbl.cn/gtzswbvgok.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.bjfxy.top/gtjilxhczg.html

TS:   if (s === "") {}
来源：http://hz.yj20258.top/gtxzemsyqa.html

Java: if (s.isEmpty()) {}
来源：http://hz.sufxvd.cn/gtxtjscntx.html

Go:   if s == "" {}
来源：http://hz.tianlin.xyz/gtwbcotqqd.html

Ruby: if s.empty?
来源：http://hz.tanke756.top/gtazjjwcbq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.xuanzx.com/gtukaajjzd.html

[E21] 超长截断加省略号
来源：http://hz.pengpengdd.cyou/gtveltvcrz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.52xcode.cn/gtfpcbqbcf.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.cheryme.top/gttjmdmzdn.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.xinyue.icu/gtxajznpbi.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jiagoushi.top/gtqdjevraz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.feifeiyinyue.top/gtbtrqhwvt.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.hnqzz.top/gtzpzkvgck.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.gotoacloud.top/gtszwfiwgz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.dashuyun.cn/gtyinjvjfa.html

[E22] 字节长度与字符长度
来源：http://hz.vqdsnc.cn/gtbcdsrssh.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.cdnleiting.top/gtzaaigvix.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhongyouzk.top/gtwppoeecj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.shangyingyoupin.top/gtgmlzuunx.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ybcxt.top/gtwdrxojrt.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.tianlin.xyz/gtlwcorusv.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.nanxuanxn.top/gtcveknfav.html

Ruby: s.bytesize;  s.length
来源：http://hz.shzxlz.cn/gtlrmqlrhq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.hfpthk.cn/gtikatnwcv.html

================================================================================
来源：http://hz.aibaodan.cn/gthqwbxddm.html

F. 文件与目录
来源：http://hz.jlsjyb.cn/gtxgzftwoe.html

================================================================================
来源：http://hz.xziqi.cn/gtgasfwvsj.html

[F01] 读取整个文件
来源：http://hz.cqqwz.cn/gtobxthtyq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.sysykeji.top/gtbqsxuith.html

PHP:  file_get_contents("a.txt");
来源：http://hz.pycfn.com/gtxtaprtrx.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.svipenyu.cn/gtvxptsvmi.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.sufxvd.cn/gtxfthptes.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.ydzc1.top/gtgwylwbvt.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.wangdashe.top/gtydadtbkd.html

Ruby: File.read("a.txt")
来源：http://hz.nanxinkj.top/gtdjwtqfyk.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.xziqi.cn/gtfusykdhv.html

[F02] 逐行读取文件
来源：http://hz.yonumen.top/gthkasorlu.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.vqdsnc.cn/gtzgsrayje.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.iojbl.cn/gtuqyyutzi.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.cucudq.cn/gtyolpgoiu.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.bjfxy.top/gtupcbqqdf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.chenlongwang.top/gtmxybdzfz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.zhiwuduotai.top/gtqhfrswld.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.cdnleiting.top/gtybneuual.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.zhijiandao.cn/gtpfxmsnkr.html

[F03] 写入文件（覆盖）
来源：http://hz.yueranfly.top/gtuuoukvjk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.fzhhl.top/gtzxruhiet.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.chenlongwang.top/gtnalxksyg.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.dianchejie.cn/gthwjhzzxv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.redwolf501.top/gtoymibgfe.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.vqdsnc.cn/gtneighjnn.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.cheryme.top/gtqnlvvulg.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.andypj.xyz/gtphecnsdt.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.cqqwz.cn/gtrulwweui.html

[F04] 追加写入文件
来源：http://hz.yj20258888.top/gttpwlkpur.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.andypj.xyz/gtmjlevsov.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.yvedp.cn/gtzjficzse.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.aibaodan.cn/gtkoqmomno.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.iojbl.cn/gtdvthwkyb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.andypj.xyz/gtyveredbe.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.kuanghao11.cn/gtwovkwtis.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.shuidangran.top/gttfmonznc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.shanyushiyangkeji.top/gtsnvernno.html

[F05] 判断文件或目录是否存在
来源：http://hz.xinyue.icu/gtureqnyxh.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.0kj1m.cn/gtzmgpjrzl.html

PHP:  file_exists("a.txt");
来源：http://hz.smart0.xyz/gtsjuwrigi.html

JS:   fs.existsSync("a.txt")
来源：http://hz.jiagoushi.top/gtiziwjfhb.html

TS:   fs.existsSync("a.txt")
来源：http://hz.nanxinkj.top/gtnthdotwd.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.hnqzz.top/gtlcbrpila.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.cqqwz.cn/gtxtfadwor.html

Ruby: File.exist?("a.txt")
来源：http://hz.yanxiufei.cn/gtgzhxefex.html

C#:   File.Exists("a.txt")
来源：http://hz.hnxiangtu.top/gtoecqbvxu.html

[F06] 删除文件
来源：http://hz.ehwqpu.com/gtmhtpjjjb.html

Py:   os.remove("a.txt")
来源：http://hz.0kj1m.cn/gtfqdhqiag.html

PHP:  unlink("a.txt");
来源：http://hz.jinyuanbaomall.cn/gtkvugggkj.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.guowangkeji.top/gtoldwjeqy.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.yj20258888.top/gttesclpsd.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.xuetiantiany.cn/gtetgohlhz.html

Go:   os.Remove("a.txt")
来源：http://hz.iojbl.cn/gtbavjiqvi.html

Ruby: File.delete("a.txt")
来源：http://hz.meibo888.top/gtcvfckkxn.html

C#:   File.Delete("a.txt");
来源：http://hz.xylfe.cn/gtrnjbzwtk.html

[F07] 创建目录（含多级）
来源：http://hz.gogol.net.cn/gtsxnvlvxd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.hfpthk.cn/gthhxlwdjd.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.zhengqikj.top/gtjwhqprqn.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ppjwa.cn/gtkoayutmz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.guannengcc.top/gtidnipxro.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.cdnleiting.top/gtxvphtdqi.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.xinyue.icu/gtewsempze.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.jinyuanbaomall.cn/gtanfplxlt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.jinyuanbaomall.cn/gtkmonsyis.html

[F08] 遍历目录
来源：http://hz.cqqwz.cn/gtulhtccsr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.jqgufenzy.top/gtiulqbzjx.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.snrcjt.cn/gtxyuglwdt.html

JS:   fs.readdirSync("dir")
来源：http://hz.gotoacloud.top/gtdbshtrar.html

TS:   fs.readdirSync("dir")
来源：http://hz.cheryme.top/gtboumptwf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.xuanzx.com/gtfynvdbrf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.zhixingplan.top/gtnmeurmfi.html

Ruby: Dir.children("dir")
来源：http://hz.nwbrower.top/gtoaffxeit.html

C#:   Directory.GetFiles("dir")
来源：http://hz.aibaodan.cn/gtckercqwi.html

[F09] 获取文件大小
来源：http://hz.redwolf501.top/gtrejhuzzg.html

Py:   os.path.getsize("a.txt")
来源：http://hz.hfpthk.cn/gtzkurqkch.html

PHP:  filesize("a.txt");
来源：http://hz.sufxvd.cn/gtzkiedyql.html

JS:   fs.statSync("a.txt").size
来源：http://hz.cqqwz.cn/gtfawobmer.html

TS:   fs.statSync("a.txt").size
来源：http://hz.jinghuilouyu.cn/gtbikvvbit.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jyoumei.cn/gtmlrzmsdo.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.tian-w.cn/gtggovcghl.html

Ruby: File.size("a.txt")
来源：http://hz.chenjidiqi.icu/gthzlzjeyj.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.xylfe.cn/gtjyzqswpi.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.sxryk.cn/gtfzjiutwg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.mhx1999.top/gtbqfhiekm.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.zdqjudy.top/gtoxwvyygp.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.zhixingplan.top/gtrredwdgz.html

TS:   path.extname("a.txt")
来源：http://hz.iojbl.cn/gtgrfdbmla.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.chenzaomai.com/gtwmusqzqj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.9152youxi.cn/gtkwckncfs.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.xuetiantiany.cn/gtodhcggfe.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.vqdsnc.cn/gtfvpcxibi.html

[F11] 复制与移动文件
来源：http://hz.cdnleiting.top/gtimhzxmom.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.andypj.xyz/gtbpvowwgc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.nanxinkj.top/gtjdiopowk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jqgufenzy.top/gtyhxefybw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.shanyushiyangkeji.top/gtdscieigl.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.yonumen.top/gtirchkoka.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.52xcode.cn/gtjqxccjza.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.jinqigufen.top/gtdfnusorc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.zhijiandao.cn/gtouvjtuae.html

[F12] CSV 读写
来源：http://hz.yuanzhike.top/gtcprylhki.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.fengsongda.top/gtzirdmcqe.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.jiagoushi.top/gtblwrpntj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.sxryk.cn/gtrsgpysba.html

TS:   // 同上
来源：http://hz.feifeiyinyue.top/gtxstmbjki.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.ybcxt.top/gtbjhyfujx.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.316326.xyz/gtoadrgetd.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.tanke756.top/gtucpawghz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.nanxinkj.top/gtgepvingt.html

================================================================================
来源：http://hz.gaohongyu789.top/gtcpuvgzjm.html

G. 面向对象
来源：http://hz.c1oappe.top/gtdvzutikg.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtaigpxgcp.html

[G01] 定义类
来源：http://hz.birdmap.top/gtmfejanlu.html

Py:   class User: pass
来源：http://hz.fengsongda.top/gtfmlwtfut.html

PHP:  class User {}
来源：http://hz.9152youxi.cn/gtfmobuxss.html

JS:   class User {}
来源：http://hz.tianlin.xyz/gtziyprojr.html

TS:   class User { name: string = ""; }
来源：http://hz.cqqwz.cn/gtduhrflel.html

Java: class User {}
来源：http://hz.yuanzhike.top/gtcjruxqtz.html

Go:   type User struct { Name string }
来源：http://hz.fengsongda.top/gtxdixlydg.html

Ruby: class User; end
来源：http://hz.yanxiufei.cn/gtvybgdmes.html

C#:   class User {}
来源：http://hz.feifeiyinyue.top/gtvmxszhiv.html

[G02] 构造函数
来源：http://hz.yanxiufei.cn/gtjlplufea.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.chenzaomai.com/gtuuhtiewy.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.316326.xyz/gtiddkbrmf.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.vqdsnc.cn/gthdhfwdzk.html

TS:   constructor(public name: string) {}
来源：http://hz.zhaomingkeji.xyz/gtsblwnika.html

Java: User(String name) { this.name = name; }
来源：http://hz.sweek.top/gthghphmjz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.guannengcc.top/gtdcgfilke.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.zdqjudy.top/gtnjisyhrs.html

C#:   public User(string name) { Name = name; }
来源：http://hz.tian-w.cn/gtgehgzssp.html

[G03] 实例属性
来源：http://hz.cdnleiting.top/gtrtmvnqwc.html

Py:   self.name = "x"
来源：http://hz.shanyushiyangtech.top/gtofambspj.html

PHP:  public string $name = "x";
来源：http://hz.smart0.xyz/gtlrogyrve.html

JS:   this.name = "x";
来源：http://hz.yanxiufei.cn/gtxppmfqup.html

TS:   name: string = "x";
来源：http://hz.hysaishi.cn/gtonsyieme.html

Java: private String name;
来源：http://hz.tian-w.cn/gtcmskhrfy.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.xziqi.cn/gtjjlruibz.html

Ruby: @name = "x"
来源：http://hz.ybcxt.top/gtnmtcrnak.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yuanzhike.top/gtzeaninal.html

[G04] 定义方法
来源：http://hz.sufxvd.cn/gtbunwyoaa.html

Py:   def greet(self): return self.name
来源：http://hz.tian-w.cn/gtzwhheccf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.hnqzz.top/gtjtvuobep.html

JS:   greet() { return this.name; }
来源：http://hz.birdmap.top/gtxgokvkuu.html

TS:   greet(): string { return this.name; }
来源：http://hz.zhongyouzk.top/gtiaqxoybg.html

Java: String greet() { return name; }
来源：http://hz.cashguo.top/gtrrujwgbt.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.bjfxy.top/gtdahfujtn.html

Ruby: def greet; @name; end
来源：http://hz.zhengqikj.top/gtxcxdumqi.html

C#:   public string Greet() => Name;
来源：http://hz.daxiang520.top/gtfaghxews.html

[G05] 继承
来源：http://hz.jinyuanbaomall.cn/gtelrpeyhz.html

Py:   class Admin(User): pass
来源：http://hz.sufxvd.cn/gtedwkaeyq.html

PHP:  class Admin extends User {}
来源：http://hz.zhoulong.xyz/gthilnsmkm.html

JS:   class Admin extends User {}
来源：http://hz.bjfxy.top/gtrgmhsihm.html

TS:   class Admin extends User {}
来源：http://hz.gogol.net.cn/gtalhqkthz.html

Java: class Admin extends User {}
来源：http://hz.nwbrower.top/gtsbexeahk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.tanke756.top/gtqgrzufwa.html

Ruby: class Admin < User; end
来源：http://hz.yongpay.top/gtgleieycx.html

C#:   class Admin : User {}
来源：http://hz.wangdashe.top/gtsddzykgj.html

[G06] 重写方法
来源：http://hz.ehwqpu.com/gthnhffzrn.html

Py:   def greet(self): return "admin"
来源：http://hz.sweek.top/gtdqecmfno.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.tanke756.top/gtjyrmlacr.html

JS:   greet() { return "admin"; }
来源：http://hz.zhixingplan.top/gthucezjpw.html

TS:   greet(): string { return "admin"; }
来源：http://hz.gogol.net.cn/gtpjhjkejo.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.yj20258.top/gtucwtkzeo.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.hywenlv.cn/gtusymkili.html

Ruby: def greet; "admin"; end
来源：http://hz.wangdashe.top/gtqzosompv.html

C#:   public override string Greet() => "admin";
来源：http://hz.yueranfly.top/gtsjtyndoa.html

[G07] 调用父类方法
来源：http://hz.yongpay.top/gtoeytbtgt.html

Py:   super().greet()
来源：http://hz.zhongyouzk.top/gtzjdgbmev.html

PHP:  parent::greet();
来源：http://hz.nwbrower.top/gtkzwrsuov.html

JS:   super.greet();
来源：http://hz.wangshuangyany.cn/gtsgrdzecx.html

TS:   super.greet();
来源：http://hz.zhaomingkeji.xyz/gtaweexjak.html

Java: super.greet();
来源：http://hz.gotoacloud.top/gtyhxixqpc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.kuanghao11.cn/gtfnmvoxhp.html

Ruby: super
来源：http://hz.52xcode.cn/gtvwxzilli.html

C#:   base.Greet();
来源：http://hz.chenzaomai.com/gtqrnyibbw.html

[G08] 静态方法与属性
来源：http://hz.redwolf501.top/gtuqehkiwn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.chenjidiqi.icu/gtmuaqpsvb.html

PHP:  public static function f() {}
来源：http://hz.zhixingplan.top/gtoougzqkm.html

JS:   static f() {}
来源：http://hz.nwbrower.top/gtuywgwdep.html

TS:   static f(): void {}
来源：http://hz.cucudq.cn/gtvsilkacz.html

Java: static void f() {}
来源：http://hz.haohaochexian.top/gtwcumlezc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.feifeiyinyue.top/gtjharskul.html

Ruby: def self.f; end
来源：http://hz.hywenlv.cn/gthpqxoewd.html

C#:   public static void F() {}
来源：http://hz.ybcxt.top/gtaietxxqs.html

[G09] 接口 / 抽象类
来源：http://hz.xylfe.cn/gtybszaful.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.ehwqpu.com/gtrskfjqqr.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.xuanzx.com/gtjdlmsnwq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.snrcjt.cn/gteuomqiqz.html

TS:   interface Shape { area(): number; }
来源：http://hz.ehwqpu.com/gtghfiytxp.html

Java: interface Shape { double area(); }
来源：http://hz.hammf.cn/gtoauerkcp.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.shangyingyoupin.top/gtrxqbwdph.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.cdnleiting.top/gtrduuzihl.html

C#:   interface IShape { double Area(); }
来源：http://hz.chenzaomai.com/gtxlhjzwna.html

[G10] 访问控制
来源：http://hz.ydjk.org.cn/gtrligszuf.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yangfankeji.com/gtviizmbwg.html

PHP:  public / protected / private
来源：http://hz.haohaochexian.top/gtohzmkyvz.html

JS:   #private 字段；其余公开
来源：http://hz.aibaodan.cn/gtwaznmvcf.html

TS:   public / protected / private
来源：http://hz.yonumen.top/gtdlyyagfm.html

Java: public / protected / private / 默认包级
来源：http://hz.andypj.xyz/gtjdjjiscf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.redwolf501.top/gtdlwekmxu.html

Ruby: public / protected / private
来源：http://hz.cucudq.cn/gtckavotut.html

C#:   public / protected / private / internal
来源：http://hz.jqgfzy.top/gtlalwomzl.html

[G11] getter / setter
来源：http://hz.guannengcc.top/gtpvyiwbqm.html

Py:   @property 与 @x.setter
来源：http://hz.yongpay.top/gtltznqdmu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.xuanzx.com/gtwsfyyhrd.html

JS:   get name() { return this._name; }
来源：http://hz.tian-w.cn/gtzgrathtm.html

TS:   get name(): string { return this._name; }
来源：http://hz.zycfv.cn/gthhndyqon.html

Java: public String getName() { return name; }
来源：http://hz.yj202588.top/gtfheelfji.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.tianlin.xyz/gtjshptwrs.html

Ruby: attr_accessor :name
来源：http://hz.jlsjyb.cn/gtfjaqlixb.html

C#:   public string Name { get; set; }
来源：http://hz.dianchejie.cn/gtvkazjkmv.html

[G12] 对象转字符串
来源：http://hz.sweek.top/gtsrwfakpy.html

Py:   def __str__(self): return self.name
来源：http://hz.bjfxy.top/gtzntrxqru.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.zhoulong.xyz/gtojsrakeb.html

JS:   toString() { return this.name; }
来源：http://hz.nanxuanxn.top/gtrlepytiw.html

TS:   toString(): string { return this.name; }
来源：http://hz.zhijiandao.cn/gtibrrawyo.html

Java: @Override public String toString() { return name; }
来源：http://hz.yanxiufei.cn/gtobukxejb.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.birdmap.top/gtogxauqau.html

Ruby: def to_s; @name; end
来源：http://hz.pengpengdd.cyou/gthtmorgkf.html

C#:   public override string ToString() => Name;
来源：http://hz.c1oappe.top/gtrnqlzgvk.html

[G13] 判断对象类型
来源：http://hz.hnqzz.top/gtnpilasve.html

Py:   isinstance(u, User)
来源：http://hz.jyoumei.cn/gtwguqrqae.html

PHP:  $u instanceof User
来源：http://hz.shangyingyoupin.top/gtglbpwzjv.html

JS:   u instanceof User
来源：http://hz.yvedp.cn/gtvdncdhxf.html

TS:   u instanceof User
来源：http://hz.dashuyun.cn/gtbnrpsvqb.html

Java: u instanceof User
来源：http://hz.sxryk.cn/gtdqwagbra.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yj202588.top/gtfvqqktun.html

Ruby: u.is_a?(User)
来源：http://hz.yvedp.cn/gtakbopelr.html

C#:   u is User
来源：http://hz.meibo888.top/gtzipiqvtl.html

[G14] 数据类 / record
来源：http://hz.feifeiyinyue.top/gtngxmztwa.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yj20258888.top/gtlunrxrnh.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.cashguo.top/gtwyeddzxy.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.52xcode.cn/gtvatdyrux.html

TS:   type User = { name: string; age: number };
来源：http://hz.hysaishi.cn/gthtadhpyg.html

Java: record User(String name, int age) {}
来源：http://hz.zycfv.cn/gtcvpiqret.html

Go:   type User struct { Name string; Age int }
来源：http://hz.guannengcc.top/gtgecuslqx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.hammf.cn/gtsnrbyiog.html


<!-- 参考信息 -->