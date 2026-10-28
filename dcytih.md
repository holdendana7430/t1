代发 wailian999

[T43] Perl：字符串插值
来源：http://hz.yvedp.cn/gtnthnemff.html

"值: $a"
来源：http://hz.mhx1999.top/gthmnjcote.html

[T44] Perl：条件
来源：http://hz.hnxiangtu.top/gtnvglbctd.html

if ($a > 0) { print "正"; }
来源：http://hz.zhoulong.xyz/gtrmyukwht.html

[T45] Perl：数组遍历
来源：http://hz.yanxiufei.cn/gtiqbxiofy.html

for my $x (@arr) { print $x; }
来源：http://hz.shzxlz.cn/gtgpggzzep.html

[T46] Perl：哈希操作
来源：http://hz.gogol.net.cn/gtqmhumugd.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.feifeiyinyue.top/gtndcxuhaf.html

[T47] Perl：正则捕获
来源：http://hz.aizwys.cn/gtoypsmoas.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.ywan-chungtsiang.top/gtidcwkeml.html

[T48] Perl：正则替换
来源：http://hz.ydzc1.top/gtznkmgwoj.html

$s =~ s/old/new/g;
来源：http://hz.nanxuanxn.top/gturkzejfo.html

[T49] Perl：函数
来源：http://hz.feifeiyinyue.top/gtlaykgbvy.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.havefunace.top/gtfrcrgfwu.html

[T50] Perl：逐行读文件
来源：http://hz.guannengcc.top/gtavqrrwab.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.jinqigufen.top/gtzpgekhoh.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.ydjk.org.cn/gtpovzsblt.html

[T51] Scala：Hello World
来源：http://hz.xuetiantiany.cn/gtphwrgrbg.html

println("Hello")
来源：http://hz.ydzc1.top/gtouxyqyvc.html

[T52] Scala：变量
来源：http://hz.ydjk.org.cn/gtfyirvptk.html

val a = 1;  var b = 2
来源：http://hz.ehwqpu.com/gtwiwgtxua.html

[T53] Scala：字符串插值
来源：http://hz.quarkkingdee.top/gtfkxtfvoz.html

s"值: $b"
来源：http://hz.ivvv.top/gtzddemagx.html

[T54] Scala：集合映射
来源：http://hz.bjfxy.top/gtrlteyrxc.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.snrcjt.cn/gtuvmussaa.html

[T55] Scala：集合过滤
来源：http://hz.zhongyouzk.top/gtlmcbacfi.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.bjfxy.top/gtqiipaqgv.html

[T56] Scala：样例类
来源：http://hz.fengsongda.top/gtvxairuek.html

case class User(name: String, age: Int)
来源：http://hz.yvedp.cn/gtcvdgsohk.html

[T57] Scala：模式匹配
来源：http://hz.yj20258.top/gtvyruamdj.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.daria6918.cn/gtnhjpbkhv.html

[T58] Scala：函数定义
来源：http://hz.52xcode.cn/gtzsxqqciw.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.xinyue.icu/gtchjmjira.html

[T59] Scala：循环
来源：http://hz.316326.xyz/gtzvdfaimu.html

for (i <- 1 to 10) println(i)
来源：http://hz.aizwys.cn/gtatwegoev.html

[T60] Scala：折叠
来源：http://hz.wangdashe.top/gtxquvgzyg.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.yanxiufei.cn/gtdqdrtmkn.html

================================================================================
来源：http://hz.guannengcc.top/gtrqfiiaha.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.9152youxi.cn/gttbntqmrk.html

================================================================================
来源：http://hz.gaohongyu789.top/gtkqkihxeu.html

[U01] Py：创建虚拟环境
来源：http://hz.cheryme.top/gtjcwszuan.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.sysykeji.top/gtmqzdrjmo.html

[U02] Py：导出 / 安装依赖
来源：http://hz.hnxiangtu.top/gtakyjohdx.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.gzhubu.top/gtvufcsopz.html

