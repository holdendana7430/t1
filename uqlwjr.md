代发 wailian999

[T43] Perl：字符串插值
来源：http://hz.xziqi.cn/gtdhbhgsqz.html

"值: $a"
来源：http://hz.hfpthk.cn/gteyzhydsw.html

[T44] Perl：条件
来源：http://hz.chenzaomai.com/gtibciueqf.html

if ($a > 0) { print "正"; }
来源：http://hz.zhijiandao.cn/gthnjdvakg.html

[T45] Perl：数组遍历
来源：http://hz.hnxiangtu.top/gtghlieopc.html

for my $x (@arr) { print $x; }
来源：http://hz.gogol.net.cn/gtfewisdud.html

[T46] Perl：哈希操作
来源：http://hz.shzxlz.cn/gtihbhqaam.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.jinqigufen.top/gtvrqqrvhv.html

[T47] Perl：正则捕获
来源：http://hz.birdmap.top/gtkkfhieqr.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.c1oappe.top/gtfvoliitd.html

[T48] Perl：正则替换
来源：http://hz.cheryme.top/gtfkyqlscj.html

$s =~ s/old/new/g;
来源：http://hz.ybcxt.top/gtfmixxykh.html

[T49] Perl：函数
来源：http://hz.bjfxy.top/gtugmkxsmf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.guowangkeji.top/gtgqyrrebs.html

[T50] Perl：逐行读文件
来源：http://hz.dianchejie.cn/gtdvjqqzfd.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.yueranfly.top/gthxneltsg.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.bjfxy.top/gtkxmugyox.html

[T51] Scala：Hello World
来源：http://hz.ydzc1.top/gtzomxogrp.html

println("Hello")
来源：http://hz.9152youxi.cn/gtgvbtelhq.html

[T52] Scala：变量
来源：http://hz.316326.xyz/gtlvqsqudh.html

val a = 1;  var b = 2
来源：http://hz.gogol.net.cn/gtablovfpw.html

[T53] Scala：字符串插值
来源：http://hz.aibaodan.cn/gtxayfqilh.html

s"值: $b"
来源：http://hz.hfpthk.cn/gtnqeldoil.html

[T54] Scala：集合映射
来源：http://hz.yj20258888.top/gtqenkzomi.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.hongshengwenyu.top/gtokaxcuwr.html

[T55] Scala：集合过滤
来源：http://hz.tian-w.cn/gtozhoqorq.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.jianghu66.top/gtyhckexzt.html

[T56] Scala：样例类
来源：http://hz.gotoacloud.top/gttuftuuxm.html

case class User(name: String, age: Int)
来源：http://hz.nanxuanxn.top/gtdgqjmfta.html

[T57] Scala：模式匹配
来源：http://hz.yj20258888.top/gttrxraqcz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.andypj.xyz/gtmxfyhmis.html

[T58] Scala：函数定义
来源：http://hz.svipenyu.cn/gtouwsijkk.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.zhaomingkeji.xyz/gtzhlvjeuo.html

[T59] Scala：循环
来源：http://hz.hfpthk.cn/gtwusqtphr.html

for (i <- 1 to 10) println(i)
来源：http://hz.shzxlz.cn/gtokiidzed.html

[T60] Scala：折叠
来源：http://hz.chenjidiqi.icu/gtbxbrjorg.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.chenlongwang.top/gtptqgvxna.html

================================================================================
来源：http://hz.nanxuanxn.top/gthbwlwoli.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.kuanghao11.cn/gtcuefprfb.html

================================================================================
来源：http://hz.daxiang520.top/gtiztbbdes.html

[U01] Py：创建虚拟环境
来源：http://hz.quarkkingdee.top/gtmfrjmunj.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.daxiang520.top/gtsqdmbimi.html

[U02] Py：导出 / 安装依赖
来源：http://hz.sweek.top/gtxksrfizs.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.yongpay.top/gtncmafxlw.html

