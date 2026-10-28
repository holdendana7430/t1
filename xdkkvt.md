代发 wailian999

[T49] Perl：函数
来源：http://hz.52xcode.cn/gtxhooxmdt.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.jqgufenzy.top/gtujlnfpfw.html

[T50] Perl：逐行读文件
来源：http://hz.jiagoushi.top/gtimuiqhiv.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.yj20258888.top/gtzqrddwys.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.yueranfly.top/gtvuzxwhmb.html

[T51] Scala：Hello World
来源：http://hz.cheryme.top/gteecwzhgz.html

println("Hello")
来源：http://hz.ywan-chungtsiang.top/gthouygvjx.html

[T52] Scala：变量
来源：http://hz.ivvv.top/gtvghysztv.html

val a = 1;  var b = 2
来源：http://hz.pycfn.com/gtgvfnfsre.html

[T53] Scala：字符串插值
来源：http://hz.bjfxy.top/gtxmdcqddl.html

s"值: $b"
来源：http://hz.0kj1m.cn/gtjqhqajkf.html

[T54] Scala：集合映射
来源：http://hz.guannengcc.top/gtdflgsomk.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.fengsongda.top/gtjdkcrpsj.html

[T55] Scala：集合过滤
来源：http://hz.nanxinkj.top/gthajwdojg.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.ywan-chungtsiang.top/gtadzwqwlr.html

[T56] Scala：样例类
来源：http://hz.sysykeji.top/gtlnearqea.html

case class User(name: String, age: Int)
来源：http://hz.redwolf501.top/gtejkhdpco.html

[T57] Scala：模式匹配
来源：http://hz.jinghuilouyu.cn/gtoidzqyru.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.feifeiyinyue.top/gthfesjvat.html

[T58] Scala：函数定义
来源：http://hz.xinyue.icu/gtmixegaoj.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.sxryk.cn/gtnqhaximn.html

[T59] Scala：循环
来源：http://hz.yj20258.top/gtbfpfqpwo.html

for (i <- 1 to 10) println(i)
来源：http://hz.quarkkingdee.top/gtmegxzglq.html

[T60] Scala：折叠
来源：http://hz.nanxinkj.top/gthicdhyzw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.gotoacloud.top/gtqakrtelq.html

================================================================================
来源：http://hz.cashguo.top/gtlfjjnhgk.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.nanxuanxn.top/gtbtrlnyhv.html

================================================================================
来源：http://hz.zycfv.cn/gttrhfiwtl.html

[U01] Py：创建虚拟环境
来源：http://hz.dashuyun.cn/gtibvgnqdn.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.chenzaomai.com/gtpmvtwdct.html

[U02] Py：导出 / 安装依赖
来源：http://hz.zhoulong.xyz/gtocstgpjg.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.zhixingplan.top/gtnjoqzany.html

[U03] Py：加载 .env 配置
来源：http://hz.yueranfly.top/gtdmyoxcer.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.snrcjt.cn/gtisdtumux.html

[U04] Py：变量调试打印
来源：http://hz.nanxinkj.top/gtinlxkiwz.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.dashuyun.cn/gtozajqfrl.html

[U05] Py：列表去重且保序
来源：http://hz.xuetiantiany.cn/gtyzxzzqdw.html

list(dict.fromkeys(arr))
来源：http://hz.xylfe.cn/gtptrtxwht.html

[U06] Py：合并两个字典
来源：http://hz.haohaochexian.top/gtvlqpkzju.html

{**a, **b}
来源：http://hz.daxiang520.top/gtdevwfhwi.html

[U07] Py：反转字典键值
来源：http://hz.316326.xyz/gtauthmpzo.html

{v: k for k, v in d.items()}
来源：http://hz.fengsongda.top/gtlegvribq.html

[U08] Py：展平二维列表
来源：http://hz.yj20258888.top/gtvbyvsajf.html

