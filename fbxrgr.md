代发 wailian999

[T47] Perl：正则捕获
来源：http://hz.aizwys.cn/gtxwzxgklw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.ydzc1.top/gtrojnkysp.html

[T48] Perl：正则替换
来源：http://hz.haohaochexian.top/gtixkvwqyj.html

$s =~ s/old/new/g;
来源：http://hz.ybcxt.top/gtfaofjvcr.html

[T49] Perl：函数
来源：http://hz.sysykeji.top/gtxlnrqqgm.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.meibo888.top/gtmzwuiopa.html

[T50] Perl：逐行读文件
来源：http://hz.havefunace.top/gtnuoheuqq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.sxryk.cn/gtjklqkxhu.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.fengsongda.top/gttxrzvaev.html

[T51] Scala：Hello World
来源：http://hz.fzhhl.top/gtqyvssffr.html

println("Hello")
来源：http://hz.birdmap.top/gtujywmaew.html

[T52] Scala：变量
来源：http://hz.hongshengwenyu.top/gtxbopysqf.html

val a = 1;  var b = 2
来源：http://hz.hnqzz.top/gtkcanwvls.html

[T53] Scala：字符串插值
来源：http://hz.bjfxy.top/gtooezgqpt.html

s"值: $b"
来源：http://hz.tian-w.cn/gtfzhfymtr.html

[T54] Scala：集合映射
来源：http://hz.hysaishi.cn/gtvfllagxl.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.sxryk.cn/gtzxckixif.html

[T55] Scala：集合过滤
来源：http://hz.sysykeji.top/gtvmetbnir.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.shanyushiyangtech.top/gtrjggwncb.html

[T56] Scala：样例类
来源：http://hz.cqqwz.cn/gtrfgditky.html

case class User(name: String, age: Int)
来源：http://hz.c1oappe.top/gtwdoehjdh.html

[T57] Scala：模式匹配
来源：http://hz.dianchejie.cn/gthllqagxp.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.sufxvd.cn/gtihndtcgu.html

[T58] Scala：函数定义
来源：http://hz.cheryme.top/gthtmzcsfg.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.pengpengdd.cyou/gtinnkalnm.html

[T59] Scala：循环
来源：http://hz.chenlongwang.top/gtbstsqghr.html

for (i <- 1 to 10) println(i)
来源：http://hz.yuxming.cn/gtuyjsvyqc.html

[T60] Scala：折叠
来源：http://hz.cashguo.top/gtodubkovo.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.hnxiangtu.top/gtnamwallx.html

================================================================================
来源：http://hz.0kj1m.cn/gtrxjtawue.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.hnqzz.top/gtfxyhjzgu.html

================================================================================
来源：http://hz.haohaochexian.top/gtrdogdfrl.html

[U01] Py：创建虚拟环境
来源：http://hz.ppjwa.cn/gtcyxdvket.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.feifeiyinyue.top/gtxaeqzykv.html

[U02] Py：导出 / 安装依赖
来源：http://hz.shanyushiyangkeji.top/gtsdfcxvow.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.hywenlv.cn/gtiskuxjfv.html

[U03] Py：加载 .env 配置
来源：http://hz.jqgfzy.top/gtxrosmaoo.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.svipenyu.cn/gtlywlnzws.html

[U04] Py：变量调试打印
来源：http://hz.wangshuangyany.cn/gtbtcimpvp.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.yj20258.top/gtclialuwb.html

[U05] Py：列表去重且保序
来源：http://hz.xylfe.cn/gtrfabzmmt.html

list(dict.fromkeys(arr))
来源：http://hz.cqqwz.cn/gtaignhvym.html

[U06] Py：合并两个字典
来源：http://hz.ppjwa.cn/gtpdgtznum.html

{**a, **b}
来源：http://hz.yanxiufei.cn/gtyjgowoim.html

[U07] Py：反转字典键值
来源：http://hz.sxryk.cn/gtayokqrgp.html

