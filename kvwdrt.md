代发 wailian999

PHP:  number_format(1234567);
来源：http://hz.yuxming.cn/gtrcnixwff.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.hysaishi.cn/gtxdzmglzf.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.hammf.cn/gtgwggxaqo.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.316326.xyz/gtyzupvtzf.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.jiagoushi.top/gtwwxuhoon.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.yueranfly.top/gthlzbikzu.html

C#:   1234567.ToString("N0")
来源：http://hz.haohaochexian.top/gtvktptwoj.html

[E17] 首字母大写
来源：http://hz.yj20258.top/gttbbfeeoh.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.yongpay.top/gtexmjqzcj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.hywenlv.cn/gtdhdastcm.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhijiandao.cn/gtihkvcqte.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.cucudq.cn/gtdvkmpirg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.yanxiufei.cn/gtlyqgrpaj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.c1oappe.top/gtexhkgqyu.html

Ruby: s.capitalize
来源：http://hz.nwbrower.top/gtqzrujuem.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.jiagoushi.top/gtblbqslpd.html

[E18] 模板占位符替换
来源：http://hz.feifeiyinyue.top/gtywfnprrp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.jinghuilouyu.cn/gtcjimgdtv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.nanxinkj.top/gtlfgttiqw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.xuanzx.com/gtmqinhufb.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.xingfuxueyuan.xyz/gtgmdlrzlx.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.jinghuilouyu.cn/gtnrsjjfxx.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.yanxiufei.cn/gtuwnisuom.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.aizwys.cn/gtbnsfzjuj.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.cucudq.cn/gtkxpsovdb.html

[E19] 多行文本按行拆分
来源：http://hz.zhaomingkeji.xyz/gthrieeang.html

Py:   s.splitlines()
来源：http://hz.yuxming.cn/gtdibzqxof.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.gaohongyu789.top/gtfiaerzfb.html

JS:   s.split(/\r?\n/)
来源：http://hz.jqgufenzy.top/gttqokvpap.html

TS:   s.split(/\r?\n/)
来源：http://hz.ehwqpu.com/gtcqgxuvmb.html

Java: s.lines().toList()
来源：http://hz.jinyuanbaomall.cn/gtuutrpwlr.html

Go:   strings.Split(s, "\n")
来源：http://hz.yj20258.top/gttqpkmfed.html

Ruby: s.lines
来源：http://hz.hfpthk.cn/gtrzsazmzc.html

C#:   s.Split('\n')
来源：http://hz.zycfv.cn/gtmrfvjseo.html

[E20] 判断字符串是否为空
来源：http://hz.aizwys.cn/gtnfyexwrf.html

Py:   if not s:
来源：http://hz.sxryk.cn/gtgqvzhzou.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.sxryk.cn/gtptvnhzzr.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.jlsjyb.cn/gtacdwsazj.html

TS:   if (s === "") {}
来源：http://hz.hnxiangtu.top/gttzrqnjur.html

Java: if (s.isEmpty()) {}
来源：http://hz.redwolf501.top/gthbueeqyv.html

Go:   if s == "" {}
来源：http://hz.gogol.net.cn/gtrmukcghq.html

Ruby: if s.empty?
来源：http://hz.hfpthk.cn/gtotbddcsr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.dianchejie.cn/gtbpfsaxpt.html

[E21] 超长截断加省略号
来源：http://hz.ivvv.top/gtyfiygnzm.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.zhixingplan.top/gtugazwtye.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.jinqigfzy.top/gtplznssyi.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.cucudq.cn/gteufkzion.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.cdnleiting.top/gtojtiyojn.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.ivvv.top/gtfvwugpdx.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.zhengqikj.top/gtuqrkyhfc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.smart0.xyz/gtjdirdvap.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.ybcxt.top/gtgtjrljvu.html

