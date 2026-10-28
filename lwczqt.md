代发 wailian999

[T45] Perl：数组遍历
来源：http://hz.cheryme.top/gtjlnooowd.html

for my $x (@arr) { print $x; }
来源：http://hz.52xcode.cn/gttskjspfp.html

[T46] Perl：哈希操作
来源：http://hz.jiagoushi.top/gtkgseppqw.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.xylfe.cn/gtkkflcslb.html

[T47] Perl：正则捕获
来源：http://hz.jinqigufen.top/gtuknpenci.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.pycfn.com/gtyjdonabd.html

[T48] Perl：正则替换
来源：http://hz.zhongyouzk.top/gtqnpgpawq.html

$s =~ s/old/new/g;
来源：http://hz.shanyushiyangtech.top/gtrnryqzke.html

[T49] Perl：函数
来源：http://hz.yanxiufei.cn/gtczyyulsa.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.pengpengdd.cyou/gtunqnsnlz.html

[T50] Perl：逐行读文件
来源：http://hz.yj202588.top/gtwysvypne.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.xziqi.cn/gtsplmncew.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.zycfv.cn/gtyjustgwo.html

[T51] Scala：Hello World
来源：http://hz.tianlin.xyz/gtqzaykqkj.html

println("Hello")
来源：http://hz.cashguo.top/gtidoxknia.html

[T52] Scala：变量
来源：http://hz.guowangkeji.top/gtrpnvnamx.html

val a = 1;  var b = 2
来源：http://hz.meibo888.top/gtewntxoyw.html

[T53] Scala：字符串插值
来源：http://hz.tanke756.top/gtswctfzjx.html

s"值: $b"
来源：http://hz.ppjwa.cn/gtejpcsdqk.html

[T54] Scala：集合映射
来源：http://hz.hysaishi.cn/gtnbfdltpo.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.ydzc1.top/gtnrvomixl.html

[T55] Scala：集合过滤
来源：http://hz.shuidangran.top/gtgokieibv.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.gzhubu.top/gtmkmbyvgm.html

[T56] Scala：样例类
来源：http://hz.jqgufenzy.top/gtfnoztisd.html

case class User(name: String, age: Int)
来源：http://hz.svipenyu.cn/gtkljuofic.html

[T57] Scala：模式匹配
来源：http://hz.sufxvd.cn/gtklppejze.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.hywenlv.cn/gtrwkoekys.html

[T58] Scala：函数定义
来源：http://hz.zycfv.cn/gttqxzdhcn.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.chenjidiqi.icu/gtpfdxdppz.html

[T59] Scala：循环
来源：http://hz.tianlin.xyz/gtwvzmmcwi.html

for (i <- 1 to 10) println(i)
来源：http://hz.aizwys.cn/gtinwsppbw.html

[T60] Scala：折叠
来源：http://hz.xylfe.cn/gtcoxwjewh.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.sweek.top/gtdfjnfeoo.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtryptzcrb.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.yuxming.cn/gtjquwedab.html

================================================================================
来源：http://hz.zhijiandao.cn/gtnmegekjm.html

[U01] Py：创建虚拟环境
来源：http://hz.zhongyouzk.top/gtigbbfrsj.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.guannengcc.top/gtyyplholk.html

[U02] Py：导出 / 安装依赖
来源：http://hz.chenjidiqi.icu/gtkbimfswp.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.wangshuangyany.cn/gtsqefzpwq.html

[U03] Py：加载 .env 配置
来源：http://hz.sufxvd.cn/gtcovclhol.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.zhijiandao.cn/gtmzjkdzvq.html

[U04] Py：变量调试打印
来源：http://hz.xuanzx.com/gteobubvas.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.nanxuanxn.top/gtiqsbivnm.html

[U05] Py：列表去重且保序
来源：http://hz.jqgfzy.top/gtpwcciuau.html

list(dict.fromkeys(arr))
来源：http://hz.jlsjyb.cn/gthwwkfkmo.html

