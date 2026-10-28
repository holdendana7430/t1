代发 wailian999

[T47] Perl：正则捕获
来源：http://hz.yuanzhike.top/gtrkdpjthx.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.ywan-chungtsiang.top/gtvkhcdwqy.html

[T48] Perl：正则替换
来源：http://hz.andypj.xyz/gtpzwrmrhj.html

$s =~ s/old/new/g;
来源：http://hz.kuanghao11.cn/gtenjwkoej.html

[T49] Perl：函数
来源：http://hz.zhoulong.xyz/gtphswbily.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.zycfv.cn/gtyrvmbfef.html

[T50] Perl：逐行读文件
来源：http://hz.haohaochexian.top/gtttdmkxhr.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.hywenlv.cn/gtkbpowhhu.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.cdnleiting.top/gttyicwjmg.html

[T51] Scala：Hello World
来源：http://hz.zycfv.cn/gtoertwzcw.html

println("Hello")
来源：http://hz.jinyuanbaomall.cn/gtnhvnmtkf.html

[T52] Scala：变量
来源：http://hz.nanxinkj.top/gthimwetwn.html

val a = 1;  var b = 2
来源：http://hz.aizwys.cn/gtgydtttun.html

[T53] Scala：字符串插值
来源：http://hz.0kj1m.cn/gtlawwrctk.html

s"值: $b"
来源：http://hz.jqgfzy.top/gtntyhsgxw.html

[T54] Scala：集合映射
来源：http://hz.meibo888.top/gtwqxabgwe.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.dianchejie.cn/gtfxvfolcj.html

[T55] Scala：集合过滤
来源：http://hz.daxiang520.top/gtfzrriezg.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.xinyue.icu/gtiszzugmz.html

[T56] Scala：样例类
来源：http://hz.jinghuilouyu.cn/gtgqilzezy.html

case class User(name: String, age: Int)
来源：http://hz.cqqwz.cn/gtszxtjqck.html

[T57] Scala：模式匹配
来源：http://hz.pengpengdd.cyou/gthdqtzjny.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.xingfuxueyuan.xyz/gtwbhyypkn.html

[T58] Scala：函数定义
来源：http://hz.xingfuxueyuan.xyz/gtzasyidpo.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.gaohongyu789.top/gtdvpdahtz.html

[T59] Scala：循环
来源：http://hz.shzxlz.cn/gttzvhedts.html

for (i <- 1 to 10) println(i)
来源：http://hz.gaohongyu789.top/gtvolpjjxm.html

[T60] Scala：折叠
来源：http://hz.zdqjudy.top/gtigntsqgv.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.bjfxy.top/gtnxdlupdu.html

================================================================================
来源：http://hz.cqqwz.cn/gtnlnixwjj.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.svipenyu.cn/gtcxubwurb.html

================================================================================
来源：http://hz.guannengcc.top/gtrxkfedvi.html

[U01] Py：创建虚拟环境
来源：http://hz.yvedp.cn/gtzyvfreyc.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.nanxinkj.top/gtksnzrnnr.html

[U02] Py：导出 / 安装依赖
来源：http://hz.havefunace.top/gtvzjufsgr.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.xylfe.cn/gtzatbqtbq.html

[U03] Py：加载 .env 配置
来源：http://hz.redwolf501.top/gtaygrpzdg.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.tanke756.top/gtonvczalo.html

[U04] Py：变量调试打印
来源：http://hz.feifeiyinyue.top/gtssyabuuz.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.yonumen.top/gttqsxofik.html

[U05] Py：列表去重且保序
来源：http://hz.9152youxi.cn/gtijugegwr.html

list(dict.fromkeys(arr))
来源：http://hz.cdnleiting.top/gtnknclxdq.html

[U06] Py：合并两个字典
来源：http://hz.jqgufenzy.top/gtuqxzmbnu.html

{**a, **b}
来源：http://hz.yvedp.cn/gtrsvgffgc.html