[E22] 字节长度与字符长度
来源：http://hz.smart0.xyz/gthxvtclqa.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.ppjwa.cn/gtypzvzbwh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.sweek.top/gtasysancf.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.shuidangran.top/gthfzhtqhm.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jqgufenzy.top/gtlyeduvuo.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.shanyushiyangkeji.top/gtckfuemne.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.chenlongwang.top/gtsvftigfk.html

Ruby: s.bytesize;  s.length
来源：http://hz.hywenlv.cn/gtrtgardic.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.sufxvd.cn/gtgamjgrxn.html

================================================================================
来源：http://hz.zhijiandao.cn/gtgsqxnwsq.html

F. 文件与目录
来源：http://hz.cucudq.cn/gtmssfvzld.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtpklwogsm.html

[F01] 读取整个文件
来源：http://hz.dianchejie.cn/gtwrvvsvrg.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.aibaodan.cn/gtmxfkacpu.html

PHP:  file_get_contents("a.txt");
来源：http://hz.316326.xyz/gtukllstvk.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.zycfv.cn/gtlxiijjpw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.jiagoushi.top/gtiewnbbnr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.tian-w.cn/gtzygvqvdl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.jinghuilouyu.cn/gtxqjsxiuk.html

Ruby: File.read("a.txt")
来源：http://hz.cucudq.cn/gtxadgpjgw.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.cqqwz.cn/gtabpjfqxd.html

[F02] 逐行读取文件
来源：http://hz.yongpay.top/gtftkkmnix.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.gotoacloud.top/gtigyjiune.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.shanyushiyangkeji.top/gtqyfpcvyn.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.dianchejie.cn/gtdkidqxel.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.shanyushiyangtech.top/gtuxfautmy.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.gotoacloud.top/gteremnvwl.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.birdmap.top/gtnjkllxzd.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.gotoacloud.top/gttvflaxsz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.jinyuanbaomall.cn/gtkwglixlw.html

[F03] 写入文件（覆盖）
来源：http://hz.gzhubu.top/gtaypherdx.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.zhixingplan.top/gtrjrhmbhm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.ehwqpu.com/gtwjckvdtq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.redwolf501.top/gtfhizaywj.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.vqdsnc.cn/gtuomplzkh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.jlsjyb.cn/gtzqkslxgl.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.0kj1m.cn/gtnjkwkyga.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.ivvv.top/gtwlxoegco.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.sweek.top/gtmzlitgjd.html

[F04] 追加写入文件
来源：http://hz.ydzc1.top/gtbnszwuqw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.52xcode.cn/gtfbshzkls.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.zhengqikj.top/gtopuxzema.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.aizwys.cn/gtrubfapsf.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.sysykeji.top/gtduvejcwx.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.cdnleiting.top/gtjrnoimph.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.yangfankeji.com/gtcfrommyb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.9152youxi.cn/gtlqzjdnhk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.nwbrower.top/gtpeswhbof.html

[F05] 判断文件或目录是否存在
来源：http://hz.sufxvd.cn/gtqfajfccp.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.yvedp.cn/gtbgqdlaoj.html

PHP:  file_exists("a.txt");
来源：http://hz.havefunace.top/gtahmlrcjw.html

JS:   fs.existsSync("a.txt")
来源：http://hz.cqqwz.cn/gtbcbajstv.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yj20258888.top/gtjbtcbnzt.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.jinqigfzy.top/gtzoxuxrpt.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.tian-w.cn/gtasqfyrup.html

Ruby: File.exist?("a.txt")
来源：http://hz.hnxiangtu.top/gtoqxwxdxx.html

C#:   File.Exists("a.txt")
来源：http://hz.yueranfly.top/gtfoiklxii.html

[F06] 删除文件
来源：http://hz.ivvv.top/gtieygngzv.html

Py:   os.remove("a.txt")
来源：http://hz.52xcode.cn/gtscnaczgl.html