[U03] Py：加载 .env 配置
来源：http://hz.xylfe.cn/gtzfkjyodo.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.hywenlv.cn/gtirsazetx.html

[U04] Py：变量调试打印
来源：http://hz.hnqzz.top/gtdsitcbtb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.mhx1999.top/gtomsuhgxh.html

[U05] Py：列表去重且保序
来源：http://hz.sufxvd.cn/gtaxsvncdo.html

list(dict.fromkeys(arr))
来源：http://hz.sufxvd.cn/gtozergmsg.html

[U06] Py：合并两个字典
来源：http://hz.zhijiandao.cn/gtbyndotjj.html

{**a, **b}
来源：http://hz.ehwqpu.com/gtymrsrybe.html

[U07] Py：反转字典键值
来源：http://hz.zhengqikj.top/gtmgfxhaqj.html

{v: k for k, v in d.items()}
来源：http://hz.gogol.net.cn/gtnhuindjf.html

[U08] Py：展平二维列表
来源：http://hz.shanyushiyangkeji.top/gtbywgizfb.html

[y for x in nested for y in x]
来源：http://hz.tanke756.top/gtlxexaflm.html

[U09] Py：字典取最大值的键
来源：http://hz.jqgufenzy.top/gttgfpwrfl.html

max(d, key=d.get)
来源：http://hz.haohaochexian.top/gtwjhmpdsv.html

[U10] Py：按值排序字典
来源：http://hz.ivvv.top/gttwlvivmf.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.jqgfzy.top/gtcvzgckwb.html

[U11] Py：生成器表达式
来源：http://hz.vqdsnc.cn/gtnzpzkiye.html

(x * 2 for x in arr)
来源：http://hz.yangfankeji.com/gtdtbpjvog.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.havefunace.top/gttcvrrtod.html

Counter(arr).most_common(3)
来源：http://hz.hongshengwenyu.top/gtrkhvdwxk.html

[U13] Py：固定长度队列
来源：http://hz.redwolf501.top/gtoalhgpkv.html

deque(maxlen=10)
来源：http://hz.yuanzhike.top/gtyocczpfv.html

[U14] Py：分组收集到列表
来源：http://hz.birdmap.top/gtmffpapcv.html

defaultdict(list)
来源：http://hz.hywenlv.cn/gtbttggubc.html

[U15] Py：高精度计时
来源：http://hz.jinqigfzy.top/gtbhkzxlqd.html

t = time.perf_counter()
来源：http://hz.xziqi.cn/gtvhdftlcu.html

[U16] Py：命令行参数解析
来源：http://hz.c1oappe.top/gteepxtvif.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.yvedp.cn/gtusvvprua.html

[U17] Py：初始化日志
来源：http://hz.jyoumei.cn/gttmchimxc.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.ydzc1.top/gthspxfycm.html

[U18] Py：预编译正则
来源：http://hz.gaohongyu789.top/gtqeuidikz.html

pat = re.compile(r"\d+")
来源：http://hz.vqdsnc.cn/gtiuylblfk.html

[U19] Py：正则替换带回调
来源：http://hz.fzhhl.top/gtlmifmual.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.xuetiantiany.cn/gtjnouuvez.html

[U20] Py：缓存函数结果
来源：http://hz.dianchejie.cn/gtlagstuio.html

@functools.lru_cache(maxsize=None)
来源：http://hz.yonumen.top/gtlelrcnmr.html

[U21] Py：自定义上下文管理器
来源：http://hz.nwbrower.top/gtjdpgobzd.html

@contextlib.contextmanager
来源：http://hz.wangdashe.top/gtpsnzhczb.html

[U22] Py：矩阵转置
来源：http://hz.guannengcc.top/gtwaxturxx.html

list(zip(*m))
来源：http://hz.cucudq.cn/gtbclvwbax.html

[U23] Py：分块读取大文件
来源：http://hz.shanyushiyangtech.top/gtldgnsrjc.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.chenjidiqi.icu/gtfgbkhuda.html