[U07] Py：反转字典键值
来源：http://hz.bjfxy.top/gtfpdeopxk.html

{v: k for k, v in d.items()}
来源：http://hz.hnqzz.top/gtjsglxsaw.html

[U08] Py：展平二维列表
来源：http://hz.ydjk.org.cn/gtykdzogrh.html

[y for x in nested for y in x]
来源：http://hz.guowangkeji.top/gtxlojpkrx.html

[U09] Py：字典取最大值的键
来源：http://hz.zhaomingkeji.xyz/gtqxheaswu.html

max(d, key=d.get)
来源：http://hz.kuanghao11.cn/gtkaqrzzdb.html

[U10] Py：按值排序字典
来源：http://hz.yanxiufei.cn/gtfbioryli.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.xziqi.cn/gttxbqcfal.html

[U11] Py：生成器表达式
来源：http://hz.snrcjt.cn/gtelxausib.html

(x * 2 for x in arr)
来源：http://hz.chenzaomai.com/gtdavmekbf.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.cheryme.top/gttzbbgmdz.html

Counter(arr).most_common(3)
来源：http://hz.snrcjt.cn/gttfubcoke.html

[U13] Py：固定长度队列
来源：http://hz.andypj.xyz/gtmwlftczd.html

deque(maxlen=10)
来源：http://hz.ivvv.top/gturvynraw.html

[U14] Py：分组收集到列表
来源：http://hz.xingfuxueyuan.xyz/gtiqfdkdfr.html

defaultdict(list)
来源：http://hz.cashguo.top/gtfrlfakld.html

[U15] Py：高精度计时
来源：http://hz.bjfxy.top/gtrwffrddb.html

t = time.perf_counter()
来源：http://hz.gotoacloud.top/gtuupzofox.html

[U16] Py：命令行参数解析
来源：http://hz.hongshengwenyu.top/gtuwavpnub.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.ivvv.top/gtwutsyyrl.html

[U17] Py：初始化日志
来源：http://hz.bjfxy.top/gtjmlwubwk.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.shanyushiyangkeji.top/gteajayveq.html

[U18] Py：预编译正则
来源：http://hz.jinyuanbaomall.cn/gtmfbvnegp.html

pat = re.compile(r"\d+")
来源：http://hz.tian-w.cn/gtnaaktotx.html

[U19] Py：正则替换带回调
来源：http://hz.cdnleiting.top/gtgyrisezh.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.ehwqpu.com/gtiwdpfemf.html

[U20] Py：缓存函数结果
来源：http://hz.sxryk.cn/gtldrvcqey.html

@functools.lru_cache(maxsize=None)
来源：http://hz.zycfv.cn/gtmkgliljw.html

[U21] Py：自定义上下文管理器
来源：http://hz.jlsjyb.cn/gtppfmfltt.html

@contextlib.contextmanager
来源：http://hz.9152youxi.cn/gtxqtprtfk.html

[U22] Py：矩阵转置
来源：http://hz.xylfe.cn/gtvtxqbwuy.html

list(zip(*m))
来源：http://hz.316326.xyz/gtmicqgfev.html

[U23] Py：分块读取大文件
来源：http://hz.birdmap.top/gtidehuior.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.c1oappe.top/gthhsznzqb.html

[U24] Py：路径操作
来源：http://hz.ybcxt.top/gtbqqbxqak.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.wangshuangyany.cn/gtxusirobf.html

[U25] Py：CSV 按字典读
来源：http://hz.tian-w.cn/gtvrlwrjsn.html

csv.DictReader(f)
来源：http://hz.tanke756.top/gteapighzj.html

[U26] Py：并发下载
来源：http://hz.ivvv.top/gtrqptvwwf.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.dashuyun.cn/gttyxlghvd.html

[U27] Py：异步 HTTP
来源：http://hz.cqqwz.cn/gtihkiexjf.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.zhixingplan.top/gtuzqsvlwl.html