PHP:  unlink("a.txt");
来源：http://hz.zhaomingkeji.xyz/gtcoyzgnra.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yueranfly.top/gtpxmgkkme.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.zhixingplan.top/gthwfrvadl.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.redwolf501.top/gtiyhjbdlm.html

Go:   os.Remove("a.txt")
来源：http://hz.hongshengwenyu.top/gtkhudufkr.html

Ruby: File.delete("a.txt")
来源：http://hz.chenlongwang.top/gtgxhfaazk.html

C#:   File.Delete("a.txt");
来源：http://hz.pengpengdd.cyou/gtcmvfottz.html

[F07] 创建目录（含多级）
来源：http://hz.snrcjt.cn/gtustpvtpn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.shanyushiyangtech.top/gtmzkyjeie.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.jinghuilouyu.cn/gthmqirxve.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhengqikj.top/gtiiuynfqs.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.havefunace.top/gtuexbexip.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.316326.xyz/gtixsbkedp.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.shangyingyoupin.top/gtursxhhdf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.zycfv.cn/gtxqfjhvzt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.ehwqpu.com/gtvjszdhvk.html

[F08] 遍历目录
来源：http://hz.haohaochexian.top/gtpfgulejn.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.mhx1999.top/gtgrtarhxx.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.gaohongyu789.top/gtfqjtecdp.html

JS:   fs.readdirSync("dir")
来源：http://hz.havefunace.top/gtdbclporu.html

TS:   fs.readdirSync("dir")
来源：http://hz.shanyushiyangkeji.top/gtdoidrqmu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.zhaomingkeji.xyz/gtykcbsjhw.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.hfpthk.cn/gtbfybdaaq.html

Ruby: Dir.children("dir")
来源：http://hz.yanxiufei.cn/gtaqddspxy.html

C#:   Directory.GetFiles("dir")
来源：http://hz.hnqzz.top/gtpfvtykqx.html

[F09] 获取文件大小
来源：http://hz.tian-w.cn/gtvqthqwvl.html

Py:   os.path.getsize("a.txt")
来源：http://hz.yuxming.cn/gtbhzvjiqq.html

PHP:  filesize("a.txt");
来源：http://hz.xinyue.icu/gtibzpugwu.html

JS:   fs.statSync("a.txt").size
来源：http://hz.hywenlv.cn/gtggcycekf.html

TS:   fs.statSync("a.txt").size
来源：http://hz.zhoulong.xyz/gtkuxxusag.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.yonumen.top/gtxmkvmtvq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.aizwys.cn/gtktussdcm.html

Ruby: File.size("a.txt")
来源：http://hz.pycfn.com/gtqqovahya.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.dashuyun.cn/gtkoibsogm.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.chenzaomai.com/gtpsqyavcr.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.ivvv.top/gtgqcvpwio.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.redwolf501.top/gtdvukfceq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.hywenlv.cn/gtqwjyudzt.html

TS:   path.extname("a.txt")
来源：http://hz.daxiang520.top/gtkfjhtmqg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.shanyushiyangtech.top/gtimjflfzg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.hnxiangtu.top/gtucvyrexh.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jinqigufen.top/gtsvxcjspr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.yonumen.top/gtuawzcniw.html

[F11] 复制与移动文件
来源：http://hz.guannengcc.top/gtiehjeaxo.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.tian-w.cn/gtwzqdatis.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.ydzc1.top/gtyblxdwnk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.daria6918.cn/gtlkrhrkos.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.dashuyun.cn/gtcfsjfjay.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.iojbl.cn/gtivkixtxz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.redwolf501.top/gtllooyzap.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.ybcxt.top/gttvckdsfj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.zycfv.cn/gtcwoyxiuh.html

[F12] CSV 读写
来源：http://hz.zhixingplan.top/gtjigihezx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.yj202588.top/gttjkfrogd.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.xuetiantiany.cn/gtorayalpv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.kuanghao11.cn/gtsqlxwoty.html

