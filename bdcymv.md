代发 wailian999

[T47] Perl：正则捕获
来源：http://hz.xziqi.cn/gtszqyaztf.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.shanyushiyangtech.top/gtxyemirwk.html

[T48] Perl：正则替换
来源：http://hz.haohaochexian.top/gtuauedbxp.html

$s =~ s/old/new/g;
来源：http://hz.ywan-chungtsiang.top/gtjkiqdobc.html

[T49] Perl：函数
来源：http://hz.xingfuxueyuan.xyz/gtsrunllmu.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.ppjwa.cn/gtrewyzmxi.html

[T50] Perl：逐行读文件
来源：http://hz.ydzc1.top/gtwzzpuvam.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.dianchejie.cn/gtjedjwtbz.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.yj202588.top/gtfvzivfik.html

[T51] Scala：Hello World
来源：http://hz.0kj1m.cn/gtqmbfdqjz.html

println("Hello")
来源：http://hz.xuanzx.com/gtpxcpmzao.html

[T52] Scala：变量
来源：http://hz.aibaodan.cn/gtsohjulll.html

val a = 1;  var b = 2
来源：http://hz.wangshuangyany.cn/gtbvgbqnem.html

[T53] Scala：字符串插值
来源：http://hz.yangfankeji.com/gtschoulkd.html

s"值: $b"
来源：http://hz.yj202588.top/gtiiivizii.html

[T54] Scala：集合映射
来源：http://hz.redwolf501.top/gtncylpuex.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.tianlin.xyz/gtuoeeqnyl.html

[T55] Scala：集合过滤
来源：http://hz.mhx1999.top/gtchoumhjj.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.vqdsnc.cn/gtkujzhgaq.html

[T56] Scala：样例类
来源：http://hz.feifeiyinyue.top/gttyqunliq.html

case class User(name: String, age: Int)
来源：http://hz.ehwqpu.com/gtqtuqrcwp.html

[T57] Scala：模式匹配
来源：http://hz.feifeiyinyue.top/gtegtxeedi.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.xingfuxueyuan.xyz/gtzkfppcca.html

[T58] Scala：函数定义
来源：http://hz.ybcxt.top/gtwythujyh.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.shanyushiyangkeji.top/gtmawbfegf.html

[T59] Scala：循环
来源：http://hz.redwolf501.top/gtoricepgn.html

for (i <- 1 to 10) println(i)
来源：http://hz.gogol.net.cn/gteezvqoae.html

[T60] Scala：折叠
来源：http://hz.yj20258.top/gtdutgrxbv.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.gzhubu.top/gtsfptrhbc.html

================================================================================
来源：http://hz.yuanzhike.top/gtsuivvlsk.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.jiagoushi.top/gtudlnpgmo.html

================================================================================
来源：http://hz.zhongyouzk.top/gtmexormye.html

[U01] Py：创建虚拟环境
来源：http://hz.shangyingyoupin.top/gtkmllslhg.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.guannengcc.top/gtmrueiogs.html

[U02] Py：导出 / 安装依赖
来源：http://hz.svipenyu.cn/gtcrilqdlb.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.gotoacloud.top/gtqpisfcgh.html

[U03] Py：加载 .env 配置
来源：http://hz.gzhubu.top/gtlykjcnoz.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.hysaishi.cn/gthaeamqxp.html

[U04] Py：变量调试打印
来源：http://hz.ydzc1.top/gteclhjgpl.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.shzxlz.cn/gtzpvvuywu.html

[U05] Py：列表去重且保序
来源：http://hz.dashuyun.cn/gtqrhfmndk.html

list(dict.fromkeys(arr))
来源：http://hz.yueranfly.top/gtxuugwfdy.html

[U06] Py：合并两个字典
来源：http://hz.ydjk.org.cn/gtktgcfaod.html

{**a, **b}
来源：http://hz.quarkkingdee.top/gtihywqzha.html

