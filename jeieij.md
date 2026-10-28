代发 wailian999

[T47] Perl：正则捕获
来源：http://hz.zhengqikj.top/gtgvhrpsav.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.ehwqpu.com/gtkighdgdm.html

[T48] Perl：正则替换
来源：http://hz.sysykeji.top/gtqbvkefai.html

$s =~ s/old/new/g;
来源：http://hz.zhaomingkeji.xyz/gtipbnvsyu.html

[T49] Perl：函数
来源：http://hz.yj20258.top/gthtwsefgp.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.jinqigufen.top/gtkfvhxiru.html

[T50] Perl：逐行读文件
来源：http://hz.shangyingyoupin.top/gtdvlfvquj.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.shangyingyoupin.top/gtpularuze.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.hysaishi.cn/gttsfpkiyc.html

[T51] Scala：Hello World
来源：http://hz.chenzaomai.com/gtmcjiemeq.html

println("Hello")
来源：http://hz.tian-w.cn/gtmzlqcekd.html

[T52] Scala：变量
来源：http://hz.zhiwuduotai.top/gtxooztlwf.html

val a = 1;  var b = 2
来源：http://hz.tian-w.cn/gtpfhcfrik.html

[T53] Scala：字符串插值
来源：http://hz.yj20258.top/gtxgruojbb.html

s"值: $b"
来源：http://hz.nanxuanxn.top/gtroonyykl.html

[T54] Scala：集合映射
来源：http://hz.ppjwa.cn/gtjokyeiwr.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.hammf.cn/gtxnjowrxx.html

[T55] Scala：集合过滤
来源：http://hz.tianlin.xyz/gtocmkgyzq.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.redwolf501.top/gtmflswiqd.html

[T56] Scala：样例类
来源：http://hz.jinqigufen.top/gtoyndqepl.html

case class User(name: String, age: Int)
来源：http://hz.guannengcc.top/gtqsexqjcy.html

[T57] Scala：模式匹配
来源：http://hz.bjfxy.top/gtcwtyqher.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.cashguo.top/gtnztyrcsj.html

[T58] Scala：函数定义
来源：http://hz.xylfe.cn/gtbpncserp.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.jlsjyb.cn/gtntzmazci.html

[T59] Scala：循环
来源：http://hz.chenlongwang.top/gterieesfj.html

for (i <- 1 to 10) println(i)
来源：http://hz.xingfuxueyuan.xyz/gtflpyxwgh.html

[T60] Scala：折叠
来源：http://hz.yvedp.cn/gtjamzscrt.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.tianlin.xyz/gtdrelgvce.html

================================================================================
来源：http://hz.9152youxi.cn/gtcmxrepnt.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.zdqjudy.top/gtarpziwsl.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtkiszwoqd.html

[U01] Py：创建虚拟环境
来源：http://hz.jinghuilouyu.cn/gtbzdlxpjb.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.yongpay.top/gthhukuqoj.html

[U02] Py：导出 / 安装依赖
来源：http://hz.iojbl.cn/gtqpvznmcm.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.jianghu66.top/gteqnbjsmt.html

[U03] Py：加载 .env 配置
来源：http://hz.fengsongda.top/gtluftfbim.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.birdmap.top/gtbtgdilyn.html

[U04] Py：变量调试打印
来源：http://hz.pengpengdd.cyou/gtkzzhvquw.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.yj20258.top/gtshgprbmr.html

[U05] Py：列表去重且保序
来源：http://hz.hnxiangtu.top/gtxlxsqpja.html

list(dict.fromkeys(arr))
来源：http://hz.iojbl.cn/gtsvalmrqt.html

[U06] Py：合并两个字典
来源：http://hz.yueranfly.top/gtbsyjhqbq.html

{**a, **b}
来源：http://hz.yvedp.cn/gthguzucqj.html

[U07] Py：反转字典键值
来源：http://hz.tanke756.top/gtkyqazczy.html