TS:   // 同上
来源：http://hz.guannengcc.top/gtwkikgxxn.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.birdmap.top/gthtztaiuv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.pengpengdd.cyou/gtcbbqnjli.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.c1oappe.top/gtzucpnbxf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.ppjwa.cn/gtstcxgfru.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtjqqzbpfy.html

G. 面向对象
来源：http://hz.wangdashe.top/gtlijudqjd.html

================================================================================
来源：http://hz.aibaodan.cn/gtsrggqbaj.html

[G01] 定义类
来源：http://hz.hywenlv.cn/gtuaqfxoyx.html

Py:   class User: pass
来源：http://hz.haohaochexian.top/gtygbdbgxn.html

PHP:  class User {}
来源：http://hz.shzxlz.cn/gtqayhdewx.html

JS:   class User {}
来源：http://hz.iojbl.cn/gtyqiltpjn.html

TS:   class User { name: string = ""; }
来源：http://hz.snrcjt.cn/gtszyqgrrm.html

Java: class User {}
来源：http://hz.daxiang520.top/gtayciwbce.html

Go:   type User struct { Name string }
来源：http://hz.nanxuanxn.top/gteusxprrg.html

Ruby: class User; end
来源：http://hz.jqgufenzy.top/gtqabthytr.html

C#:   class User {}
来源：http://hz.shuidangran.top/gtxpklccva.html

[G02] 构造函数
来源：http://hz.aibaodan.cn/gthktpvpvy.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yonumen.top/gtroldijiy.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yj202588.top/gtezemnxvf.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.tian-w.cn/gtudunqrpc.html

TS:   constructor(public name: string) {}
来源：http://hz.zhiwuduotai.top/gtakywthep.html

Java: User(String name) { this.name = name; }
来源：http://hz.zdqjudy.top/gthaaityim.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.cucudq.cn/gtathxqvjy.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.iojbl.cn/gttvmqjqzp.html

C#:   public User(string name) { Name = name; }
来源：http://hz.yj20258888.top/gtmmlzwrux.html

[G03] 实例属性
来源：http://hz.yj20258888.top/gtwicnojqq.html

Py:   self.name = "x"
来源：http://hz.xingfuxueyuan.xyz/gtgspsiqdc.html

PHP:  public string $name = "x";
来源：http://hz.birdmap.top/gtdgrniycu.html

JS:   this.name = "x";
来源：http://hz.kuanghao11.cn/gtnhogtdsl.html

TS:   name: string = "x";
来源：http://hz.haohaochexian.top/gtmzilyphw.html

Java: private String name;
来源：http://hz.yuxming.cn/gtmrdtnmos.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yanxiufei.cn/gtjrsutore.html

Ruby: @name = "x"
来源：http://hz.chenlongwang.top/gtryjperpq.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.xinyue.icu/gtfwoktzlo.html

[G04] 定义方法
来源：http://hz.ydzc1.top/gtdgigswdd.html

Py:   def greet(self): return self.name
来源：http://hz.jinghuilouyu.cn/gtvzikvlcl.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.ybcxt.top/gtjrlmezbc.html

JS:   greet() { return this.name; }
来源：http://hz.yuxming.cn/gtcdrgmdlx.html

TS:   greet(): string { return this.name; }
来源：http://hz.ywan-chungtsiang.top/gtwosuzjui.html

Java: String greet() { return name; }
来源：http://hz.tanke756.top/gtfglpgkns.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.quarkkingdee.top/gtomhcpayz.html

Ruby: def greet; @name; end
来源：http://hz.tianlin.xyz/gtqpudxfet.html

C#:   public string Greet() => Name;
来源：http://hz.pycfn.com/gttqsxcham.html

[G05] 继承
来源：http://hz.tian-w.cn/gtmdpbrvqx.html

Py:   class Admin(User): pass
来源：http://hz.gogol.net.cn/gtdoyfrnho.html

PHP:  class Admin extends User {}
来源：http://hz.tanke756.top/gtxordnnjl.html

