代发 wailian999

[T41] Perl：Hello World
来源：http://hz.xylfe.cn/gtlscbeboj.html

print "Hello\n";
来源：http://hz.chenzaomai.com/gtzqehakjq.html

[T42] Perl：变量类型
来源：http://hz.jinghuilouyu.cn/gteygxymib.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.cashguo.top/gtugfqckyh.html

[T43] Perl：字符串插值
来源：http://hz.0kj1m.cn/gtnbgavwhv.html

"值: $a"
来源：http://hz.sufxvd.cn/gtyvcdqskn.html

[T44] Perl：条件
来源：http://hz.yuanzhike.top/gtnzqoeguj.html

if ($a > 0) { print "正"; }
来源：http://hz.dashuyun.cn/gtetfmdyth.html

[T45] Perl：数组遍历
来源：http://hz.gzhubu.top/gtzuvpvuei.html

for my $x (@arr) { print $x; }
来源：http://hz.yuanzhike.top/gtmrpejdhh.html

[T46] Perl：哈希操作
来源：http://hz.jqgufenzy.top/gtgbkcciyc.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.gotoacloud.top/gtetibumno.html

[T47] Perl：正则捕获
来源：http://hz.jyoumei.cn/gtcmbgbmxm.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.zhijiandao.cn/gtyiovsyui.html

[T48] Perl：正则替换
来源：http://hz.ivvv.top/gtopesozfr.html

$s =~ s/old/new/g;
来源：http://hz.kuanghao11.cn/gtigttvltx.html

[T49] Perl：函数
来源：http://hz.yuxming.cn/gtbuldxgwv.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.gogol.net.cn/gtrzbeirbr.html

[T50] Perl：逐行读文件
来源：http://hz.chenjidiqi.icu/gtirlvacjc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.aibaodan.cn/gtcvfozdrf.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.ybcxt.top/gtggwtaxgo.html

[T51] Scala：Hello World
来源：http://hz.ydzc1.top/gtgamsxuel.html

println("Hello")
来源：http://hz.pycfn.com/gtnhivbowo.html

[T52] Scala：变量
来源：http://hz.xingfuxueyuan.xyz/gtnhtsfxht.html

val a = 1;  var b = 2
来源：http://hz.aibaodan.cn/gtnowwdqgl.html

[T53] Scala：字符串插值
来源：http://hz.wangshuangyany.cn/gtkznnltbb.html

s"值: $b"
来源：http://hz.zhixingplan.top/gtlqxqkwnv.html

[T54] Scala：集合映射
来源：http://hz.gotoacloud.top/gtyktqkvdw.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.shangyingyoupin.top/gtoowkkewo.html

[T55] Scala：集合过滤
来源：http://hz.shzxlz.cn/gtfiwxegtx.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.xuanzx.com/gtangbkail.html

[T56] Scala：样例类
来源：http://hz.jiagoushi.top/gtotfctqrn.html

case class User(name: String, age: Int)
来源：http://hz.yuanzhike.top/gthrhghjhi.html

[T57] Scala：模式匹配
来源：http://hz.wangshuangyany.cn/gtmaifgnek.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.guannengcc.top/gtqyysgedu.html

[T58] Scala：函数定义
来源：http://hz.jinyuanbaomall.cn/gtpplgyigv.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.chenlongwang.top/gtaljewnay.html

[T59] Scala：循环
来源：http://hz.0kj1m.cn/gtbwvffoyn.html

for (i <- 1 to 10) println(i)
来源：http://hz.aibaodan.cn/gtikouwfeu.html

[T60] Scala：折叠
来源：http://hz.zdqjudy.top/gtgiwsxlsg.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.sweek.top/gtuoxqxvkf.html

================================================================================
来源：http://hz.guowangkeji.top/gteadzaeuv.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.chenzaomai.com/gtpgqqpfyr.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtomeiiiaq.html