{v: k for k, v in d.items()}
来源：http://hz.shangyingyoupin.top/gtspovoqzg.html

[U08] Py：展平二维列表
来源：http://hz.shzxlz.cn/gtukmrzjvm.html

[y for x in nested for y in x]
来源：http://hz.pycfn.com/gtrlkbalrk.html

[U09] Py：字典取最大值的键
来源：http://hz.svipenyu.cn/gtpofmdlsx.html

max(d, key=d.get)
来源：http://hz.redwolf501.top/gtkjheivwx.html

[U10] Py：按值排序字典
来源：http://hz.dashuyun.cn/gttafkduja.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.cqqwz.cn/gtjodtgtbj.html

[U11] Py：生成器表达式
来源：http://hz.0kj1m.cn/gtosstgbzi.html

(x * 2 for x in arr)
来源：http://hz.ehwqpu.com/gtdifgdhxh.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.pengpengdd.cyou/gtjepvkdzb.html

Counter(arr).most_common(3)
来源：http://hz.jinqigufen.top/gtvjnsdivk.html

[U13] Py：固定长度队列
来源：http://hz.ydjk.org.cn/gthjsivzig.html

deque(maxlen=10)
来源：http://hz.iojbl.cn/gtwmjwraav.html

[U14] Py：分组收集到列表
来源：http://hz.tianlin.xyz/gtfnbaustl.html

defaultdict(list)
来源：http://hz.chenjidiqi.icu/gtbflomfvu.html

[U15] Py：高精度计时
来源：http://hz.gzhubu.top/gtyuoazakz.html

t = time.perf_counter()
来源：http://hz.aizwys.cn/gtvfpupucs.html

[U16] Py：命令行参数解析
来源：http://hz.cheryme.top/gtcqhqoxfa.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.pengpengdd.cyou/gteqksggay.html

[U17] Py：初始化日志
来源：http://hz.shanyushiyangtech.top/gtjckamdvl.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.snrcjt.cn/gtuxfgqroj.html

[U18] Py：预编译正则
来源：http://hz.meibo888.top/gtyepcucld.html

pat = re.compile(r"\d+")
来源：http://hz.52xcode.cn/gtbfluygjp.html

[U19] Py：正则替换带回调
来源：http://hz.xuetiantiany.cn/gtpwpembkj.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.zhaomingkeji.xyz/gtiqndtyyg.html

[U20] Py：缓存函数结果
来源：http://hz.zhiwuduotai.top/gtjnthezop.html

@functools.lru_cache(maxsize=None)
来源：http://hz.chenlongwang.top/gtytcnginj.html

[U21] Py：自定义上下文管理器
来源：http://hz.hfpthk.cn/gtqvpwotdo.html

@contextlib.contextmanager
来源：http://hz.yvedp.cn/gttvftcrqr.html

[U22] Py：矩阵转置
来源：http://hz.cucudq.cn/gtfszoywqi.html

list(zip(*m))
来源：http://hz.tian-w.cn/gtmvbihzzl.html

[U23] Py：分块读取大文件
来源：http://hz.yanxiufei.cn/gtpxmqwpwb.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.dianchejie.cn/gtcjjpelvr.html

[U24] Py：路径操作
来源：http://hz.wangshuangyany.cn/gtbecacujd.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.wangdashe.top/gteammtxfm.html

[U25] Py：CSV 按字典读
来源：http://hz.cashguo.top/gtddkumjpm.html

csv.DictReader(f)
来源：http://hz.hywenlv.cn/gtnlabykao.html

[U26] Py：并发下载
来源：http://hz.kuanghao11.cn/gtrizctvih.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.316326.xyz/gtcgpguzqt.html

[U27] Py：异步 HTTP
来源：http://hz.316326.xyz/gtyxpgaqnj.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.kuanghao11.cn/gtmwndbjwd.html

[U28] Py：类型别名
来源：http://hz.gzhubu.top/gtjaiqvfbs.html

