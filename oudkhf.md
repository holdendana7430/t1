代发 wailian999

[T49] Perl：函数
来源：http://hz.zhixingplan.top/gtsdxnqfzz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.meibo888.top/gtjxekekqw.html

[T50] Perl：逐行读文件
来源：http://hz.hysaishi.cn/gtxplehsrw.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.yonumen.top/gtklfkmqmn.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.9152youxi.cn/gtsgdlntjp.html

[T51] Scala：Hello World
来源：http://hz.chenzaomai.com/gtlowinkkg.html

println("Hello")
来源：http://hz.nanxinkj.top/gtsbifaajp.html

[T52] Scala：变量
来源：http://hz.kuanghao11.cn/gtdvfmkurl.html

val a = 1;  var b = 2
来源：http://hz.redwolf501.top/gtmxxozjqi.html

[T53] Scala：字符串插值
来源：http://hz.smart0.xyz/gtfzpgnfyw.html

s"值: $b"
来源：http://hz.shzxlz.cn/gtgfmvmutq.html

[T54] Scala：集合映射
来源：http://hz.xylfe.cn/gtugayjbfa.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.ppjwa.cn/gtusxdglkw.html

[T55] Scala：集合过滤
来源：http://hz.jianghu66.top/gtrgddnlmg.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.zdqjudy.top/gtunwmgaiv.html

[T56] Scala：样例类
来源：http://hz.feifeiyinyue.top/gtivqaqomm.html

case class User(name: String, age: Int)
来源：http://hz.tianlin.xyz/gtryehevbp.html

[T57] Scala：模式匹配
来源：http://hz.cucudq.cn/gtfzhubcpz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.cucudq.cn/gtoonnzzdw.html

[T58] Scala：函数定义
来源：http://hz.xinyue.icu/gtkcwiualr.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.wangshuangyany.cn/gttfziigoj.html

[T59] Scala：循环
来源：http://hz.tian-w.cn/gtjtasyiam.html

for (i <- 1 to 10) println(i)
来源：http://hz.chenjidiqi.icu/gtqhaguucx.html

[T60] Scala：折叠
来源：http://hz.sweek.top/gtdbgjkmne.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.zhixingplan.top/gtarawpojh.html

================================================================================
来源：http://hz.shuidangran.top/gtoippwmnw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.wangshuangyany.cn/gtzvbouxcg.html

================================================================================
来源：http://hz.cdnleiting.top/gtryjvvqvg.html

[U01] Py：创建虚拟环境
来源：http://hz.shangyingyoupin.top/gtgrhfirfy.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.mhx1999.top/gtnnacswss.html

[U02] Py：导出 / 安装依赖
来源：http://hz.jqgfzy.top/gtywniohmr.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.meibo888.top/gtngcmejrk.html

[U03] Py：加载 .env 配置
来源：http://hz.yangfankeji.com/gtrhfspqig.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.daria6918.cn/gtakfsfbsp.html

[U04] Py：变量调试打印
来源：http://hz.jinqigufen.top/gtuqwrcarn.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.ehwqpu.com/gtqenbizat.html

[U05] Py：列表去重且保序
来源：http://hz.zhijiandao.cn/gtwfntkkqs.html

list(dict.fromkeys(arr))
来源：http://hz.smart0.xyz/gtfipsxere.html

[U06] Py：合并两个字典
来源：http://hz.jianghu66.top/gtjkrrffpj.html

{**a, **b}
来源：http://hz.gogol.net.cn/gtwrelgnra.html

[U07] Py：反转字典键值
来源：http://hz.smart0.xyz/gtfbrobkfp.html

{v: k for k, v in d.items()}
来源：http://hz.meibo888.top/gtczyjcfvj.html

[U08] Py：展平二维列表
来源：http://hz.fzhhl.top/gtaajdrawb.html

[y for x in nested for y in x]
来源：http://hz.yanxiufei.cn/gtlhzaumfd.html