[U06] Py：合并两个字典
来源：http://hz.yj20258.top/gtmvffndlo.html

{**a, **b}
来源：http://hz.sysykeji.top/gthmscwins.html

[U07] Py：反转字典键值
来源：http://hz.yanxiufei.cn/gtsozzjkwp.html

{v: k for k, v in d.items()}
来源：http://hz.cdnleiting.top/gtmzzuhcrg.html

[U08] Py：展平二维列表
来源：http://hz.dashuyun.cn/gturkpghsf.html

[y for x in nested for y in x]
来源：http://hz.wangshuangyany.cn/gtwknynjjs.html

[U09] Py：字典取最大值的键
来源：http://hz.hongshengwenyu.top/gtceorvhsh.html

max(d, key=d.get)
来源：http://hz.hnqzz.top/gtvahibkxa.html

[U10] Py：按值排序字典
来源：http://hz.ybcxt.top/gtnxvxiwtb.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.sysykeji.top/gtxqqsexvo.html

[U11] Py：生成器表达式
来源：http://hz.zhijiandao.cn/gtpubdcpiw.html

(x * 2 for x in arr)
来源：http://hz.fengsongda.top/gtnrwrnbqs.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.nwbrower.top/gtjxpacfii.html

Counter(arr).most_common(3)
来源：http://hz.gotoacloud.top/gtlucaxdey.html

[U13] Py：固定长度队列
来源：http://hz.fengsongda.top/gtauddalxy.html

deque(maxlen=10)
来源：http://hz.tianlin.xyz/gtshngiypw.html

[U14] Py：分组收集到列表
来源：http://hz.jianghu66.top/gtifhbyeef.html

defaultdict(list)
来源：http://hz.zhengqikj.top/gtltpxfjun.html

[U15] Py：高精度计时
来源：http://hz.mhx1999.top/gtbcimcwba.html

t = time.perf_counter()
来源：http://hz.c1oappe.top/gtntbpnhix.html

[U16] Py：命令行参数解析
来源：http://hz.yuanzhike.top/gtbcdaaica.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.snrcjt.cn/gtjcrsufdk.html

[U17] Py：初始化日志
来源：http://hz.shzxlz.cn/gtuwvbmptd.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.jyoumei.cn/gtanbrumnt.html

[U18] Py：预编译正则
来源：http://hz.c1oappe.top/gtftluqxha.html

pat = re.compile(r"\d+")
来源：http://hz.guannengcc.top/gtwslzocdg.html

[U19] Py：正则替换带回调
来源：http://hz.nanxinkj.top/gtkhfeelrd.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.yuxming.cn/gtpymhmlmc.html

[U20] Py：缓存函数结果
来源：http://hz.xingfuxueyuan.xyz/gtymbhyfhz.html

@functools.lru_cache(maxsize=None)
来源：http://hz.cheryme.top/gtsfunvafb.html

[U21] Py：自定义上下文管理器
来源：http://hz.hongshengwenyu.top/gtmcofweqn.html

@contextlib.contextmanager
来源：http://hz.gaohongyu789.top/gtfbowhvfk.html

[U22] Py：矩阵转置
来源：http://hz.xuanzx.com/gtybgkkodk.html

list(zip(*m))
来源：http://hz.ybcxt.top/gtjiiigcvh.html

[U23] Py：分块读取大文件
来源：http://hz.yueranfly.top/gtjoldvrgu.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.feifeiyinyue.top/gtcyyyqmgx.html

[U24] Py：路径操作
来源：http://hz.ivvv.top/gtnvljkldy.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.birdmap.top/gtteigfyfq.html

[U25] Py：CSV 按字典读
来源：http://hz.tian-w.cn/gtqfrevzye.html

csv.DictReader(f)
来源：http://hz.jianghu66.top/gtigdpnlwa.html

