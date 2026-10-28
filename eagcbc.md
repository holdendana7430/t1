代发 wailian999

[T49] Perl：函数
来源：http://hz.fengsongda.top/gtgkreubah.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.sufxvd.cn/gtvyddqhlu.html

[T50] Perl：逐行读文件
来源：http://hz.yj202588.top/gtwmylanxj.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.gaohongyu789.top/gtplbpzrfl.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.aibaodan.cn/gtdtinfqgw.html

[T51] Scala：Hello World
来源：http://hz.wangdashe.top/gtbwebqawm.html

println("Hello")
来源：http://hz.shuidangran.top/gtmvzgltgz.html

[T52] Scala：变量
来源：http://hz.wangdashe.top/gtagrdneqy.html

val a = 1;  var b = 2
来源：http://hz.jlsjyb.cn/gtyhvhdrgn.html

[T53] Scala：字符串插值
来源：http://hz.feifeiyinyue.top/gtelwltzam.html

s"值: $b"
来源：http://hz.pycfn.com/gtwinihjyw.html

[T54] Scala：集合映射
来源：http://hz.jinqigufen.top/gtaypkboes.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.feifeiyinyue.top/gtaitsgnga.html

[T55] Scala：集合过滤
来源：http://hz.9152youxi.cn/gthnqtwfbv.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.aizwys.cn/gtlarfmqib.html

[T56] Scala：样例类
来源：http://hz.zhiwuduotai.top/gtnkdfgllu.html

case class User(name: String, age: Int)
来源：http://hz.cashguo.top/gtfourqdys.html

[T57] Scala：模式匹配
来源：http://hz.kuanghao11.cn/gtiotjqtqu.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.jinqigfzy.top/gthbuprzaj.html

[T58] Scala：函数定义
来源：http://hz.vqdsnc.cn/gteporytfx.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.hongshengwenyu.top/gtcccsnhhf.html

[T59] Scala：循环
来源：http://hz.zhijiandao.cn/gtaxmpdffg.html

for (i <- 1 to 10) println(i)
来源：http://hz.pycfn.com/gtgzieekch.html

[T60] Scala：折叠
来源：http://hz.pengpengdd.cyou/gtnqirryiw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.shangyingyoupin.top/gtiumirmmc.html

================================================================================
来源：http://hz.daxiang520.top/gtjxueehqc.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.yongpay.top/gthbeumtnc.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtnxsakxnx.html

[U01] Py：创建虚拟环境
来源：http://hz.nanxuanxn.top/gtqespcasz.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.yueranfly.top/gtenzctpnm.html

[U02] Py：导出 / 安装依赖
来源：http://hz.zhengqikj.top/gthkfpyvrp.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.hfpthk.cn/gtnkfxpaao.html

[U03] Py：加载 .env 配置
来源：http://hz.sufxvd.cn/gtpcdtkbwf.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.jinyuanbaomall.cn/gtquadrdjz.html

[U04] Py：变量调试打印
来源：http://hz.shuidangran.top/gtdhuigvwc.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.dashuyun.cn/gtggccjjms.html

[U05] Py：列表去重且保序
来源：http://hz.zhijiandao.cn/gtzhrjkhoq.html

list(dict.fromkeys(arr))
来源：http://hz.shzxlz.cn/gtsfbjkiai.html

[U06] Py：合并两个字典
来源：http://hz.dashuyun.cn/gtpunccjvy.html

{**a, **b}
来源：http://hz.shangyingyoupin.top/gtsywhmttf.html

[U07] Py：反转字典键值
来源：http://hz.cucudq.cn/gtmxvuwnib.html

{v: k for k, v in d.items()}
来源：http://hz.zhoulong.xyz/gtlstwctzt.html

[U08] Py：展平二维列表
来源：http://hz.xziqi.cn/gthqcfqeys.html

[y for x in nested for y in x]
来源：http://hz.yj20258888.top/gteqghejzx.html