[U28] Py：类型别名
来源：http://hz.birdmap.top/gtroozxbck.html

UserId = int
来源：http://hz.chenjidiqi.icu/gtshvbfjbt.html

[U29] Py：属性校验
来源：http://hz.yangfankeji.com/gtqqhziamn.html

@property 与 @x.setter 配合
来源：http://hz.ydzc1.top/gtrnpcexhl.html

[U30] Py：数据类
来源：http://hz.xingfuxueyuan.xyz/gthazyeoja.html

@dataclass(slots=True)
来源：http://hz.meibo888.top/gtwdhjduct.html

[U31] Py：单测
来源：http://hz.yj20258888.top/gtnqnmfcul.html

python -m pytest -q
来源：http://hz.hnxiangtu.top/gtpdsmmwqu.html

[U32] Py：代码格式化
来源：http://hz.ivvv.top/gteptzkivl.html

ruff format . && ruff check --fix .
来源：http://hz.shangyingyoupin.top/gtqqjpmsbv.html

[U33] Py：打包发布
来源：http://hz.bjfxy.top/gtklckjcud.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.jqgufenzy.top/gtjpirgmlf.html

[U34] Py：判断编码
来源：http://hz.zhijiandao.cn/gtycddcryh.html

chardet.detect(raw)
来源：http://hz.jiagoushi.top/gtsukvhmqb.html

[U35] Py：发送邮件
来源：http://hz.gotoacloud.top/gtbrrvgvre.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.nwbrower.top/gtsppgvqwz.html

[U36] Py：定时任务
来源：http://hz.iojbl.cn/gtlgvptbnb.html

schedule.every(10).minutes.do(job)
来源：http://hz.fzhhl.top/gtkofmzpsg.html

[U37] Py：读写 Excel
来源：http://hz.guannengcc.top/gtvpuegxjw.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.tanke756.top/gtqmnewxbg.html

[U38] Py：获取脚本所在目录
来源：http://hz.xylfe.cn/gtqsbhascw.html

Path(__file__).resolve().parent
来源：http://hz.zhaomingkeji.xyz/gtlcnhdnzm.html

[U39] Py：判断是否在交互环境
来源：http://hz.tianlin.xyz/gtlleidmkr.html

sys.stdout.isatty()
来源：http://hz.0kj1m.cn/gtrrdkwynf.html

[U40] Py：打印到标准错误
来源：http://hz.shzxlz.cn/gtqjxhqwra.html

print("err", file=sys.stderr)
来源：http://hz.andypj.xyz/gtbuwoxfic.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.cqqwz.cn/gtsmrwhjgc.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.sufxvd.cn/gtlcdsicmi.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.zhijiandao.cn/gtozqrdezb.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.ppjwa.cn/gtknihaxqu.html

[U43] PHP：声明命名空间
来源：http://hz.52xcode.cn/gtahyzsaeh.html

namespace App\Http;
来源：http://hz.c1oappe.top/gtvdoulpmj.html

[U44] PHP：开启严格类型
来源：http://hz.smart0.xyz/gtxyuuwmzy.html

declare(strict_types=1);
来源：http://hz.gotoacloud.top/gtquynzmlk.html

[U45] PHP：类型声明与返回类型
来源：http://hz.guowangkeji.top/gtiijvdsuy.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.xziqi.cn/gtpdmyjfjf.html

[U46] PHP：可空类型
来源：http://hz.snrcjt.cn/gtwklhnvkh.html

?string $name = null
来源：http://hz.pengpengdd.cyou/gtmijmvrub.html

[U47] PHP：联合类型
来源：http://hz.tian-w.cn/gtkdscztyc.html

int|string $id
来源：http://hz.hywenlv.cn/gtqncwifjw.html

[U48] PHP：纯枚举
来源：http://hz.xinyue.icu/gtayqhnwvu.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.xuanzx.com/gtzvilgojm.html