[U26] Py：并发下载
来源：http://hz.xingfuxueyuan.xyz/gtzthakddp.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.fzhhl.top/gtxruoxswn.html

[U27] Py：异步 HTTP
来源：http://hz.yongpay.top/gtjgmlpotv.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.jiagoushi.top/gtcqhctvbj.html

[U28] Py：类型别名
来源：http://hz.iojbl.cn/gtowtbfgiq.html

UserId = int
来源：http://hz.jinyuanbaomall.cn/gtouixqxrh.html

[U29] Py：属性校验
来源：http://hz.xuanzx.com/gtjdcjapns.html

@property 与 @x.setter 配合
来源：http://hz.sxryk.cn/gtwznmgxsp.html

[U30] Py：数据类
来源：http://hz.pengpengdd.cyou/gtiyshmlew.html

@dataclass(slots=True)
来源：http://hz.hfpthk.cn/gtnambagsy.html

[U31] Py：单测
来源：http://hz.zhixingplan.top/gtcsomlfij.html

python -m pytest -q
来源：http://hz.sxryk.cn/gtexvwcdha.html

[U32] Py：代码格式化
来源：http://hz.yonumen.top/gtxaayjkrb.html

ruff format . && ruff check --fix .
来源：http://hz.zhongyouzk.top/gtjqjzoovh.html

[U33] Py：打包发布
来源：http://hz.svipenyu.cn/gtbtscjfjv.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.ybcxt.top/gtdrzrbpzg.html

[U34] Py：判断编码
来源：http://hz.yj202588.top/gtlotkgwjy.html

chardet.detect(raw)
来源：http://hz.xziqi.cn/gtwmvqdspc.html

[U35] Py：发送邮件
来源：http://hz.vqdsnc.cn/gteiukizzr.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.zycfv.cn/gtbphpncht.html

[U36] Py：定时任务
来源：http://hz.cdnleiting.top/gtjxlkpdrj.html

schedule.every(10).minutes.do(job)
来源：http://hz.xziqi.cn/gtbahweiky.html

[U37] Py：读写 Excel
来源：http://hz.nanxuanxn.top/gtomchalur.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.chenjidiqi.icu/gtxxibujss.html

[U38] Py：获取脚本所在目录
来源：http://hz.ivvv.top/gtcrrltzlu.html

Path(__file__).resolve().parent
来源：http://hz.hammf.cn/gthyqyigst.html

[U39] Py：判断是否在交互环境
来源：http://hz.yangfankeji.com/gtxdcxnliu.html

sys.stdout.isatty()
来源：http://hz.zhengqikj.top/gtvtimnzth.html

[U40] Py：打印到标准错误
来源：http://hz.cqqwz.cn/gtkyzerpvh.html

print("err", file=sys.stderr)
来源：http://hz.iojbl.cn/gtrvqzlxea.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.yanxiufei.cn/gtwewhadax.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.ydzc1.top/gtevzijrcc.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.xingfuxueyuan.xyz/gtmtotstkx.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.svipenyu.cn/gtrasymbwd.html

[U43] PHP：声明命名空间
来源：http://hz.zhiwuduotai.top/gtbjnteavy.html

namespace App\Http;
来源：http://hz.zhijiandao.cn/gtlwnsrtwh.html

[U44] PHP：开启严格类型
来源：http://hz.gogol.net.cn/gtlorsmsrk.html

declare(strict_types=1);
来源：http://hz.316326.xyz/gtyauvpxps.html

[U45] PHP：类型声明与返回类型
来源：http://hz.redwolf501.top/gtmcskduhj.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.mhx1999.top/gtxpbjrgdb.html

[U46] PHP：可空类型
来源：http://hz.jiagoushi.top/gtuzjqppgl.html

?string $name = null
来源：http://hz.xziqi.cn/gtouikihug.html

[U47] PHP：联合类型
来源：http://hz.haohaochexian.top/gtbthlkgcv.html

int|string $id
来源：http://hz.chenjidiqi.icu/gtslbfqcyl.html