[U09] Py：字典取最大值的键
来源：http://hz.jqgufenzy.top/gtvjosqecv.html

max(d, key=d.get)
来源：http://hz.cqqwz.cn/gtozhpaawb.html

[U10] Py：按值排序字典
来源：http://hz.yueranfly.top/gtqttcqpcp.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.c1oappe.top/gtgnnxmqqa.html

[U11] Py：生成器表达式
来源：http://hz.jqgufenzy.top/gtsyqcrtnc.html

(x * 2 for x in arr)
来源：http://hz.jinqigfzy.top/gtektkcoox.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.zhengqikj.top/gtfdhsanye.html

Counter(arr).most_common(3)
来源：http://hz.meibo888.top/gtztatvwmz.html

[U13] Py：固定长度队列
来源：http://hz.zhengqikj.top/gtqgdujvps.html

deque(maxlen=10)
来源：http://hz.mhx1999.top/gtdzqisede.html

[U14] Py：分组收集到列表
来源：http://hz.dashuyun.cn/gtrouakljf.html

defaultdict(list)
来源：http://hz.hysaishi.cn/gtrpuskdzx.html

[U15] Py：高精度计时
来源：http://hz.zdqjudy.top/gtdcwyeijv.html

t = time.perf_counter()
来源：http://hz.haohaochexian.top/gtrxrwwdeg.html

[U16] Py：命令行参数解析
来源：http://hz.yuanzhike.top/gtzqrbtuiu.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.gotoacloud.top/gtjxndkauh.html

[U17] Py：初始化日志
来源：http://hz.ydzc1.top/gtqayxlboe.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.wangshuangyany.cn/gtuwluvrwy.html

[U18] Py：预编译正则
来源：http://hz.smart0.xyz/gttgrrpqde.html

pat = re.compile(r"\d+")
来源：http://hz.bjfxy.top/gtejmrshto.html

[U19] Py：正则替换带回调
来源：http://hz.pycfn.com/gtxarxwjde.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.xziqi.cn/gtbotqxcww.html

[U20] Py：缓存函数结果
来源：http://hz.316326.xyz/gtmtxfzsvj.html

@functools.lru_cache(maxsize=None)
来源：http://hz.jinyuanbaomall.cn/gtcafvaakg.html

[U21] Py：自定义上下文管理器
来源：http://hz.zhoulong.xyz/gtqaiyaxif.html

@contextlib.contextmanager
来源：http://hz.ivvv.top/gtghunbiak.html

[U22] Py：矩阵转置
来源：http://hz.wangshuangyany.cn/gthmzbhooz.html

list(zip(*m))
来源：http://hz.hfpthk.cn/gtlewvpcay.html

[U23] Py：分块读取大文件
来源：http://hz.jinqigfzy.top/gtsogzgnrw.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.kuanghao11.cn/gtdnnkpcwz.html

[U24] Py：路径操作
来源：http://hz.sufxvd.cn/gtdrrgvrts.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.chenlongwang.top/gtqnhabpvw.html

[U25] Py：CSV 按字典读
来源：http://hz.ivvv.top/gtdfnwqcdo.html

csv.DictReader(f)
来源：http://hz.smart0.xyz/gtovjsbipd.html

[U26] Py：并发下载
来源：http://hz.pengpengdd.cyou/gtujcxyohc.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.ppjwa.cn/gtfncvjjmh.html

[U27] Py：异步 HTTP
来源：http://hz.9152youxi.cn/gtrfbzlhss.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.quarkkingdee.top/gtcveatakf.html

[U28] Py：类型别名
来源：http://hz.yj20258888.top/gtnetvtmtp.html

UserId = int
来源：http://hz.hysaishi.cn/gtksggbbhw.html

[U29] Py：属性校验
来源：http://hz.yvedp.cn/gtsclqzgfi.html