[U07] Py：反转字典键值
来源：http://hz.guannengcc.top/gtuyoedjnk.html

{v: k for k, v in d.items()}
来源：http://hz.jqgufenzy.top/gtcnxiajdv.html

[U08] Py：展平二维列表
来源：http://hz.guowangkeji.top/gtplwjprws.html

[y for x in nested for y in x]
来源：http://hz.ehwqpu.com/gtvojjcoog.html

[U09] Py：字典取最大值的键
来源：http://hz.jyoumei.cn/gtdafewefx.html

max(d, key=d.get)
来源：http://hz.sxryk.cn/gtfvjikwhk.html

[U10] Py：按值排序字典
来源：http://hz.316326.xyz/gtipmkooio.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.jinqigfzy.top/gtxtgxrmnd.html

[U11] Py：生成器表达式
来源：http://hz.guannengcc.top/gtiwryjgyw.html

(x * 2 for x in arr)
来源：http://hz.jianghu66.top/gtceyodeii.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.xinyue.icu/gtnygywrop.html

Counter(arr).most_common(3)
来源：http://hz.dashuyun.cn/gtwxenatds.html

[U13] Py：固定长度队列
来源：http://hz.shuidangran.top/gtwyffswpy.html

deque(maxlen=10)
来源：http://hz.xziqi.cn/gtufwczzdi.html

[U14] Py：分组收集到列表
来源：http://hz.yongpay.top/gtoacwhghb.html

defaultdict(list)
来源：http://hz.zhaomingkeji.xyz/gtjtnefwqq.html

[U15] Py：高精度计时
来源：http://hz.shzxlz.cn/gtblushchl.html

t = time.perf_counter()
来源：http://hz.gogol.net.cn/gtdvfwitsw.html

[U16] Py：命令行参数解析
来源：http://hz.aibaodan.cn/gtdglkoozr.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.fengsongda.top/gtekbkqlop.html

[U17] Py：初始化日志
来源：http://hz.zhijiandao.cn/gtermdwuxp.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.cucudq.cn/gtdaszpzwl.html

[U18] Py：预编译正则
来源：http://hz.xingfuxueyuan.xyz/gtgwywvzjx.html

pat = re.compile(r"\d+")
来源：http://hz.0kj1m.cn/gtkvfsfkas.html

[U19] Py：正则替换带回调
来源：http://hz.zhaomingkeji.xyz/gtxwewkypz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.yvedp.cn/gtdrkftncg.html

[U20] Py：缓存函数结果
来源：http://hz.gotoacloud.top/gtdywvuvfv.html

@functools.lru_cache(maxsize=None)
来源：http://hz.guowangkeji.top/gtxtcpcxke.html

[U21] Py：自定义上下文管理器
来源：http://hz.snrcjt.cn/gtcaiypzhe.html

@contextlib.contextmanager
来源：http://hz.cheryme.top/gtgrhebbro.html

[U22] Py：矩阵转置
来源：http://hz.9152youxi.cn/gtzfmucvzv.html

list(zip(*m))
来源：http://hz.c1oappe.top/gtdigqpvjy.html

[U23] Py：分块读取大文件
来源：http://hz.gaohongyu789.top/gtjxptsksv.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.hongshengwenyu.top/gteeubiets.html

[U24] Py：路径操作
来源：http://hz.aizwys.cn/gtgzfnghii.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.redwolf501.top/gtbjtzzugr.html

[U25] Py：CSV 按字典读
来源：http://hz.yj20258888.top/gtpzgqgfzw.html

csv.DictReader(f)
来源：http://hz.ybcxt.top/gtdstwvmeo.html

[U26] Py：并发下载
来源：http://hz.cheryme.top/gtchrxheft.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.dianchejie.cn/gtadlbdegy.html

[U27] Py：异步 HTTP
来源：http://hz.shanyushiyangkeji.top/gtlhjvamtf.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.bjfxy.top/gtjwkyuygn.html