[U09] Py：字典取最大值的键
来源：http://hz.feifeiyinyue.top/gthmtfawmm.html

max(d, key=d.get)
来源：http://hz.shangyingyoupin.top/gtuibateuq.html

[U10] Py：按值排序字典
来源：http://hz.aibaodan.cn/gtncjtxwuy.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.wangdashe.top/gtpbudomsk.html

[U11] Py：生成器表达式
来源：http://hz.yj202588.top/gtwfzuahxt.html

(x * 2 for x in arr)
来源：http://hz.vqdsnc.cn/gtesvexgak.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.andypj.xyz/gtrkjhktpo.html

Counter(arr).most_common(3)
来源：http://hz.gzhubu.top/gtfadvxjbk.html

[U13] Py：固定长度队列
来源：http://hz.cqqwz.cn/gtkyphrjbn.html

deque(maxlen=10)
来源：http://hz.jiagoushi.top/gtcjkmoitm.html

[U14] Py：分组收集到列表
来源：http://hz.zhixingplan.top/gtpwulfudu.html

defaultdict(list)
来源：http://hz.iojbl.cn/gtbygpjctw.html

[U15] Py：高精度计时
来源：http://hz.shuidangran.top/gtlwaxbjdx.html

t = time.perf_counter()
来源：http://hz.jqgufenzy.top/gtdykpqjvo.html

[U16] Py：命令行参数解析
来源：http://hz.hongshengwenyu.top/gthrfmwpbh.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.aibaodan.cn/gtjpdzddvt.html

[U17] Py：初始化日志
来源：http://hz.gotoacloud.top/gtncexwigo.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.chenzaomai.com/gtxsndrixk.html

[U18] Py：预编译正则
来源：http://hz.pycfn.com/gtoxkfgckz.html

pat = re.compile(r"\d+")
来源：http://hz.0kj1m.cn/gtnlyvxzzc.html

[U19] Py：正则替换带回调
来源：http://hz.sweek.top/gtlxlejmed.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.xinyue.icu/gtcrpfjubn.html

[U20] Py：缓存函数结果
来源：http://hz.zdqjudy.top/gtbfyfbhmx.html

@functools.lru_cache(maxsize=None)
来源：http://hz.iojbl.cn/gtwegetvcu.html

[U21] Py：自定义上下文管理器
来源：http://hz.tianlin.xyz/gtsnflilod.html

@contextlib.contextmanager
来源：http://hz.cdnleiting.top/gtxwjacezi.html

[U22] Py：矩阵转置
来源：http://hz.havefunace.top/gtczfbihrt.html

list(zip(*m))
来源：http://hz.tanke756.top/gtjlzcxcon.html

[U23] Py：分块读取大文件
来源：http://hz.ehwqpu.com/gtfanjtbrf.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.jinqigufen.top/gtmycxmbdv.html

[U24] Py：路径操作
来源：http://hz.sufxvd.cn/gtsdxowmvd.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.daria6918.cn/gtjyufiqph.html

[U25] Py：CSV 按字典读
来源：http://hz.hammf.cn/gtkefgikiy.html

csv.DictReader(f)
来源：http://hz.havefunace.top/gtxpsgrrsf.html

[U26] Py：并发下载
来源：http://hz.ydzc1.top/gtjjktfezy.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.zhaomingkeji.xyz/gtjlskqcye.html

[U27] Py：异步 HTTP
来源：http://hz.nwbrower.top/gtnnfjjhcp.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.fzhhl.top/gtsoagxutp.html

[U28] Py：类型别名
来源：http://hz.tanke756.top/gtujiihdnb.html

UserId = int
来源：http://hz.guannengcc.top/gtoijbsmns.html

[U29] Py：属性校验
来源：http://hz.yvedp.cn/gttvramokx.html

@property 与 @x.setter 配合
来源：http://hz.fengsongda.top/gtkulqrhip.html