{v: k for k, v in d.items()}
来源：http://hz.shanyushiyangkeji.top/gtbtjsphgh.html

[U08] Py：展平二维列表
来源：http://hz.ivvv.top/gtuytzzlin.html

[y for x in nested for y in x]
来源：http://hz.ehwqpu.com/gtpnmkcmum.html

[U09] Py：字典取最大值的键
来源：http://hz.hammf.cn/gterkmbyho.html

max(d, key=d.get)
来源：http://hz.wangdashe.top/gtnfokzehy.html

[U10] Py：按值排序字典
来源：http://hz.jqgufenzy.top/gtmhjkgceg.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.cdnleiting.top/gtoapjcalp.html

[U11] Py：生成器表达式
来源：http://hz.pycfn.com/gtiizymnwg.html

(x * 2 for x in arr)
来源：http://hz.kuanghao11.cn/gtaiiarebt.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.ivvv.top/gtpvcqurgi.html

Counter(arr).most_common(3)
来源：http://hz.yuanzhike.top/gttxvqpxux.html

[U13] Py：固定长度队列
来源：http://hz.jiagoushi.top/gtaqwlirsx.html

deque(maxlen=10)
来源：http://hz.iojbl.cn/gtycuxarki.html

[U14] Py：分组收集到列表
来源：http://hz.zhaomingkeji.xyz/gtqgguvbde.html

defaultdict(list)
来源：http://hz.zdqjudy.top/gtsqnthoxg.html

[U15] Py：高精度计时
来源：http://hz.shzxlz.cn/gtsjivaumn.html

t = time.perf_counter()
来源：http://hz.yj20258.top/gtibpmefgt.html

[U16] Py：命令行参数解析
来源：http://hz.jqgfzy.top/gtscvvljqv.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.cheryme.top/gtnrpuxcmr.html

[U17] Py：初始化日志
来源：http://hz.pengpengdd.cyou/gtvoajhxtt.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.nwbrower.top/gtxwlxcdih.html

[U18] Py：预编译正则
来源：http://hz.ydjk.org.cn/gtbhdeywli.html

pat = re.compile(r"\d+")
来源：http://hz.ywan-chungtsiang.top/gtmdelbpau.html

[U19] Py：正则替换带回调
来源：http://hz.hysaishi.cn/gtaqhdbitp.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.aibaodan.cn/gtkvopydbj.html

[U20] Py：缓存函数结果
来源：http://hz.jinqigufen.top/gtpwiqctfo.html

@functools.lru_cache(maxsize=None)
来源：http://hz.xingfuxueyuan.xyz/gtottzuczy.html

[U21] Py：自定义上下文管理器
来源：http://hz.aizwys.cn/gtlmdlwuit.html

@contextlib.contextmanager
来源：http://hz.hnqzz.top/gtvmbsxpef.html

[U22] Py：矩阵转置
来源：http://hz.hnxiangtu.top/gtblgksyom.html

list(zip(*m))
来源：http://hz.wangdashe.top/gtulksxmsy.html

[U23] Py：分块读取大文件
来源：http://hz.hfpthk.cn/gtgfyjlstr.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.vqdsnc.cn/gtduzqvxkn.html

[U24] Py：路径操作
来源：http://hz.hywenlv.cn/gtworywmtv.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.pengpengdd.cyou/gtnresxzla.html

[U25] Py：CSV 按字典读
来源：http://hz.aizwys.cn/gthssecqwn.html

csv.DictReader(f)
来源：http://hz.chenzaomai.com/gtyvocfoqe.html

[U26] Py：并发下载
来源：http://hz.hysaishi.cn/gtvaacjtpd.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.chenzaomai.com/gtnsgxpuxl.html

[U27] Py：异步 HTTP
来源：http://hz.fzhhl.top/gtrkhffwwz.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.zhengqikj.top/gtlwbcbjjd.html