[U03] Py：加载 .env 配置
来源：http://hz.cashguo.top/gtzfnhzway.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.9152youxi.cn/gtdiyyqzav.html

[U04] Py：变量调试打印
来源：http://hz.xziqi.cn/gtyzvlmaks.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.havefunace.top/gtdzghgnuc.html

[U05] Py：列表去重且保序
来源：http://hz.meibo888.top/gttjssiodj.html

list(dict.fromkeys(arr))
来源：http://hz.dianchejie.cn/gtfwpmrcuy.html

[U06] Py：合并两个字典
来源：http://hz.jinqigfzy.top/gtryngslar.html

{**a, **b}
来源：http://hz.cucudq.cn/gtoadqlgfk.html

[U07] Py：反转字典键值
来源：http://hz.xuanzx.com/gtwmfcosay.html

{v: k for k, v in d.items()}
来源：http://hz.wangdashe.top/gtocehhglp.html

[U08] Py：展平二维列表
来源：http://hz.zhengqikj.top/gtosccuibo.html

[y for x in nested for y in x]
来源：http://hz.c1oappe.top/gtrypjsovu.html

[U09] Py：字典取最大值的键
来源：http://hz.ehwqpu.com/gtslqeoagq.html

max(d, key=d.get)
来源：http://hz.9152youxi.cn/gtrjzqvnuf.html

[U10] Py：按值排序字典
来源：http://hz.ydzc1.top/gtbelgeved.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.nanxuanxn.top/gtjvplbsri.html

[U11] Py：生成器表达式
来源：http://hz.yuanzhike.top/gtggcjqguk.html

(x * 2 for x in arr)
来源：http://hz.havefunace.top/gtmxdfxumj.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.yj20258.top/gtsnceycjb.html

Counter(arr).most_common(3)
来源：http://hz.hammf.cn/gtzvllisca.html

[U13] Py：固定长度队列
来源：http://hz.tianlin.xyz/gtdezzjqcj.html

deque(maxlen=10)
来源：http://hz.yj20258.top/gtmnxbvfhd.html

[U14] Py：分组收集到列表
来源：http://hz.hfpthk.cn/gtegvgvdce.html

defaultdict(list)
来源：http://hz.yj202588.top/gtxgfvohql.html

[U15] Py：高精度计时
来源：http://hz.tianlin.xyz/gtcpxrmgrg.html

t = time.perf_counter()
来源：http://hz.zhoulong.xyz/gthbrocggn.html

[U16] Py：命令行参数解析
来源：http://hz.yuanzhike.top/gtnwfywhag.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.hnqzz.top/gtumegilfc.html

[U17] Py：初始化日志
来源：http://hz.ppjwa.cn/gtmhcpyhdu.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.nanxuanxn.top/gtqzxvazab.html

[U18] Py：预编译正则
来源：http://hz.jinqigfzy.top/gtqozqmhav.html

pat = re.compile(r"\d+")
来源：http://hz.guannengcc.top/gtwnhinwmj.html

[U19] Py：正则替换带回调
来源：http://hz.smart0.xyz/gtnytciswd.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.yj202588.top/gtiahetpfs.html

[U20] Py：缓存函数结果
来源：http://hz.svipenyu.cn/gtydnqjmvz.html

@functools.lru_cache(maxsize=None)
来源：http://hz.zhengqikj.top/gtngzybzlt.html

[U21] Py：自定义上下文管理器
来源：http://hz.cdnleiting.top/gtlifsvvnp.html

@contextlib.contextmanager
来源：http://hz.sysykeji.top/gtuleeyzmw.html

[U22] Py：矩阵转置
来源：http://hz.316326.xyz/gtpgyrooxm.html

list(zip(*m))
来源：http://hz.zhongyouzk.top/gtwiiarisk.html

[U23] Py：分块读取大文件
来源：http://hz.ydzc1.top/gtvskwhlsl.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.yj20258.top/gtundcewwf.html