[U01] Py：创建虚拟环境
来源：http://hz.xuetiantiany.cn/gttgeyijjl.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.zhijiandao.cn/gtipixqxdg.html

[U02] Py：导出 / 安装依赖
来源：http://hz.xylfe.cn/gtvgnhqfdb.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.zhengqikj.top/gtatubhqog.html

[U03] Py：加载 .env 配置
来源：http://hz.xuanzx.com/gtubsfatob.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.hnxiangtu.top/gtoacvmudp.html

[U04] Py：变量调试打印
来源：http://hz.jiagoushi.top/gtzkexycwj.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.jqgfzy.top/gtcnfxrhhx.html

[U05] Py：列表去重且保序
来源：http://hz.shuidangran.top/gtuurlunhr.html

list(dict.fromkeys(arr))
来源：http://hz.fzhhl.top/gtgnsxgkmq.html

[U06] Py：合并两个字典
来源：http://hz.zhongyouzk.top/gtgdrjrgvd.html

{**a, **b}
来源：http://hz.ppjwa.cn/gtwwvbnteu.html

[U07] Py：反转字典键值
来源：http://hz.ydzc1.top/gtvnggwlft.html

{v: k for k, v in d.items()}
来源：http://hz.hnqzz.top/gtpogpdqts.html

[U08] Py：展平二维列表
来源：http://hz.nwbrower.top/gtspjuejda.html

[y for x in nested for y in x]
来源：http://hz.mhx1999.top/gtdxjjvdlu.html

[U09] Py：字典取最大值的键
来源：http://hz.yangfankeji.com/gtqldgimwm.html

max(d, key=d.get)
来源：http://hz.chenzaomai.com/gtclwrnobe.html

[U10] Py：按值排序字典
来源：http://hz.ydjk.org.cn/gtwdsqszxa.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.cashguo.top/gttijpdoar.html

[U11] Py：生成器表达式
来源：http://hz.daxiang520.top/gtyopeinbf.html

(x * 2 for x in arr)
来源：http://hz.pycfn.com/gtintigcoj.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.jqgufenzy.top/gtaoutangu.html

Counter(arr).most_common(3)
来源：http://hz.ywan-chungtsiang.top/gtbagzwncs.html

[U13] Py：固定长度队列
来源：http://hz.tianlin.xyz/gtyfdszbau.html

deque(maxlen=10)
来源：http://hz.shanyushiyangtech.top/gtvimilkin.html

[U14] Py：分组收集到列表
来源：http://hz.xylfe.cn/gtkgusqhzb.html

defaultdict(list)
来源：http://hz.smart0.xyz/gtvnqvhfew.html

[U15] Py：高精度计时
来源：http://hz.vqdsnc.cn/gtorqjyefn.html

t = time.perf_counter()
来源：http://hz.zhijiandao.cn/gtjbudseor.html

[U16] Py：命令行参数解析
来源：http://hz.0kj1m.cn/gtiesrhtmb.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.yongpay.top/gtjpbavpuw.html

[U17] Py：初始化日志
来源：http://hz.zhoulong.xyz/gtoqpnqpxb.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.xylfe.cn/gtzstwxaai.html

[U18] Py：预编译正则
来源：http://hz.fengsongda.top/gtpjqcvhzl.html

pat = re.compile(r"\d+")
来源：http://hz.hysaishi.cn/gtnlamzefk.html

[U19] Py：正则替换带回调
来源：http://hz.yueranfly.top/gtxpjnovao.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.daria6918.cn/gttengttvf.html

[U20] Py：缓存函数结果
来源：http://hz.svipenyu.cn/gtdfwiwpry.html

@functools.lru_cache(maxsize=None)
来源：http://hz.cheryme.top/gtufztqkpu.html

[U21] Py：自定义上下文管理器
来源：http://hz.birdmap.top/gtradsldzc.html

@contextlib.contextmanager
来源：http://hz.xingfuxueyuan.xyz/gtyztcrnnq.html