UserId = int
来源：http://hz.meibo888.top/gtvcmmgvtu.html

[U29] Py：属性校验
来源：http://hz.hnxiangtu.top/gtyamapfyj.html

@property 与 @x.setter 配合
来源：http://hz.yj202588.top/gtlhzvjgub.html

[U30] Py：数据类
来源：http://hz.52xcode.cn/gtoqzufaiq.html

@dataclass(slots=True)
来源：http://hz.xziqi.cn/gtxxwywkez.html

[U31] Py：单测
来源：http://hz.xuetiantiany.cn/gttzvkecri.html

python -m pytest -q
来源：http://hz.yuanzhike.top/gtmliwivzc.html

[U32] Py：代码格式化
来源：http://hz.chenlongwang.top/gtuccunukd.html

ruff format . && ruff check --fix .
来源：http://hz.dashuyun.cn/gtvfodyaie.html

[U33] Py：打包发布
来源：http://hz.birdmap.top/gtdmycqvkm.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.ydjk.org.cn/gtmturwomt.html

[U34] Py：判断编码
来源：http://hz.wangshuangyany.cn/gtnfmcqigl.html

chardet.detect(raw)
来源：http://hz.zhiwuduotai.top/gtnakslfgi.html

[U35] Py：发送邮件
来源：http://hz.mhx1999.top/gtooefrjeh.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.jyoumei.cn/gtvkhzgazh.html

[U36] Py：定时任务
来源：http://hz.aizwys.cn/gtpffcpnom.html

schedule.every(10).minutes.do(job)
来源：http://hz.nwbrower.top/gtjuduluqb.html

[U37] Py：读写 Excel
来源：http://hz.ywan-chungtsiang.top/gtijxczgzd.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.cdnleiting.top/gtsidkoouy.html

[U38] Py：获取脚本所在目录
来源：http://hz.yueranfly.top/gtpkgpqnrl.html

Path(__file__).resolve().parent
来源：http://hz.zhijiandao.cn/gtebklsgjm.html

[U39] Py：判断是否在交互环境
来源：http://hz.cqqwz.cn/gtdklhewof.html

sys.stdout.isatty()
来源：http://hz.andypj.xyz/gtcppxscmm.html

[U40] Py：打印到标准错误
来源：http://hz.svipenyu.cn/gtdqfpgsxf.html

print("err", file=sys.stderr)
来源：http://hz.smart0.xyz/gtpvawauxy.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.jyoumei.cn/gtmoagdfff.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.fengsongda.top/gtasimvhmh.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.snrcjt.cn/gtxxpldrxh.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.birdmap.top/gtbcvxexql.html

[U43] PHP：声明命名空间
来源：http://hz.shangyingyoupin.top/gtybqmkaxi.html

namespace App\Http;
来源：http://hz.ywan-chungtsiang.top/gtcgozdgkf.html

[U44] PHP：开启严格类型
来源：http://hz.52xcode.cn/gtsazzjsyi.html

declare(strict_types=1);
来源：http://hz.smart0.xyz/gtmfulsfur.html

[U45] PHP：类型声明与返回类型
来源：http://hz.quarkkingdee.top/gtfmknildq.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ivvv.top/gthzbymczs.html

[U46] PHP：可空类型
来源：http://hz.snrcjt.cn/gtcpsmhgtt.html

?string $name = null
来源：http://hz.shangyingyoupin.top/gtpkvdwuhh.html

[U47] PHP：联合类型
来源：http://hz.jinqigfzy.top/gthqbyrrdn.html

int|string $id
来源：http://hz.hongshengwenyu.top/gtnrejbzml.html

[U48] PHP：纯枚举
来源：http://hz.yangfankeji.com/gtshicnxjz.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.0kj1m.cn/gtgvkorret.html

[U49] PHP：只读属性
来源：http://hz.smart0.xyz/gttnlkmlkx.html