[U28] Py：类型别名
来源：http://hz.iojbl.cn/gtfjffzurz.html

UserId = int
来源：http://hz.zdqjudy.top/gtszjyjcrt.html

[U29] Py：属性校验
来源：http://hz.redwolf501.top/gttwehozlp.html

@property 与 @x.setter 配合
来源：http://hz.yueranfly.top/gtzfzkoacx.html

[U30] Py：数据类
来源：http://hz.feifeiyinyue.top/gtmharxgjf.html

@dataclass(slots=True)
来源：http://hz.c1oappe.top/gttveriqol.html

[U31] Py：单测
来源：http://hz.yangfankeji.com/gtekugsipp.html

python -m pytest -q
来源：http://hz.dashuyun.cn/gtacncyywm.html

[U32] Py：代码格式化
来源：http://hz.chenlongwang.top/gtdwrdxbwu.html

ruff format . && ruff check --fix .
来源：http://hz.birdmap.top/gtgkocgjgn.html

[U33] Py：打包发布
来源：http://hz.0kj1m.cn/gtkrvbydgq.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.ybcxt.top/gtasanysak.html

[U34] Py：判断编码
来源：http://hz.ydzc1.top/gttrmjjxjy.html

chardet.detect(raw)
来源：http://hz.jinqigufen.top/gtmfppubxz.html

[U35] Py：发送邮件
来源：http://hz.dianchejie.cn/gtudydlihc.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.shanyushiyangtech.top/gttqbgxkxt.html

[U36] Py：定时任务
来源：http://hz.316326.xyz/gtczepoogn.html

schedule.every(10).minutes.do(job)
来源：http://hz.zdqjudy.top/gtowzfnovl.html

[U37] Py：读写 Excel
来源：http://hz.xuetiantiany.cn/gthliwwjje.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.zhiwuduotai.top/gtrxlqtvlj.html

[U38] Py：获取脚本所在目录
来源：http://hz.gaohongyu789.top/gtwxbhxtzc.html

Path(__file__).resolve().parent
来源：http://hz.meibo888.top/gtlsrkcapf.html

[U39] Py：判断是否在交互环境
来源：http://hz.hnxiangtu.top/gtpwkvbqzq.html

sys.stdout.isatty()
来源：http://hz.jqgfzy.top/gtqgleqqol.html

[U40] Py：打印到标准错误
来源：http://hz.nwbrower.top/gtfslgyazp.html

print("err", file=sys.stderr)
来源：http://hz.xinyue.icu/gtvuafejpi.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.jinqigufen.top/gtkxogzkyr.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.meibo888.top/gtjsywdqbc.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.aibaodan.cn/gtqakcfytr.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.hfpthk.cn/gtshttstsk.html

[U43] PHP：声明命名空间
来源：http://hz.zycfv.cn/gtgubgxpws.html

namespace App\Http;
来源：http://hz.iojbl.cn/gtuybcescg.html

[U44] PHP：开启严格类型
来源：http://hz.kuanghao11.cn/gtpnnoorhg.html

declare(strict_types=1);
来源：http://hz.ydzc1.top/gtkoheexoi.html

[U45] PHP：类型声明与返回类型
来源：http://hz.yueranfly.top/gtnubeqeay.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.tanke756.top/gtffdeggon.html

[U46] PHP：可空类型
来源：http://hz.smart0.xyz/gtniqpnlxl.html

?string $name = null
来源：http://hz.haohaochexian.top/gtuzrdvjbg.html

[U47] PHP：联合类型
来源：http://hz.snrcjt.cn/gtftngcldx.html

int|string $id
来源：http://hz.cdnleiting.top/gtfpggqvrk.html

[U48] PHP：纯枚举
来源：http://hz.sufxvd.cn/gtjwoasfzm.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.zhiwuduotai.top/gtqlzhoros.html

[U49] PHP：只读属性
来源：http://hz.sufxvd.cn/gtggjmysym.html