[U48] PHP：纯枚举
来源：http://hz.9152youxi.cn/gtlaupskma.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.yvedp.cn/gtjugiwsfk.html

[U49] PHP：只读属性
来源：http://hz.jinyuanbaomall.cn/gtlkptdyoo.html

public readonly string $name
来源：http://hz.hnqzz.top/gtgvuqdebn.html

[U50] PHP：构造器属性提升
来源：http://hz.gogol.net.cn/gtviyanxgx.html

public function __construct(private int $id) {}
来源：http://hz.yj20258.top/gtfisknvtn.html

[U51] PHP：数组解构
来源：http://hz.gzhubu.top/gtjuleiuaf.html

[$a, $b] = $arr;
来源：http://hz.ivvv.top/gtwbkrrodq.html

[U52] PHP：箭头函数
来源：http://hz.hnxiangtu.top/gtxqacmlki.html

$double = fn($x) => $x * 2;
来源：http://hz.cucudq.cn/gtcseemygm.html

[U53] PHP：空合并运算符
来源：http://hz.guowangkeji.top/gthpqifbcr.html

$v = $a ?? $b ?? "default";
来源：http://hz.shangyingyoupin.top/gtzskarzfy.html

[U54] PHP：空安全调用
来源：http://hz.yuanzhike.top/gtnbpufcgb.html

$obj?->method()
来源：http://hz.svipenyu.cn/gtsikraihs.html

[U55] PHP：match 表达式
来源：http://hz.9152youxi.cn/gtphefenvj.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.tian-w.cn/gtlpalsaew.html

[U56] PHP：命名参数
来源：http://hz.zdqjudy.top/gtdvchuezw.html

f(a: 1, b: 2)
来源：http://hz.svipenyu.cn/gtmeoxhbeb.html

[U57] PHP：字符串插值
来源：http://hz.jinghuilouyu.cn/gtqwnivpvw.html

"值: {$a}"
来源：http://hz.fzhhl.top/gtodrfpzop.html

[U58] PHP：数组三件套
来源：http://hz.zhengqikj.top/gtxvseczvp.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.cqqwz.cn/gtoocmqpmp.html

[U59] PHP：自定义排序
来源：http://hz.aibaodan.cn/gtxijemqch.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.hywenlv.cn/gtgbkhuvwm.html

[U60] PHP：JSON 编解码
来源：http://hz.ehwqpu.com/gtxacsltgi.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.birdmap.top/gtvkqynlpe.html

[U61] PHP：正则
来源：http://hz.shuidangran.top/gtuileytye.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.dashuyun.cn/gtvshrgies.html

[U62] PHP：日期对象
来源：http://hz.jyoumei.cn/gtwsijrtvd.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.sweek.top/gtgfqtopyt.html

[U63] PHP：文件读写
来源：http://hz.zdqjudy.top/gtnzxlvmlr.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.jinghuilouyu.cn/gtmltrmrxn.html

[U64] PHP：目录遍历
来源：http://hz.0kj1m.cn/gttccblksp.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.zhaomingkeji.xyz/gtogfjnazq.html

[U65] PHP：会话
来源：http://hz.jqgufenzy.top/gttyepwmqn.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.jinqigfzy.top/gtoduweyrf.html

[U66] PHP：设置 Cookie
来源：http://hz.nanxuanxn.top/gtfspieorg.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.ppjwa.cn/gtwteubrek.html

[U67] PHP：处理文件上传
来源：http://hz.jinqigfzy.top/gtzneswboo.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.c1oappe.top/gtfzczkdia.html

[U68] PHP：PDO 连接
来源：http://hz.xuetiantiany.cn/gtouzpgsgd.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.meibo888.top/gtlllazrmj.html

[U69] PHP：PDO 预处理
来源：http://hz.vqdsnc.cn/gtsinockmj.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.yonumen.top/gtuwjobfzq.html