@property 与 @x.setter 配合
来源：http://hz.chenjidiqi.icu/gtcovjbfzo.html

[U30] Py：数据类
来源：http://hz.wangdashe.top/gtfpvltwga.html

@dataclass(slots=True)
来源：http://hz.ppjwa.cn/gtmohntzmr.html

[U31] Py：单测
来源：http://hz.c1oappe.top/gtnyceejki.html

python -m pytest -q
来源：http://hz.smart0.xyz/gtirrputsk.html

[U32] Py：代码格式化
来源：http://hz.ydzc1.top/gtzlmomqkl.html

ruff format . && ruff check --fix .
来源：http://hz.dashuyun.cn/gtrckketwn.html

[U33] Py：打包发布
来源：http://hz.guowangkeji.top/gtjgeodvss.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.ppjwa.cn/gtihkzennm.html

[U34] Py：判断编码
来源：http://hz.sxryk.cn/gtsltxkcit.html

chardet.detect(raw)
来源：http://hz.fzhhl.top/gtqbtkqagx.html

[U35] Py：发送邮件
来源：http://hz.yueranfly.top/gtodehmeda.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.yvedp.cn/gtzdmincrh.html

[U36] Py：定时任务
来源：http://hz.hnqzz.top/gtuqrvdpyp.html

schedule.every(10).minutes.do(job)
来源：http://hz.guowangkeji.top/gtrqgzgkkm.html

[U37] Py：读写 Excel
来源：http://hz.zhengqikj.top/gtiwdmuwlk.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.fzhhl.top/gthdmliuid.html

[U38] Py：获取脚本所在目录
来源：http://hz.316326.xyz/gtonihhbsp.html

Path(__file__).resolve().parent
来源：http://hz.yongpay.top/gtkhjfbgqx.html

[U39] Py：判断是否在交互环境
来源：http://hz.dashuyun.cn/gtibdoefac.html

sys.stdout.isatty()
来源：http://hz.nanxinkj.top/gtquvlwbdv.html

[U40] Py：打印到标准错误
来源：http://hz.tian-w.cn/gtqnaipppp.html

print("err", file=sys.stderr)
来源：http://hz.chenzaomai.com/gtbvjpwkwe.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.yangfankeji.com/gtfebdzsbc.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.xuanzx.com/gtedkwigvu.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.haohaochexian.top/gtrdifrtno.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.yongpay.top/gtjnommakh.html

[U43] PHP：声明命名空间
来源：http://hz.feifeiyinyue.top/gtmurwffcx.html

namespace App\Http;
来源：http://hz.shuidangran.top/gtgwrpwqid.html

[U44] PHP：开启严格类型
来源：http://hz.mhx1999.top/gtmwrouema.html

declare(strict_types=1);
来源：http://hz.haohaochexian.top/gtrapjcncn.html

[U45] PHP：类型声明与返回类型
来源：http://hz.chenjidiqi.icu/gthsezhimn.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.aibaodan.cn/gtqmjorbgt.html

[U46] PHP：可空类型
来源：http://hz.wangdashe.top/gtbddplunr.html

?string $name = null
来源：http://hz.gzhubu.top/gtrcpuylwq.html

[U47] PHP：联合类型
来源：http://hz.tian-w.cn/gtuepqttri.html

int|string $id
来源：http://hz.sweek.top/gtokenacoz.html

[U48] PHP：纯枚举
来源：http://hz.zhongyouzk.top/gtdyzmxbkw.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.yueranfly.top/gtvevazkyn.html

[U49] PHP：只读属性
来源：http://hz.9152youxi.cn/gtjrdxkrcm.html

public readonly string $name
来源：http://hz.dashuyun.cn/gtqxjkxdtd.html

[U50] PHP：构造器属性提升
来源：http://hz.andypj.xyz/gtllecrmcm.html

public function __construct(private int $id) {}
来源：http://hz.hywenlv.cn/gtjqiicczc.html