[U30] Py：数据类
来源：http://hz.dashuyun.cn/gtrnjxdemk.html

@dataclass(slots=True)
来源：http://hz.redwolf501.top/gtzyyjapgn.html

[U31] Py：单测
来源：http://hz.jinghuilouyu.cn/gtoauraqvg.html

python -m pytest -q
来源：http://hz.hammf.cn/gtaxmccvui.html

[U32] Py：代码格式化
来源：http://hz.aizwys.cn/gttkdcdcyj.html

ruff format . && ruff check --fix .
来源：http://hz.guannengcc.top/gtyennnfqj.html

[U33] Py：打包发布
来源：http://hz.52xcode.cn/gtujzcuods.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.cucudq.cn/gttlxvvtlt.html

[U34] Py：判断编码
来源：http://hz.shzxlz.cn/gtcsrooysn.html

chardet.detect(raw)
来源：http://hz.ydjk.org.cn/gtkhxrlyct.html

[U35] Py：发送邮件
来源：http://hz.zhongyouzk.top/gtrvajxyry.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.svipenyu.cn/gtkdesbrsd.html

[U36] Py：定时任务
来源：http://hz.gotoacloud.top/gtvbhqlnpy.html

schedule.every(10).minutes.do(job)
来源：http://hz.haohaochexian.top/gtbqonoeob.html

[U37] Py：读写 Excel
来源：http://hz.zhaomingkeji.xyz/gtzrnlmtsa.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.sxryk.cn/gtddupfouo.html

[U38] Py：获取脚本所在目录
来源：http://hz.zhijiandao.cn/gtguaezphv.html

Path(__file__).resolve().parent
来源：http://hz.birdmap.top/gtzsohlqvm.html

[U39] Py：判断是否在交互环境
来源：http://hz.316326.xyz/gtqwnjnxnx.html

sys.stdout.isatty()
来源：http://hz.quarkkingdee.top/gtjtgfcjyw.html

[U40] Py：打印到标准错误
来源：http://hz.wangdashe.top/gtrroevfri.html

print("err", file=sys.stderr)
来源：http://hz.nanxinkj.top/gtszkaentt.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.zhixingplan.top/gtymndpspc.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.jinghuilouyu.cn/gtvrsasysa.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.shuidangran.top/gtinqkdpqe.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.wangshuangyany.cn/gtbqkdmzxc.html

[U43] PHP：声明命名空间
来源：http://hz.yj20258888.top/gtkxustblg.html

namespace App\Http;
来源：http://hz.yj20258.top/gtrywxuhrx.html

[U44] PHP：开启严格类型
来源：http://hz.xylfe.cn/gtppxnxfyx.html

declare(strict_types=1);
来源：http://hz.zhiwuduotai.top/gthxskmeie.html

[U45] PHP：类型声明与返回类型
来源：http://hz.zhaomingkeji.xyz/gtudzifelb.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.svipenyu.cn/gthsnjttrm.html

[U46] PHP：可空类型
来源：http://hz.haohaochexian.top/gtrinmisnt.html

?string $name = null
来源：http://hz.yj202588.top/gthgnythze.html

[U47] PHP：联合类型
来源：http://hz.redwolf501.top/gtngxwvkdy.html

int|string $id
来源：http://hz.jqgfzy.top/gtekntlpwh.html

[U48] PHP：纯枚举
来源：http://hz.jinghuilouyu.cn/gtdgpqktbi.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.jiagoushi.top/gtoyohnfgx.html

[U49] PHP：只读属性
来源：http://hz.mhx1999.top/gtvlmcasch.html

public readonly string $name
来源：http://hz.yj20258.top/gtllvpdpxd.html

[U50] PHP：构造器属性提升
来源：http://hz.shangyingyoupin.top/gthsitizcf.html

public function __construct(private int $id) {}
来源：http://hz.pycfn.com/gtvpjhbyvd.html