[y for x in nested for y in x]
来源：http://hz.tianlin.xyz/gtrypmzefh.html

[U09] Py：字典取最大值的键
来源：http://hz.pengpengdd.cyou/gtwzqhzdrs.html

max(d, key=d.get)
来源：http://hz.hammf.cn/gtafzxzauq.html

[U10] Py：按值排序字典
来源：http://hz.shanyushiyangtech.top/gtqxguavcz.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.zdqjudy.top/gtnelrpike.html

[U11] Py：生成器表达式
来源：http://hz.zhiwuduotai.top/gtozqwqfcq.html

(x * 2 for x in arr)
来源：http://hz.yangfankeji.com/gtzzryqczt.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.0kj1m.cn/gturwrblje.html

Counter(arr).most_common(3)
来源：http://hz.cdnleiting.top/gtpybuwwyt.html

[U13] Py：固定长度队列
来源：http://hz.yangfankeji.com/gtcggrrnur.html

deque(maxlen=10)
来源：http://hz.nanxinkj.top/gtuusbpqdk.html

[U14] Py：分组收集到列表
来源：http://hz.daxiang520.top/gtqswdgksj.html

defaultdict(list)
来源：http://hz.zhaomingkeji.xyz/gtncxvyqji.html

[U15] Py：高精度计时
来源：http://hz.zhengqikj.top/gtkzjnream.html

t = time.perf_counter()
来源：http://hz.nwbrower.top/gtldeqaqdk.html

[U16] Py：命令行参数解析
来源：http://hz.zycfv.cn/gtwuxfrwnv.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.tianlin.xyz/gtqjohapuu.html

[U17] Py：初始化日志
来源：http://hz.ydjk.org.cn/gtnqnuoswn.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.shanyushiyangtech.top/gtcspvdjli.html

[U18] Py：预编译正则
来源：http://hz.redwolf501.top/gtzghtnfwo.html

pat = re.compile(r"\d+")
来源：http://hz.jinqigfzy.top/gttaxngede.html

[U19] Py：正则替换带回调
来源：http://hz.cheryme.top/gtlwompnag.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.chenzaomai.com/gttgnepxcm.html

[U20] Py：缓存函数结果
来源：http://hz.hammf.cn/gtsygrqlsy.html

@functools.lru_cache(maxsize=None)
来源：http://hz.jinghuilouyu.cn/gtfybrqxdc.html

[U21] Py：自定义上下文管理器
来源：http://hz.gzhubu.top/gthwyzvzal.html

@contextlib.contextmanager
来源：http://hz.jinyuanbaomall.cn/gtgmsqjglc.html

[U22] Py：矩阵转置
来源：http://hz.meibo888.top/gtadfgfrnq.html

list(zip(*m))
来源：http://hz.ivvv.top/gtyickugyf.html

[U23] Py：分块读取大文件
来源：http://hz.zhongyouzk.top/gtavevespu.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.sxryk.cn/gtgicvzwib.html

[U24] Py：路径操作
来源：http://hz.zdqjudy.top/gtsiqwizsi.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.yonumen.top/gtuulpokrj.html

[U25] Py：CSV 按字典读
来源：http://hz.hongshengwenyu.top/gtrfkkwvsq.html

csv.DictReader(f)
来源：http://hz.dashuyun.cn/gthuasxwxo.html

[U26] Py：并发下载
来源：http://hz.9152youxi.cn/gttshosini.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.feifeiyinyue.top/gtzemnxgnh.html

[U27] Py：异步 HTTP
来源：http://hz.haohaochexian.top/gtwwdrznfo.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.vqdsnc.cn/gtyromwuzg.html

[U28] Py：类型别名
来源：http://hz.yanxiufei.cn/gtlxdoilky.html

UserId = int
来源：http://hz.yvedp.cn/gtslmgmxrz.html

[U29] Py：属性校验
来源：http://hz.ydjk.org.cn/gthntdaoyw.html