[U28] Py：类型别名
来源：http://hz.sxryk.cn/gtmorqhorh.html

UserId = int
来源：http://hz.mhx1999.top/gtiaysekxn.html

[U29] Py：属性校验
来源：http://hz.hysaishi.cn/gtmyrsqhkf.html

@property 与 @x.setter 配合
来源：http://hz.zhongyouzk.top/gtukybosyy.html

[U30] Py：数据类
来源：http://hz.tianlin.xyz/gtsstejphz.html

@dataclass(slots=True)
来源：http://hz.cucudq.cn/gtiwumlmoq.html

[U31] Py：单测
来源：http://hz.wangshuangyany.cn/gtbnphanao.html

python -m pytest -q
来源：http://hz.tian-w.cn/gtbmvyhnhk.html

[U32] Py：代码格式化
来源：http://hz.xuetiantiany.cn/gtbddqqllx.html

ruff format . && ruff check --fix .
来源：http://hz.ydzc1.top/gtwtxfogzw.html

[U33] Py：打包发布
来源：http://hz.shzxlz.cn/gtdllmsrkn.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.nwbrower.top/gtxztturab.html

[U34] Py：判断编码
来源：http://hz.cucudq.cn/gtzjgayajt.html

chardet.detect(raw)
来源：http://hz.bjfxy.top/gtwjpinmco.html

[U35] Py：发送邮件
来源：http://hz.cheryme.top/gthnbjheio.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.yj20258888.top/gtunreygvu.html

[U36] Py：定时任务
来源：http://hz.hysaishi.cn/gtohddnxvi.html

schedule.every(10).minutes.do(job)
来源：http://hz.9152youxi.cn/gtvorbelzz.html

[U37] Py：读写 Excel
来源：http://hz.jqgufenzy.top/gtswuwcurv.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.hongshengwenyu.top/gtucmtpcnp.html

[U38] Py：获取脚本所在目录
来源：http://hz.quarkkingdee.top/gtnwasvtyy.html

Path(__file__).resolve().parent
来源：http://hz.jyoumei.cn/gtoshuhacp.html

[U39] Py：判断是否在交互环境
来源：http://hz.redwolf501.top/gtzrbooyjv.html

sys.stdout.isatty()
来源：http://hz.dianchejie.cn/gtasgeifeg.html

[U40] Py：打印到标准错误
来源：http://hz.tianlin.xyz/gtyydkmgvl.html

print("err", file=sys.stderr)
来源：http://hz.hnxiangtu.top/gtaiwnlkkb.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.iojbl.cn/gtaepcyqni.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.yangfankeji.com/gtublsolzl.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.zhengqikj.top/gtzuhofglt.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.zhoulong.xyz/gtsdsxnxaz.html

[U43] PHP：声明命名空间
来源：http://hz.yuxming.cn/gtzpkbwwyf.html

namespace App\Http;
来源：http://hz.birdmap.top/gtbauyvcat.html

[U44] PHP：开启严格类型
来源：http://hz.feifeiyinyue.top/gtpcjlxabs.html

declare(strict_types=1);
来源：http://hz.yuxming.cn/gtuyavqugw.html

[U45] PHP：类型声明与返回类型
来源：http://hz.yuanzhike.top/gtqnfjgacb.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hongshengwenyu.top/gtmqamorio.html

[U46] PHP：可空类型
来源：http://hz.chenjidiqi.icu/gtqnzjrwcg.html

?string $name = null
来源：http://hz.mhx1999.top/gtauqxmaqy.html

[U47] PHP：联合类型
来源：http://hz.sxryk.cn/gtpkjkauqp.html

int|string $id
来源：http://hz.cdnleiting.top/gteptgduhk.html

[U48] PHP：纯枚举
来源：http://hz.dianchejie.cn/gtkjapdrkn.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.hysaishi.cn/gthnssinuz.html

[U49] PHP：只读属性
来源：http://hz.nwbrower.top/gtctmpapgx.html

