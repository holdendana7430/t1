代发 wailian999

[T47] Perl：正则捕获
来源：http://hz.zhixingplan.top/gtctnuxuyd.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.snrcjt.cn/gtgezqpwkm.html

[T48] Perl：正则替换
来源：http://hz.ivvv.top/gtawrutqhk.html

$s =~ s/old/new/g;
来源：http://hz.hnqzz.top/gtbvstgwsi.html

[T49] Perl：函数
来源：http://hz.yj20258888.top/gtjgygjfzr.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.fengsongda.top/gtubtvrbcb.html

[T50] Perl：逐行读文件
来源：http://hz.jyoumei.cn/gthgegqcun.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.ybcxt.top/gtefaifovx.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.yj202588.top/gtqkembgvi.html

[T51] Scala：Hello World
来源：http://hz.jqgufenzy.top/gtjozsxist.html

println("Hello")
来源：http://hz.wangdashe.top/gtdtspnsju.html

[T52] Scala：变量
来源：http://hz.cucudq.cn/gtxgaleqbq.html

val a = 1;  var b = 2
来源：http://hz.jqgufenzy.top/gtgnmnpfyq.html

[T53] Scala：字符串插值
来源：http://hz.zdqjudy.top/gthgfdtzqy.html

s"值: $b"
来源：http://hz.ydjk.org.cn/gtfiyqqbyq.html

[T54] Scala：集合映射
来源：http://hz.chenzaomai.com/gtbpnrecma.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.gaohongyu789.top/gtytkpkgtd.html

[T55] Scala：集合过滤
来源：http://hz.chenlongwang.top/gtlbmygwmy.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.zhoulong.xyz/gtsqjiqmxp.html

[T56] Scala：样例类
来源：http://hz.aibaodan.cn/gtiaqsnvhf.html

case class User(name: String, age: Int)
来源：http://hz.yueranfly.top/gtohycuoru.html

[T57] Scala：模式匹配
来源：http://hz.sweek.top/gtsqbzfvqz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.wangshuangyany.cn/gtlthkmyrl.html

[T58] Scala：函数定义
来源：http://hz.haohaochexian.top/gtbwbelani.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.birdmap.top/gtztycgwta.html

[T59] Scala：循环
来源：http://hz.ywan-chungtsiang.top/gtcccleojg.html

for (i <- 1 to 10) println(i)
来源：http://hz.gogol.net.cn/gtfvlpwdoq.html

[T60] Scala：折叠
来源：http://hz.daria6918.cn/gtzzvbecdi.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.jinyuanbaomall.cn/gtdnevwvwm.html

================================================================================
来源：http://hz.52xcode.cn/gtjxczmnxy.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.shanyushiyangkeji.top/gtodnfqnpm.html

================================================================================
来源：http://hz.fzhhl.top/gtcwwnnboi.html

[U01] Py：创建虚拟环境
来源：http://hz.svipenyu.cn/gtjmhfptld.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.cashguo.top/gthqakgsao.html

[U02] Py：导出 / 安装依赖
来源：http://hz.cqqwz.cn/gtpfuqyxhz.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.hfpthk.cn/gtogcbhnra.html

[U03] Py：加载 .env 配置
来源：http://hz.ppjwa.cn/gtfzxxiolm.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.shangyingyoupin.top/gtwgeetxhz.html

[U04] Py：变量调试打印
来源：http://hz.yanxiufei.cn/gtvbrdanen.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.dashuyun.cn/gtbyygjjrh.html

[U05] Py：列表去重且保序
来源：http://hz.aizwys.cn/gtvzycosnq.html

list(dict.fromkeys(arr))
来源：http://hz.shangyingyoupin.top/gtpuqmvviz.html

[U06] Py：合并两个字典
来源：http://hz.jinyuanbaomall.cn/gtgvlgdvgr.html

{**a, **b}
来源：http://hz.dianchejie.cn/gtydzzsilf.html