[U51] PHP：数组解构
来源：http://hz.kuanghao11.cn/gtgmekfcmu.html

[$a, $b] = $arr;
来源：http://hz.jiagoushi.top/gtapavktxt.html

[U52] PHP：箭头函数
来源：http://hz.mhx1999.top/gtkylgwoan.html

$double = fn($x) => $x * 2;
来源：http://hz.zhoulong.xyz/gtiftyfdzp.html

[U53] PHP：空合并运算符
来源：http://hz.ivvv.top/gtqnmxzzcq.html

$v = $a ?? $b ?? "default";
来源：http://hz.sxryk.cn/gtwbgtgsli.html

[U54] PHP：空安全调用
来源：http://hz.316326.xyz/gtseelhssi.html

$obj?->method()
来源：http://hz.iojbl.cn/gthlakjawu.html

[U55] PHP：match 表达式
来源：http://hz.shangyingyoupin.top/gtbuxcaejo.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.sweek.top/gtzpxprdjg.html

[U56] PHP：命名参数
来源：http://hz.shanyushiyangtech.top/gtgpjksjiv.html

f(a: 1, b: 2)
来源：http://hz.yvedp.cn/gtdudxxfsb.html

[U57] PHP：字符串插值
来源：http://hz.birdmap.top/gtkgwnezmj.html

"值: {$a}"
来源：http://hz.cheryme.top/gtyvcltouu.html

[U58] PHP：数组三件套
来源：http://hz.yanxiufei.cn/gtgxxhehon.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.yj202588.top/gtpnzxsite.html

[U59] PHP：自定义排序
来源：http://hz.zhaomingkeji.xyz/gtisrlpzis.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.c1oappe.top/gtlrbajzfe.html

[U60] PHP：JSON 编解码
来源：http://hz.jinqigufen.top/gtasmlnkxa.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.gogol.net.cn/gtabpbsfpj.html

[U61] PHP：正则
来源：http://hz.fzhhl.top/gtfqopsiqt.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.daxiang520.top/gtpxrupunj.html

[U62] PHP：日期对象
来源：http://hz.andypj.xyz/gttgcrzrtx.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.xuanzx.com/gtlqzcjtzu.html

[U63] PHP：文件读写
来源：http://hz.chenlongwang.top/gtgohibhbt.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.chenjidiqi.icu/gtnnnmomin.html

[U64] PHP：目录遍历
来源：http://hz.0kj1m.cn/gtmsbimell.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.yuanzhike.top/gtxphadtiy.html

[U65] PHP：会话
来源：http://hz.yongpay.top/gtsyvoulnq.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.hnxiangtu.top/gtsfzafuwa.html

[U66] PHP：设置 Cookie
来源：http://hz.tianlin.xyz/gtsymyeghp.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.havefunace.top/gtaplisklj.html

[U67] PHP：处理文件上传
来源：http://hz.nanxinkj.top/gtmzikodsb.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.yj202588.top/gttqhcckgn.html

[U68] PHP：PDO 连接
来源：http://hz.yanxiufei.cn/gtlhntlaxv.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.zdqjudy.top/gtxezxmvkj.html

[U69] PHP：PDO 预处理
来源：http://hz.svipenyu.cn/gttwneocgz.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.zhixingplan.top/gttybjaaec.html

[U70] PHP：PDO 事务
来源：http://hz.guowangkeji.top/gthsgegukv.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.guowangkeji.top/gthsjulail.html

[U71] PHP：抛出异常
来源：http://hz.jinqigufen.top/gtpcrqujxd.html

throw new RuntimeException("失败", 500);
来源：http://hz.feifeiyinyue.top/gtcshgpdcz.html

[U72] PHP：写错误日志
来源：http://hz.dianchejie.cn/gtwatrygst.html

error_log("失败: " . $e->getMessage());
来源：http://hz.52xcode.cn/gtaenmbwry.html