public readonly string $name
来源：http://hz.zycfv.cn/gtzdpqmyqb.html

[U50] PHP：构造器属性提升
来源：http://hz.tianlin.xyz/gthaddnpwn.html

public function __construct(private int $id) {}
来源：http://hz.hnqzz.top/gtumcsllhg.html

[U51] PHP：数组解构
来源：http://hz.xuanzx.com/gtjvqgbsnn.html

[$a, $b] = $arr;
来源：http://hz.zhengqikj.top/gtebxctmzn.html

[U52] PHP：箭头函数
来源：http://hz.zdqjudy.top/gtwyedwbmb.html

$double = fn($x) => $x * 2;
来源：http://hz.vqdsnc.cn/gtunwptcej.html

[U53] PHP：空合并运算符
来源：http://hz.shzxlz.cn/gtaitxtqpb.html

$v = $a ?? $b ?? "default";
来源：http://hz.jinqigfzy.top/gterewfrnf.html

[U54] PHP：空安全调用
来源：http://hz.tanke756.top/gtseqnibel.html

$obj?->method()
来源：http://hz.svipenyu.cn/gtxpypwwid.html

[U55] PHP：match 表达式
来源：http://hz.cdnleiting.top/gtjawinrpf.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.snrcjt.cn/gtulwykhld.html

[U56] PHP：命名参数
来源：http://hz.dianchejie.cn/gtgcvqfmwc.html

f(a: 1, b: 2)
来源：http://hz.cdnleiting.top/gtxnqmdyjl.html

[U57] PHP：字符串插值
来源：http://hz.gaohongyu789.top/gtxhdmotac.html

"值: {$a}"
来源：http://hz.andypj.xyz/gtgtgrmqgv.html

[U58] PHP：数组三件套
来源：http://hz.cashguo.top/gtphcpzqtq.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.zhongyouzk.top/gtdwbripcy.html

[U59] PHP：自定义排序
来源：http://hz.yj20258.top/gtlujthkjo.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yuanzhike.top/gtewdrxncb.html

[U60] PHP：JSON 编解码
来源：http://hz.sxryk.cn/gtkczlpjvi.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.shuidangran.top/gtzqwaqerh.html

[U61] PHP：正则
来源：http://hz.ehwqpu.com/gtzfhdbzqw.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.sweek.top/gtdzxctqhh.html

[U62] PHP：日期对象
来源：http://hz.zhongyouzk.top/gtazciyodi.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.sufxvd.cn/gtxeapjrre.html

[U63] PHP：文件读写
来源：http://hz.haohaochexian.top/gtofxutibk.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.yj20258888.top/gtyjtkehjm.html

[U64] PHP：目录遍历
来源：http://hz.yj20258888.top/gtgqwchgki.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.yj20258.top/gtfivteiqf.html

[U65] PHP：会话
来源：http://hz.haohaochexian.top/gtezzmkzop.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.jqgufenzy.top/gtqfnxulzl.html

[U66] PHP：设置 Cookie
来源：http://hz.xuanzx.com/gtavbmalrk.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.redwolf501.top/gtjsegvnig.html

[U67] PHP：处理文件上传
来源：http://hz.xinyue.icu/gthkhyurky.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.nwbrower.top/gtiaxxfczo.html

[U68] PHP：PDO 连接
来源：http://hz.jlsjyb.cn/gtptoxddmi.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.yj20258888.top/gtjucgmuwe.html

[U69] PHP：PDO 预处理
来源：http://hz.dashuyun.cn/gtumplesgp.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.nanxinkj.top/gtkfnjnpan.html

[U70] PHP：PDO 事务
来源：http://hz.cqqwz.cn/gtawkhfngy.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.xinyue.icu/gtwqwveryb.html

[U71] PHP：抛出异常
来源：http://hz.mhx1999.top/gtqvdehlgj.html

throw new RuntimeException("失败", 500);
来源：http://hz.9152youxi.cn/gtekmeprvy.html