[U07] Py：反转字典键值
来源：http://hz.pengpengdd.cyou/gtdnixohws.html

{v: k for k, v in d.items()}
来源：http://hz.tianlin.xyz/gtubkncxkz.html

[U08] Py：展平二维列表
来源：http://hz.sufxvd.cn/gtuqfhrqsm.html

[y for x in nested for y in x]
来源：http://hz.tanke756.top/gtiascbuqe.html

[U09] Py：字典取最大值的键
来源：http://hz.feifeiyinyue.top/gtgygcewwj.html

max(d, key=d.get)
来源：http://hz.hnqzz.top/gtjzdzlsdd.html

[U10] Py：按值排序字典
来源：http://hz.zhiwuduotai.top/gtorehajdd.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.jinghuilouyu.cn/gtvqfbhdqt.html

[U11] Py：生成器表达式
来源：http://hz.shuidangran.top/gtcxmtlgce.html

(x * 2 for x in arr)
来源：http://hz.yongpay.top/gtwjtdvisz.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.wangshuangyany.cn/gtgzdmqoee.html

Counter(arr).most_common(3)
来源：http://hz.jqgfzy.top/gturbaaxlp.html

[U13] Py：固定长度队列
来源：http://hz.hywenlv.cn/gtwygwjnlh.html

deque(maxlen=10)
来源：http://hz.wangdashe.top/gtzpjuqsja.html

[U14] Py：分组收集到列表
来源：http://hz.shuidangran.top/gtvfcieljb.html

defaultdict(list)
来源：http://hz.xylfe.cn/gtkbwsddnk.html

[U15] Py：高精度计时
来源：http://hz.aizwys.cn/gtgnuprnud.html

t = time.perf_counter()
来源：http://hz.jinghuilouyu.cn/gtpmjzfxzq.html

[U16] Py：命令行参数解析
来源：http://hz.meibo888.top/gtgsyqyhmf.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.cheryme.top/gtbgbhhmsv.html

[U17] Py：初始化日志
来源：http://hz.zhengqikj.top/gtltjwcfvh.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.xingfuxueyuan.xyz/gtclkbgaql.html

[U18] Py：预编译正则
来源：http://hz.xziqi.cn/gtjyredccm.html

pat = re.compile(r"\d+")
来源：http://hz.hywenlv.cn/gtfbvwopej.html

[U19] Py：正则替换带回调
来源：http://hz.jinqigfzy.top/gtrcsetvig.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.yonumen.top/gtuajmlcbp.html

[U20] Py：缓存函数结果
来源：http://hz.pycfn.com/gtgypaowme.html

@functools.lru_cache(maxsize=None)
来源：http://hz.ehwqpu.com/gtiafzvtnl.html

[U21] Py：自定义上下文管理器
来源：http://hz.xuetiantiany.cn/gtspdeqvaz.html

@contextlib.contextmanager
来源：http://hz.zhengqikj.top/gtmpwtumpx.html

[U22] Py：矩阵转置
来源：http://hz.quarkkingdee.top/gtogtuvsze.html

list(zip(*m))
来源：http://hz.hammf.cn/gtbcpieqra.html

[U23] Py：分块读取大文件
来源：http://hz.hywenlv.cn/gtugdeorls.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.xinyue.icu/gttrlcxwaa.html

[U24] Py：路径操作
来源：http://hz.jinghuilouyu.cn/gtsoehkkkz.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.sweek.top/gtprdvlvtv.html

[U25] Py：CSV 按字典读
来源：http://hz.sxryk.cn/gtfbomiaaw.html

csv.DictReader(f)
来源：http://hz.zhongyouzk.top/gtzugahfvn.html

[U26] Py：并发下载
来源：http://hz.cashguo.top/gtmsshrmpl.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.daxiang520.top/gtdpduptmn.html

[U27] Py：异步 HTTP
来源：http://hz.xuetiantiany.cn/gtvwaoaxjx.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.9152youxi.cn/gtmehuovad.html