[U24] Py：路径操作
来源：http://hz.bjfxy.top/gtjazzissa.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.xinyue.icu/gtlpypjqyb.html

[U25] Py：CSV 按字典读
来源：http://hz.xylfe.cn/gtleigbjlm.html

csv.DictReader(f)
来源：http://hz.0kj1m.cn/gtpiavrbap.html

[U26] Py：并发下载
来源：http://hz.jinqigfzy.top/gtgynaolow.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.jiagoushi.top/gtakqfwjas.html

[U27] Py：异步 HTTP
来源：http://hz.fengsongda.top/gtvvuhkzpt.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.yuanzhike.top/gtdtjoszqm.html

[U28] Py：类型别名
来源：http://hz.hysaishi.cn/gtyrjxprhs.html

UserId = int
来源：http://hz.jinyuanbaomall.cn/gtcmxwzykm.html

[U29] Py：属性校验
来源：http://hz.zhengqikj.top/gtypcvkwrv.html

@property 与 @x.setter 配合
来源：http://hz.hysaishi.cn/gttzbpvlqj.html

[U30] Py：数据类
来源：http://hz.xuanzx.com/gtzmkzqxod.html

@dataclass(slots=True)
来源：http://hz.jlsjyb.cn/gtgjkcflwf.html

[U31] Py：单测
来源：http://hz.aibaodan.cn/gtiynxmpxr.html

python -m pytest -q
来源：http://hz.daxiang520.top/gtlapxgueh.html

[U32] Py：代码格式化
来源：http://hz.jianghu66.top/gtduraplsq.html

ruff format . && ruff check --fix .
来源：http://hz.hammf.cn/gtbworfqrr.html

[U33] Py：打包发布
来源：http://hz.xuanzx.com/gtplmazfhb.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.kuanghao11.cn/gtblmzndbn.html

[U34] Py：判断编码
来源：http://hz.gotoacloud.top/gtwgvmzoic.html

chardet.detect(raw)
来源：http://hz.shanyushiyangtech.top/gtqhlsavrf.html

[U35] Py：发送邮件
来源：http://hz.jinqigufen.top/gtfcjopnoh.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.wangdashe.top/gtehxmpmon.html

[U36] Py：定时任务
来源：http://hz.jinyuanbaomall.cn/gtbfanqmyb.html

schedule.every(10).minutes.do(job)
来源：http://hz.jiagoushi.top/gtixofzcwa.html

[U37] Py：读写 Excel
来源：http://hz.52xcode.cn/gthubqqzth.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.hongshengwenyu.top/gtbkhqfmbd.html

[U38] Py：获取脚本所在目录
来源：http://hz.jiagoushi.top/gtssenogou.html

Path(__file__).resolve().parent
来源：http://hz.c1oappe.top/gtuzzztmwb.html

[U39] Py：判断是否在交互环境
来源：http://hz.nanxinkj.top/gtkqrzrnwx.html

sys.stdout.isatty()
来源：http://hz.gzhubu.top/gtzsgwteyb.html

[U40] Py：打印到标准错误
来源：http://hz.svipenyu.cn/gtymzoxfob.html

print("err", file=sys.stderr)
来源：http://hz.yj202588.top/gtochbihes.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.cheryme.top/gtilubdpjp.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.jqgufenzy.top/gtnovurtcs.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.yuanzhike.top/gtfuycgzvz.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.redwolf501.top/gtxqcbxjer.html

[U43] PHP：声明命名空间
来源：http://hz.yj202588.top/gthghfsbia.html

namespace App\Http;
来源：http://hz.52xcode.cn/gtpbqtjhmp.html

[U44] PHP：开启严格类型
来源：http://hz.jianghu66.top/gtxvffdhnb.html

declare(strict_types=1);
来源：http://hz.hysaishi.cn/gtzffpfbbk.html

[U45] PHP：类型声明与返回类型
来源：http://hz.tian-w.cn/gtuqqqpjxf.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yuxming.cn/gtaziigcng.html