[U72] PHP：写错误日志
来源：http://hz.shanyushiyangkeji.top/gtmqqudhjn.html

error_log("失败: " . $e->getMessage());
来源：http://hz.nanxuanxn.top/gttovzobuh.html

[U73] PHP：读取 ini 配置
来源：http://hz.jinghuilouyu.cn/gtzlwiytyk.html

parse_ini_file("config.ini", true)
来源：http://hz.jinyuanbaomall.cn/gtchvhlgip.html

[U74] PHP：读取环境变量
来源：http://hz.svipenyu.cn/gtxqzxogpf.html

getenv("APP_ENV") ?: "production"
来源：http://hz.hnqzz.top/gtnzfsvegt.html

[U75] PHP：依赖注入
来源：http://hz.316326.xyz/gtxqqqphpc.html

composer require psr/container
来源：http://hz.hfpthk.cn/gtvwrimnec.html

[U76] PHP：简单路由
来源：http://hz.cdnleiting.top/gtovrivggh.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.andypj.xyz/gtklqnhomy.html

[U77] PHP：模板渲染
来源：http://hz.nwbrower.top/gtfxjphcgq.html

composer require twig/twig
来源：http://hz.snrcjt.cn/gtyvstsuav.html

[U78] PHP：单元测试
来源：http://hz.feifeiyinyue.top/gtvuiivhoj.html

composer require --dev phpunit/phpunit
来源：http://hz.jinghuilouyu.cn/gteckaeiyq.html

[U79] PHP：静态分析
来源：http://hz.jianghu66.top/gtgtdznkfk.html

composer require --dev phpstan/phpstan
来源：http://hz.yuxming.cn/gtvjsoktii.html

[U80] PHP：代码规范修复
来源：http://hz.9152youxi.cn/gtrwplfdqr.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.chenjidiqi.icu/gtpbaykyrb.html

[U81] JS：初始化项目
来源：http://hz.yj202588.top/gtpyfsxaby.html

npm init -y;  npm i express
来源：http://hz.jqgfzy.top/gttjmxqymu.html

[U82] JS：package.json 脚本
来源：http://hz.316326.xyz/gtiouktraw.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.yvedp.cn/gtemlrryfi.html

[U83] JS：ES Module 导入导出
来源：http://hz.xziqi.cn/gtmekuvvux.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.hnqzz.top/gtxjftgqwe.html

[U84] JS：CommonJS 写法
来源：http://hz.cheryme.top/gtsviqqxfe.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.zhixingplan.top/gtezyzrgkx.html

[U85] JS：可选链
来源：http://hz.hywenlv.cn/gtdvyashrm.html

a?.b?.c
来源：http://hz.xinyue.icu/gtrrveuyqh.html

[U86] JS：空值合并
来源：http://hz.yj20258.top/gtqvdrkhmz.html

a ?? b
来源：http://hz.gaohongyu789.top/gtfhnymovt.html

[U87] JS：解构默认值
来源：http://hz.dianchejie.cn/gtuasmrquf.html

const { a = 1, b = 2 } = obj;
来源：http://hz.dianchejie.cn/gtmztjudhj.html

[U88] JS：对象展开合并
来源：http://hz.zhongyouzk.top/gtzwuywvvz.html

{ ...a, ...b }
来源：http://hz.52xcode.cn/gtrawqgvfi.html

[U89] JS：数组去重
来源：http://hz.chenzaomai.com/gtwiiosyzf.html

[...new Set(arr)]
来源：http://hz.mhx1999.top/gthvxiqewa.html

[U90] JS：数字数组排序
来源：http://hz.yj20258.top/gtarqrzzyw.html

[...arr].sort((a, b) => a - b)
来源：http://hz.fengsongda.top/gtxtbwomuc.html

[U91] JS：对象键值遍历
来源：http://hz.ydzc1.top/gtggrldrnn.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.cheryme.top/gtmbaoixhs.html