public readonly string $name
来源：http://hz.aibaodan.cn/gterkldcsw.html

[U50] PHP：构造器属性提升
来源：http://hz.tian-w.cn/gtunqrzvdw.html

public function __construct(private int $id) {}
来源：http://hz.c1oappe.top/gtlyerjbdo.html

[U51] PHP：数组解构
来源：http://hz.daria6918.cn/gtrajpzokv.html

[$a, $b] = $arr;
来源：http://hz.aibaodan.cn/gtdnwbwejg.html

[U52] PHP：箭头函数
来源：http://hz.hfpthk.cn/gtjrohlvhg.html

$double = fn($x) => $x * 2;
来源：http://hz.xziqi.cn/gtrtzpdcgk.html

[U53] PHP：空合并运算符
来源：http://hz.fengsongda.top/gtdhxypoou.html

$v = $a ?? $b ?? "default";
来源：http://hz.cdnleiting.top/gtxxyrpxvo.html

[U54] PHP：空安全调用
来源：http://hz.yuanzhike.top/gtdxrveosb.html

$obj?->method()
来源：http://hz.zhijiandao.cn/gtngcocjsa.html

[U55] PHP：match 表达式
来源：http://hz.aibaodan.cn/gtcgayazry.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.aizwys.cn/gtqbpnydnk.html

[U56] PHP：命名参数
来源：http://hz.mhx1999.top/gtjbkixfsj.html

f(a: 1, b: 2)
来源：http://hz.cashguo.top/gtrwtmfzvk.html

[U57] PHP：字符串插值
来源：http://hz.jiagoushi.top/gtrajccdxs.html

"值: {$a}"
来源：http://hz.chenjidiqi.icu/gtkxucwgqx.html

[U58] PHP：数组三件套
来源：http://hz.jyoumei.cn/gtfzganfwe.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.ywan-chungtsiang.top/gtfqoskgsv.html

[U59] PHP：自定义排序
来源：http://hz.chenjidiqi.icu/gtuteeshyo.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.52xcode.cn/gtvqznbvfr.html

[U60] PHP：JSON 编解码
来源：http://hz.havefunace.top/gtmixhmitk.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.hnqzz.top/gtqhpdzisz.html

[U61] PHP：正则
来源：http://hz.aibaodan.cn/gtwxtwbruv.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.316326.xyz/gtayoxohca.html

[U62] PHP：日期对象
来源：http://hz.shuidangran.top/gtvqfxmsdu.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.ywan-chungtsiang.top/gtgivyfzki.html

[U63] PHP：文件读写
来源：http://hz.kuanghao11.cn/gtxpgrwiso.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.cheryme.top/gtozrikiwo.html

[U64] PHP：目录遍历
来源：http://hz.snrcjt.cn/gtiuvoynoj.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.jianghu66.top/gtupycbylw.html

[U65] PHP：会话
来源：http://hz.gotoacloud.top/gtgughopmq.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.jlsjyb.cn/gtgsptaurm.html

[U66] PHP：设置 Cookie
来源：http://hz.meibo888.top/gtxlhtieuh.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.ppjwa.cn/gtbsubuxua.html

[U67] PHP：处理文件上传
来源：http://hz.dianchejie.cn/gtyacjtcrr.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.snrcjt.cn/gtldshdzmr.html

[U68] PHP：PDO 连接
来源：http://hz.shuidangran.top/gttltpoqpn.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.xziqi.cn/gtpmxttkdf.html

[U69] PHP：PDO 预处理
来源：http://hz.havefunace.top/gtanmyiqtd.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.jqgfzy.top/gtuihhaqvv.html

[U70] PHP：PDO 事务
来源：http://hz.yj202588.top/gttcipkyod.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.iojbl.cn/gttfchxuib.html

[U71] PHP：抛出异常
来源：http://hz.wangdashe.top/gtehzmmcor.html