[U28] Py：类型别名
来源：http://hz.bjfxy.top/gtxeigzaua.html

UserId = int
来源：http://hz.zhiwuduotai.top/gtbhpnefdd.html

[U29] Py：属性校验
来源：http://hz.fengsongda.top/gtkdejdzew.html

@property 与 @x.setter 配合
来源：http://hz.yueranfly.top/gtsfjlmodt.html

[U30] Py：数据类
来源：http://hz.zdqjudy.top/gtkrqtrglw.html

@dataclass(slots=True)
来源：http://hz.xylfe.cn/gthgypwodk.html

[U31] Py：单测
来源：http://hz.jinqigfzy.top/gthjdpblik.html

python -m pytest -q
来源：http://hz.xuetiantiany.cn/gtulcjhhce.html

[U32] Py：代码格式化
来源：http://hz.zhixingplan.top/gtfphrvkra.html

ruff format . && ruff check --fix .
来源：http://hz.yvedp.cn/gtfmzrrfqe.html

[U33] Py：打包发布
来源：http://hz.hysaishi.cn/gtzdscmquk.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.fzhhl.top/gtuwebwfcf.html

[U34] Py：判断编码
来源：http://hz.chenlongwang.top/gtazqrkwvj.html

chardet.detect(raw)
来源：http://hz.andypj.xyz/gthhyqufzw.html

[U35] Py：发送邮件
来源：http://hz.gotoacloud.top/gtxjocgmro.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.9152youxi.cn/gtcvprntkh.html

[U36] Py：定时任务
来源：http://hz.cucudq.cn/gtoywhlbla.html

schedule.every(10).minutes.do(job)
来源：http://hz.ivvv.top/gtbppsoapt.html

[U37] Py：读写 Excel
来源：http://hz.sufxvd.cn/gtgebanmbm.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.jlsjyb.cn/gtbvuiewhv.html

[U38] Py：获取脚本所在目录
来源：http://hz.nwbrower.top/gtstlqtbez.html

Path(__file__).resolve().parent
来源：http://hz.cheryme.top/gtmfhkuxqo.html

[U39] Py：判断是否在交互环境
来源：http://hz.316326.xyz/gtjgtvqszq.html

sys.stdout.isatty()
来源：http://hz.wangdashe.top/gtojyzcpsc.html

[U40] Py：打印到标准错误
来源：http://hz.jyoumei.cn/gtnhedxojl.html

print("err", file=sys.stderr)
来源：http://hz.cdnleiting.top/gtduebennq.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.gogol.net.cn/gtnzaysosb.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.zhixingplan.top/gteequfaad.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.daria6918.cn/gtgpqqjlsi.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.quarkkingdee.top/gtygdviytf.html

[U43] PHP：声明命名空间
来源：http://hz.gogol.net.cn/gtvozrfsyp.html

namespace App\Http;
来源：http://hz.redwolf501.top/gtvjxwianf.html

[U44] PHP：开启严格类型
来源：http://hz.hongshengwenyu.top/gtmaqdvyen.html

declare(strict_types=1);
来源：http://hz.redwolf501.top/gttbhawtox.html

[U45] PHP：类型声明与返回类型
来源：http://hz.zhiwuduotai.top/gtigcjmqlp.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yj20258.top/gtxebajpjh.html

[U46] PHP：可空类型
来源：http://hz.hywenlv.cn/gtjebkwrml.html

?string $name = null
来源：http://hz.gaohongyu789.top/gtdwfavcng.html

[U47] PHP：联合类型
来源：http://hz.havefunace.top/gtyyymzxaz.html

int|string $id
来源：http://hz.zhaomingkeji.xyz/gtslctrskw.html

[U48] PHP：纯枚举
来源：http://hz.yvedp.cn/gtuvqxhunu.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.fengsongda.top/gtincjdgmc.html

[U49] PHP：只读属性
来源：http://hz.tanke756.top/gtavwqqovy.html