@property 与 @x.setter 配合
来源：http://hz.tanke756.top/gtjqqeorwg.html

[U30] Py：数据类
来源：http://hz.jinqigufen.top/gtnloyqzpz.html

@dataclass(slots=True)
来源：http://hz.aizwys.cn/gtprnzdiaa.html

[U31] Py：单测
来源：http://hz.316326.xyz/gtvyhoorct.html

python -m pytest -q
来源：http://hz.fzhhl.top/gtgbvpoirs.html

[U32] Py：代码格式化
来源：http://hz.jinghuilouyu.cn/gtqnhyoshx.html

ruff format . && ruff check --fix .
来源：http://hz.quarkkingdee.top/gtuxvrekeb.html

[U33] Py：打包发布
来源：http://hz.zhaomingkeji.xyz/gtimoynkbc.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.ydjk.org.cn/gtymhnqwat.html

[U34] Py：判断编码
来源：http://hz.meibo888.top/gtiqelqyrz.html

chardet.detect(raw)
来源：http://hz.jianghu66.top/gtzghbotzp.html

[U35] Py：发送邮件
来源：http://hz.feifeiyinyue.top/gtilvfgxbe.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.jiagoushi.top/gtqgwajvpk.html

[U36] Py：定时任务
来源：http://hz.shuidangran.top/gtylfsilfa.html

schedule.every(10).minutes.do(job)
来源：http://hz.zhixingplan.top/gtlsejwqby.html

[U37] Py：读写 Excel
来源：http://hz.gzhubu.top/gtcqgkpwtx.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.cdnleiting.top/gtdvoypcqb.html

[U38] Py：获取脚本所在目录
来源：http://hz.ehwqpu.com/gttmrxsxou.html

Path(__file__).resolve().parent
来源：http://hz.yangfankeji.com/gtozzvwfdm.html

[U39] Py：判断是否在交互环境
来源：http://hz.xuetiantiany.cn/gtfvpcqimx.html

sys.stdout.isatty()
来源：http://hz.tanke756.top/gtuarzjerk.html

[U40] Py：打印到标准错误
来源：http://hz.zhengqikj.top/gtwmkjgden.html

print("err", file=sys.stderr)
来源：http://hz.sysykeji.top/gtrdkacltv.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.zhiwuduotai.top/gtpkbtcjyy.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.hywenlv.cn/gtwooxpvrs.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.chenzaomai.com/gtkvyobmxq.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.cqqwz.cn/gtgdzeccsk.html

[U43] PHP：声明命名空间
来源：http://hz.xylfe.cn/gtbzjebwhc.html

namespace App\Http;
来源：http://hz.guowangkeji.top/gtnuguipzc.html

[U44] PHP：开启严格类型
来源：http://hz.smart0.xyz/gtotqjxfss.html

declare(strict_types=1);
来源：http://hz.feifeiyinyue.top/gtenkysywc.html

[U45] PHP：类型声明与返回类型
来源：http://hz.dashuyun.cn/gtlotxblqq.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.sxryk.cn/gtzdsfxlvf.html

[U46] PHP：可空类型
来源：http://hz.jinqigfzy.top/gtulbtrcsl.html

?string $name = null
来源：http://hz.cqqwz.cn/gthfjqtlcg.html

[U47] PHP：联合类型
来源：http://hz.hfpthk.cn/gtdheyjnsi.html

int|string $id
来源：http://hz.cqqwz.cn/gtgewtaugs.html

[U48] PHP：纯枚举
来源：http://hz.feifeiyinyue.top/gtzilwgxlu.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.yuxming.cn/gtpsdowgbp.html

[U49] PHP：只读属性
来源：http://hz.wangdashe.top/gtonruibug.html

public readonly string $name
来源：http://hz.sweek.top/gtsrdyrbvj.html

[U50] PHP：构造器属性提升
来源：http://hz.chenzaomai.com/gtdvxvklzj.html