throw new RuntimeException("失败", 500);
来源：http://hz.shangyingyoupin.top/gtcasaohmt.html

[U72] PHP：写错误日志
来源：http://hz.pengpengdd.cyou/gtcoqoakns.html

error_log("失败: " . $e->getMessage());
来源：http://hz.gaohongyu789.top/gtlltcrwsq.html

[U73] PHP：读取 ini 配置
来源：http://hz.zhoulong.xyz/gtaljzxpil.html

parse_ini_file("config.ini", true)
来源：http://hz.ppjwa.cn/gtoavjhamw.html

[U74] PHP：读取环境变量
来源：http://hz.hongshengwenyu.top/gtqsqyezti.html

getenv("APP_ENV") ?: "production"
来源：http://hz.hnxiangtu.top/gtmuyheohg.html

[U75] PHP：依赖注入
来源：http://hz.hywenlv.cn/gtynvmhdkg.html

composer require psr/container
来源：http://hz.chenlongwang.top/gtbruxnznt.html

[U76] PHP：简单路由
来源：http://hz.hongshengwenyu.top/gtgdpeuusl.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.chenlongwang.top/gtueaqzzcz.html

[U77] PHP：模板渲染
来源：http://hz.ybcxt.top/gtqhteyyux.html

composer require twig/twig
来源：http://hz.gaohongyu789.top/gtokaprztc.html

[U78] PHP：单元测试
来源：http://hz.feifeiyinyue.top/gtlkardrxf.html

composer require --dev phpunit/phpunit
来源：http://hz.chenlongwang.top/gtptazubvf.html

[U79] PHP：静态分析
来源：http://hz.shzxlz.cn/gtglwlpone.html

composer require --dev phpstan/phpstan
来源：http://hz.yangfankeji.com/gtpadinuav.html

[U80] PHP：代码规范修复
来源：http://hz.yuanzhike.top/gthtzvyadp.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.yongpay.top/gtthgprbhq.html

[U81] JS：初始化项目
来源：http://hz.jyoumei.cn/gtqscyiimu.html

npm init -y;  npm i express
来源：http://hz.zhiwuduotai.top/gtmxoleisq.html

[U82] JS：package.json 脚本
来源：http://hz.sweek.top/gtvurragpr.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.sysykeji.top/gthomlhavw.html

[U83] JS：ES Module 导入导出
来源：http://hz.jinghuilouyu.cn/gtcljphpkh.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.jinqigufen.top/gtdkucqwuj.html

[U84] JS：CommonJS 写法
来源：http://hz.quarkkingdee.top/gtvxwzseyd.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.kuanghao11.cn/gtbddggpkf.html

[U85] JS：可选链
来源：http://hz.fzhhl.top/gtwfbmjvoo.html

a?.b?.c
来源：http://hz.hysaishi.cn/gtasuoppqt.html

[U86] JS：空值合并
来源：http://hz.jinqigufen.top/gtgtrqrffk.html

a ?? b
来源：http://hz.sufxvd.cn/gtffdpggej.html

[U87] JS：解构默认值
来源：http://hz.jiagoushi.top/gtfouuawjm.html

const { a = 1, b = 2 } = obj;
来源：http://hz.daria6918.cn/gtpfytxbny.html

[U88] JS：对象展开合并
来源：http://hz.zhongyouzk.top/gtlxbiweaz.html

{ ...a, ...b }
来源：http://hz.hnxiangtu.top/gtfvftlzwh.html

[U89] JS：数组去重
来源：http://hz.hfpthk.cn/gtbmzoziiu.html

[...new Set(arr)]
来源：http://hz.yvedp.cn/gtdzlzcywp.html

[U90] JS：数字数组排序
来源：http://hz.redwolf501.top/gttowwapfo.html

[...arr].sort((a, b) => a - b)
来源：http://hz.jqgfzy.top/gtijwnaqcr.html

[U91] JS：对象键值遍历
来源：http://hz.zhengqikj.top/gtantdavur.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.xuetiantiany.cn/gtatarkfig.html