JS:   class Admin extends User {}
来源：http://hz.zhaomingkeji.xyz/gtyrikoflf.html

TS:   class Admin extends User {}
来源：http://hz.ybcxt.top/gtaxhxczfx.html

Java: class Admin extends User {}
来源：http://hz.tian-w.cn/gtklrqezgf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.tanke756.top/gtbcxoazuu.html

Ruby: class Admin < User; end
来源：http://hz.yj202588.top/gtgeprruab.html

C#:   class Admin : User {}
来源：http://hz.vqdsnc.cn/gtorkivnhp.html

[G06] 重写方法
来源：http://hz.zhongyouzk.top/gtjnfufwrg.html

Py:   def greet(self): return "admin"
来源：http://hz.shanyushiyangtech.top/gthbuvwuaf.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jyoumei.cn/gtxdqwwttn.html

JS:   greet() { return "admin"; }
来源：http://hz.yanxiufei.cn/gtjcwjhnqf.html

TS:   greet(): string { return "admin"; }
来源：http://hz.316326.xyz/gterdppuex.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.ehwqpu.com/gtdtozkxyc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.yueranfly.top/gtlsfkotcc.html

Ruby: def greet; "admin"; end
来源：http://hz.wangshuangyany.cn/gtuqdjtsoe.html

C#:   public override string Greet() => "admin";
来源：http://hz.chenlongwang.top/gtcszmmooi.html

[G07] 调用父类方法
来源：http://hz.jinqigfzy.top/gtdohbhdwf.html

Py:   super().greet()
来源：http://hz.zhiwuduotai.top/gtpzjnyrrc.html

PHP:  parent::greet();
来源：http://hz.zhiwuduotai.top/gtaqplahgz.html

JS:   super.greet();
来源：http://hz.sxryk.cn/gttbxmevrk.html

TS:   super.greet();
来源：http://hz.hywenlv.cn/gtsmdqdrri.html

Java: super.greet();
来源：http://hz.cqqwz.cn/gtaxmugppj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.316326.xyz/gtytpxllcx.html

Ruby: super
来源：http://hz.jlsjyb.cn/gtnztnxehk.html

C#:   base.Greet();
来源：http://hz.gaohongyu789.top/gtczmqiqma.html

[G08] 静态方法与属性
来源：http://hz.jinghuilouyu.cn/gtfejjommb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.redwolf501.top/gtbzittams.html

PHP:  public static function f() {}
来源：http://hz.guowangkeji.top/gtijzngcrj.html

JS:   static f() {}
来源：http://hz.hnxiangtu.top/gtxymfncum.html

TS:   static f(): void {}
来源：http://hz.cashguo.top/gtufkydsww.html

Java: static void f() {}
来源：http://hz.bjfxy.top/gtpkggqhth.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jianghu66.top/gtnhfqtyzp.html

Ruby: def self.f; end
来源：http://hz.shangyingyoupin.top/gtdvowwwum.html

C#:   public static void F() {}
来源：http://hz.shzxlz.cn/gtxinzdwaa.html

[G09] 接口 / 抽象类
来源：http://hz.hnxiangtu.top/gtmsxamxhw.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.xziqi.cn/gtzjacnkkd.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.quarkkingdee.top/gtestwamkx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.hongshengwenyu.top/gtlxtidhwv.html

TS:   interface Shape { area(): number; }
来源：http://hz.chenlongwang.top/gtlshkzaxu.html

Java: interface Shape { double area(); }
来源：http://hz.316326.xyz/gtighnnjgr.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.jinyuanbaomall.cn/gtqfmadyrq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.tianlin.xyz/gtrddxhpzx.html

C#:   interface IShape { double Area(); }
来源：http://hz.zhiwuduotai.top/gtnpvzbhxt.html

[G10] 访问控制
来源：http://hz.yangfankeji.com/gtjwksjbqd.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.feifeiyinyue.top/gtccqoaokk.html