public function __construct(private int $id) {}
来源：http://hz.feifeiyinyue.top/gtjzfoavxu.html

[U51] PHP：数组解构
来源：http://hz.wangshuangyany.cn/gtutpebujp.html

[$a, $b] = $arr;
来源：http://hz.cucudq.cn/gtnsnlbidd.html

[U52] PHP：箭头函数
来源：http://hz.xziqi.cn/gtwdcfyjuo.html

$double = fn($x) => $x * 2;
来源：http://hz.hysaishi.cn/gtmilnryge.html

[U53] PHP：空合并运算符
来源：http://hz.hysaishi.cn/gtilpqcovr.html

$v = $a ?? $b ?? "default";
来源：http://hz.jlsjyb.cn/gtxryivqlj.html

[U54] PHP：空安全调用
来源：http://hz.316326.xyz/gtryweumba.html

$obj?->method()
来源：http://hz.gaohongyu789.top/gtpallpwob.html

[U55] PHP：match 表达式
来源：http://hz.guannengcc.top/gtpgfgwhee.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.xuetiantiany.cn/gtpghteygn.html

[U56] PHP：命名参数
来源：http://hz.yj202588.top/gtdejneexr.html

f(a: 1, b: 2)
来源：http://hz.sweek.top/gtuvjuptlp.html

[U57] PHP：字符串插值
来源：http://hz.zhiwuduotai.top/gthpmsbxxm.html

"值: {$a}"
来源：http://hz.sufxvd.cn/gtnsgimtev.html

[U58] PHP：数组三件套
来源：http://hz.xylfe.cn/gttxdaeizk.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.xziqi.cn/gtmcyxikda.html

[U59] PHP：自定义排序
来源：http://hz.316326.xyz/gtfnplduqh.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.c1oappe.top/gtmrgjdznp.html

[U60] PHP：JSON 编解码
来源：http://hz.nwbrower.top/gtxogspvzo.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.zhengqikj.top/gtvxeqibgq.html

[U61] PHP：正则
来源：http://hz.ehwqpu.com/gtlkwwubpb.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.yongpay.top/gtivqmqrrv.html

[U62] PHP：日期对象
来源：http://hz.yj20258.top/gtdhbwodnk.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.nanxinkj.top/gtlctiuxnz.html

[U63] PHP：文件读写
来源：http://hz.cqqwz.cn/gtwvpgmmcu.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.quarkkingdee.top/gtdcaqqiid.html

[U64] PHP：目录遍历
来源：http://hz.jqgfzy.top/gtipiwsrwl.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.havefunace.top/gtyvwrlggv.html

[U65] PHP：会话
来源：http://hz.cashguo.top/gtifyyuysv.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.jiagoushi.top/gtfvqxmszi.html

[U66] PHP：设置 Cookie
来源：http://hz.sufxvd.cn/gtdfkojzcq.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.sufxvd.cn/gtcvbubfsv.html

[U67] PHP：处理文件上传
来源：http://hz.yanxiufei.cn/gtkuqpxund.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.feifeiyinyue.top/gtavhblprs.html

[U68] PHP：PDO 连接
来源：http://hz.chenjidiqi.icu/gtomqoomsn.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.jinqigfzy.top/gtobsilkia.html

[U69] PHP：PDO 预处理
来源：http://hz.tanke756.top/gtwljatqis.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.52xcode.cn/gtveuzhvuo.html

[U70] PHP：PDO 事务
来源：http://hz.xuanzx.com/gtdwhbrubo.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.hammf.cn/gtoskbzgqn.html

[U71] PHP：抛出异常
来源：http://hz.daria6918.cn/gtwmzoxfbl.html

throw new RuntimeException("失败", 500);
来源：http://hz.aibaodan.cn/gtdehaazgf.html

[U72] PHP：写错误日志
来源：http://hz.gotoacloud.top/gtlrdkyuaw.html

error_log("失败: " . $e->getMessage());
来源：http://hz.sxryk.cn/gtcosphiew.html