[U22] Py：矩阵转置
来源：http://hz.wangdashe.top/gtbqzgjmvi.html

list(zip(*m))
来源：http://hz.jinqigufen.top/gtdoywogbx.html

[U23] Py：分块读取大文件
来源：http://hz.zhengqikj.top/gtakoeoase.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.jyoumei.cn/gtxalnsurh.html

[U24] Py：路径操作
来源：http://hz.zhoulong.xyz/gtyusymgaz.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.havefunace.top/gtmjwcwkfx.html

[U25] Py：CSV 按字典读
来源：http://hz.xuanzx.com/gtdxryolnc.html

csv.DictReader(f)
来源：http://hz.cqqwz.cn/gtaesqddud.html

[U26] Py：并发下载
来源：http://hz.dianchejie.cn/gtbwtmgjjm.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.shanyushiyangkeji.top/gtuubwykkl.html

[U27] Py：异步 HTTP
来源：http://hz.sxryk.cn/gtkeembppe.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.cheryme.top/gtxtrmbxfx.html

[U28] Py：类型别名
来源：http://hz.daria6918.cn/gtfvvnrisp.html

UserId = int
来源：http://hz.wangshuangyany.cn/gtmhucbojo.html

[U29] Py：属性校验
来源：http://hz.52xcode.cn/gtndmbsara.html

@property 与 @x.setter 配合
来源：http://hz.sysykeji.top/gtjhbdsaro.html

[U30] Py：数据类
来源：http://hz.haohaochexian.top/gtczstwtux.html

@dataclass(slots=True)
来源：http://hz.jinyuanbaomall.cn/gtyvdfuepm.html

[U31] Py：单测
来源：http://hz.guannengcc.top/gticnvdluf.html

python -m pytest -q
来源：http://hz.vqdsnc.cn/gtrcoasydn.html

[U32] Py：代码格式化
来源：http://hz.yanxiufei.cn/gtbqfvhadi.html

ruff format . && ruff check --fix .
来源：http://hz.aibaodan.cn/gtlguwngzz.html

[U33] Py：打包发布
来源：http://hz.ywan-chungtsiang.top/gthtmqikrd.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.ydzc1.top/gtnjfgxviq.html

[U34] Py：判断编码
来源：http://hz.shuidangran.top/gtnziiorsi.html

chardet.detect(raw)
来源：http://hz.xuetiantiany.cn/gtwwbiyfws.html

[U35] Py：发送邮件
来源：http://hz.wangshuangyany.cn/gtoumhzpml.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.ehwqpu.com/gtelmvgzpz.html

[U36] Py：定时任务
来源：http://hz.shanyushiyangtech.top/gtcovazrpr.html

schedule.every(10).minutes.do(job)
来源：http://hz.jinghuilouyu.cn/gtkkrfmwdr.html

[U37] Py：读写 Excel
来源：http://hz.smart0.xyz/gtonlmhnie.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.andypj.xyz/gtwpgumpcd.html

[U38] Py：获取脚本所在目录
来源：http://hz.sxryk.cn/gtwqgehigh.html

Path(__file__).resolve().parent
来源：http://hz.chenlongwang.top/gtgbsssick.html

[U39] Py：判断是否在交互环境
来源：http://hz.jqgufenzy.top/gtwbxuyxfi.html

sys.stdout.isatty()
来源：http://hz.hywenlv.cn/gtxjidffme.html

[U40] Py：打印到标准错误
来源：http://hz.0kj1m.cn/gtjwxqsntx.html

print("err", file=sys.stderr)
来源：http://hz.yj20258888.top/gtgcpwrmtu.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.snrcjt.cn/gtjteayues.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.ydjk.org.cn/gtsrqzfaof.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.yvedp.cn/gtvfhuwmqn.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.sysykeji.top/gtyrihmjco.html

[U43] PHP：声明命名空间
来源：http://hz.guannengcc.top/gtizcbfomn.html

namespace App\Http;
来源：http://hz.birdmap.top/gtpsevddbm.html