public readonly string $name
来源：http://hz.yongpay.top/gtiwehflsn.html

[U50] PHP：构造器属性提升
来源：http://hz.kuanghao11.cn/gtixtuwsij.html

public function __construct(private int $id) {}
来源：http://hz.tian-w.cn/gtuqzngbdb.html

[U51] PHP：数组解构
来源：http://hz.daria6918.cn/gtvrimqiov.html

[$a, $b] = $arr;
来源：http://hz.hnqzz.top/gtjztamidv.html

[U52] PHP：箭头函数
来源：http://hz.shuidangran.top/gtwmypvnjp.html

$double = fn($x) => $x * 2;
来源：http://hz.yj20258.top/gtexlkifds.html

[U53] PHP：空合并运算符
来源：http://hz.hywenlv.cn/gtwdwgzrgj.html

$v = $a ?? $b ?? "default";
来源：http://hz.gotoacloud.top/gtliullowa.html

[U54] PHP：空安全调用
来源：http://hz.chenjidiqi.icu/gttvxertnf.html

$obj?->method()
来源：http://hz.vqdsnc.cn/gtqmlwlneo.html

[U55] PHP：match 表达式
来源：http://hz.hysaishi.cn/gtahenwavk.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.zhoulong.xyz/gtcrsykgmq.html

[U56] PHP：命名参数
来源：http://hz.jqgfzy.top/gtukjzdkva.html

f(a: 1, b: 2)
来源：http://hz.wangdashe.top/gtslnbufue.html

[U57] PHP：字符串插值
来源：http://hz.ivvv.top/gtaelqowoo.html

"值: {$a}"
来源：http://hz.jqgfzy.top/gtvpglwcfb.html

[U58] PHP：数组三件套
来源：http://hz.nanxinkj.top/gtpsknwxdx.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.gogol.net.cn/gtwtyqjjuc.html

[U59] PHP：自定义排序
来源：http://hz.hnxiangtu.top/gtrtaktdjm.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.bjfxy.top/gtsszdklbg.html

[U60] PHP：JSON 编解码
来源：http://hz.gogol.net.cn/gtvjlylzfm.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.zhijiandao.cn/gtvyrnaesm.html

[U61] PHP：正则
来源：http://hz.pengpengdd.cyou/gtrbdxxifi.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.guannengcc.top/gtmyhxcpmu.html

[U62] PHP：日期对象
来源：http://hz.hammf.cn/gtniguuvxf.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.shzxlz.cn/gtpcxjpiih.html

[U63] PHP：文件读写
来源：http://hz.ywan-chungtsiang.top/gtnbyskfuz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.yueranfly.top/gtrsfcqzgt.html

[U64] PHP：目录遍历
来源：http://hz.zdqjudy.top/gtvpojiqte.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.316326.xyz/gtibkhrnyh.html

[U65] PHP：会话
来源：http://hz.zhiwuduotai.top/gtxzislitk.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.gzhubu.top/gtqblitfnj.html

[U66] PHP：设置 Cookie
来源：http://hz.kuanghao11.cn/gtslxtlcqc.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.zhaomingkeji.xyz/gttsrrjdwy.html

[U67] PHP：处理文件上传
来源：http://hz.jinqigufen.top/gtmnmounzm.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.hywenlv.cn/gtxmlssnrj.html

[U68] PHP：PDO 连接
来源：http://hz.zhijiandao.cn/gtbntnebla.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.jinghuilouyu.cn/gtkavlymmx.html

[U69] PHP：PDO 预处理
来源：http://hz.cdnleiting.top/gtxmmnbkbm.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.jqgfzy.top/gtejypnmkn.html

[U70] PHP：PDO 事务
来源：http://hz.andypj.xyz/gtqzuafywt.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.haohaochexian.top/gtdybbmfyw.html

[U71] PHP：抛出异常
来源：http://hz.ydzc1.top/gtrwbhkttr.html