[U24] Py：路径操作
来源：http://hz.vqdsnc.cn/gtweykbdpg.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.9152youxi.cn/gtbqffjfmt.html

[U25] Py：CSV 按字典读
来源：http://hz.jlsjyb.cn/gtzhaucgyz.html

csv.DictReader(f)
来源：http://hz.daria6918.cn/gtxuzaiclw.html

[U26] Py：并发下载
来源：http://hz.quarkkingdee.top/gtllfazkal.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.ydzc1.top/gtzfvjyfwk.html

[U27] Py：异步 HTTP
来源：http://hz.shzxlz.cn/gtuadbwxgg.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.andypj.xyz/gtmvkfuprk.html

[U28] Py：类型别名
来源：http://hz.yongpay.top/gtkdfiexhz.html

UserId = int
来源：http://hz.wangshuangyany.cn/gthoxexbbm.html

[U29] Py：属性校验
来源：http://hz.jinyuanbaomall.cn/gtwhadxpys.html

@property 与 @x.setter 配合
来源：http://hz.daxiang520.top/gthxkqsiil.html

[U30] Py：数据类
来源：http://hz.hammf.cn/gtdxjcogiy.html

@dataclass(slots=True)
来源：http://hz.shanyushiyangtech.top/gtzbeukmlf.html

[U31] Py：单测
来源：http://hz.fzhhl.top/gtgsuowjbd.html

python -m pytest -q
来源：http://hz.nwbrower.top/gtiutqtqhs.html

[U32] Py：代码格式化
来源：http://hz.gogol.net.cn/gttfjyujda.html

ruff format . && ruff check --fix .
来源：http://hz.yueranfly.top/gtjeefzdad.html

[U33] Py：打包发布
来源：http://hz.feifeiyinyue.top/gtptnpthqk.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.xuanzx.com/gtcfteojku.html

[U34] Py：判断编码
来源：http://hz.yvedp.cn/gtfxokyxqu.html

chardet.detect(raw)
来源：http://hz.jinqigfzy.top/gtapupfcav.html

[U35] Py：发送邮件
来源：http://hz.sysykeji.top/gtyfaikvxc.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.ydjk.org.cn/gtbvyvdwbu.html

[U36] Py：定时任务
来源：http://hz.hnxiangtu.top/gtysuscyhp.html

schedule.every(10).minutes.do(job)
来源：http://hz.birdmap.top/gtcdusxssa.html

[U37] Py：读写 Excel
来源：http://hz.haohaochexian.top/gtzduvhtnt.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.snrcjt.cn/gtmazgyvhi.html

[U38] Py：获取脚本所在目录
来源：http://hz.sxryk.cn/gtzphrhzkj.html

Path(__file__).resolve().parent
来源：http://hz.snrcjt.cn/gtpqdkfeut.html

[U39] Py：判断是否在交互环境
来源：http://hz.dashuyun.cn/gtdobokbfn.html

sys.stdout.isatty()
来源：http://hz.cdnleiting.top/gtgbosrnbx.html

[U40] Py：打印到标准错误
来源：http://hz.xinyue.icu/gtlhpzwqdd.html

print("err", file=sys.stderr)
来源：http://hz.chenjidiqi.icu/gtxtluepno.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.jiagoushi.top/gteddxpmef.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.meibo888.top/gteaktgmdq.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.zycfv.cn/gtkzazxddv.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.zhoulong.xyz/gtjcnimovu.html

[U43] PHP：声明命名空间
来源：http://hz.ehwqpu.com/gtjeceequr.html

namespace App\Http;
来源：http://hz.cheryme.top/gtldpfhodk.html

[U44] PHP：开启严格类型
来源：http://hz.cheryme.top/gtqrpzvbdz.html

declare(strict_types=1);
来源：http://hz.dianchejie.cn/gtbghhmlqh.html

[U45] PHP：类型声明与返回类型
来源：http://hz.feifeiyinyue.top/gtjcocswlz.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.shanyushiyangkeji.top/gtrovadrkj.html