[U92] JS：深拷贝
来源：http://hz.xuanzx.com/gtnxoblibt.html

structuredClone(obj)
来源：http://hz.zdqjudy.top/gtmdeeflpo.html

[U93] JS：模板字符串
来源：http://hz.vqdsnc.cn/gtxewhpena.html

`共 ${n} 条`
来源：http://hz.0kj1m.cn/gtsspmdoad.html

[U94] JS：箭头函数
来源：http://hz.zhiwuduotai.top/gtycddynog.html

const double = x => x * 2;
来源：http://hz.sufxvd.cn/gtrytujypq.html

[U95] JS：Promise 包装
来源：http://hz.tian-w.cn/gtywnoyjqp.html

new Promise((resolve, reject) => {})
来源：http://hz.dashuyun.cn/gtlkrniikp.html

[U96] JS：async/await 与异常
来源：http://hz.316326.xyz/gtubgtdptj.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.jlsjyb.cn/gtyehpcujv.html

[U97] JS：并发请求
来源：http://hz.jinghuilouyu.cn/gtualovwfh.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yonumen.top/gtgaejixhr.html

[U98] JS：fetch 带 JSON
来源：http://hz.jianghu66.top/gtggkcjdmb.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.ivvv.top/gtcjptibyz.html

[U99] JS：事件监听
来源：http://hz.xylfe.cn/gtmnkcxmbz.html

el.addEventListener("click", e => {})
来源：http://hz.smart0.xyz/gtgkcxxkti.html

[U100] JS：DOM 查询
来源：http://hz.yvedp.cn/gtiobxszyz.html

document.querySelector(".item")
来源：http://hz.aizwys.cn/gtthjzeeoq.html

[U101] JS：classList 操作
来源：http://hz.cucudq.cn/gtwfiyzkza.html

el.classList.toggle("active")
来源：http://hz.snrcjt.cn/gtqfufmslp.html

[U102] JS：本地存储
来源：http://hz.chenjidiqi.icu/gtunikuwks.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.fengsongda.top/gtwamksvtg.html

[U103] JS：定时器
来源：http://hz.jianghu66.top/gtxfnjvseu.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.shanyushiyangkeji.top/gtexjvgmpv.html

[U104] JS：防抖
来源：http://hz.zhaomingkeji.xyz/gtkwynpfmd.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.quarkkingdee.top/gtdinshahi.html

[U105] JS：节流
来源：http://hz.cucudq.cn/gtmhndjwff.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.ywan-chungtsiang.top/gtdvtqhllz.html

[U106] JS：日期格式化
来源：http://hz.redwolf501.top/gtylynvxop.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.yueranfly.top/gtmhfafjre.html

[U107] JS：数字千分位
来源：http://hz.haohaochexian.top/gtgxwumfzz.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.ywan-chungtsiang.top/gtwnckdbnw.html

[U108] JS：随机整数
来源：http://hz.hongshengwenyu.top/gtpirixsjt.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.ppjwa.cn/gtibwsjasf.html

[U109] JS：数组分组
来源：http://hz.xylfe.cn/gtdtffbkgj.html

Object.groupBy(arr, x => x.type)
来源：http://hz.pycfn.com/gtcvirhsza.html

[U110] JS：数组分块
来源：http://hz.yuxming.cn/gtptxiuzfn.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.tanke756.top/gtgjmwrfic.html

[U111] JS：对象转 Map
来源：http://hz.feifeiyinyue.top/gtqpwjjtyx.html

new Map(Object.entries(obj))
来源：http://hz.mhx1999.top/gtjirwuemq.html

[U112] JS：字符串补位
来源：http://hz.nanxuanxn.top/gtbpilorkj.html

"7".padStart(3, "0")
来源：http://hz.aibaodan.cn/gtynntvhri.html

[U113] JS：正则替换全部
来源：http://hz.ybcxt.top/gtcheezdig.html