[U46] PHP：可空类型
来源：http://hz.smart0.xyz/gtxlpxjjod.html

?string $name = null
来源：http://hz.cashguo.top/gtnuoowxpq.html

[U47] PHP：联合类型
来源：http://hz.pycfn.com/gtbfsxpcdj.html

int|string $id
来源：http://hz.smart0.xyz/gtvvamfrhu.html

[U48] PHP：纯枚举
来源：http://hz.shangyingyoupin.top/gtimeaydcq.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.yongpay.top/gtfhfvdhim.html

[U49] PHP：只读属性
来源：http://hz.cqqwz.cn/gtmmkipslc.html

public readonly string $name
来源：http://hz.yj202588.top/gtnudggfxe.html

[U50] PHP：构造器属性提升
来源：http://hz.aibaodan.cn/gtktamktgc.html

public function __construct(private int $id) {}
来源：http://hz.sweek.top/gtsivmoykl.html

[U51] PHP：数组解构
来源：http://hz.shzxlz.cn/gtabjvpdjw.html

[$a, $b] = $arr;
来源：http://hz.quarkkingdee.top/gtnkyvxwkb.html

[U52] PHP：箭头函数
来源：http://hz.daxiang520.top/gtmzvhzepv.html

$double = fn($x) => $x * 2;
来源：http://hz.jyoumei.cn/gthpwjgyei.html

[U53] PHP：空合并运算符
来源：http://hz.yj20258888.top/gtxfxlqrkj.html

$v = $a ?? $b ?? "default";
来源：http://hz.bjfxy.top/gtnubqvonq.html

[U54] PHP：空安全调用
来源：http://hz.yj20258.top/gthevgkbdj.html

$obj?->method()
来源：http://hz.dianchejie.cn/gtsaihadpe.html

[U55] PHP：match 表达式
来源：http://hz.zhaomingkeji.xyz/gtrqyapmpm.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.sufxvd.cn/gtexsfipxw.html

[U56] PHP：命名参数
来源：http://hz.xziqi.cn/gtgvfwffch.html

f(a: 1, b: 2)
来源：http://hz.jianghu66.top/gttfhzlbdu.html

[U57] PHP：字符串插值
来源：http://hz.zhixingplan.top/gtmipabunf.html

"值: {$a}"
来源：http://hz.zycfv.cn/gtbandigte.html

[U58] PHP：数组三件套
来源：http://hz.dashuyun.cn/gtkerjvidy.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.shanyushiyangtech.top/gtergzdjig.html

[U59] PHP：自定义排序
来源：http://hz.wangshuangyany.cn/gtrnsdzocv.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.daxiang520.top/gtzgyzvhmm.html

[U60] PHP：JSON 编解码
来源：http://hz.gaohongyu789.top/gtnqfwcthq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.sxryk.cn/gtyqrkwrmj.html

[U61] PHP：正则
来源：http://hz.zhiwuduotai.top/gtlvncqlzy.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.ybcxt.top/gtfmdutvgf.html

[U62] PHP：日期对象
来源：http://hz.pengpengdd.cyou/gtdprpacfc.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.wangdashe.top/gtwcftnrzc.html

[U63] PHP：文件读写
来源：http://hz.andypj.xyz/gthazepsxn.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.smart0.xyz/gtbnuosfah.html

[U64] PHP：目录遍历
来源：http://hz.svipenyu.cn/gtcxspjmyt.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.ivvv.top/gtlgmgpaoo.html

[U65] PHP：会话
来源：http://hz.jinqigufen.top/gtrlbykyho.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.zhengqikj.top/gtkhumrgmu.html

[U66] PHP：设置 Cookie
来源：http://hz.jianghu66.top/gteehmpimx.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.yonumen.top/gtlzqfeoas.html

[U67] PHP：处理文件上传
来源：http://hz.wangshuangyany.cn/gtulvrpqkd.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.fengsongda.top/gtrbwnodlp.html