public readonly string $name
来源：http://hz.tanke756.top/gtsngtthpl.html

[U50] PHP：构造器属性提升
来源：http://hz.zdqjudy.top/gtlgcjpozf.html

public function __construct(private int $id) {}
来源：http://hz.quarkkingdee.top/gtalepiswe.html

[U51] PHP：数组解构
来源：http://hz.nanxinkj.top/gtvawfcsxe.html

[$a, $b] = $arr;
来源：http://hz.cheryme.top/gtttnbsdxt.html

[U52] PHP：箭头函数
来源：http://hz.wangdashe.top/gtzvmsirkr.html

$double = fn($x) => $x * 2;
来源：http://hz.sweek.top/gtlhvrkjdh.html

[U53] PHP：空合并运算符
来源：http://hz.smart0.xyz/gtyijptczj.html

$v = $a ?? $b ?? "default";
来源：http://hz.jinqigufen.top/gtqqaeoxnk.html

[U54] PHP：空安全调用
来源：http://hz.gogol.net.cn/gtqjkllenl.html

$obj?->method()
来源：http://hz.hysaishi.cn/gtumhvoizp.html

[U55] PHP：match 表达式
来源：http://hz.cucudq.cn/gtqxksxfyd.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.havefunace.top/gtkylbpkdc.html

[U56] PHP：命名参数
来源：http://hz.tanke756.top/gtwozqcniv.html

f(a: 1, b: 2)
来源：http://hz.iojbl.cn/gtzjvmwczt.html

[U57] PHP：字符串插值
来源：http://hz.9152youxi.cn/gtmxmiqsgl.html

"值: {$a}"
来源：http://hz.feifeiyinyue.top/gtsltpoxvb.html

[U58] PHP：数组三件套
来源：http://hz.ehwqpu.com/gtagpjlavd.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.zhoulong.xyz/gtwoijsnby.html

[U59] PHP：自定义排序
来源：http://hz.jinqigufen.top/gttcwhkrar.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.ivvv.top/gtalsewwqo.html

[U60] PHP：JSON 编解码
来源：http://hz.yonumen.top/gtcbzymcaq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.bjfxy.top/gtadlgyjgm.html

[U61] PHP：正则
来源：http://hz.shangyingyoupin.top/gtmsxnplgb.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.cdnleiting.top/gtorgywcty.html

[U62] PHP：日期对象
来源：http://hz.ehwqpu.com/gtomktoqag.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.hywenlv.cn/gtezsowzbe.html

[U63] PHP：文件读写
来源：http://hz.shanyushiyangtech.top/gttbegdqek.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.smart0.xyz/gtrecppegg.html

[U64] PHP：目录遍历
来源：http://hz.cashguo.top/gtlmkinhlf.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.xylfe.cn/gttdzlxomk.html

[U65] PHP：会话
来源：http://hz.shangyingyoupin.top/gtittohrrp.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.jinghuilouyu.cn/gtazywwhfi.html

[U66] PHP：设置 Cookie
来源：http://hz.svipenyu.cn/gtoqpjgcqa.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.xingfuxueyuan.xyz/gtsglbytqn.html

[U67] PHP：处理文件上传
来源：http://hz.hysaishi.cn/gthjrejtco.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.chenlongwang.top/gtxckudcoa.html

[U68] PHP：PDO 连接
来源：http://hz.shanyushiyangkeji.top/gtepkpyujo.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.jyoumei.cn/gtzxzvgoky.html

[U69] PHP：PDO 预处理
来源：http://hz.shanyushiyangkeji.top/gtgsydvmbx.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.cdnleiting.top/gtrsvbdvmq.html

[U70] PHP：PDO 事务
来源：http://hz.ydjk.org.cn/gtfxmnebfz.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.c1oappe.top/gtjivqiowk.html

[U71] PHP：抛出异常
来源：http://hz.cheryme.top/gtdnosyfrr.html