[U46] PHP：可空类型
来源：http://hz.zhongyouzk.top/gtzuzdpzha.html

?string $name = null
来源：http://hz.yj202588.top/gtuskbgjls.html

[U47] PHP：联合类型
来源：http://hz.hammf.cn/gtrquuxbfw.html

int|string $id
来源：http://hz.redwolf501.top/gthijcpdwq.html

[U48] PHP：纯枚举
来源：http://hz.ydjk.org.cn/gtawxgennl.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.jinqigufen.top/gtkyygypsn.html

[U49] PHP：只读属性
来源：http://hz.redwolf501.top/gtoxkhbdbo.html

public readonly string $name
来源：http://hz.chenjidiqi.icu/gtxjqjajkx.html

[U50] PHP：构造器属性提升
来源：http://hz.jianghu66.top/gtvmhwgnvo.html

public function __construct(private int $id) {}
来源：http://hz.daria6918.cn/gtejexnfby.html

[U51] PHP：数组解构
来源：http://hz.dianchejie.cn/gtmrkagpll.html

[$a, $b] = $arr;
来源：http://hz.yuxming.cn/gtoznwxayo.html

[U52] PHP：箭头函数
来源：http://hz.shuidangran.top/gtfudfpiar.html

$double = fn($x) => $x * 2;
来源：http://hz.316326.xyz/gtjgexusrg.html

[U53] PHP：空合并运算符
来源：http://hz.zhaomingkeji.xyz/gtvxyuzqxy.html

$v = $a ?? $b ?? "default";
来源：http://hz.yuxming.cn/gtwllyaxaz.html

[U54] PHP：空安全调用
来源：http://hz.kuanghao11.cn/gtpqgguual.html

$obj?->method()
来源：http://hz.yj20258.top/gtwvtnutzg.html

[U55] PHP：match 表达式
来源：http://hz.hammf.cn/gtinzgwimp.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.kuanghao11.cn/gtcdffvwhr.html

[U56] PHP：命名参数
来源：http://hz.hammf.cn/gtlwkseujn.html

f(a: 1, b: 2)
来源：http://hz.zdqjudy.top/gtxhmpofqz.html

[U57] PHP：字符串插值
来源：http://hz.kuanghao11.cn/gtcoovsbzz.html

"值: {$a}"
来源：http://hz.316326.xyz/gtoyrfysuf.html

[U58] PHP：数组三件套
来源：http://hz.zhiwuduotai.top/gtvrxjmzsv.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.xingfuxueyuan.xyz/gtinhbnsln.html

[U59] PHP：自定义排序
来源：http://hz.nanxinkj.top/gtkdsulqkx.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.ybcxt.top/gtzcgbnxvq.html

[U60] PHP：JSON 编解码
来源：http://hz.nwbrower.top/gtpdtfhyob.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.xylfe.cn/gtimcxpydh.html

[U61] PHP：正则
来源：http://hz.feifeiyinyue.top/gteykhddyx.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.hywenlv.cn/gtfhiqzolt.html

[U62] PHP：日期对象
来源：http://hz.fzhhl.top/gtildkyvpe.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.yongpay.top/gtkrlcmdjn.html

[U63] PHP：文件读写
来源：http://hz.havefunace.top/gtpsgffpnt.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.birdmap.top/gtgsogvrbp.html

[U64] PHP：目录遍历
来源：http://hz.yj20258888.top/gtaxdndfhr.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.hfpthk.cn/gtbpehlnky.html

[U65] PHP：会话
来源：http://hz.haohaochexian.top/gtyzkhomab.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.9152youxi.cn/gtalywmcbm.html

[U66] PHP：设置 Cookie
来源：http://hz.dianchejie.cn/gtdxudfvnm.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.daxiang520.top/gtvjruxypt.html