[U44] PHP：开启严格类型
来源：http://hz.9152youxi.cn/gthfpfmzse.html

declare(strict_types=1);
来源：http://hz.jqgufenzy.top/gtqeliuryi.html

[U45] PHP：类型声明与返回类型
来源：http://hz.sufxvd.cn/gtqfoirnfy.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yuanzhike.top/gtfusaqxeo.html

[U46] PHP：可空类型
来源：http://hz.nwbrower.top/gtxlsboepg.html

?string $name = null
来源：http://hz.mhx1999.top/gtmcaszdhh.html

[U47] PHP：联合类型
来源：http://hz.cashguo.top/gtrfsemynr.html

int|string $id
来源：http://hz.zhixingplan.top/gtoyjhqkvy.html

[U48] PHP：纯枚举
来源：http://hz.birdmap.top/gteviuklgt.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.xuetiantiany.cn/gtqkpybwnq.html

[U49] PHP：只读属性
来源：http://hz.zdqjudy.top/gtdzqkluhs.html

public readonly string $name
来源：http://hz.yj20258888.top/gtlmxkmrmz.html

[U50] PHP：构造器属性提升
来源：http://hz.yongpay.top/gtopbuiwhp.html

public function __construct(private int $id) {}
来源：http://hz.52xcode.cn/gtjrzjizlz.html

[U51] PHP：数组解构
来源：http://hz.jianghu66.top/gtlbvufsng.html

[$a, $b] = $arr;
来源：http://hz.gzhubu.top/gtbwfdxhfp.html

[U52] PHP：箭头函数
来源：http://hz.shanyushiyangkeji.top/gtucfpwmvz.html

$double = fn($x) => $x * 2;
来源：http://hz.shanyushiyangkeji.top/gtnbjpaqur.html

[U53] PHP：空合并运算符
来源：http://hz.jianghu66.top/gtcyqjscbw.html

$v = $a ?? $b ?? "default";
来源：http://hz.xuetiantiany.cn/gtstuyzeqp.html

[U54] PHP：空安全调用
来源：http://hz.yj20258888.top/gteftdrild.html

$obj?->method()
来源：http://hz.bjfxy.top/gtqzkytvyl.html

[U55] PHP：match 表达式
来源：http://hz.52xcode.cn/gtdvkwsfec.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.zhongyouzk.top/gtkeypyvka.html

[U56] PHP：命名参数
来源：http://hz.ppjwa.cn/gtxeuayklz.html

f(a: 1, b: 2)
来源：http://hz.jqgfzy.top/gtsfauvwrh.html

[U57] PHP：字符串插值
来源：http://hz.havefunace.top/gtjmfliovl.html

"值: {$a}"
来源：http://hz.xziqi.cn/gtwmieidlo.html

[U58] PHP：数组三件套
来源：http://hz.haohaochexian.top/gtmziqurda.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.hfpthk.cn/gtmjccxend.html

[U59] PHP：自定义排序
来源：http://hz.zhijiandao.cn/gtqhvenkjn.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.birdmap.top/gtnkpeojbo.html

[U60] PHP：JSON 编解码
来源：http://hz.dashuyun.cn/gtfnxdvcjx.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.yuxming.cn/gtnxypxtfv.html

[U61] PHP：正则
来源：http://hz.sysykeji.top/gtfpsidfgv.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.hongshengwenyu.top/gtsmxadcxs.html

[U62] PHP：日期对象
来源：http://hz.yuxming.cn/gtuikjjvla.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.zhongyouzk.top/gtqjsjygxm.html

[U63] PHP：文件读写
来源：http://hz.quarkkingdee.top/gttehecbsf.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.shuidangran.top/gtlhlpfgak.html

[U64] PHP：目录遍历
来源：http://hz.xingfuxueyuan.xyz/gtzqdadizj.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.ybcxt.top/gtohwihqqa.html