throw new RuntimeException("失败", 500);
来源：http://hz.yanxiufei.cn/gtfpyjjqus.html

[U72] PHP：写错误日志
来源：http://hz.andypj.xyz/gtuocuzpjw.html

error_log("失败: " . $e->getMessage());
来源：http://hz.nanxinkj.top/gtdamqvplz.html

[U73] PHP：读取 ini 配置
来源：http://hz.jqgufenzy.top/gtftlqyyse.html

parse_ini_file("config.ini", true)
来源：http://hz.aizwys.cn/gtwitumovg.html

[U74] PHP：读取环境变量
来源：http://hz.jyoumei.cn/gtssoikkuk.html

getenv("APP_ENV") ?: "production"
来源：http://hz.sweek.top/gtnsnliafg.html

[U75] PHP：依赖注入
来源：http://hz.zycfv.cn/gtntccrvvp.html

composer require psr/container
来源：http://hz.ivvv.top/gtigdzmmxo.html

[U76] PHP：简单路由
来源：http://hz.pengpengdd.cyou/gtwkosbieg.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.chenjidiqi.icu/gtoajhdyfv.html

[U77] PHP：模板渲染
来源：http://hz.andypj.xyz/gtrvuvfuje.html

composer require twig/twig
来源：http://hz.fengsongda.top/gtoxpkfasp.html

[U78] PHP：单元测试
来源：http://hz.xingfuxueyuan.xyz/gtbujdfumy.html

composer require --dev phpunit/phpunit
来源：http://hz.aibaodan.cn/gtyeroxvte.html

[U79] PHP：静态分析
来源：http://hz.pengpengdd.cyou/gtqmeumies.html

composer require --dev phpstan/phpstan
来源：http://hz.shanyushiyangtech.top/gtcaejcvrq.html

[U80] PHP：代码规范修复
来源：http://hz.xylfe.cn/gtsyqbsbaf.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.jianghu66.top/gtbaamtuxw.html

[U81] JS：初始化项目
来源：http://hz.svipenyu.cn/gtdoqvygor.html

npm init -y;  npm i express
来源：http://hz.wangshuangyany.cn/gtqhylhaaa.html

[U82] JS：package.json 脚本
来源：http://hz.zhijiandao.cn/gtojvwzssp.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.c1oappe.top/gtgvrqcrsu.html

[U83] JS：ES Module 导入导出
来源：http://hz.guannengcc.top/gtitfteyew.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.tanke756.top/gtecnosucw.html

[U84] JS：CommonJS 写法
来源：http://hz.cdnleiting.top/gtfaxhozps.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.zhoulong.xyz/gtfjilsfxq.html

[U85] JS：可选链
来源：http://hz.0kj1m.cn/gthucctxyn.html

a?.b?.c
来源：http://hz.haohaochexian.top/gtsuudincd.html

[U86] JS：空值合并
来源：http://hz.jinqigfzy.top/gtotirwtit.html

a ?? b
来源：http://hz.hnxiangtu.top/gtcdtcycrj.html

[U87] JS：解构默认值
来源：http://hz.nanxuanxn.top/gtuicpdylz.html

const { a = 1, b = 2 } = obj;
来源：http://hz.jlsjyb.cn/gturkfanuo.html

[U88] JS：对象展开合并
来源：http://hz.yanxiufei.cn/gtzuuuldox.html

{ ...a, ...b }
来源：http://hz.xingfuxueyuan.xyz/gtvrxsplec.html

[U89] JS：数组去重
来源：http://hz.yongpay.top/gtstzupgoy.html

[...new Set(arr)]
来源：http://hz.ehwqpu.com/gtmpkyygwd.html

[U90] JS：数字数组排序
来源：http://hz.iojbl.cn/gtwhpzguxq.html

[...arr].sort((a, b) => a - b)
来源：http://hz.316326.xyz/gtmshhlekt.html

[U91] JS：对象键值遍历
来源：http://hz.yuanzhike.top/gtrpdvgzfv.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.yonumen.top/gtbvxeqbbj.html