[U70] PHP：PDO 事务
来源：http://hz.gaohongyu789.top/gtwksyhdrs.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.52xcode.cn/gtevashoki.html

[U71] PHP：抛出异常
来源：http://hz.jiagoushi.top/gtycctzpee.html

throw new RuntimeException("失败", 500);
来源：http://hz.tanke756.top/gtesakpzpf.html

[U72] PHP：写错误日志
来源：http://hz.jiagoushi.top/gtneqywfsf.html

error_log("失败: " . $e->getMessage());
来源：http://hz.jinghuilouyu.cn/gttgpjcdvy.html

[U73] PHP：读取 ini 配置
来源：http://hz.ydzc1.top/gtznhemqos.html

parse_ini_file("config.ini", true)
来源：http://hz.sweek.top/gtbequmgkl.html

[U74] PHP：读取环境变量
来源：http://hz.hammf.cn/gtjwcdouzx.html

getenv("APP_ENV") ?: "production"
来源：http://hz.zhiwuduotai.top/gtaspjmpjl.html

[U75] PHP：依赖注入
来源：http://hz.jqgfzy.top/gtgozhupso.html

composer require psr/container
来源：http://hz.aizwys.cn/gtpulidntf.html

[U76] PHP：简单路由
来源：http://hz.nanxinkj.top/gtqpukesrc.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.jqgufenzy.top/gtoadxvsja.html

[U77] PHP：模板渲染
来源：http://hz.ehwqpu.com/gtspmvljct.html

composer require twig/twig
来源：http://hz.shangyingyoupin.top/gtxtgigkdw.html

[U78] PHP：单元测试
来源：http://hz.chenlongwang.top/gtjsxnoxur.html

composer require --dev phpunit/phpunit
来源：http://hz.xuetiantiany.cn/gtsxaeoeyp.html

[U79] PHP：静态分析
来源：http://hz.ywan-chungtsiang.top/gtzcfddmpz.html

composer require --dev phpstan/phpstan
来源：http://hz.snrcjt.cn/gtrzlzidnv.html

[U80] PHP：代码规范修复
来源：http://hz.zhiwuduotai.top/gtwyateodz.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.c1oappe.top/gtkrnshaor.html

[U81] JS：初始化项目
来源：http://hz.meibo888.top/gtpujvvnfq.html

npm init -y;  npm i express
来源：http://hz.chenzaomai.com/gtnzwuhiod.html

[U82] JS：package.json 脚本
来源：http://hz.xinyue.icu/gtirhozsxk.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.cashguo.top/gtvpdfqicm.html

[U83] JS：ES Module 导入导出
来源：http://hz.hnqzz.top/gttelrprdt.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.gotoacloud.top/gtobynqtzw.html

[U84] JS：CommonJS 写法
来源：http://hz.nanxinkj.top/gtkqdzwlhd.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.xingfuxueyuan.xyz/gtgalcznhc.html

[U85] JS：可选链
来源：http://hz.cheryme.top/gtoedyqvbi.html

a?.b?.c
来源：http://hz.ywan-chungtsiang.top/gtctokvial.html

[U86] JS：空值合并
来源：http://hz.jiagoushi.top/gtjwujevqf.html

a ?? b
来源：http://hz.0kj1m.cn/gtwxbupqtn.html

[U87] JS：解构默认值
来源：http://hz.ybcxt.top/gtbpyofyae.html

const { a = 1, b = 2 } = obj;
来源：http://hz.guowangkeji.top/gtlrqjsivs.html

[U88] JS：对象展开合并
来源：http://hz.jlsjyb.cn/gtpljwkalh.html

{ ...a, ...b }
来源：http://hz.ydzc1.top/gtnhwgldyo.html

[U89] JS：数组去重
来源：http://hz.9152youxi.cn/gtjqdihmqb.html

[...new Set(arr)]
来源：http://hz.yj20258.top/gtvucaqscs.html