[U68] PHP：PDO 连接
来源：http://hz.yanxiufei.cn/gtwczrbqbo.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.52xcode.cn/gtprppzequ.html

[U69] PHP：PDO 预处理
来源：http://hz.fengsongda.top/gtluqscfhz.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.cucudq.cn/gtphkolnuw.html

[U70] PHP：PDO 事务
来源：http://hz.gotoacloud.top/gthyawsyud.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.guannengcc.top/gtidmmfsgv.html

[U71] PHP：抛出异常
来源：http://hz.hfpthk.cn/gtfadxnpjf.html

throw new RuntimeException("失败", 500);
来源：http://hz.shanyushiyangtech.top/gtowlgghzx.html

[U72] PHP：写错误日志
来源：http://hz.yj20258.top/gtidxusetf.html

error_log("失败: " . $e->getMessage());
来源：http://hz.ydzc1.top/gtkjcwrwco.html

[U73] PHP：读取 ini 配置
来源：http://hz.hongshengwenyu.top/gtgpyzsrrt.html

parse_ini_file("config.ini", true)
来源：http://hz.guowangkeji.top/gtezpjruum.html

[U74] PHP：读取环境变量
来源：http://hz.jlsjyb.cn/gtalkgyqfe.html

getenv("APP_ENV") ?: "production"
来源：http://hz.zhixingplan.top/gtzhhahqpv.html

[U75] PHP：依赖注入
来源：http://hz.fzhhl.top/gtwypucegc.html

composer require psr/container
来源：http://hz.dianchejie.cn/gtzsmtpiva.html

[U76] PHP：简单路由
来源：http://hz.ydjk.org.cn/gtctthpojn.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.quarkkingdee.top/gtxqpqyoep.html

[U77] PHP：模板渲染
来源：http://hz.sxryk.cn/gtrvmiwfoe.html

composer require twig/twig
来源：http://hz.kuanghao11.cn/gtpmzwmqbq.html

[U78] PHP：单元测试
来源：http://hz.meibo888.top/gtdywzbolc.html

composer require --dev phpunit/phpunit
来源：http://hz.yj20258.top/gtbxfiiuah.html

[U79] PHP：静态分析
来源：http://hz.9152youxi.cn/gthaebpgbx.html

composer require --dev phpstan/phpstan
来源：http://hz.bjfxy.top/gtcoxqnsvu.html

[U80] PHP：代码规范修复
来源：http://hz.9152youxi.cn/gtonqbcmsc.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.sufxvd.cn/gthwjjrlkv.html

[U81] JS：初始化项目
来源：http://hz.shzxlz.cn/gtkbpodlgg.html

npm init -y;  npm i express
来源：http://hz.havefunace.top/gtnaveuwfo.html

[U82] JS：package.json 脚本
来源：http://hz.shangyingyoupin.top/gtwfwplzlk.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.wangdashe.top/gtkthkzgpb.html

[U83] JS：ES Module 导入导出
来源：http://hz.daria6918.cn/gtlguxclav.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.ywan-chungtsiang.top/gtvhbnpory.html

[U84] JS：CommonJS 写法
来源：http://hz.shangyingyoupin.top/gtzqqjapwx.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.jianghu66.top/gtkkrvenvk.html

[U85] JS：可选链
来源：http://hz.aizwys.cn/gtjeqqfdpd.html

a?.b?.c
来源：http://hz.zhoulong.xyz/gthbybdcao.html

[U86] JS：空值合并
来源：http://hz.xinyue.icu/gtnkwllzej.html

a ?? b
来源：http://hz.dianchejie.cn/gtcowutwtk.html

[U87] JS：解构默认值
来源：http://hz.pycfn.com/gtreerjwnc.html

const { a = 1, b = 2 } = obj;
来源：http://hz.yuanzhike.top/gtcpfcedmd.html

[U88] JS：对象展开合并
来源：http://hz.chenzaomai.com/gtooknocyz.html