[U92] JS：深拷贝
来源：http://hz.mhx1999.top/gtnpeezfui.html

structuredClone(obj)
来源：http://hz.snrcjt.cn/gtcfyrqatb.html

[U93] JS：模板字符串
来源：http://hz.gaohongyu789.top/gtywxfbmjg.html

`共 ${n} 条`
来源：http://hz.daria6918.cn/gtwlptdkdu.html

[U94] JS：箭头函数
来源：http://hz.yj20258888.top/gtucmbbuaa.html

const double = x => x * 2;
来源：http://hz.jinyuanbaomall.cn/gtzzgvdctn.html

[U95] JS：Promise 包装
来源：http://hz.gotoacloud.top/gtygplccej.html

new Promise((resolve, reject) => {})
来源：http://hz.hnqzz.top/gtigndzirb.html

[U96] JS：async/await 与异常
来源：http://hz.meibo888.top/gtsekaynxy.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.yj202588.top/gtchlhpqcx.html

[U97] JS：并发请求
来源：http://hz.hysaishi.cn/gtzrezwadb.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shzxlz.cn/gtllqvfibn.html

[U98] JS：fetch 带 JSON
来源：http://hz.vqdsnc.cn/gtanihbpkj.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.316326.xyz/gtsjewivbm.html

[U99] JS：事件监听
来源：http://hz.guannengcc.top/gtvjajbhin.html

el.addEventListener("click", e => {})
来源：http://hz.wangdashe.top/gtttvndrlb.html

[U100] JS：DOM 查询
来源：http://hz.nwbrower.top/gtewugwxnm.html

document.querySelector(".item")
来源：http://hz.meibo888.top/gtezitoift.html

[U101] JS：classList 操作
来源：http://hz.ydzc1.top/gtdxwgnrwq.html

el.classList.toggle("active")
来源：http://hz.andypj.xyz/gtexjvuydu.html

[U102] JS：本地存储
来源：http://hz.yonumen.top/gthlkccyal.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.cdnleiting.top/gtmgcokzlq.html

[U103] JS：定时器
来源：http://hz.jinqigfzy.top/gtkfaarvwh.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.feifeiyinyue.top/gtrrqlgrgr.html

[U104] JS：防抖
来源：http://hz.hnqzz.top/gtktamrskb.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hnqzz.top/gtrgeryrma.html

[U105] JS：节流
来源：http://hz.hfpthk.cn/gtqfqxobfc.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.birdmap.top/gtrerqqgys.html

[U106] JS：日期格式化
来源：http://hz.gotoacloud.top/gtyospnbmw.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.wangshuangyany.cn/gtoifhiyml.html

[U107] JS：数字千分位
来源：http://hz.nanxinkj.top/gtswsyavfe.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.gzhubu.top/gtwviokugj.html

[U108] JS：随机整数
来源：http://hz.guowangkeji.top/gtoifqzyzt.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.kuanghao11.cn/gtjfowjpig.html

[U109] JS：数组分组
来源：http://hz.jiagoushi.top/gthdbiaedp.html

Object.groupBy(arr, x => x.type)
来源：http://hz.jqgufenzy.top/gtktrbmvuu.html

[U110] JS：数组分块
来源：http://hz.yangfankeji.com/gtjqzgzepf.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.zdqjudy.top/gtsxwvxxfv.html

[U111] JS：对象转 Map
来源：http://hz.yuxming.cn/gtycyezgyv.html

new Map(Object.entries(obj))
来源：http://hz.yueranfly.top/gtzrgpzekx.html

[U112] JS：字符串补位
来源：http://hz.nanxuanxn.top/gtpojdcucd.html

"7".padStart(3, "0")
来源：http://hz.hywenlv.cn/gtvxvttagc.html

[U113] JS：正则替换全部
来源：http://hz.c1oappe.top/gtaljfxlpz.html