[U90] JS：数字数组排序
来源：http://hz.jinqigfzy.top/gthzkbejya.html

[...arr].sort((a, b) => a - b)
来源：http://hz.hongshengwenyu.top/gtyoiheeaj.html

[U91] JS：对象键值遍历
来源：http://hz.ppjwa.cn/gtqkhtzwvj.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.feifeiyinyue.top/gtzbqopdwo.html

[U92] JS：深拷贝
来源：http://hz.chenjidiqi.icu/gthpkaoimz.html

structuredClone(obj)
来源：http://hz.shuidangran.top/gtryxkthrz.html

[U93] JS：模板字符串
来源：http://hz.cucudq.cn/gtgxesukbt.html

`共 ${n} 条`
来源：http://hz.tanke756.top/gtazfibcji.html

[U94] JS：箭头函数
来源：http://hz.hywenlv.cn/gtskmvkpkx.html

const double = x => x * 2;
来源：http://hz.nanxuanxn.top/gtvwotavvv.html

[U95] JS：Promise 包装
来源：http://hz.aizwys.cn/gtjwlziuss.html

new Promise((resolve, reject) => {})
来源：http://hz.jianghu66.top/gtoegsvikk.html

[U96] JS：async/await 与异常
来源：http://hz.hammf.cn/gtnzzwwyhi.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.wangshuangyany.cn/gtwmhafput.html

[U97] JS：并发请求
来源：http://hz.jinqigfzy.top/gtokxjecqd.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhixingplan.top/gtdbplhqis.html

[U98] JS：fetch 带 JSON
来源：http://hz.nanxinkj.top/gtklljnokc.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.wangshuangyany.cn/gtojdgfqvw.html

[U99] JS：事件监听
来源：http://hz.gotoacloud.top/gtmftzlmuq.html

el.addEventListener("click", e => {})
来源：http://hz.jyoumei.cn/gtpneuidjn.html

[U100] JS：DOM 查询
来源：http://hz.jinyuanbaomall.cn/gtxvxzkigz.html

document.querySelector(".item")
来源：http://hz.dianchejie.cn/gteaynasrk.html

[U101] JS：classList 操作
来源：http://hz.ydjk.org.cn/gttitfswgf.html

el.classList.toggle("active")
来源：http://hz.mhx1999.top/gttssqosdd.html

[U102] JS：本地存储
来源：http://hz.hywenlv.cn/gtdwzzqxso.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.xinyue.icu/gtwjscrewh.html

[U103] JS：定时器
来源：http://hz.daria6918.cn/gtnuclfqqm.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.xinyue.icu/gtsrtsvvvy.html

[U104] JS：防抖
来源：http://hz.yuxming.cn/gtqcrhlgel.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jqgfzy.top/gtephclhze.html

[U105] JS：节流
来源：http://hz.zhoulong.xyz/gtwhmghnlm.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.snrcjt.cn/gtwoykzurb.html

[U106] JS：日期格式化
来源：http://hz.aizwys.cn/gttdajzfkh.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.yuxming.cn/gtwposvhul.html

[U107] JS：数字千分位
来源：http://hz.ywan-chungtsiang.top/gtzewkeake.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.yongpay.top/gtmrszxnij.html

[U108] JS：随机整数
来源：http://hz.ehwqpu.com/gtylhnjtmo.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.aizwys.cn/gtgxrbdnwg.html

[U109] JS：数组分组
来源：http://hz.pycfn.com/gtovzrmpqh.html

Object.groupBy(arr, x => x.type)
来源：http://hz.hongshengwenyu.top/gtrwhpkcss.html

[U110] JS：数组分块
来源：http://hz.xylfe.cn/gtfckrpsto.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.dianchejie.cn/gtxftczudt.html

[U111] JS：对象转 Map
来源：http://hz.sufxvd.cn/gtehywkaeq.html

new Map(Object.entries(obj))
来源：http://hz.sufxvd.cn/gtdamgrxcn.html