[U67] PHP：处理文件上传
来源：http://hz.gaohongyu789.top/gtmzmkogcx.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.nanxuanxn.top/gtvhmaatpj.html

[U68] PHP：PDO 连接
来源：http://hz.shanyushiyangkeji.top/gtuiinjfdu.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.jqgfzy.top/gtlgyumpoz.html

[U69] PHP：PDO 预处理
来源：http://hz.zhiwuduotai.top/gtjsbcjlwz.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.xinyue.icu/gtasgnqfce.html

[U70] PHP：PDO 事务
来源：http://hz.jinqigfzy.top/gtgrchccbu.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.yonumen.top/gtirlqdgbd.html

[U71] PHP：抛出异常
来源：http://hz.aibaodan.cn/gtxuvkmtnn.html

throw new RuntimeException("失败", 500);
来源：http://hz.sysykeji.top/gtkwslxwgg.html

[U72] PHP：写错误日志
来源：http://hz.dashuyun.cn/gtmxwhgycn.html

error_log("失败: " . $e->getMessage());
来源：http://hz.sufxvd.cn/gtiqpfrzye.html

[U73] PHP：读取 ini 配置
来源：http://hz.redwolf501.top/gttrmtresq.html

parse_ini_file("config.ini", true)
来源：http://hz.meibo888.top/gthkdyweqy.html

[U74] PHP：读取环境变量
来源：http://hz.ivvv.top/gtufpcofhw.html

getenv("APP_ENV") ?: "production"
来源：http://hz.zhongyouzk.top/gthrujkmeh.html

[U75] PHP：依赖注入
来源：http://hz.gaohongyu789.top/gtcfjotjkh.html

composer require psr/container
来源：http://hz.fengsongda.top/gtdatdrwqt.html

[U76] PHP：简单路由
来源：http://hz.havefunace.top/gtfaycyvlo.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.havefunace.top/gtounynche.html

[U77] PHP：模板渲染
来源：http://hz.aibaodan.cn/gtfoksedse.html

composer require twig/twig
来源：http://hz.tanke756.top/gtzwxtykir.html

[U78] PHP：单元测试
来源：http://hz.xziqi.cn/gtjbfacuwu.html

composer require --dev phpunit/phpunit
来源：http://hz.hysaishi.cn/gtmpntgato.html

[U79] PHP：静态分析
来源：http://hz.jinyuanbaomall.cn/gtzycjrpnv.html

composer require --dev phpstan/phpstan
来源：http://hz.tianlin.xyz/gtzbdsqkmy.html

[U80] PHP：代码规范修复
来源：http://hz.hysaishi.cn/gtxgglvrjs.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.cqqwz.cn/gtwlhwlkcg.html

[U81] JS：初始化项目
来源：http://hz.xuanzx.com/gtvhehypap.html

npm init -y;  npm i express
来源：http://hz.yongpay.top/gtggwkhkqh.html

[U82] JS：package.json 脚本
来源：http://hz.xingfuxueyuan.xyz/gtzxfcivql.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.jinqigfzy.top/gthgrqyswn.html

[U83] JS：ES Module 导入导出
来源：http://hz.gotoacloud.top/gtctpqidaa.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.yueranfly.top/gtncqidgbc.html

[U84] JS：CommonJS 写法
来源：http://hz.jyoumei.cn/gtmhhbepob.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.9152youxi.cn/gtgiiwrzup.html

[U85] JS：可选链
来源：http://hz.yueranfly.top/gtjjlomjzp.html

a?.b?.c
来源：http://hz.guowangkeji.top/gtacefmzbq.html

[U86] JS：空值合并
来源：http://hz.zhengqikj.top/gtsnupfhly.html

a ?? b
来源：http://hz.gotoacloud.top/gtytalccod.html

[U87] JS：解构默认值
来源：http://hz.fzhhl.top/gtqtshjywj.html

const { a = 1, b = 2 } = obj;
来源：http://hz.hnqzz.top/gtefqmwxte.html