[U92] JS：深拷贝
来源：http://hz.zdqjudy.top/gtogkyppyu.html

structuredClone(obj)
来源：http://hz.hongshengwenyu.top/gtkerxambx.html

[U93] JS：模板字符串
来源：http://hz.zhijiandao.cn/gtsfjufufl.html

`共 ${n} 条`
来源：http://hz.shuidangran.top/gtjrnnuttn.html

[U94] JS：箭头函数
来源：http://hz.wangshuangyany.cn/gtspdgdlhh.html

const double = x => x * 2;
来源：http://hz.zhongyouzk.top/gtdrkotwru.html

[U95] JS：Promise 包装
来源：http://hz.nanxuanxn.top/gtorfbofev.html

new Promise((resolve, reject) => {})
来源：http://hz.tian-w.cn/gtxipjqqhn.html

[U96] JS：async/await 与异常
来源：http://hz.hammf.cn/gtuazbcimj.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.jiagoushi.top/gtjcciopxh.html

[U97] JS：并发请求
来源：http://hz.hnqzz.top/gtsvtcnksq.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.guowangkeji.top/gtutzxyhnn.html

[U98] JS：fetch 带 JSON
来源：http://hz.hnqzz.top/gtxnmawojx.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.xuanzx.com/gtmttbybjq.html

[U99] JS：事件监听
来源：http://hz.zhiwuduotai.top/gtwdxwrybi.html

el.addEventListener("click", e => {})
来源：http://hz.ehwqpu.com/gtgnpzdvkv.html

[U100] JS：DOM 查询
来源：http://hz.shuidangran.top/gtogjnxuda.html

document.querySelector(".item")
来源：http://hz.xingfuxueyuan.xyz/gthkfbdtpx.html

[U101] JS：classList 操作
来源：http://hz.jqgufenzy.top/gtcjibiijn.html

el.classList.toggle("active")
来源：http://hz.hnqzz.top/gtcbonoijd.html

[U102] JS：本地存储
来源：http://hz.ivvv.top/gtlttucgjr.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.feifeiyinyue.top/gtdusqzoab.html

[U103] JS：定时器
来源：http://hz.xuanzx.com/gttxagodyp.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.c1oappe.top/gthonwojsz.html

[U104] JS：防抖
来源：http://hz.hongshengwenyu.top/gtwfnmntcd.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xuanzx.com/gtuywaklnm.html

[U105] JS：节流
来源：http://hz.xinyue.icu/gtwgfkwedo.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.kuanghao11.cn/gtfljlgvpt.html

[U106] JS：日期格式化
来源：http://hz.zdqjudy.top/gtngdnskcr.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.feifeiyinyue.top/gtvhsdrmev.html

[U107] JS：数字千分位
来源：http://hz.wangdashe.top/gteuubbngh.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.zhiwuduotai.top/gtmxlqunre.html

[U108] JS：随机整数
来源：http://hz.zhongyouzk.top/gthidsmubb.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.ydjk.org.cn/gtfyoxqmrm.html

[U109] JS：数组分组
来源：http://hz.zhoulong.xyz/gtyqprthxx.html

Object.groupBy(arr, x => x.type)
来源：http://hz.cheryme.top/gtzpddprqt.html

[U110] JS：数组分块
来源：http://hz.jinqigfzy.top/gtgyrjfysd.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.andypj.xyz/gtxmhhbxkh.html

[U111] JS：对象转 Map
来源：http://hz.daxiang520.top/gttgoxjpup.html

new Map(Object.entries(obj))
来源：http://hz.c1oappe.top/gtnrtbmzbi.html

[U112] JS：字符串补位
来源：http://hz.shzxlz.cn/gtaamttwyc.html

"7".padStart(3, "0")
来源：http://hz.hywenlv.cn/gtbtpfhcif.html

[U113] JS：正则替换全部
来源：http://hz.dianchejie.cn/gtrslxylap.html