[U51] PHP：数组解构
来源：http://hz.sysykeji.top/gtdvsxhfdt.html

[$a, $b] = $arr;
来源：http://hz.fengsongda.top/gtdunnlukf.html

[U52] PHP：箭头函数
来源：http://hz.guowangkeji.top/gtjyyugjef.html

$double = fn($x) => $x * 2;
来源：http://hz.cdnleiting.top/gtvvnuwyzr.html

[U53] PHP：空合并运算符
来源：http://hz.pycfn.com/gtwuashxgt.html

$v = $a ?? $b ?? "default";
来源：http://hz.jqgufenzy.top/gtlqobwghn.html

[U54] PHP：空安全调用
来源：http://hz.cqqwz.cn/gtvjdwvzye.html

$obj?->method()
来源：http://hz.zhixingplan.top/gtmupexxhg.html

[U55] PHP：match 表达式
来源：http://hz.dianchejie.cn/gtqzzsaffl.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.yanxiufei.cn/gtviwybrkh.html

[U56] PHP：命名参数
来源：http://hz.ppjwa.cn/gtrbbwxahr.html

f(a: 1, b: 2)
来源：http://hz.52xcode.cn/gtlkxkkrms.html

[U57] PHP：字符串插值
来源：http://hz.aizwys.cn/gtvpcnezhd.html

"值: {$a}"
来源：http://hz.jinqigfzy.top/gtxphzynrp.html

[U58] PHP：数组三件套
来源：http://hz.cqqwz.cn/gtvzdbqrwb.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.aibaodan.cn/gtbjkltgzp.html

[U59] PHP：自定义排序
来源：http://hz.316326.xyz/gtfiykobds.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.guannengcc.top/gtrrrnesjc.html

[U60] PHP：JSON 编解码
来源：http://hz.nanxinkj.top/gtbgqpcajv.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.pycfn.com/gtxuqnorox.html

[U61] PHP：正则
来源：http://hz.dianchejie.cn/gtegsijpgz.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.hammf.cn/gtmyhhzwyg.html

[U62] PHP：日期对象
来源：http://hz.jiagoushi.top/gtujjblesj.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.zhiwuduotai.top/gtwawdgsus.html

[U63] PHP：文件读写
来源：http://hz.jyoumei.cn/gturjtmtqz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.sufxvd.cn/gtpkhpdhtn.html

[U64] PHP：目录遍历
来源：http://hz.316326.xyz/gtoogfzhqj.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.svipenyu.cn/gtjrourwue.html

[U65] PHP：会话
来源：http://hz.chenlongwang.top/gtflmxjhij.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.kuanghao11.cn/gtrakndrsj.html

[U66] PHP：设置 Cookie
来源：http://hz.hywenlv.cn/gtwxhpkqnz.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.gaohongyu789.top/gthsypcuge.html

[U67] PHP：处理文件上传
来源：http://hz.nwbrower.top/gtviscdjao.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.hammf.cn/gtfxeyfelv.html

[U68] PHP：PDO 连接
来源：http://hz.c1oappe.top/gtkuialbrz.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.chenjidiqi.icu/gtjshfobsz.html

[U69] PHP：PDO 预处理
来源：http://hz.zhijiandao.cn/gtewyqsurn.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.tian-w.cn/gtukubwzzr.html

[U70] PHP：PDO 事务
来源：http://hz.hysaishi.cn/gtpejiualx.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.pengpengdd.cyou/gtpbjthwqk.html

[U71] PHP：抛出异常
来源：http://hz.meibo888.top/gtcwoungww.html

throw new RuntimeException("失败", 500);
来源：http://hz.ehwqpu.com/gtlcmnfgmh.html

[U72] PHP：写错误日志
来源：http://hz.gogol.net.cn/gtlqvvgcor.html

error_log("失败: " . $e->getMessage());
来源：http://hz.hammf.cn/gtctlatgob.html