[U49] PHP：只读属性
来源：http://hz.yongpay.top/gtjcgbgfvc.html

public readonly string $name
来源：http://hz.snrcjt.cn/gtiojoambp.html

[U50] PHP：构造器属性提升
来源：http://hz.yuxming.cn/gtrqiildkg.html

public function __construct(private int $id) {}
来源：http://hz.yangfankeji.com/gtihdcnwpy.html

[U51] PHP：数组解构
来源：http://hz.sysykeji.top/gtwmhiqhle.html

[$a, $b] = $arr;
来源：http://hz.wangdashe.top/gtyrhzqjmf.html

[U52] PHP：箭头函数
来源：http://hz.yj20258.top/gteyleiutj.html

$double = fn($x) => $x * 2;
来源：http://hz.hysaishi.cn/gtucuyezdr.html

[U53] PHP：空合并运算符
来源：http://hz.tianlin.xyz/gtvuzgunuv.html

$v = $a ?? $b ?? "default";
来源：http://hz.shanyushiyangkeji.top/gtcpuezixk.html

[U54] PHP：空安全调用
来源：http://hz.ivvv.top/gtvzxfbbii.html

$obj?->method()
来源：http://hz.xingfuxueyuan.xyz/gtqtqflgjd.html

[U55] PHP：match 表达式
来源：http://hz.hammf.cn/gtadfovhwd.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.fzhhl.top/gtuyamrszf.html

[U56] PHP：命名参数
来源：http://hz.wangdashe.top/gtzscaemzd.html

f(a: 1, b: 2)
来源：http://hz.yuxming.cn/gtwsquerlc.html

[U57] PHP：字符串插值
来源：http://hz.shanyushiyangtech.top/gtxwxrbqck.html

"值: {$a}"
来源：http://hz.havefunace.top/gtyszkqlur.html

[U58] PHP：数组三件套
来源：http://hz.yongpay.top/gtvqenzzwv.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.haohaochexian.top/gtmbvyykbq.html

[U59] PHP：自定义排序
来源：http://hz.yuanzhike.top/gtlncycktw.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.shanyushiyangkeji.top/gtaxcdlvwe.html

[U60] PHP：JSON 编解码
来源：http://hz.gotoacloud.top/gtssyvjndy.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.cdnleiting.top/gtygfuelnn.html

[U61] PHP：正则
来源：http://hz.zdqjudy.top/gtdfqmgdhi.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.ywan-chungtsiang.top/gtcwnwdecp.html

[U62] PHP：日期对象
来源：http://hz.chenjidiqi.icu/gtuvllymjx.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.nwbrower.top/gtziolvgqv.html

[U63] PHP：文件读写
来源：http://hz.mhx1999.top/gtkvfexxal.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.andypj.xyz/gtnjlxkgxh.html

[U64] PHP：目录遍历
来源：http://hz.aibaodan.cn/gtcriutdtw.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.jianghu66.top/gtdfuflisq.html

[U65] PHP：会话
来源：http://hz.dashuyun.cn/gtlsactybs.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.jiagoushi.top/gtfehyuyay.html

[U66] PHP：设置 Cookie
来源：http://hz.guowangkeji.top/gtviycgesq.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.jinyuanbaomall.cn/gtdrulcsth.html

[U67] PHP：处理文件上传
来源：http://hz.yangfankeji.com/gtgmordqtq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.tianlin.xyz/gtnoxxjqda.html

[U68] PHP：PDO 连接
来源：http://hz.nwbrower.top/gtcdceddag.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.bjfxy.top/gtplprwdbj.html

[U69] PHP：PDO 预处理
来源：http://hz.xylfe.cn/gtyunwalov.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.haohaochexian.top/gtiogcdjdy.html

[U70] PHP：PDO 事务
来源：http://hz.zycfv.cn/gtkcvexped.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.gzhubu.top/gtiulhvigk.html

[U71] PHP：抛出异常
来源：http://hz.gotoacloud.top/gtxrospfog.html