[U112] JS：字符串补位
来源：http://hz.havefunace.top/gtvvvkvwik.html

"7".padStart(3, "0")
来源：http://hz.tian-w.cn/gtwjpsyslq.html

[U113] JS：正则替换全部
来源：http://hz.havefunace.top/gtduwxiarr.html

s.replaceAll("a", "b")
来源：http://hz.tianlin.xyz/gtfpmbmfpu.html

[U114] JS：JSON 深比较
来源：http://hz.zhoulong.xyz/gtmnsyqncm.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yangfankeji.com/gtibvtscnx.html

[U115] JS：生成 UUID
来源：http://hz.hywenlv.cn/gtpszpiyjz.html

crypto.randomUUID()
来源：http://hz.daxiang520.top/gtdlqovuqd.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.gzhubu.top/gthrsgpiez.html

/** @param {string} name */ function f(name) {}
来源：http://hz.316326.xyz/gtpxscwagc.html

[U117] JS：单元测试
来源：http://hz.ybcxt.top/gtqwpelcrh.html

npm i -D vitest;  npx vitest
来源：http://hz.nanxuanxn.top/gtxwfgspuq.html

[U118] JS：开发服务器
来源：http://hz.snrcjt.cn/gtoueollrj.html

npm i -D vite;  npx vite
来源：http://hz.xylfe.cn/gtqjpgiryz.html

[U119] JS：生产构建
来源：http://hz.ivvv.top/gtcsrzmqrm.html

npx vite build
来源：http://hz.svipenyu.cn/gtiesphrux.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.jqgfzy.top/gtgzmtucph.html

import.meta.env.VITE_API_URL
来源：http://hz.yueranfly.top/gtzgcpnpgg.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtsxfdmqur.html

统计汇总
来源：http://hz.zhixingplan.top/gtlxnzdpyj.html

================================================================================
来源：http://hz.hnxiangtu.top/gtefwqtqgo.html

按语言统计（条）：
来源：http://hz.chenzaomai.com/gtqhvfrhpb.html

Python ......... 252
来源：http://hz.quarkkingdee.top/gtqgpoxlnp.html

PHP ............ 252
来源：http://hz.bjfxy.top/gtnlhslucu.html

JavaScript ..... 252
来源：http://hz.0kj1m.cn/gtsvofviox.html

TypeScript ..... 212
来源：http://hz.ydzc1.top/gtlsludtlt.html

Java ........... 212
来源：http://hz.0kj1m.cn/gtgnqruszn.html

Go ............. 212
来源：http://hz.quarkkingdee.top/gtkuogebdp.html

Ruby ........... 212
来源：http://hz.gotoacloud.top/gtwppwurtu.html

C# ............. 212
来源：http://hz.wangdashe.top/gtajfdusdb.html

C .............. 30
来源：http://hz.jyoumei.cn/gtkrtdlksc.html

C++ ............ 30
来源：http://hz.yuxming.cn/gtptrxkoml.html

SQL ............ 90
来源：http://hz.c1oappe.top/gtrzvwrfwo.html

Bash ........... 80
来源：http://hz.tian-w.cn/gtohudhegn.html

Kotlin ......... 15
来源：http://hz.zhongyouzk.top/gttvjhiddb.html

Swift .......... 15
来源：http://hz.hongshengwenyu.top/gtjrvcwqzl.html

Lua ............ 10
来源：http://hz.nwbrower.top/gthwcshhdf.html

Perl ........... 10
来源：http://hz.cucudq.cn/gtzrkzmhdq.html

Scala .......... 10
来源：http://hz.chenzaomai.com/gtzhsotuyd.html

------------------------------------
来源：http://hz.jianghu66.top/gtrwaxadra.html

合计 ........... 2106 条
来源：http://hz.vqdsnc.cn/gtmypnbhtz.html

按章节统计：
来源：http://hz.yuanzhike.top/gtfruucinf.html


<!-- 参考信息 -->