[U73] PHP：读取 ini 配置
来源：http://hz.chenlongwang.top/gtsxxyhcis.html

parse_ini_file("config.ini", true)
来源：http://hz.zhiwuduotai.top/gtdfpwobqh.html

[U74] PHP：读取环境变量
来源：http://hz.vqdsnc.cn/gtpigtqmvx.html

getenv("APP_ENV") ?: "production"
来源：http://hz.birdmap.top/gtsptbddug.html

[U75] PHP：依赖注入
来源：http://hz.xuetiantiany.cn/gtdqmxobaj.html

composer require psr/container
来源：http://hz.yanxiufei.cn/gtnofowgvo.html

[U76] PHP：简单路由
来源：http://hz.hnqzz.top/gtjufxclro.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.jlsjyb.cn/gtrfqmrkgk.html

[U77] PHP：模板渲染
来源：http://hz.gogol.net.cn/gtjzysnykw.html

composer require twig/twig
来源：http://hz.tanke756.top/gtlostbcag.html

[U78] PHP：单元测试
来源：http://hz.jqgfzy.top/gtxidpimep.html

composer require --dev phpunit/phpunit
来源：http://hz.jinyuanbaomall.cn/gtlwchocwe.html

[U79] PHP：静态分析
来源：http://hz.cheryme.top/gtlgbkffyi.html

composer require --dev phpstan/phpstan
来源：http://hz.chenzaomai.com/gtmejbgnky.html

[U80] PHP：代码规范修复
来源：http://hz.tian-w.cn/gtnzvheuil.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.sufxvd.cn/gtrxhqijnj.html

[U81] JS：初始化项目
来源：http://hz.nanxinkj.top/gtpjfbtcxi.html

npm init -y;  npm i express
来源：http://hz.hfpthk.cn/gtchpojtsu.html

[U82] JS：package.json 脚本
来源：http://hz.pycfn.com/gtntbzjuki.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.yongpay.top/gtcejhuqzo.html

[U83] JS：ES Module 导入导出
来源：http://hz.zhaomingkeji.xyz/gtoasexrvm.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.shangyingyoupin.top/gtpvwkdxxz.html

[U84] JS：CommonJS 写法
来源：http://hz.52xcode.cn/gtyvngulpy.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.sweek.top/gtojvkcdyz.html

[U85] JS：可选链
来源：http://hz.cqqwz.cn/gtswlihrtj.html

a?.b?.c
来源：http://hz.yvedp.cn/gtmjiominc.html

[U86] JS：空值合并
来源：http://hz.zhaomingkeji.xyz/gtnsvwonpt.html

a ?? b
来源：http://hz.hywenlv.cn/gtzodkxpfn.html

[U87] JS：解构默认值
来源：http://hz.ivvv.top/gtyxdwxynk.html

const { a = 1, b = 2 } = obj;
来源：http://hz.sufxvd.cn/gtwxceumfy.html

[U88] JS：对象展开合并
来源：http://hz.shangyingyoupin.top/gtkrkwckow.html

{ ...a, ...b }
来源：http://hz.hammf.cn/gtgcxiuaiw.html

[U89] JS：数组去重
来源：http://hz.jinghuilouyu.cn/gtkkqmryad.html

[...new Set(arr)]
来源：http://hz.tian-w.cn/gtfcjnapxo.html

[U90] JS：数字数组排序
来源：http://hz.tanke756.top/gtioatlulc.html

[...arr].sort((a, b) => a - b)
来源：http://hz.zhaomingkeji.xyz/gturkirmzq.html

[U91] JS：对象键值遍历
来源：http://hz.pycfn.com/gtytagfqtc.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.guowangkeji.top/gtryqxgwmt.html

[U92] JS：深拷贝
来源：http://hz.hfpthk.cn/gtfcokbaxw.html

structuredClone(obj)
来源：http://hz.c1oappe.top/gtfipccvws.html