[U73] PHP：读取 ini 配置
来源：http://hz.zhongyouzk.top/gtvhwgcizi.html

parse_ini_file("config.ini", true)
来源：http://hz.bjfxy.top/gtzujavske.html

[U74] PHP：读取环境变量
来源：http://hz.mhx1999.top/gtkktqwafx.html

getenv("APP_ENV") ?: "production"
来源：http://hz.jlsjyb.cn/gtdkfyncnl.html

[U75] PHP：依赖注入
来源：http://hz.birdmap.top/gtxrbcwpgl.html

composer require psr/container
来源：http://hz.zdqjudy.top/gtgjlqxrjf.html

[U76] PHP：简单路由
来源：http://hz.sxryk.cn/gtrnvqjpke.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.jqgfzy.top/gtlqfvsmfd.html

[U77] PHP：模板渲染
来源：http://hz.shuidangran.top/gtflkpgwas.html

composer require twig/twig
来源：http://hz.yonumen.top/gtysgilooj.html

[U78] PHP：单元测试
来源：http://hz.52xcode.cn/gtvtqrwhbi.html

composer require --dev phpunit/phpunit
来源：http://hz.tian-w.cn/gtwcodddvu.html

[U79] PHP：静态分析
来源：http://hz.wangdashe.top/gtpkjandcv.html

composer require --dev phpstan/phpstan
来源：http://hz.ydzc1.top/gtlqtbifgm.html

[U80] PHP：代码规范修复
来源：http://hz.c1oappe.top/gtisqqcodk.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.jiagoushi.top/gtvqxluaik.html

[U81] JS：初始化项目
来源：http://hz.haohaochexian.top/gtyckkywgp.html

npm init -y;  npm i express
来源：http://hz.cheryme.top/gtqgyajlgh.html

[U82] JS：package.json 脚本
来源：http://hz.yvedp.cn/gtgzltaopv.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.xinyue.icu/gtjokgiglm.html

[U83] JS：ES Module 导入导出
来源：http://hz.chenzaomai.com/gtniyyhtyh.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.haohaochexian.top/gtkpkuijpq.html

[U84] JS：CommonJS 写法
来源：http://hz.gzhubu.top/gtwglbgjzb.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.yj20258888.top/gtegbpljvs.html

[U85] JS：可选链
来源：http://hz.haohaochexian.top/gtrdkxdgfn.html

a?.b?.c
来源：http://hz.dashuyun.cn/gtacpgpdsd.html

[U86] JS：空值合并
来源：http://hz.zhengqikj.top/gtlmzzfhnb.html

a ?? b
来源：http://hz.hnxiangtu.top/gtziextkit.html

[U87] JS：解构默认值
来源：http://hz.hnqzz.top/gtlspbjccd.html

const { a = 1, b = 2 } = obj;
来源：http://hz.shanyushiyangtech.top/gtmdhckgpv.html

[U88] JS：对象展开合并
来源：http://hz.yanxiufei.cn/gthgcgtcpc.html

{ ...a, ...b }
来源：http://hz.9152youxi.cn/gtkudlhbes.html

[U89] JS：数组去重
来源：http://hz.hongshengwenyu.top/gtlbulydox.html

[...new Set(arr)]
来源：http://hz.hfpthk.cn/gtzzwimtxl.html

[U90] JS：数字数组排序
来源：http://hz.nanxinkj.top/gtlhplawkz.html

[...arr].sort((a, b) => a - b)
来源：http://hz.zhaomingkeji.xyz/gtijbnstab.html

[U91] JS：对象键值遍历
来源：http://hz.zhaomingkeji.xyz/gtbsynviyr.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.aibaodan.cn/gterwnkliz.html

[U92] JS：深拷贝
来源：http://hz.sweek.top/gtlfpzseve.html

structuredClone(obj)
来源：http://hz.jqgufenzy.top/gtyfegtmnh.html