throw new RuntimeException("失败", 500);
来源：http://hz.sysykeji.top/gtliajzclg.html

[U72] PHP：写错误日志
来源：http://hz.jqgufenzy.top/gtssaghohn.html

error_log("失败: " . $e->getMessage());
来源：http://hz.hnqzz.top/gtjkitpxse.html

[U73] PHP：读取 ini 配置
来源：http://hz.jinghuilouyu.cn/gtemdyloij.html

parse_ini_file("config.ini", true)
来源：http://hz.gogol.net.cn/gtcycsogyo.html

[U74] PHP：读取环境变量
来源：http://hz.sysykeji.top/gtidmjzzfy.html

getenv("APP_ENV") ?: "production"
来源：http://hz.fzhhl.top/gtvwkavmku.html

[U75] PHP：依赖注入
来源：http://hz.wangdashe.top/gtevfontmj.html

composer require psr/container
来源：http://hz.zhongyouzk.top/gtnzuigjds.html

[U76] PHP：简单路由
来源：http://hz.zycfv.cn/gtblqayzes.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.yvedp.cn/gtyfsoiief.html

[U77] PHP：模板渲染
来源：http://hz.hammf.cn/gtfnjupmxa.html

composer require twig/twig
来源：http://hz.yj20258888.top/gtyvjfnppz.html

[U78] PHP：单元测试
来源：http://hz.snrcjt.cn/gtncumichj.html

composer require --dev phpunit/phpunit
来源：http://hz.shzxlz.cn/gtoapbtqvy.html

[U79] PHP：静态分析
来源：http://hz.shangyingyoupin.top/gtfdzwqokx.html

composer require --dev phpstan/phpstan
来源：http://hz.wangshuangyany.cn/gtfeyunxpj.html

[U80] PHP：代码规范修复
来源：http://hz.chenlongwang.top/gtgqoqhoxl.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.xuetiantiany.cn/gtcoiokzig.html

[U81] JS：初始化项目
来源：http://hz.guannengcc.top/gtvogfwita.html

npm init -y;  npm i express
来源：http://hz.jinqigufen.top/gtpjambrnw.html

[U82] JS：package.json 脚本
来源：http://hz.zdqjudy.top/gtmjeaoahq.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.hongshengwenyu.top/gtrpokhfwf.html

[U83] JS：ES Module 导入导出
来源：http://hz.guowangkeji.top/gtwandpnic.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.sysykeji.top/gttljxojqu.html

[U84] JS：CommonJS 写法
来源：http://hz.shanyushiyangkeji.top/gtfzjwdiab.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.ywan-chungtsiang.top/gtttjcoyii.html

[U85] JS：可选链
来源：http://hz.dashuyun.cn/gtwsewugfj.html

a?.b?.c
来源：http://hz.jianghu66.top/gtuqxghncc.html

[U86] JS：空值合并
来源：http://hz.smart0.xyz/gturbifueb.html

a ?? b
来源：http://hz.shuidangran.top/gtfcuivbuj.html

[U87] JS：解构默认值
来源：http://hz.jinqigufen.top/gtveysqomz.html

const { a = 1, b = 2 } = obj;
来源：http://hz.tianlin.xyz/gtklayetnn.html

[U88] JS：对象展开合并
来源：http://hz.yj20258.top/gteshlsyep.html

{ ...a, ...b }
来源：http://hz.sysykeji.top/gtfjnfgnhj.html

[U89] JS：数组去重
来源：http://hz.jinqigufen.top/gtdqdqrlfh.html

[...new Set(arr)]
来源：http://hz.xinyue.icu/gtmmodxxdg.html

[U90] JS：数字数组排序
来源：http://hz.316326.xyz/gtjyfkthim.html

[...arr].sort((a, b) => a - b)
来源：http://hz.zdqjudy.top/gtdejzbvot.html

[U91] JS：对象键值遍历
来源：http://hz.kuanghao11.cn/gtkgedcwbk.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.chenlongwang.top/gtwhxxcagu.html