[U93] JS：模板字符串
来源：http://hz.hammf.cn/gtybyyzprm.html

`共 ${n} 条`
来源：http://hz.pengpengdd.cyou/gtaoqxlmiv.html

[U94] JS：箭头函数
来源：http://hz.quarkkingdee.top/gtysjwuwwy.html

const double = x => x * 2;
来源：http://hz.zhijiandao.cn/gtdecqofwl.html

[U95] JS：Promise 包装
来源：http://hz.zhijiandao.cn/gtnwhgdabl.html

new Promise((resolve, reject) => {})
来源：http://hz.xuetiantiany.cn/gtelcvegne.html

[U96] JS：async/await 与异常
来源：http://hz.zhengqikj.top/gtfpcdtoyi.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.snrcjt.cn/gtcfgsmbvr.html

[U97] JS：并发请求
来源：http://hz.jinqigufen.top/gtzqywcklp.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.pycfn.com/gtptzripar.html

[U98] JS：fetch 带 JSON
来源：http://hz.yj20258.top/gtxxbzepbg.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.c1oappe.top/gtxotpdghm.html

[U99] JS：事件监听
来源：http://hz.sweek.top/gtlpvojgps.html

el.addEventListener("click", e => {})
来源：http://hz.feifeiyinyue.top/gtahexmqco.html

[U100] JS：DOM 查询
来源：http://hz.shuidangran.top/gtwgwjhrik.html

document.querySelector(".item")
来源：http://hz.fengsongda.top/gtpimtfewr.html

[U101] JS：classList 操作
来源：http://hz.ivvv.top/gtegvlhtmx.html

el.classList.toggle("active")
来源：http://hz.tian-w.cn/gtakmruvxp.html

[U102] JS：本地存储
来源：http://hz.shzxlz.cn/gtonwjbsgm.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.cashguo.top/gtgtjogypd.html

[U103] JS：定时器
来源：http://hz.snrcjt.cn/gtbdflmlwr.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.hysaishi.cn/gtumtwhobm.html

[U104] JS：防抖
来源：http://hz.xuetiantiany.cn/gtsabssxaa.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.gaohongyu789.top/gtbsukirdf.html

[U105] JS：节流
来源：http://hz.jinghuilouyu.cn/gtpadxutzx.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.daxiang520.top/gtoiwrikoo.html

[U106] JS：日期格式化
来源：http://hz.hammf.cn/gttvvuemjl.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.ydjk.org.cn/gtpnhxlilj.html

[U107] JS：数字千分位
来源：http://hz.haohaochexian.top/gtmcbhxcbr.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.hnxiangtu.top/gtgwyejqev.html

[U108] JS：随机整数
来源：http://hz.meibo888.top/gtuzzihvpa.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.fzhhl.top/gtlzsyurcm.html

[U109] JS：数组分组
来源：http://hz.hammf.cn/gtwiyubmnv.html

Object.groupBy(arr, x => x.type)
来源：http://hz.ybcxt.top/gtakqoyfhf.html

[U110] JS：数组分块
来源：http://hz.c1oappe.top/gtizuxrvdt.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.ehwqpu.com/gttsahtomv.html

[U111] JS：对象转 Map
来源：http://hz.zhixingplan.top/gtfvyhrwlp.html

new Map(Object.entries(obj))
来源：http://hz.zhoulong.xyz/gtntekstbo.html

[U112] JS：字符串补位
来源：http://hz.jyoumei.cn/gtkrcanbkm.html

"7".padStart(3, "0")
来源：http://hz.0kj1m.cn/gtauwlqihn.html

[U113] JS：正则替换全部
来源：http://hz.wangshuangyany.cn/gtbpblcowm.html

s.replaceAll("a", "b")
来源：http://hz.jinghuilouyu.cn/gtraatnxxk.html

[U114] JS：JSON 深比较
来源：http://hz.xuanzx.com/gtrwtmfckp.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zdqjudy.top/gtrdephftr.html