s.replaceAll("a", "b")
来源：http://hz.wangdashe.top/gtghjsvyvv.html

[U114] JS：JSON 深比较
来源：http://hz.haohaochexian.top/gtidskinbn.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.dashuyun.cn/gtcktpvntu.html

[U115] JS：生成 UUID
来源：http://hz.aibaodan.cn/gtlxthocvm.html

crypto.randomUUID()
来源：http://hz.0kj1m.cn/gtlxfkoddo.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.zhaomingkeji.xyz/gtqmsewqth.html

/** @param {string} name */ function f(name) {}
来源：http://hz.tanke756.top/gtkkcxbwlp.html

[U117] JS：单元测试
来源：http://hz.0kj1m.cn/gtnfnnbrfo.html

npm i -D vitest;  npx vitest
来源：http://hz.birdmap.top/gtwchhjcgf.html

[U118] JS：开发服务器
来源：http://hz.zhaomingkeji.xyz/gtpvwfutio.html

npm i -D vite;  npx vite
来源：http://hz.shanyushiyangkeji.top/gtktwenbpe.html

[U119] JS：生产构建
来源：http://hz.jiagoushi.top/gtmjvgfwym.html

npx vite build
来源：http://hz.yonumen.top/gtltomiicd.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.shanyushiyangkeji.top/gtfuxsvfhs.html

import.meta.env.VITE_API_URL
来源：http://hz.guannengcc.top/gtuzjewyzd.html

================================================================================
来源：http://hz.ybcxt.top/gtjwjggzrc.html

统计汇总
来源：http://hz.redwolf501.top/gtpmixsykl.html

================================================================================
来源：http://hz.jinqigfzy.top/gtffiecamg.html

按语言统计（条）：
来源：http://hz.smart0.xyz/gtndlaizie.html

Python ......... 252
来源：http://hz.cashguo.top/gtacqtrueu.html

PHP ............ 252
来源：http://hz.jianghu66.top/gtjhyuprpb.html

JavaScript ..... 252
来源：http://hz.hfpthk.cn/gtyctzfxih.html

TypeScript ..... 212
来源：http://hz.andypj.xyz/gtaqyalbdj.html

Java ........... 212
来源：http://hz.daxiang520.top/gtsyzfrjcy.html

Go ............. 212
来源：http://hz.jinghuilouyu.cn/gtrkgygldd.html

Ruby ........... 212
来源：http://hz.ybcxt.top/gterhdoefi.html

C# ............. 212
来源：http://hz.vqdsnc.cn/gtltzfbalm.html

C .............. 30
来源：http://hz.meibo888.top/gtkaqjotpb.html

C++ ............ 30
来源：http://hz.nanxuanxn.top/gtcrzwkpkq.html

SQL ............ 90
来源：http://hz.zhiwuduotai.top/gtlrumyhnh.html

Bash ........... 80
来源：http://hz.zhijiandao.cn/gtamzvdkhd.html

Kotlin ......... 15
来源：http://hz.ydjk.org.cn/gtkfimvyae.html

Swift .......... 15
来源：http://hz.xylfe.cn/gtewklhinf.html

Lua ............ 10
来源：http://hz.zhongyouzk.top/gtqyfvtqbs.html

Perl ........... 10
来源：http://hz.hnqzz.top/gtlnrqarna.html

Scala .......... 10
来源：http://hz.yongpay.top/gtrpitrwsr.html

------------------------------------
来源：http://hz.sysykeji.top/gtkjfjbmpc.html

合计 ........... 2106 条
来源：http://hz.zhongyouzk.top/gtjygcnalz.html

按章节统计：
来源：http://hz.chenzaomai.com/gtcgfmvypu.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.nwbrower.top/gtdkliqgvr.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.bjfxy.top/gtxxnkgktj.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.yueranfly.top/gtwknlzfnm.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.chenlongwang.top/gtexxqkehg.html


<!-- 参考信息 -->