[U73] PHP：读取 ini 配置
来源：http://hz.hongshengwenyu.top/gtfgqkqdwc.html

parse_ini_file("config.ini", true)
来源：http://hz.hnqzz.top/gtvdjxqowf.html

[U74] PHP：读取环境变量
来源：http://hz.jinqigufen.top/gtabxbvepu.html

getenv("APP_ENV") ?: "production"
来源：http://hz.fengsongda.top/gtqemtrmqs.html

[U75] PHP：依赖注入
来源：http://hz.zycfv.cn/gtypnnwlip.html

composer require psr/container
来源：http://hz.cdnleiting.top/gtxaqucsmv.html

[U76] PHP：简单路由
来源：http://hz.316326.xyz/gtwdgsxgov.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.smart0.xyz/gtuyscmfwa.html

[U77] PHP：模板渲染
来源：http://hz.guannengcc.top/gtjvqtkytl.html

composer require twig/twig
来源：http://hz.fengsongda.top/gtpvivxvze.html

[U78] PHP：单元测试
来源：http://hz.pengpengdd.cyou/gtutzwalyu.html

composer require --dev phpunit/phpunit
来源：http://hz.smart0.xyz/gtheeyarjl.html

[U79] PHP：静态分析
来源：http://hz.ppjwa.cn/gtaxkulefx.html

composer require --dev phpstan/phpstan
来源：http://hz.ydzc1.top/gtuvanckhv.html

[U80] PHP：代码规范修复
来源：http://hz.sweek.top/gthpshknzo.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.zhiwuduotai.top/gtyxlfzvhc.html

[U81] JS：初始化项目
来源：http://hz.chenjidiqi.icu/gtylubrwmr.html

npm init -y;  npm i express
来源：http://hz.jinqigfzy.top/gtlbcpfgkv.html

[U82] JS：package.json 脚本
来源：http://hz.bjfxy.top/gtwfkcaysb.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.gzhubu.top/gtuxarhlzl.html

[U83] JS：ES Module 导入导出
来源：http://hz.gaohongyu789.top/gtzdiusvtu.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.pycfn.com/gtnsuddniz.html

[U84] JS：CommonJS 写法
来源：http://hz.jiagoushi.top/gtfkvtfigi.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.gzhubu.top/gtwbijikqu.html

[U85] JS：可选链
来源：http://hz.yangfankeji.com/gtqodmvwwh.html

a?.b?.c
来源：http://hz.shzxlz.cn/gtylgrcojf.html

[U86] JS：空值合并
来源：http://hz.zhaomingkeji.xyz/gttlnswgfd.html

a ?? b
来源：http://hz.zhaomingkeji.xyz/gtxsdbrani.html

[U87] JS：解构默认值
来源：http://hz.hnxiangtu.top/gtrwibizvf.html

const { a = 1, b = 2 } = obj;
来源：http://hz.birdmap.top/gtvvtozury.html

[U88] JS：对象展开合并
来源：http://hz.zhixingplan.top/gtqwhexcgj.html

{ ...a, ...b }
来源：http://hz.haohaochexian.top/gtzadbpsll.html

[U89] JS：数组去重
来源：http://hz.sysykeji.top/gtazhvlhln.html

[...new Set(arr)]
来源：http://hz.zhaomingkeji.xyz/gttfenxkwr.html

[U90] JS：数字数组排序
来源：http://hz.guannengcc.top/gtdbokreqh.html

[...arr].sort((a, b) => a - b)
来源：http://hz.hammf.cn/gttukonajm.html

[U91] JS：对象键值遍历
来源：http://hz.zhongyouzk.top/gtwthbznsq.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.ydjk.org.cn/gtixebazmt.html

[U92] JS：深拷贝
来源：http://hz.cashguo.top/gthvtoravd.html

structuredClone(obj)
来源：http://hz.yj20258.top/gtodctkokz.html