[U88] JS：对象展开合并
来源：http://hz.jinyuanbaomall.cn/gtwpkzkhvl.html

{ ...a, ...b }
来源：http://hz.zhongyouzk.top/gtelxypklc.html

[U89] JS：数组去重
来源：http://hz.chenlongwang.top/gtiphzskhp.html

[...new Set(arr)]
来源：http://hz.smart0.xyz/gtryexgvci.html

[U90] JS：数字数组排序
来源：http://hz.nanxuanxn.top/gthwqobosg.html

[...arr].sort((a, b) => a - b)
来源：http://hz.ehwqpu.com/gtoubauzak.html

[U91] JS：对象键值遍历
来源：http://hz.chenjidiqi.icu/gtrfdtyhde.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.zhiwuduotai.top/gtcanvklnp.html

[U92] JS：深拷贝
来源：http://hz.jinghuilouyu.cn/gtmblzoohp.html

structuredClone(obj)
来源：http://hz.sweek.top/gtiakmcfmf.html

[U93] JS：模板字符串
来源：http://hz.yuanzhike.top/gtldewprav.html

`共 ${n} 条`
来源：http://hz.jqgufenzy.top/gtuqfgicaz.html

[U94] JS：箭头函数
来源：http://hz.jqgufenzy.top/gtqbhbwsrc.html

const double = x => x * 2;
来源：http://hz.zhiwuduotai.top/gtjhblmfri.html

[U95] JS：Promise 包装
来源：http://hz.jlsjyb.cn/gtjschhmji.html

new Promise((resolve, reject) => {})
来源：http://hz.shangyingyoupin.top/gtdqwqtskr.html

[U96] JS：async/await 与异常
来源：http://hz.nwbrower.top/gtydntqspa.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.gzhubu.top/gtcfphaxpr.html

[U97] JS：并发请求
来源：http://hz.jqgufenzy.top/gtwrrvvmhg.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhijiandao.cn/gtrgnkbmfa.html

[U98] JS：fetch 带 JSON
来源：http://hz.redwolf501.top/gtjnsxqztx.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.zhoulong.xyz/gtzkowjwto.html

[U99] JS：事件监听
来源：http://hz.yj20258888.top/gtpmabvehf.html

el.addEventListener("click", e => {})
来源：http://hz.pengpengdd.cyou/gtnnrvocue.html

[U100] JS：DOM 查询
来源：http://hz.fengsongda.top/gtoqspvgvx.html

document.querySelector(".item")
来源：http://hz.sweek.top/gteqogrjvs.html

[U101] JS：classList 操作
来源：http://hz.cdnleiting.top/gtliubxdoc.html

el.classList.toggle("active")
来源：http://hz.cqqwz.cn/gtxiqtrevn.html

[U102] JS：本地存储
来源：http://hz.ydzc1.top/gtmnscrqyh.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.dianchejie.cn/gtfseyojlq.html

[U103] JS：定时器
来源：http://hz.zhixingplan.top/gtienlmjhg.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.xylfe.cn/gtfvuptllp.html

[U104] JS：防抖
来源：http://hz.guannengcc.top/gtcffqlmvh.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hammf.cn/gtulwhqxjq.html

[U105] JS：节流
来源：http://hz.havefunace.top/gturtvowdj.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.hfpthk.cn/gtthugjcai.html

[U106] JS：日期格式化
来源：http://hz.jlsjyb.cn/gtywnpittq.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.fengsongda.top/gtirqsuhbm.html

[U107] JS：数字千分位
来源：http://hz.ydjk.org.cn/gtakrgausq.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.sysykeji.top/gtbbvosfqc.html

[U108] JS：随机整数
来源：http://hz.havefunace.top/gtpnasmvdi.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.nwbrower.top/gtcaqzfkbw.html

[U109] JS：数组分组
来源：http://hz.yonumen.top/gtmjzznwce.html

Object.groupBy(arr, x => x.type)
来源：http://hz.jiagoushi.top/gtqpcbbmst.html