s.replaceAll("a", "b")
来源：http://hz.birdmap.top/gtcqpltmgd.html

[U114] JS：JSON 深比较
来源：http://hz.chenlongwang.top/gtrjivzzbg.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.gaohongyu789.top/gtnhgrwihc.html

[U115] JS：生成 UUID
来源：http://hz.jinghuilouyu.cn/gtyfdhwybd.html

crypto.randomUUID()
来源：http://hz.zhaomingkeji.xyz/gtrysxvuki.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.pengpengdd.cyou/gtdytnejim.html

/** @param {string} name */ function f(name) {}
来源：http://hz.pengpengdd.cyou/gttotzaphy.html

[U117] JS：单元测试
来源：http://hz.zdqjudy.top/gtfdbyrqoi.html

npm i -D vitest;  npx vitest
来源：http://hz.pengpengdd.cyou/gtfcnsiawe.html

[U118] JS：开发服务器
来源：http://hz.chenlongwang.top/gtxlpqjpqg.html

npm i -D vite;  npx vite
来源：http://hz.daxiang520.top/gtcdnxjajm.html

[U119] JS：生产构建
来源：http://hz.jqgfzy.top/gtagmoopdv.html

npx vite build
来源：http://hz.tian-w.cn/gtchhlcgog.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.shzxlz.cn/gtzkfotysb.html

import.meta.env.VITE_API_URL
来源：http://hz.zdqjudy.top/gtzpcecnku.html

================================================================================
来源：http://hz.hfpthk.cn/gtexwlgodg.html

统计汇总
来源：http://hz.ydzc1.top/gtyspqhshs.html

================================================================================
来源：http://hz.zycfv.cn/gtgtpdwqcl.html

按语言统计（条）：
来源：http://hz.cqqwz.cn/gtohljyrcp.html

Python ......... 252
来源：http://hz.zhongyouzk.top/gtigiuaehw.html

PHP ............ 252
来源：http://hz.aibaodan.cn/gtnngmhqzi.html

JavaScript ..... 252
来源：http://hz.zhongyouzk.top/gtqerawych.html

TypeScript ..... 212
来源：http://hz.zhongyouzk.top/gtrlmggfif.html

Java ........... 212
来源：http://hz.shangyingyoupin.top/gtcbvhtcbg.html

Go ............. 212
来源：http://hz.haohaochexian.top/gtvoadaxhz.html

Ruby ........... 212
来源：http://hz.vqdsnc.cn/gttgsnadsw.html

C# ............. 212
来源：http://hz.jinyuanbaomall.cn/gtjflaakzt.html

C .............. 30
来源：http://hz.yj20258.top/gtyihtgwcz.html

C++ ............ 30
来源：http://hz.cdnleiting.top/gtinrvmrvb.html

SQL ............ 90
来源：http://hz.zhengqikj.top/gtcoswwgnm.html

Bash ........... 80
来源：http://hz.zhiwuduotai.top/gtdqpijakk.html

Kotlin ......... 15
来源：http://hz.9152youxi.cn/gtlpzpkrch.html

Swift .......... 15
来源：http://hz.jinqigufen.top/gtquhigamt.html

Lua ............ 10
来源：http://hz.gzhubu.top/gtytjijpfq.html

Perl ........... 10
来源：http://hz.sxryk.cn/gtcanbxhxz.html

Scala .......... 10
来源：http://hz.andypj.xyz/gtdlicfuys.html

------------------------------------
来源：http://hz.gzhubu.top/gtkohoxuoy.html

合计 ........... 2106 条
来源：http://hz.guannengcc.top/gtmmbbqtfx.html

按章节统计：
来源：http://hz.haohaochexian.top/gtsbpoheoj.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.cucudq.cn/gthtbmjfzo.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.yj20258.top/gtiezdjvfq.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.nwbrower.top/gttxdtcega.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.hongshengwenyu.top/gtlvnzjyee.html


<!-- 参考信息 -->