[U65] PHP：会话
来源：http://hz.zhoulong.xyz/gthpiorskg.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.ydjk.org.cn/gtszmtdtws.html

[U66] PHP：设置 Cookie
来源：http://hz.havefunace.top/gtncdmbeqv.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.zdqjudy.top/gtvuycudjp.html

[U67] PHP：处理文件上传
来源：http://hz.kuanghao11.cn/gtoqeuadto.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.316326.xyz/gtgkmqcwcq.html

[U68] PHP：PDO 连接
来源：http://hz.shangyingyoupin.top/gtfretggnm.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.gogol.net.cn/gtsddmbvrm.html

[U69] PHP：PDO 预处理
来源：http://hz.jlsjyb.cn/gtustvhgno.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.yvedp.cn/gtjbrcqmav.html

[U70] PHP：PDO 事务
来源：http://hz.hongshengwenyu.top/gtisegtlps.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.shangyingyoupin.top/gtuvearvrk.html

[U71] PHP：抛出异常
来源：http://hz.xinyue.icu/gtqblarsar.html

throw new RuntimeException("失败", 500);
来源：http://hz.birdmap.top/gtkfpnxfeo.html

[U72] PHP：写错误日志
来源：http://hz.mhx1999.top/gteyjryuat.html

error_log("失败: " . $e->getMessage());
来源：http://hz.zhengqikj.top/gtfgzakosd.html

[U73] PHP：读取 ini 配置
来源：http://hz.gotoacloud.top/gtmiadrpvm.html

parse_ini_file("config.ini", true)
来源：http://hz.nanxuanxn.top/gttxmppdvu.html

[U74] PHP：读取环境变量
来源：http://hz.cashguo.top/gtqbthfhrl.html

getenv("APP_ENV") ?: "production"
来源：http://hz.cdnleiting.top/gtsezrrlil.html

[U75] PHP：依赖注入
来源：http://hz.nanxuanxn.top/gtscisdrhh.html

composer require psr/container
来源：http://hz.shzxlz.cn/gtwwtpqjkr.html

[U76] PHP：简单路由
来源：http://hz.zycfv.cn/gtkqflyopk.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.smart0.xyz/gtnzgsuyxb.html

[U77] PHP：模板渲染
来源：http://hz.ehwqpu.com/gtrzgewcap.html

composer require twig/twig
来源：http://hz.jinghuilouyu.cn/gtyyrzszmk.html

[U78] PHP：单元测试
来源：http://hz.yueranfly.top/gtytdpthgt.html

composer require --dev phpunit/phpunit
来源：http://hz.ydzc1.top/gtdlainvrr.html

[U79] PHP：静态分析
来源：http://hz.sufxvd.cn/gtarrujxik.html

composer require --dev phpstan/phpstan
来源：http://hz.snrcjt.cn/gtyujaybey.html

[U80] PHP：代码规范修复
来源：http://hz.ywan-chungtsiang.top/gtkiszoifn.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.pycfn.com/gttoeufrbv.html

[U81] JS：初始化项目
来源：http://hz.cqqwz.cn/gtqscdzkjc.html

npm init -y;  npm i express
来源：http://hz.iojbl.cn/gtxzvobtui.html

[U82] JS：package.json 脚本
来源：http://hz.yuanzhike.top/gtqznhhmrd.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.xuetiantiany.cn/gtcvpiiecs.html

[U83] JS：ES Module 导入导出
来源：http://hz.hongshengwenyu.top/gtgqgxmsmi.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.xziqi.cn/gtfvtovhov.html

[U84] JS：CommonJS 写法
来源：http://hz.ivvv.top/gtflevypix.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.aibaodan.cn/gtsiqfntxn.html

[U85] JS：可选链
来源：http://hz.xziqi.cn/gtyujwavwz.html

a?.b?.c
来源：http://hz.zhoulong.xyz/gthkwnemfq.html

[U86] JS：空值合并
来源：http://hz.ywan-chungtsiang.top/gtrfackcne.html