[U93] JS：模板字符串
来源：http://hz.xuetiantiany.cn/gtqmmjlrqc.html

`共 ${n} 条`
来源：http://hz.hongshengwenyu.top/gtiwognoik.html

[U94] JS：箭头函数
来源：http://hz.yj20258.top/gtiaslqdul.html

const double = x => x * 2;
来源：http://hz.ppjwa.cn/gtlddidqxs.html

[U95] JS：Promise 包装
来源：http://hz.ydjk.org.cn/gtjodxoecn.html

new Promise((resolve, reject) => {})
来源：http://hz.cucudq.cn/gtwnpozurt.html

[U96] JS：async/await 与异常
来源：http://hz.jlsjyb.cn/gtqchrdxzc.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.shanyushiyangkeji.top/gtgfebquty.html

[U97] JS：并发请求
来源：http://hz.feifeiyinyue.top/gtaicqekdl.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jianghu66.top/gtdqebyqun.html

[U98] JS：fetch 带 JSON
来源：http://hz.feifeiyinyue.top/gtjsimewuv.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.jinyuanbaomall.cn/gtrxpbtlxk.html

[U99] JS：事件监听
来源：http://hz.birdmap.top/gtsfkkgxrl.html

el.addEventListener("click", e => {})
来源：http://hz.fzhhl.top/gtboguadtj.html

[U100] JS：DOM 查询
来源：http://hz.jianghu66.top/gtvzlsteug.html

document.querySelector(".item")
来源：http://hz.shangyingyoupin.top/gtdxykmuzq.html

[U101] JS：classList 操作
来源：http://hz.ydzc1.top/gtyvozpfrg.html

el.classList.toggle("active")
来源：http://hz.gogol.net.cn/gtvvtmdpnj.html

[U102] JS：本地存储
来源：http://hz.feifeiyinyue.top/gtkmxgeyln.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.xziqi.cn/gtukrsyeav.html

[U103] JS：定时器
来源：http://hz.birdmap.top/gtbmmqeosb.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.zhixingplan.top/gtzsglylef.html

[U104] JS：防抖
来源：http://hz.yuxming.cn/gtafsbjcdh.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.havefunace.top/gthvqhlbpi.html

[U105] JS：节流
来源：http://hz.hongshengwenyu.top/gtundvswts.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.c1oappe.top/gtijmhyofa.html

[U106] JS：日期格式化
来源：http://hz.sysykeji.top/gtfynjlbpb.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.xinyue.icu/gtxjkopxhm.html

[U107] JS：数字千分位
来源：http://hz.iojbl.cn/gtlnikxpui.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.daxiang520.top/gtqtqqbvrq.html

[U108] JS：随机整数
来源：http://hz.jinqigfzy.top/gtzkdjhnsf.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.hnxiangtu.top/gtnuefyvkh.html

[U109] JS：数组分组
来源：http://hz.redwolf501.top/gtzjzpiopo.html

Object.groupBy(arr, x => x.type)
来源：http://hz.feifeiyinyue.top/gtnzxkwvkv.html

[U110] JS：数组分块
来源：http://hz.hnqzz.top/gtifsbkxpc.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.ivvv.top/gtmxdaurfx.html

[U111] JS：对象转 Map
来源：http://hz.chenzaomai.com/gtoijjzqsy.html

new Map(Object.entries(obj))
来源：http://hz.sxryk.cn/gtwwgeydjy.html

[U112] JS：字符串补位
来源：http://hz.ybcxt.top/gtpyvfhoui.html

"7".padStart(3, "0")
来源：http://hz.gotoacloud.top/gthodawczj.html

[U113] JS：正则替换全部
来源：http://hz.snrcjt.cn/gthwbrlwbl.html

s.replaceAll("a", "b")
来源：http://hz.jiagoushi.top/gtvzvdareb.html