{ ...a, ...b }
来源：http://hz.gzhubu.top/gthadnzopl.html

[U89] JS：数组去重
来源：http://hz.jqgufenzy.top/gtdjbrwphs.html

[...new Set(arr)]
来源：http://hz.andypj.xyz/gtzewslanu.html

[U90] JS：数字数组排序
来源：http://hz.xingfuxueyuan.xyz/gtkmshnofg.html

[...arr].sort((a, b) => a - b)
来源：http://hz.fengsongda.top/gtrmvufjpf.html

[U91] JS：对象键值遍历
来源：http://hz.sufxvd.cn/gtynwjgzdh.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.havefunace.top/gtanvfwmdb.html

[U92] JS：深拷贝
来源：http://hz.dashuyun.cn/gtbgbxwsvs.html

structuredClone(obj)
来源：http://hz.pycfn.com/gtfmwhuoja.html

[U93] JS：模板字符串
来源：http://hz.316326.xyz/gtrcsxydzd.html

`共 ${n} 条`
来源：http://hz.yuanzhike.top/gtrgnuxppk.html

[U94] JS：箭头函数
来源：http://hz.gzhubu.top/gtnvgwnsff.html

const double = x => x * 2;
来源：http://hz.jiagoushi.top/gtbhazvjci.html

[U95] JS：Promise 包装
来源：http://hz.jinyuanbaomall.cn/gtkfsqwzme.html

new Promise((resolve, reject) => {})
来源：http://hz.shangyingyoupin.top/gtvyodslkc.html

[U96] JS：async/await 与异常
来源：http://hz.bjfxy.top/gtonkuzjim.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.gzhubu.top/gtpsnckdcn.html

[U97] JS：并发请求
来源：http://hz.zhengqikj.top/gtuxdcyuyi.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jqgufenzy.top/gtmvaoncur.html

[U98] JS：fetch 带 JSON
来源：http://hz.yangfankeji.com/gtljdordrb.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.hongshengwenyu.top/gtxpxpsesh.html

[U99] JS：事件监听
来源：http://hz.xingfuxueyuan.xyz/gtshgandci.html

el.addEventListener("click", e => {})
来源：http://hz.bjfxy.top/gtmaolxdxx.html

[U100] JS：DOM 查询
来源：http://hz.zhoulong.xyz/gtvdvgnspv.html

document.querySelector(".item")
来源：http://hz.cqqwz.cn/gthfjixusa.html

[U101] JS：classList 操作
来源：http://hz.cqqwz.cn/gtgjlqpcey.html

el.classList.toggle("active")
来源：http://hz.zhaomingkeji.xyz/gtkedzgwrw.html

[U102] JS：本地存储
来源：http://hz.yonumen.top/gtlvjvriqn.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.shzxlz.cn/gtqbyzmngr.html

[U103] JS：定时器
来源：http://hz.kuanghao11.cn/gtorbrxuhg.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.meibo888.top/gteqrhzooh.html

[U104] JS：防抖
来源：http://hz.chenzaomai.com/gtygovfxef.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.gzhubu.top/gtwozxvuif.html

[U105] JS：节流
来源：http://hz.meibo888.top/gtqcjathtq.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.yuanzhike.top/gtlnxuijft.html

[U106] JS：日期格式化
来源：http://hz.yuanzhike.top/gtrdrxertn.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.hfpthk.cn/gtkjhamzzk.html

[U107] JS：数字千分位
来源：http://hz.yj202588.top/gthwofcdrm.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.yanxiufei.cn/gtziyyyyds.html

[U108] JS：随机整数
来源：http://hz.shanyushiyangtech.top/gtstwatrtw.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.ybcxt.top/gtrcuvjwmn.html

[U109] JS：数组分组
来源：http://hz.kuanghao11.cn/gtalmozbqk.html

Object.groupBy(arr, x => x.type)
来源：http://hz.yanxiufei.cn/gthgyfysup.html