s.replaceAll("a", "b")
来源：http://hz.havefunace.top/gtdlzuwnyu.html

[U114] JS：JSON 深比较
来源：http://hz.tianlin.xyz/gtzcxelgmy.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.iojbl.cn/gtwqxmilob.html

[U115] JS：生成 UUID
来源：http://hz.cucudq.cn/gttytybiec.html

crypto.randomUUID()
来源：http://hz.cashguo.top/gttgjjqtzr.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.shangyingyoupin.top/gtwqlzsvjz.html

/** @param {string} name */ function f(name) {}
来源：http://hz.gaohongyu789.top/gtkkqvflfd.html

[U117] JS：单元测试
来源：http://hz.vqdsnc.cn/gtkwcljkqp.html

npm i -D vitest;  npx vitest
来源：http://hz.nanxinkj.top/gtnpaaksqg.html

[U118] JS：开发服务器
来源：http://hz.nanxuanxn.top/gtuwnmjbtt.html

npm i -D vite;  npx vite
来源：http://hz.zhaomingkeji.xyz/gtydildjhf.html

[U119] JS：生产构建
来源：http://hz.c1oappe.top/gthejnavtp.html

npx vite build
来源：http://hz.shuidangran.top/gtjrqsmzjo.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.jianghu66.top/gttujlljix.html

import.meta.env.VITE_API_URL
来源：http://hz.quarkkingdee.top/gtckutnbwr.html

================================================================================
来源：http://hz.birdmap.top/gtqwklbivw.html

统计汇总
来源：http://hz.jyoumei.cn/gtxqyzokdo.html

================================================================================
来源：http://hz.nanxinkj.top/gtrtucsvwp.html

按语言统计（条）：
来源：http://hz.hongshengwenyu.top/gtaknwmkzp.html

Python ......... 252
来源：http://hz.meibo888.top/gthelaybet.html

PHP ............ 252
来源：http://hz.ppjwa.cn/gttlfmgroj.html

JavaScript ..... 252
来源：http://hz.mhx1999.top/gtenqdugex.html

TypeScript ..... 212
来源：http://hz.hfpthk.cn/gtuchkzezn.html

Java ........... 212
来源：http://hz.yj20258.top/gtpqqjclgx.html

Go ............. 212
来源：http://hz.haohaochexian.top/gtmjhgqlbl.html

Ruby ........... 212
来源：http://hz.ivvv.top/gtpocfkahs.html

C# ............. 212
来源：http://hz.hammf.cn/gtejorlqbc.html

C .............. 30
来源：http://hz.chenlongwang.top/gtywrzrtxr.html

C++ ............ 30
来源：http://hz.dashuyun.cn/gtcsoopver.html

SQL ............ 90
来源：http://hz.yonumen.top/gtmjtpgwyp.html

Bash ........... 80
来源：http://hz.52xcode.cn/gtvwqtafms.html

Kotlin ......... 15
来源：http://hz.chenjidiqi.icu/gttqmgljwq.html

Swift .......... 15
来源：http://hz.jqgufenzy.top/gtozxppodd.html

Lua ............ 10
来源：http://hz.jinyuanbaomall.cn/gtqnyqwhiu.html

Perl ........... 10
来源：http://hz.jqgufenzy.top/gtjmpupgqs.html

Scala .......... 10
来源：http://hz.jqgfzy.top/gtbmzowhiu.html

------------------------------------
来源：http://hz.iojbl.cn/gtdwkytupa.html

合计 ........... 2106 条
来源：http://hz.iojbl.cn/gtujzhyomf.html

按章节统计：
来源：http://hz.dashuyun.cn/gtqxqjplpg.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.guowangkeji.top/gtctinapta.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.pengpengdd.cyou/gtugpsznou.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.dianchejie.cn/gtocxctdqq.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.cdnleiting.top/gtwqkhmcze.html


<!-- 参考信息 -->