[U114] JS：JSON 深比较
来源：http://hz.chenlongwang.top/gtoaeqrbsm.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jlsjyb.cn/gtgpfqksws.html

[U115] JS：生成 UUID
来源：http://hz.aibaodan.cn/gtpplazvfn.html

crypto.randomUUID()
来源：http://hz.52xcode.cn/gtbgyiiytn.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.gogol.net.cn/gtkcvxlefc.html

/** @param {string} name */ function f(name) {}
来源：http://hz.jqgufenzy.top/gtnrhnewmg.html

[U117] JS：单元测试
来源：http://hz.nwbrower.top/gtdtgimckl.html

npm i -D vitest;  npx vitest
来源：http://hz.redwolf501.top/gtuuucnngm.html

[U118] JS：开发服务器
来源：http://hz.jinqigufen.top/gtcdsessky.html

npm i -D vite;  npx vite
来源：http://hz.dianchejie.cn/gtntqebbde.html

[U119] JS：生产构建
来源：http://hz.dashuyun.cn/gtpptmhlxf.html

npx vite build
来源：http://hz.daxiang520.top/gtqfysgffz.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.fengsongda.top/gttdhheijt.html

import.meta.env.VITE_API_URL
来源：http://hz.daria6918.cn/gtstueoeoz.html

================================================================================
来源：http://hz.sysykeji.top/gthczzkevj.html

统计汇总
来源：http://hz.hnqzz.top/gtneitcpnc.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtwmpknkko.html

按语言统计（条）：
来源：http://hz.316326.xyz/gttpgepedh.html

Python ......... 252
来源：http://hz.cheryme.top/gtuovsphwh.html

PHP ............ 252
来源：http://hz.gzhubu.top/gtjzgnlebj.html

JavaScript ..... 252
来源：http://hz.ydjk.org.cn/gtxvylgqdh.html

TypeScript ..... 212
来源：http://hz.fengsongda.top/gthvkvgyhp.html

Java ........... 212
来源：http://hz.cdnleiting.top/gtynfwgzuk.html

Go ............. 212
来源：http://hz.pycfn.com/gtzpfrvgmw.html

Ruby ........... 212
来源：http://hz.yongpay.top/gtgdspeosy.html

C# ............. 212
来源：http://hz.jinqigfzy.top/gtlnpogmve.html

C .............. 30
来源：http://hz.guannengcc.top/gthvlfjpqw.html

C++ ............ 30
来源：http://hz.vqdsnc.cn/gtgqayuawp.html

SQL ............ 90
来源：http://hz.zhaomingkeji.xyz/gtsooyzhlr.html

Bash ........... 80
来源：http://hz.pengpengdd.cyou/gtfpxwgdlc.html

Kotlin ......... 15
来源：http://hz.kuanghao11.cn/gtchnhqgfd.html

Swift .......... 15
来源：http://hz.cashguo.top/gtjilboioj.html

Lua ............ 10
来源：http://hz.ydjk.org.cn/gtsmfkcava.html

Perl ........... 10
来源：http://hz.sysykeji.top/gtxvmtwjqt.html

Scala .......... 10
来源：http://hz.ydzc1.top/gtjkkdetzg.html

------------------------------------
来源：http://hz.jqgfzy.top/gthgtcpwhz.html

合计 ........... 2106 条
来源：http://hz.jiagoushi.top/gtfhmpgftx.html

按章节统计：
来源：http://hz.zhiwuduotai.top/gtgxjozdbc.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.xziqi.cn/gtojoqwhmf.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.haohaochexian.top/gtgiqqbkxg.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.ydjk.org.cn/gtkogujsmu.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.sufxvd.cn/gtvrscsvlw.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.gzhubu.top/gtrsetlowv.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.haohaochexian.top/gtbbpvzkor.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.52xcode.cn/gthlrntbrt.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.redwolf501.top/gtexhmwbat.html


<!-- 参考信息 -->