[U92] JS：深拷贝
来源：http://hz.mhx1999.top/gtsersigei.html

structuredClone(obj)
来源：http://hz.jqgfzy.top/gtzqlczqvb.html

[U93] JS：模板字符串
来源：http://hz.52xcode.cn/gtgrpigipd.html

`共 ${n} 条`
来源：http://hz.cqqwz.cn/gtuoyaxbjh.html

[U94] JS：箭头函数
来源：http://hz.svipenyu.cn/gtzfobejbg.html

const double = x => x * 2;
来源：http://hz.sufxvd.cn/gtwaiwaldx.html

[U95] JS：Promise 包装
来源：http://hz.zhiwuduotai.top/gtvqsxepjf.html

new Promise((resolve, reject) => {})
来源：http://hz.haohaochexian.top/gtotaxsqii.html

[U96] JS：async/await 与异常
来源：http://hz.sufxvd.cn/gtkebzvpvn.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.ydjk.org.cn/gtjychpvvh.html

[U97] JS：并发请求
来源：http://hz.jiagoushi.top/gtmzqovrsr.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jinqigfzy.top/gtfnqsxzge.html

[U98] JS：fetch 带 JSON
来源：http://hz.haohaochexian.top/gtycdzppan.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.zycfv.cn/gtpkcmhtkm.html

[U99] JS：事件监听
来源：http://hz.dashuyun.cn/gtxvlunere.html

el.addEventListener("click", e => {})
来源：http://hz.andypj.xyz/gtntoejomb.html

[U100] JS：DOM 查询
来源：http://hz.jqgufenzy.top/gtvwbzibcz.html

document.querySelector(".item")
来源：http://hz.shanyushiyangtech.top/gtogemivoe.html

[U101] JS：classList 操作
来源：http://hz.jyoumei.cn/gtygrciuxg.html

el.classList.toggle("active")
来源：http://hz.daria6918.cn/gtoshytzbi.html

[U102] JS：本地存储
来源：http://hz.guowangkeji.top/gtxxugiyqh.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.shanyushiyangtech.top/gtxjkjuvst.html

[U103] JS：定时器
来源：http://hz.yj20258888.top/gtaogdsnzi.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.52xcode.cn/gtjwhvmotr.html

[U104] JS：防抖
来源：http://hz.birdmap.top/gtrptqgnyu.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yanxiufei.cn/gtirygqwdw.html

[U105] JS：节流
来源：http://hz.chenlongwang.top/gtadodqjvb.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.bjfxy.top/gtmbymybcx.html

[U106] JS：日期格式化
来源：http://hz.zhijiandao.cn/gtsfsmcksj.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.nanxuanxn.top/gtcfoyvina.html

[U107] JS：数字千分位
来源：http://hz.gogol.net.cn/gttocsgrzi.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.zhaomingkeji.xyz/gtrsihgwky.html

[U108] JS：随机整数
来源：http://hz.jqgufenzy.top/gtjeobfmcf.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.quarkkingdee.top/gtftlrqafu.html

[U109] JS：数组分组
来源：http://hz.hfpthk.cn/gtishirgug.html

Object.groupBy(arr, x => x.type)
来源：http://hz.nwbrower.top/gterryklvu.html

[U110] JS：数组分块
来源：http://hz.dianchejie.cn/gtazibfxji.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.yanxiufei.cn/gtqkvybjud.html

[U111] JS：对象转 Map
来源：http://hz.jinqigufen.top/gthvoszyya.html

new Map(Object.entries(obj))
来源：http://hz.svipenyu.cn/gtduqqunfz.html

[U112] JS：字符串补位
来源：http://hz.yj202588.top/gtuwcfotku.html

"7".padStart(3, "0")
来源：http://hz.zhengqikj.top/gtivsjjrzq.html

[U113] JS：正则替换全部
来源：http://hz.jinyuanbaomall.cn/gtswayecdn.html