a ?? b
来源：http://hz.daria6918.cn/gtmpyvfqog.html

[U87] JS：解构默认值
来源：http://hz.jinghuilouyu.cn/gtpcrrkadl.html

const { a = 1, b = 2 } = obj;
来源：http://hz.chenjidiqi.icu/gtbhyifkep.html

[U88] JS：对象展开合并
来源：http://hz.cucudq.cn/gtzgmvxgml.html

{ ...a, ...b }
来源：http://hz.chenlongwang.top/gtiykmocka.html

[U89] JS：数组去重
来源：http://hz.iojbl.cn/gtgtxyddnl.html

[...new Set(arr)]
来源：http://hz.sweek.top/gtgdsrdkcc.html

[U90] JS：数字数组排序
来源：http://hz.dianchejie.cn/gtmrdxvngl.html

[...arr].sort((a, b) => a - b)
来源：http://hz.c1oappe.top/gthclufhje.html

[U91] JS：对象键值遍历
来源：http://hz.aibaodan.cn/gtwdazjuif.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.xziqi.cn/gtlfbeavez.html

[U92] JS：深拷贝
来源：http://hz.cqqwz.cn/gtpqhjmidf.html

structuredClone(obj)
来源：http://hz.nanxinkj.top/gtnwzfhghk.html

[U93] JS：模板字符串
来源：http://hz.yj202588.top/gtwkpfxfbc.html

`共 ${n} 条`
来源：http://hz.sweek.top/gtxiskqdbf.html

[U94] JS：箭头函数
来源：http://hz.vqdsnc.cn/gtjuzrwhee.html

const double = x => x * 2;
来源：http://hz.ybcxt.top/gthunhtsxd.html

[U95] JS：Promise 包装
来源：http://hz.zhaomingkeji.xyz/gtztensvtg.html

new Promise((resolve, reject) => {})
来源：http://hz.pengpengdd.cyou/gtordtsgkx.html

[U96] JS：async/await 与异常
来源：http://hz.yonumen.top/gtrmtuyubj.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.sysykeji.top/gtnptopfbb.html

[U97] JS：并发请求
来源：http://hz.hfpthk.cn/gtcxeodzfy.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shangyingyoupin.top/gtxmhcbebl.html

[U98] JS：fetch 带 JSON
来源：http://hz.fengsongda.top/gtsoynpfsy.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.hammf.cn/gtzddbiafj.html

[U99] JS：事件监听
来源：http://hz.dashuyun.cn/gtxzmzhjmf.html

el.addEventListener("click", e => {})
来源：http://hz.jianghu66.top/gtjifvknax.html

[U100] JS：DOM 查询
来源：http://hz.sufxvd.cn/gtumkvxpna.html

document.querySelector(".item")
来源：http://hz.haohaochexian.top/gtrqrvpphu.html

[U101] JS：classList 操作
来源：http://hz.jqgfzy.top/gthvyaisrd.html

el.classList.toggle("active")
来源：http://hz.bjfxy.top/gtkteqslry.html

[U102] JS：本地存储
来源：http://hz.smart0.xyz/gtixsljkww.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.redwolf501.top/gtnppdkezr.html

[U103] JS：定时器
来源：http://hz.ydjk.org.cn/gtlyohtlcc.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.yj20258888.top/gtevboxkdp.html

[U104] JS：防抖
来源：http://hz.cdnleiting.top/gtgyrwswia.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.sweek.top/gtwnirecti.html

[U105] JS：节流
来源：http://hz.yueranfly.top/gtrxallius.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.sufxvd.cn/gtkrgsmlfh.html

[U106] JS：日期格式化
来源：http://hz.fengsongda.top/gtflaepote.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.c1oappe.top/gtxvqsgqnn.html

[U107] JS：数字千分位
来源：http://hz.chenjidiqi.icu/gtrbtjrvyi.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.bjfxy.top/gtpifidyjx.html