throw new RuntimeException("失败", 500);
来源：http://hz.jqgfzy.top/gtrbytsxgx.html

[U72] PHP：写错误日志
来源：http://hz.iojbl.cn/gtbwbckofq.html

error_log("失败: " . $e->getMessage());
来源：http://hz.9152youxi.cn/gtjvlndnbf.html

[U73] PHP：读取 ini 配置
来源：http://hz.jinqigfzy.top/gtvrpctsgw.html

parse_ini_file("config.ini", true)
来源：http://hz.yj20258888.top/gttbhlibel.html

[U74] PHP：读取环境变量
来源：http://hz.xingfuxueyuan.xyz/gteaovecqu.html

getenv("APP_ENV") ?: "production"
来源：http://hz.pengpengdd.cyou/gtraxapklt.html

[U75] PHP：依赖注入
来源：http://hz.ybcxt.top/gtfamodnqu.html

composer require psr/container
来源：http://hz.yuanzhike.top/gtlsntpnjp.html

[U76] PHP：简单路由
来源：http://hz.guannengcc.top/gtdjwyzcap.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.nanxuanxn.top/gtdyguambd.html

[U77] PHP：模板渲染
来源：http://hz.sufxvd.cn/gtrvvofggt.html

composer require twig/twig
来源：http://hz.sysykeji.top/gtkrdqatvw.html

[U78] PHP：单元测试
来源：http://hz.haohaochexian.top/gtrhwudamo.html

composer require --dev phpunit/phpunit
来源：http://hz.tanke756.top/gtbdziqvqg.html

[U79] PHP：静态分析
来源：http://hz.yongpay.top/gtmzqxakgi.html

composer require --dev phpstan/phpstan
来源：http://hz.ywan-chungtsiang.top/gtwupnxgff.html

[U80] PHP：代码规范修复
来源：http://hz.shzxlz.cn/gtouifhchf.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.ppjwa.cn/gtxikoastm.html

[U81] JS：初始化项目
来源：http://hz.nanxuanxn.top/gtuczsdsco.html

npm init -y;  npm i express
来源：http://hz.andypj.xyz/gtwszjpexy.html

[U82] JS：package.json 脚本
来源：http://hz.shangyingyoupin.top/gtvxenwgre.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.fengsongda.top/gtfhfhlwds.html

[U83] JS：ES Module 导入导出
来源：http://hz.xylfe.cn/gtempnawpr.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.hammf.cn/gtyuzypbbo.html

[U84] JS：CommonJS 写法
来源：http://hz.nwbrower.top/gtodpjhgxe.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.cheryme.top/gtzzjsjkxf.html

[U85] JS：可选链
来源：http://hz.jianghu66.top/gtehxjamdj.html

a?.b?.c
来源：http://hz.shanyushiyangkeji.top/gtoxdrlyhz.html

[U86] JS：空值合并
来源：http://hz.yj20258.top/gtqbpephoo.html

a ?? b
来源：http://hz.316326.xyz/gtyuuoqezw.html

[U87] JS：解构默认值
来源：http://hz.hfpthk.cn/gtszonsxhv.html

const { a = 1, b = 2 } = obj;
来源：http://hz.bjfxy.top/gthleoiuql.html

[U88] JS：对象展开合并
来源：http://hz.chenjidiqi.icu/gtwlypesfw.html

{ ...a, ...b }
来源：http://hz.xylfe.cn/gtxgqmszgh.html

[U89] JS：数组去重
来源：http://hz.xuanzx.com/gtebrolwnf.html

[...new Set(arr)]
来源：http://hz.hongshengwenyu.top/gtdykyarvl.html

[U90] JS：数字数组排序
来源：http://hz.svipenyu.cn/gtispqertq.html

[...arr].sort((a, b) => a - b)
来源：http://hz.zhengqikj.top/gtufydhcar.html