[U110] JS：数组分块
来源：http://hz.bjfxy.top/gtvaqrdxgg.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.jiagoushi.top/gtpxlifhcn.html

[U111] JS：对象转 Map
来源：http://hz.wangshuangyany.cn/gtsvjgezrc.html

new Map(Object.entries(obj))
来源：http://hz.shuidangran.top/gtrktaginv.html

[U112] JS：字符串补位
来源：http://hz.chenzaomai.com/gtzmyudrhh.html

"7".padStart(3, "0")
来源：http://hz.zhoulong.xyz/gtinsdopna.html

[U113] JS：正则替换全部
来源：http://hz.haohaochexian.top/gthwrscuus.html

s.replaceAll("a", "b")
来源：http://hz.chenlongwang.top/gtnqqccocp.html

[U114] JS：JSON 深比较
来源：http://hz.shzxlz.cn/gttspbuick.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.hfpthk.cn/gtaulyrowk.html

[U115] JS：生成 UUID
来源：http://hz.shanyushiyangkeji.top/gtucsdjmvb.html

crypto.randomUUID()
来源：http://hz.zhixingplan.top/gtcptaajvz.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.xylfe.cn/gtgkfjzvvt.html

/** @param {string} name */ function f(name) {}
来源：http://hz.cashguo.top/gtoruwkske.html

[U117] JS：单元测试
来源：http://hz.smart0.xyz/gtawnfwdur.html

npm i -D vitest;  npx vitest
来源：http://hz.ydjk.org.cn/gtzbdpjynw.html

[U118] JS：开发服务器
来源：http://hz.wangshuangyany.cn/gtwztftztm.html

npm i -D vite;  npx vite
来源：http://hz.dianchejie.cn/gtkqrxwmaw.html

[U119] JS：生产构建
来源：http://hz.bjfxy.top/gtasidcmcl.html

npx vite build
来源：http://hz.c1oappe.top/gtqowqdkol.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.hammf.cn/gtspgjmajp.html

import.meta.env.VITE_API_URL
来源：http://hz.ppjwa.cn/gttiswpvxf.html

================================================================================
来源：http://hz.hywenlv.cn/gtbhqvgnbm.html

统计汇总
来源：http://hz.dashuyun.cn/gtdivohemj.html

================================================================================
来源：http://hz.hammf.cn/gtltllavmq.html

按语言统计（条）：
来源：http://hz.chenzaomai.com/gthcxndiow.html

Python ......... 252
来源：http://hz.hnqzz.top/gtbqdkpwue.html

PHP ............ 252
来源：http://hz.chenzaomai.com/gtfrghxtzl.html

JavaScript ..... 252
来源：http://hz.andypj.xyz/gtnhfhgovy.html

TypeScript ..... 212
来源：http://hz.yonumen.top/gtonqzieun.html

Java ........... 212
来源：http://hz.hnxiangtu.top/gtvhxeotfg.html

Go ............. 212
来源：http://hz.shangyingyoupin.top/gtjorkdoyy.html

Ruby ........... 212
来源：http://hz.gogol.net.cn/gtigptphul.html

C# ............. 212
来源：http://hz.yongpay.top/gtjktgsgwi.html

C .............. 30
来源：http://hz.wangshuangyany.cn/gtpdlikhhq.html

C++ ............ 30
来源：http://hz.yvedp.cn/gtrnonynnp.html

SQL ............ 90
来源：http://hz.jyoumei.cn/gtcovmiqfx.html

Bash ........... 80
来源：http://hz.daria6918.cn/gtjrsshvid.html

Kotlin ......... 15
来源：http://hz.meibo888.top/gtgbpapivr.html

Swift .......... 15
来源：http://hz.xziqi.cn/gtaoworwvy.html

Lua ............ 10
来源：http://hz.yvedp.cn/gteepxvkzh.html

Perl ........... 10
来源：http://hz.hysaishi.cn/gtmcbioxpc.html


<!-- 参考信息 -->