[U93] JS：模板字符串
来源：http://hz.ywan-chungtsiang.top/gtebskxrtn.html

`共 ${n} 条`
来源：http://hz.yuxming.cn/gtbgzppdas.html

[U94] JS：箭头函数
来源：http://hz.hysaishi.cn/gtnevgbvnh.html

const double = x => x * 2;
来源：http://hz.yj202588.top/gtptvwszri.html

[U95] JS：Promise 包装
来源：http://hz.jlsjyb.cn/gtdqgpiiog.html

new Promise((resolve, reject) => {})
来源：http://hz.zhaomingkeji.xyz/gtublxdjul.html

[U96] JS：async/await 与异常
来源：http://hz.nanxuanxn.top/gtruefokpl.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.xziqi.cn/gtltojggow.html

[U97] JS：并发请求
来源：http://hz.yj202588.top/gtdugazwku.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.redwolf501.top/gttltejhgc.html

[U98] JS：fetch 带 JSON
来源：http://hz.jinqigufen.top/gtisfcfiep.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.pycfn.com/gthhbqhyrt.html

[U99] JS：事件监听
来源：http://hz.tian-w.cn/gtrkghrdiy.html

el.addEventListener("click", e => {})
来源：http://hz.xingfuxueyuan.xyz/gttuybwjgj.html

[U100] JS：DOM 查询
来源：http://hz.xuetiantiany.cn/gtrzvnwqau.html

document.querySelector(".item")
来源：http://hz.yueranfly.top/gtmcuovzbp.html

[U101] JS：classList 操作
来源：http://hz.cucudq.cn/gtkhnajdtd.html

el.classList.toggle("active")
来源：http://hz.zhixingplan.top/gtrqmcddhi.html

[U102] JS：本地存储
来源：http://hz.yanxiufei.cn/gtkgvujhhn.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.smart0.xyz/gtxqlisqgy.html

[U103] JS：定时器
来源：http://hz.iojbl.cn/gtgyxlacsg.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.hongshengwenyu.top/gtfdbwkiea.html

[U104] JS：防抖
来源：http://hz.redwolf501.top/gtzdxpbbni.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.andypj.xyz/gtugofzorc.html

[U105] JS：节流
来源：http://hz.gogol.net.cn/gtpcxlyeew.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.yj20258888.top/gtqeeytbix.html

[U106] JS：日期格式化
来源：http://hz.hammf.cn/gtvwdxtbou.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.yonumen.top/gtnzwbtlmd.html

[U107] JS：数字千分位
来源：http://hz.pycfn.com/gtylwtwchw.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.yongpay.top/gtczpoesav.html

[U108] JS：随机整数
来源：http://hz.pycfn.com/gtmioqdkxh.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.yonumen.top/gtwgvtorhq.html

[U109] JS：数组分组
来源：http://hz.redwolf501.top/gtlgvbmuws.html

Object.groupBy(arr, x => x.type)
来源：http://hz.bjfxy.top/gtkfpoycws.html

[U110] JS：数组分块
来源：http://hz.guannengcc.top/gtgxxnxscj.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.316326.xyz/gtasngyhtw.html

[U111] JS：对象转 Map
来源：http://hz.ydzc1.top/gtreovmufz.html

new Map(Object.entries(obj))
来源：http://hz.yj202588.top/gtszeitsai.html

[U112] JS：字符串补位
来源：http://hz.nanxuanxn.top/gtjmlagoun.html

"7".padStart(3, "0")
来源：http://hz.fengsongda.top/gtceoqkqtb.html

[U113] JS：正则替换全部
来源：http://hz.pycfn.com/gtzvrmalhl.html

s.replaceAll("a", "b")
来源：http://hz.quarkkingdee.top/gtzdyxdxzy.html

[U114] JS：JSON 深比较
来源：http://hz.dianchejie.cn/gtfeeypyok.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.aibaodan.cn/gtcaerlpxm.html