[U91] JS：对象键值遍历
来源：http://hz.316326.xyz/gtkpdhvwut.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.zhaomingkeji.xyz/gtjmyukocy.html

[U92] JS：深拷贝
来源：http://hz.hnxiangtu.top/gtvsisnaiq.html

structuredClone(obj)
来源：http://hz.zhijiandao.cn/gtroenwpav.html

[U93] JS：模板字符串
来源：http://hz.chenjidiqi.icu/gtmruosxpi.html

`共 ${n} 条`
来源：http://hz.yonumen.top/gtvcrsxgwh.html

[U94] JS：箭头函数
来源：http://hz.iojbl.cn/gtdrbhiyyu.html

const double = x => x * 2;
来源：http://hz.shzxlz.cn/gtbzpzdpjl.html

[U95] JS：Promise 包装
来源：http://hz.ehwqpu.com/gtjcpglcey.html

new Promise((resolve, reject) => {})
来源：http://hz.xziqi.cn/gttfmzopjd.html

[U96] JS：async/await 与异常
来源：http://hz.aibaodan.cn/gtqzibtyro.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.zhixingplan.top/gtayynxwjf.html

[U97] JS：并发请求
来源：http://hz.ivvv.top/gtlktaomyh.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yvedp.cn/gtdbcqkftx.html

[U98] JS：fetch 带 JSON
来源：http://hz.xingfuxueyuan.xyz/gtrekoucwx.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.tian-w.cn/gtdqvfefiw.html

[U99] JS：事件监听
来源：http://hz.ppjwa.cn/gtcmynwviv.html

el.addEventListener("click", e => {})
来源：http://hz.nanxuanxn.top/gtkdysanpl.html

[U100] JS：DOM 查询
来源：http://hz.chenjidiqi.icu/gtpwduastg.html

document.querySelector(".item")
来源：http://hz.fengsongda.top/gtuazzuknx.html

[U101] JS：classList 操作
来源：http://hz.sweek.top/gtmmcvonzp.html

el.classList.toggle("active")
来源：http://hz.ybcxt.top/gtrssfmydz.html

[U102] JS：本地存储
来源：http://hz.ybcxt.top/gtfdtnqqhz.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.quarkkingdee.top/gtwsgfwqhv.html

[U103] JS：定时器
来源：http://hz.xziqi.cn/gtrmaarphz.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.guannengcc.top/gtuvjvpvsl.html

[U104] JS：防抖
来源：http://hz.gotoacloud.top/gtmlcdqwwl.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhoulong.xyz/gtlzjwkhuv.html

[U105] JS：节流
来源：http://hz.birdmap.top/gtlsqgyntl.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.chenlongwang.top/gthdgaznlq.html

[U106] JS：日期格式化
来源：http://hz.pycfn.com/gtmoaqkmim.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.wangshuangyany.cn/gtitisrzbm.html

[U107] JS：数字千分位
来源：http://hz.yj20258888.top/gtxeydrbpj.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.chenlongwang.top/gthxjwbyia.html

[U108] JS：随机整数
来源：http://hz.guowangkeji.top/gtebprmtzw.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.shanyushiyangkeji.top/gtvcuruqgy.html

[U109] JS：数组分组
来源：http://hz.birdmap.top/gtnyapizib.html

Object.groupBy(arr, x => x.type)
来源：http://hz.xylfe.cn/gtlyhjuxxg.html

[U110] JS：数组分块
来源：http://hz.aizwys.cn/gtsfzrnkcu.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.yuanzhike.top/gtsgdygede.html

[U111] JS：对象转 Map
来源：http://hz.bjfxy.top/gtrnudgnza.html

new Map(Object.entries(obj))
来源：http://hz.smart0.xyz/gtmvkqbpbl.html

[U112] JS：字符串补位
来源：http://hz.nwbrower.top/gtelddvidn.html

"7".padStart(3, "0")
来源：http://hz.wangshuangyany.cn/gtggvjkomu.html