PHP:  public / protected / private
来源：http://hz.cdnleiting.top/gtsiktiaxg.html

JS:   #private 字段；其余公开
来源：http://hz.ydzc1.top/gtzyapsrde.html

TS:   public / protected / private
来源：http://hz.jinyuanbaomall.cn/gteqazltqe.html

Java: public / protected / private / 默认包级
来源：http://hz.mhx1999.top/gtrsrhendq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.52xcode.cn/gtybuklmco.html

Ruby: public / protected / private
来源：http://hz.gotoacloud.top/gtytqkfbrf.html

C#:   public / protected / private / internal
来源：http://hz.xinyue.icu/gtbdilvtxr.html

[G11] getter / setter
来源：http://hz.dianchejie.cn/gtiywmkrcu.html

Py:   @property 与 @x.setter
来源：http://hz.yueranfly.top/gttpcponhf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.chenzaomai.com/gtyoeujpwv.html

JS:   get name() { return this._name; }
来源：http://hz.hfpthk.cn/gtiyjewytn.html

TS:   get name(): string { return this._name; }
来源：http://hz.aizwys.cn/gtsbotntby.html

Java: public String getName() { return name; }
来源：http://hz.feifeiyinyue.top/gtspgftmun.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.fengsongda.top/gtoauxbhhw.html

Ruby: attr_accessor :name
来源：http://hz.snrcjt.cn/gtfbjofyml.html

C#:   public string Name { get; set; }
来源：http://hz.ywan-chungtsiang.top/gttlkbdnda.html

[G12] 对象转字符串
来源：http://hz.xingfuxueyuan.xyz/gtnauirowx.html

Py:   def __str__(self): return self.name
来源：http://hz.hammf.cn/gtfotlspec.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.redwolf501.top/gtrjlundpk.html

JS:   toString() { return this.name; }
来源：http://hz.daxiang520.top/gtfxsghrst.html

TS:   toString(): string { return this.name; }
来源：http://hz.sysykeji.top/gtgpwqbats.html

Java: @Override public String toString() { return name; }
来源：http://hz.fzhhl.top/gtghysowxq.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.tanke756.top/gttzkgphjg.html

Ruby: def to_s; @name; end
来源：http://hz.jqgfzy.top/gtiyljglwc.html

C#:   public override string ToString() => Name;
来源：http://hz.fengsongda.top/gtwozmrfdy.html

[G13] 判断对象类型
来源：http://hz.aizwys.cn/gtmsiofdjw.html

Py:   isinstance(u, User)
来源：http://hz.xylfe.cn/gtwxlaeqtt.html

PHP:  $u instanceof User
来源：http://hz.hywenlv.cn/gtjghnatsf.html

JS:   u instanceof User
来源：http://hz.mhx1999.top/gtrzpqlxxm.html

TS:   u instanceof User
来源：http://hz.smart0.xyz/gtsgdghbqd.html

Java: u instanceof User
来源：http://hz.aizwys.cn/gticvwuppe.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.aibaodan.cn/gtkzuaeqyp.html

Ruby: u.is_a?(User)
来源：http://hz.cqqwz.cn/gthkmbktps.html

C#:   u is User
来源：http://hz.yuanzhike.top/gtplwprzoh.html

[G14] 数据类 / record
来源：http://hz.havefunace.top/gtphtmzbke.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.c1oappe.top/gtmektwhyd.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.zhixingplan.top/gtzheeeamk.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.xinyue.icu/gteuabyoev.html

TS:   type User = { name: string; age: number };
来源：http://hz.xinyue.icu/gtbhutlegn.html

Java: record User(String name, int age) {}
来源：http://hz.hnqzz.top/gteyyxontm.html

Go:   type User struct { Name string; Age int }
来源：http://hz.yueranfly.top/gtcwulpeay.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.yuanzhike.top/gtqnfbjvab.html


<!-- 参考信息 -->