[U115] JS：生成 UUID
来源：http://hz.tian-w.cn/gtoexadbdh.html

crypto.randomUUID()
来源：http://hz.shanyushiyangtech.top/gtpxmeffiz.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.jinqigfzy.top/gtdesbljfi.html

/** @param {string} name */ function f(name) {}
来源：http://hz.dashuyun.cn/gtxzspekvl.html

[U117] JS：单元测试
来源：http://hz.shangyingyoupin.top/gttqihklic.html

npm i -D vitest;  npx vitest
来源：http://hz.yongpay.top/gttppgardp.html

[U118] JS：开发服务器
来源：http://hz.ehwqpu.com/gtmsjqxrbd.html

npm i -D vite;  npx vite
来源：http://hz.haohaochexian.top/gtmssryjwb.html

[U119] JS：生产构建
来源：http://hz.birdmap.top/gthhooygwk.html

npx vite build
来源：http://hz.xinyue.icu/gtclwrwdyt.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.ydjk.org.cn/gtlitytzpr.html

import.meta.env.VITE_API_URL
来源：http://hz.9152youxi.cn/gtqiqwkxgi.html

================================================================================
来源：http://hz.316326.xyz/gtsvigiryi.html

统计汇总
来源：http://hz.jlsjyb.cn/gtmluvtfkt.html

================================================================================
来源：http://hz.cashguo.top/gtcihjnhoe.html

按语言统计（条）：
来源：http://hz.andypj.xyz/gtpusbcgpm.html

Python ......... 252
来源：http://hz.jiagoushi.top/gtyvrczsca.html

PHP ............ 252
来源：http://hz.gaohongyu789.top/gtfdpnalkq.html

JavaScript ..... 252
来源：http://hz.cucudq.cn/gtdlfiebtw.html

TypeScript ..... 212
来源：http://hz.yonumen.top/gtqtcxjilc.html

Java ........... 212
来源：http://hz.aibaodan.cn/gtqntpxszy.html

Go ............. 212
来源：http://hz.xylfe.cn/gtwhzapfgk.html

Ruby ........... 212
来源：http://hz.xuanzx.com/gtpaxsqhrg.html

C# ............. 212
来源：http://hz.xuetiantiany.cn/gtgnosifvq.html

C .............. 30
来源：http://hz.cqqwz.cn/gtwysaiyaq.html

C++ ............ 30
来源：http://hz.nwbrower.top/gtidokkcat.html

SQL ............ 90
来源：http://hz.jqgfzy.top/gtsbckhqam.html

Bash ........... 80
来源：http://hz.zhaomingkeji.xyz/gthdpnquid.html

Kotlin ......... 15
来源：http://hz.zhoulong.xyz/gtzrxyuyhw.html

Swift .......... 15
来源：http://hz.daria6918.cn/gtbmnbqiuo.html

Lua ............ 10
来源：http://hz.quarkkingdee.top/gtknpmbkpy.html

Perl ........... 10
来源：http://hz.jlsjyb.cn/gtkivkamvz.html

Scala .......... 10
来源：http://hz.ivvv.top/gtbbwjgtxs.html

------------------------------------
来源：http://hz.shanyushiyangtech.top/gtazghnbxa.html

合计 ........... 2106 条
来源：http://hz.jlsjyb.cn/gtcihotqci.html

按章节统计：
来源：http://hz.jinqigufen.top/gtnafxghxa.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.tanke756.top/gtgjzuqoyl.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.zhoulong.xyz/gtltgyyorn.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.hywenlv.cn/gtnrfbqsyj.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.9152youxi.cn/gtufkxdqbz.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.pengpengdd.cyou/gtdfhlcxku.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.ydzc1.top/gtzetfawrm.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.c1oappe.top/gtrfudgpub.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.gaohongyu789.top/gtcrhiasli.html


<!-- 参考信息 -->