[U113] JS：正则替换全部
来源：http://hz.xinyue.icu/gteiefssoe.html

s.replaceAll("a", "b")
来源：http://hz.havefunace.top/gtcaujgjod.html

[U114] JS：JSON 深比较
来源：http://hz.nanxinkj.top/gtzbfylktd.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.316326.xyz/gtprqjnduv.html

[U115] JS：生成 UUID
来源：http://hz.guowangkeji.top/gtngesjjdt.html

crypto.randomUUID()
来源：http://hz.sufxvd.cn/gthhhzmvjv.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.quarkkingdee.top/gtoflhezif.html

/** @param {string} name */ function f(name) {}
来源：http://hz.ydjk.org.cn/gtkziidkiz.html

[U117] JS：单元测试
来源：http://hz.nanxuanxn.top/gtyrmhrdwj.html

npm i -D vitest;  npx vitest
来源：http://hz.ydzc1.top/gtdsgsvbck.html

[U118] JS：开发服务器
来源：http://hz.jqgufenzy.top/gthvyeziur.html

npm i -D vite;  npx vite
来源：http://hz.haohaochexian.top/gtuaznxwae.html

[U119] JS：生产构建
来源：http://hz.cheryme.top/gtaciiywxb.html

npx vite build
来源：http://hz.gotoacloud.top/gthqentyks.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.ydjk.org.cn/gtpzuqvcjv.html

import.meta.env.VITE_API_URL
来源：http://hz.shzxlz.cn/gtbxtvafxs.html

================================================================================
来源：http://hz.jqgufenzy.top/gtadpaoaub.html

统计汇总
来源：http://hz.shzxlz.cn/gtsfowzbay.html

================================================================================
来源：http://hz.sufxvd.cn/gtrtscoovs.html

按语言统计（条）：
来源：http://hz.yonumen.top/gtxhdppzlk.html

Python ......... 252
来源：http://hz.0kj1m.cn/gthcbpvalu.html

PHP ............ 252
来源：http://hz.jinqigfzy.top/gttnqesscs.html

JavaScript ..... 252
来源：http://hz.andypj.xyz/gtndipjfxm.html

TypeScript ..... 212
来源：http://hz.xinyue.icu/gtyqspknxs.html

Java ........... 212
来源：http://hz.zhongyouzk.top/gtmitmjgnf.html

Go ............. 212
来源：http://hz.ydzc1.top/gtgurvdmye.html

Ruby ........... 212
来源：http://hz.nwbrower.top/gtkzkyaobt.html

C# ............. 212
来源：http://hz.shzxlz.cn/gtknryeods.html

C .............. 30
来源：http://hz.hysaishi.cn/gtrjtjvzio.html

C++ ............ 30
来源：http://hz.sufxvd.cn/gtflqapaet.html

SQL ............ 90
来源：http://hz.chenzaomai.com/gtuqvvvwha.html

Bash ........... 80
来源：http://hz.daxiang520.top/gtmjdwirpy.html

Kotlin ......... 15
来源：http://hz.xylfe.cn/gtggyodmdc.html

Swift .......... 15
来源：http://hz.dashuyun.cn/gtxpjacgzc.html

Lua ............ 10
来源：http://hz.guowangkeji.top/gtlvgtmqyf.html

Perl ........... 10
来源：http://hz.fengsongda.top/gtofpgxwle.html

Scala .......... 10
来源：http://hz.cashguo.top/gtwmbgwzrf.html

------------------------------------
来源：http://hz.zhoulong.xyz/gtjawyuolj.html

合计 ........... 2106 条
来源：http://hz.wangdashe.top/gtxfjltkpb.html

按章节统计：
来源：http://hz.cdnleiting.top/gtongnhzlw.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.iojbl.cn/gthlxpbiro.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.xuanzx.com/gteucdziqk.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.fzhhl.top/gtpxarbyse.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.ybcxt.top/gtiqvrrxee.html


<!-- 参考信息 -->