s.replaceAll("a", "b")
来源：http://hz.shangyingyoupin.top/gthdvjdnfi.html

[U114] JS：JSON 深比较
来源：http://hz.tanke756.top/gtexjvdvzm.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.hfpthk.cn/gtvzniaqdb.html

[U115] JS：生成 UUID
来源：http://hz.hnqzz.top/gthgcqyamu.html

crypto.randomUUID()
来源：http://hz.ehwqpu.com/gtybpvmyoc.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.gotoacloud.top/gtbkkocxff.html

/** @param {string} name */ function f(name) {}
来源：http://hz.shuidangran.top/gtjuvhwebs.html

[U117] JS：单元测试
来源：http://hz.guannengcc.top/gtrpemsylf.html

npm i -D vitest;  npx vitest
来源：http://hz.xuetiantiany.cn/gtaxezibdp.html

[U118] JS：开发服务器
来源：http://hz.cdnleiting.top/gtmbkbgwzw.html

npm i -D vite;  npx vite
来源：http://hz.zhijiandao.cn/gtctxnojrp.html

[U119] JS：生产构建
来源：http://hz.ydjk.org.cn/gtzchqnfji.html

npx vite build
来源：http://hz.xuetiantiany.cn/gtpmeateev.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.9152youxi.cn/gtujysywqe.html

import.meta.env.VITE_API_URL
来源：http://hz.tanke756.top/gtdknekpqf.html

================================================================================
来源：http://hz.zycfv.cn/gtzrvxggal.html

统计汇总
来源：http://hz.yangfankeji.com/gtpvbqktcz.html

================================================================================
来源：http://hz.jqgfzy.top/gtgbozdhaj.html

按语言统计（条）：
来源：http://hz.jiagoushi.top/gtkzyapmwp.html

Python ......... 252
来源：http://hz.yonumen.top/gtywwcaeft.html

PHP ............ 252
来源：http://hz.ydjk.org.cn/gtflrfoqck.html

JavaScript ..... 252
来源：http://hz.dianchejie.cn/gtqesbhkim.html

TypeScript ..... 212
来源：http://hz.meibo888.top/gtgfurladz.html

Java ........... 212
来源：http://hz.daria6918.cn/gtxoxkgwge.html

Go ............. 212
来源：http://hz.tanke756.top/gtwlhoomco.html

Ruby ........... 212
来源：http://hz.c1oappe.top/gtfyujzyxa.html

C# ............. 212
来源：http://hz.aizwys.cn/gtyyzcntrr.html

C .............. 30
来源：http://hz.guowangkeji.top/gtyzinwxkz.html

C++ ............ 30
来源：http://hz.sufxvd.cn/gtxtgmgtmm.html

SQL ............ 90
来源：http://hz.hongshengwenyu.top/gtdfhspimt.html

Bash ........... 80
来源：http://hz.cdnleiting.top/gtbniyasek.html

Kotlin ......... 15
来源：http://hz.guannengcc.top/gtkuqctbpq.html

Swift .......... 15
来源：http://hz.zhoulong.xyz/gtlggdsygq.html

Lua ............ 10
来源：http://hz.sufxvd.cn/gtlbwaxiee.html

Perl ........... 10
来源：http://hz.xinyue.icu/gtplvvhyha.html

Scala .......... 10
来源：http://hz.yj20258.top/gtuqvkuoiz.html

------------------------------------
来源：http://hz.yj202588.top/gtxbpzgbfy.html

合计 ........... 2106 条
来源：http://hz.xingfuxueyuan.xyz/gthmesivvy.html

按章节统计：
来源：http://hz.zhaomingkeji.xyz/gtyavvjlwe.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.zhixingplan.top/gtokkzdmvb.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.hammf.cn/gthyzllfvv.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.snrcjt.cn/gtucgxzirc.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.shuidangran.top/gtjejwvabj.html


<!-- 参考信息 -->