[U110] JS：数组分块
来源：http://hz.xziqi.cn/gtmeijzzcu.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.nwbrower.top/gtofyyuagd.html

[U111] JS：对象转 Map
来源：http://hz.52xcode.cn/gtvxeboffw.html

new Map(Object.entries(obj))
来源：http://hz.hammf.cn/gtistirnxf.html

[U112] JS：字符串补位
来源：http://hz.xinyue.icu/gtynuszuzm.html

"7".padStart(3, "0")
来源：http://hz.aizwys.cn/gtzoopugus.html

[U113] JS：正则替换全部
来源：http://hz.tian-w.cn/gtxjgoefld.html

s.replaceAll("a", "b")
来源：http://hz.chenlongwang.top/gtaxuelhze.html

[U114] JS：JSON 深比较
来源：http://hz.yj20258.top/gtyqjatqww.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.chenlongwang.top/gtyhjttofx.html

[U115] JS：生成 UUID
来源：http://hz.sysykeji.top/gtfcvpeiiv.html

crypto.randomUUID()
来源：http://hz.ivvv.top/gtjedkyved.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.hywenlv.cn/gtcjqhhoau.html

/** @param {string} name */ function f(name) {}
来源：http://hz.quarkkingdee.top/gtdffaplau.html

[U117] JS：单元测试
来源：http://hz.jiagoushi.top/gtunuejqxe.html

npm i -D vitest;  npx vitest
来源：http://hz.daxiang520.top/gtaowxlzgc.html

[U118] JS：开发服务器
来源：http://hz.zhijiandao.cn/gtzbbmyvpe.html

npm i -D vite;  npx vite
来源：http://hz.nanxinkj.top/gtrerludnw.html

[U119] JS：生产构建
来源：http://hz.gaohongyu789.top/gtijlvpksf.html

npx vite build
来源：http://hz.jqgfzy.top/gtfisdhmow.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.daria6918.cn/gtpwjrvasy.html

import.meta.env.VITE_API_URL
来源：http://hz.hongshengwenyu.top/gtmbursbmg.html

================================================================================
来源：http://hz.yuxming.cn/gtgbcgsjwq.html

统计汇总
来源：http://hz.xinyue.icu/gteqvecjqg.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtzezqvtdk.html

按语言统计（条）：
来源：http://hz.tanke756.top/gtehjiktoj.html

Python ......... 252
来源：http://hz.fengsongda.top/gtquauyhtm.html

PHP ............ 252
来源：http://hz.fzhhl.top/gtgwlhypzh.html

JavaScript ..... 252
来源：http://hz.daria6918.cn/gtvemwegad.html

TypeScript ..... 212
来源：http://hz.ybcxt.top/gtlnxmmdvj.html

Java ........... 212
来源：http://hz.nanxuanxn.top/gtrrizniug.html

Go ............. 212
来源：http://hz.cdnleiting.top/gtqweftnnv.html

Ruby ........... 212
来源：http://hz.jinqigufen.top/gtmzzkumnl.html

C# ............. 212
来源：http://hz.bjfxy.top/gttxgtpxxh.html

C .............. 30
来源：http://hz.cucudq.cn/gtjdkpfzca.html

C++ ............ 30
来源：http://hz.jianghu66.top/gtfjseauqm.html

SQL ............ 90
来源：http://hz.bjfxy.top/gtqyzgguhm.html

Bash ........... 80
来源：http://hz.shanyushiyangtech.top/gtzdyjbtkr.html

Kotlin ......... 15
来源：http://hz.hnqzz.top/gtvoeiwkeb.html

Swift .......... 15
来源：http://hz.ehwqpu.com/gtvwaketsw.html

Lua ............ 10
来源：http://hz.chenjidiqi.icu/gtqupfgual.html

Perl ........... 10
来源：http://hz.yanxiufei.cn/gteepmfglw.html


<!-- 参考信息 -->