[U108] JS：随机整数
来源：http://hz.zhiwuduotai.top/gtvswlwnoq.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.zhiwuduotai.top/gtnmuyrfmu.html

[U109] JS：数组分组
来源：http://hz.redwolf501.top/gtvaolxljb.html

Object.groupBy(arr, x => x.type)
来源：http://hz.guowangkeji.top/gtgjbvvxip.html

[U110] JS：数组分块
来源：http://hz.wangshuangyany.cn/gttoessmev.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.ehwqpu.com/gtotcbvjpm.html

[U111] JS：对象转 Map
来源：http://hz.yuanzhike.top/gtcbosadte.html

new Map(Object.entries(obj))
来源：http://hz.guowangkeji.top/gtkzlldvqg.html

[U112] JS：字符串补位
来源：http://hz.xylfe.cn/gtdzdbedfm.html

"7".padStart(3, "0")
来源：http://hz.9152youxi.cn/gtfbwqjett.html

[U113] JS：正则替换全部
来源：http://hz.yuxming.cn/gtnqkovzrh.html

s.replaceAll("a", "b")
来源：http://hz.svipenyu.cn/gturyuobdc.html

[U114] JS：JSON 深比较
来源：http://hz.fzhhl.top/gtvrndvizp.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.havefunace.top/gtxfwzvzey.html

[U115] JS：生成 UUID
来源：http://hz.zdqjudy.top/gtuiqlhkyx.html

crypto.randomUUID()
来源：http://hz.jyoumei.cn/gtfuplshkj.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.gogol.net.cn/gtllqvrmws.html

/** @param {string} name */ function f(name) {}
来源：http://hz.dianchejie.cn/gttrbiacvr.html

[U117] JS：单元测试
来源：http://hz.aizwys.cn/gteilvtghq.html

npm i -D vitest;  npx vitest
来源：http://hz.snrcjt.cn/gtnfajhuse.html

[U118] JS：开发服务器
来源：http://hz.jyoumei.cn/gtvuhyujvq.html

npm i -D vite;  npx vite
来源：http://hz.xziqi.cn/gtunkegikr.html

[U119] JS：生产构建
来源：http://hz.yuanzhike.top/gtvmovzfcr.html

npx vite build
来源：http://hz.hysaishi.cn/gtopwthsko.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.hnxiangtu.top/gtskleiwob.html

import.meta.env.VITE_API_URL
来源：http://hz.vqdsnc.cn/gtzbqcjxsl.html

================================================================================
来源：http://hz.svipenyu.cn/gtmcnvmjll.html

统计汇总
来源：http://hz.jinghuilouyu.cn/gtvteuooyu.html

================================================================================
来源：http://hz.svipenyu.cn/gtehnrganz.html

按语言统计（条）：
来源：http://hz.andypj.xyz/gtirycsbmi.html

Python ......... 252
来源：http://hz.xingfuxueyuan.xyz/gtbmkkpnnq.html

PHP ............ 252
来源：http://hz.birdmap.top/gtmcaisifj.html

JavaScript ..... 252
来源：http://hz.jqgfzy.top/gttvexickq.html

TypeScript ..... 212
来源：http://hz.svipenyu.cn/gtautvaptt.html

Java ........... 212
来源：http://hz.smart0.xyz/gthuqmkaue.html

Go ............. 212
来源：http://hz.sufxvd.cn/gtusghmedd.html

Ruby ........... 212
来源：http://hz.cheryme.top/gtfegyfhxw.html

C# ............. 212
来源：http://hz.vqdsnc.cn/gtazcyqxjk.html

C .............. 30
来源：http://hz.sweek.top/gtoldpedhn.html

C++ ............ 30
来源：http://hz.smart0.xyz/gtwtzrvhpq.html

SQL ............ 90
来源：http://hz.sysykeji.top/gtlpvjugkm.html

Bash ........... 80
来源：http://hz.iojbl.cn/gtxvybubdg.html


<!-- 参考信息 -->