[U115] JS：生成 UUID
来源：http://hz.sysykeji.top/gtxlbqewfs.html

crypto.randomUUID()
来源：http://hz.jinqigufen.top/gtctyxhwyt.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.nanxinkj.top/gtlvnyrmly.html

/** @param {string} name */ function f(name) {}
来源：http://hz.shanyushiyangkeji.top/gtlvvlfhbe.html

[U117] JS：单元测试
来源：http://hz.shuidangran.top/gtkvmnvmkf.html

npm i -D vitest;  npx vitest
来源：http://hz.tanke756.top/gtcejwimgz.html

[U118] JS：开发服务器
来源：http://hz.ybcxt.top/gtdcibhqzb.html

npm i -D vite;  npx vite
来源：http://hz.0kj1m.cn/gtefbzqqeb.html

[U119] JS：生产构建
来源：http://hz.nanxinkj.top/gtevamzxqe.html

npx vite build
来源：http://hz.quarkkingdee.top/gtcrndhrui.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.vqdsnc.cn/gtalcbgzyb.html

import.meta.env.VITE_API_URL
来源：http://hz.cucudq.cn/gtnhshmeaq.html

================================================================================
来源：http://hz.chenzaomai.com/gtgydidocn.html

统计汇总
来源：http://hz.shangyingyoupin.top/gtsaibmkrz.html

================================================================================
来源：http://hz.gogol.net.cn/gtliqfulap.html

按语言统计（条）：
来源：http://hz.0kj1m.cn/gtjhytlonw.html

Python ......... 252
来源：http://hz.gaohongyu789.top/gtoicxpnzh.html

PHP ............ 252
来源：http://hz.zhiwuduotai.top/gthzwhtrtd.html

JavaScript ..... 252
来源：http://hz.zhixingplan.top/gtmrufpzhh.html

TypeScript ..... 212
来源：http://hz.cucudq.cn/gtwzbmmzbk.html

Java ........... 212
来源：http://hz.yj20258.top/gtvaeimwkx.html

Go ............. 212
来源：http://hz.316326.xyz/gtaxhxwprq.html

Ruby ........... 212
来源：http://hz.pengpengdd.cyou/gtuasazgqe.html

C# ............. 212
来源：http://hz.bjfxy.top/gtledtzpqj.html

C .............. 30
来源：http://hz.ehwqpu.com/gtzxclmvvx.html

C++ ............ 30
来源：http://hz.wangdashe.top/gtsjhqtjhw.html

SQL ............ 90
来源：http://hz.dianchejie.cn/gtgfdtofbi.html

Bash ........... 80
来源：http://hz.chenjidiqi.icu/gtqjnuqbrp.html

Kotlin ......... 15
来源：http://hz.ydzc1.top/gtjoldxhzw.html

Swift .......... 15
来源：http://hz.wangdashe.top/gtjebivrac.html

Lua ............ 10
来源：http://hz.fengsongda.top/gtortbepjh.html

Perl ........... 10
来源：http://hz.zhijiandao.cn/gtvnjiyciy.html

Scala .......... 10
来源：http://hz.tian-w.cn/gtowfqdmhl.html

------------------------------------
来源：http://hz.gaohongyu789.top/gttifswwnq.html

合计 ........... 2106 条
来源：http://hz.jinghuilouyu.cn/gtgjhkzwgu.html

按章节统计：
来源：http://hz.gzhubu.top/gtfydzjnwc.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.chenjidiqi.icu/gtqyjzfgdz.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.yangfankeji.com/gtlkypekcp.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.guowangkeji.top/gtamliloaj.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.xuanzx.com/gtubauphhx.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.kuanghao11.cn/gtpkcogrnj.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.xuetiantiany.cn/gtetyamvuh.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.pycfn.com/gtpyfzpcev.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.cqqwz.cn/gtvvpymzap.html


<!-- 参考信息 -->