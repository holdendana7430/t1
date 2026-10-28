代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://hz.tanke756.top/gttjwkymze.html

[T51] Scala：Hello World
来源：http://hz.dashuyun.cn/gtwcwpqyjk.html

println("Hello")
来源：http://hz.hywenlv.cn/gtjvbhdrtm.html

[T52] Scala：变量
来源：http://hz.yj20258888.top/gtgvxigqqx.html

val a = 1;  var b = 2
来源：http://hz.shanyushiyangtech.top/gtawknfztu.html

[T53] Scala：字符串插值
来源：http://hz.ydjk.org.cn/gtibkkyyvx.html

s"值: $b"
来源：http://hz.iojbl.cn/gtywapeebw.html

[T54] Scala：集合映射
来源：http://hz.bjfxy.top/gtwrpwozmv.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.c1oappe.top/gtnfkzeemr.html

[T55] Scala：集合过滤
来源：http://hz.gaohongyu789.top/gtaozrkimg.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.daria6918.cn/gtrdnrkdnm.html

[T56] Scala：样例类
来源：http://hz.gzhubu.top/gtuxvgryhd.html

case class User(name: String, age: Int)
来源：http://hz.yvedp.cn/gtrjyrlchw.html

[T57] Scala：模式匹配
来源：http://hz.nanxinkj.top/gtlroqljwh.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.sweek.top/gtmtzgeoas.html

[T58] Scala：函数定义
来源：http://hz.xylfe.cn/gtjekuidhz.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.yangfankeji.com/gtbavpzrfn.html

[T59] Scala：循环
来源：http://hz.mhx1999.top/gtbhripxbr.html

for (i <- 1 to 10) println(i)
来源：http://hz.andypj.xyz/gtbpcohsik.html

[T60] Scala：折叠
来源：http://hz.guowangkeji.top/gtdgnfcpfb.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.snrcjt.cn/gtaxfebwfd.html

================================================================================
来源：http://hz.yuanzhike.top/gtyadiwaqe.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.jqgfzy.top/gtuclgppbw.html

================================================================================
来源：http://hz.jqgfzy.top/gtmgmhvmld.html

[U01] Py：创建虚拟环境
来源：http://hz.ybcxt.top/gtftstovvf.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.yongpay.top/gtafbpykoe.html

[U02] Py：导出 / 安装依赖
来源：http://hz.jinyuanbaomall.cn/gtgaxckvwb.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.feifeiyinyue.top/gtotukxugv.html

[U03] Py：加载 .env 配置
来源：http://hz.pycfn.com/gtoxraqlvg.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.cqqwz.cn/gtunaakrqr.html

[U04] Py：变量调试打印
来源：http://hz.chenzaomai.com/gtqbsxsgtk.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.yongpay.top/gtpxlzetws.html

[U05] Py：列表去重且保序
来源：http://hz.fengsongda.top/gtmkomsduk.html

list(dict.fromkeys(arr))
来源：http://hz.yj20258888.top/gtgwzqrasb.html

[U06] Py：合并两个字典
来源：http://hz.hfpthk.cn/gtakfcztdt.html

{**a, **b}
来源：http://hz.cqqwz.cn/gtmnocknvt.html

[U07] Py：反转字典键值
来源：http://hz.xingfuxueyuan.xyz/gtfjcdffnc.html

{v: k for k, v in d.items()}
来源：http://hz.zhixingplan.top/gtojfiiqty.html

[U08] Py：展平二维列表
来源：http://hz.jiagoushi.top/gtaosnqsyy.html

[y for x in nested for y in x]
来源：http://hz.haohaochexian.top/gtjjfqnrgx.html

[U09] Py：字典取最大值的键
来源：http://hz.vqdsnc.cn/gtgunrcqjb.html

max(d, key=d.get)
来源：http://hz.zycfv.cn/gthyjalwlc.html

[U10] Py：按值排序字典
来源：http://hz.ydzc1.top/gtdazeepcm.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.jinyuanbaomall.cn/gtvgxerjfm.html

[U11] Py：生成器表达式
来源：http://hz.jqgfzy.top/gtdiuysuoh.html

(x * 2 for x in arr)
来源：http://hz.chenzaomai.com/gtdhumoktt.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.jlsjyb.cn/gtpxvdhvpq.html

Counter(arr).most_common(3)
来源：http://hz.zhijiandao.cn/gtwjdrfnvl.html

[U13] Py：固定长度队列
来源：http://hz.zhaomingkeji.xyz/gtdjljjscj.html

deque(maxlen=10)
来源：http://hz.nanxinkj.top/gtoffyjykz.html

[U14] Py：分组收集到列表
来源：http://hz.quarkkingdee.top/gthurgxfxb.html

defaultdict(list)
来源：http://hz.sufxvd.cn/gtklhwsiap.html

[U15] Py：高精度计时
来源：http://hz.snrcjt.cn/gtfftfiqng.html

t = time.perf_counter()
来源：http://hz.shanyushiyangtech.top/gthkadgmbh.html

[U16] Py：命令行参数解析
来源：http://hz.hysaishi.cn/gttqcgmmeg.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.shuidangran.top/gtggxkvymx.html

[U17] Py：初始化日志
来源：http://hz.jinghuilouyu.cn/gtgyjznhzo.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.ydjk.org.cn/gtdmmztyaf.html

[U18] Py：预编译正则
来源：http://hz.ywan-chungtsiang.top/gtdwfvojkw.html

pat = re.compile(r"\d+")
来源：http://hz.yueranfly.top/gtycrrhvaw.html

[U19] Py：正则替换带回调
来源：http://hz.shangyingyoupin.top/gtiszftsmw.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.dashuyun.cn/gtbtxmnjzr.html

[U20] Py：缓存函数结果
来源：http://hz.guannengcc.top/gtbmekintr.html

@functools.lru_cache(maxsize=None)
来源：http://hz.gaohongyu789.top/gtitttiapw.html

[U21] Py：自定义上下文管理器
来源：http://hz.ydjk.org.cn/gtxlhyliak.html

@contextlib.contextmanager
来源：http://hz.zhongyouzk.top/gtffgtrfei.html

[U22] Py：矩阵转置
来源：http://hz.shuidangran.top/gtzheeywpq.html

list(zip(*m))
来源：http://hz.cucudq.cn/gtpexhqocq.html

[U23] Py：分块读取大文件
来源：http://hz.cashguo.top/gtnqxfvsxp.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.pycfn.com/gtctqsetxh.html

[U24] Py：路径操作
来源：http://hz.ydzc1.top/gtzcgpgvwr.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.shzxlz.cn/gtvudekqzo.html

[U25] Py：CSV 按字典读
来源：http://hz.shangyingyoupin.top/gtuxkciisw.html

csv.DictReader(f)
来源：http://hz.shanyushiyangkeji.top/gtinzrathx.html

[U26] Py：并发下载
来源：http://hz.shanyushiyangkeji.top/gtyydkcozb.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.shangyingyoupin.top/gtjskvwtdn.html

[U27] Py：异步 HTTP
来源：http://hz.ivvv.top/gtdceqechc.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.gzhubu.top/gtzfandzeo.html

[U28] Py：类型别名
来源：http://hz.c1oappe.top/gtslmyhjyw.html

UserId = int
来源：http://hz.hysaishi.cn/gtknpxtzzl.html

[U29] Py：属性校验
来源：http://hz.xziqi.cn/gtoymlprly.html

@property 与 @x.setter 配合
来源：http://hz.jqgufenzy.top/gtcpkngfoq.html

[U30] Py：数据类
来源：http://hz.hnxiangtu.top/gtyonalutj.html

@dataclass(slots=True)
来源：http://hz.jinqigufen.top/gtkkcliqno.html

[U31] Py：单测
来源：http://hz.jianghu66.top/gtnolzmxvy.html

python -m pytest -q
来源：http://hz.feifeiyinyue.top/gtuwlhrvpg.html

[U32] Py：代码格式化
来源：http://hz.52xcode.cn/gttixekjaw.html

ruff format . && ruff check --fix .
来源：http://hz.cashguo.top/gtxaefwbgd.html

[U33] Py：打包发布
来源：http://hz.sxryk.cn/gtwvckguhl.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.xinyue.icu/gtbolsvesy.html

[U34] Py：判断编码
来源：http://hz.hnqzz.top/gtjzbhnqto.html

chardet.detect(raw)
来源：http://hz.fengsongda.top/gtmqohford.html

[U35] Py：发送邮件
来源：http://hz.jyoumei.cn/gtdwmzrhdt.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.xinyue.icu/gthdxjwbcb.html

[U36] Py：定时任务
来源：http://hz.zhengqikj.top/gtoypyyxaa.html

schedule.every(10).minutes.do(job)
来源：http://hz.shzxlz.cn/gtfibhuakt.html

[U37] Py：读写 Excel
来源：http://hz.aizwys.cn/gtdprxykbq.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.havefunace.top/gtbslngsxn.html

[U38] Py：获取脚本所在目录
来源：http://hz.zhongyouzk.top/gtgbbwnsko.html

Path(__file__).resolve().parent
来源：http://hz.nanxinkj.top/gtkkvdtypf.html

[U39] Py：判断是否在交互环境
来源：http://hz.sxryk.cn/gtumwqcmvl.html

sys.stdout.isatty()
来源：http://hz.xinyue.icu/gtjxvribla.html

[U40] Py：打印到标准错误
来源：http://hz.hammf.cn/gtwrgscmqs.html

print("err", file=sys.stderr)
来源：http://hz.yanxiufei.cn/gtrmwwxebu.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.yj20258.top/gtbuqxjhjm.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.cashguo.top/gtspjhqdcp.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.bjfxy.top/gtolyprkeg.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.zhixingplan.top/gtpjwncqlq.html

[U43] PHP：声明命名空间
来源：http://hz.jinyuanbaomall.cn/gtvethfxjg.html

namespace App\Http;
来源：http://hz.ppjwa.cn/gtemzqxmcw.html

[U44] PHP：开启严格类型
来源：http://hz.cheryme.top/gtwdsjbaop.html

declare(strict_types=1);
来源：http://hz.jqgfzy.top/gtpeyqzsor.html

[U45] PHP：类型声明与返回类型
来源：http://hz.chenlongwang.top/gtfungusuw.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.vqdsnc.cn/gtgyjjszdy.html

[U46] PHP：可空类型
来源：http://hz.cashguo.top/gtayasmtit.html

?string $name = null
来源：http://hz.zhixingplan.top/gtxetycwcj.html

[U47] PHP：联合类型
来源：http://hz.ehwqpu.com/gtfehwojte.html

int|string $id
来源：http://hz.hnqzz.top/gtnorgstqx.html

[U48] PHP：纯枚举
来源：http://hz.hywenlv.cn/gtliglyxgs.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.zycfv.cn/gtbsmitgkm.html

[U49] PHP：只读属性
来源：http://hz.jinqigfzy.top/gtuzkdspvz.html

public readonly string $name
来源：http://hz.hongshengwenyu.top/gtkvvjozww.html

[U50] PHP：构造器属性提升
来源：http://hz.hfpthk.cn/gtxpofhkqm.html

public function __construct(private int $id) {}
来源：http://hz.zhaomingkeji.xyz/gtlvtpfqzw.html

[U51] PHP：数组解构
来源：http://hz.ivvv.top/gtlfjawxkz.html

[$a, $b] = $arr;
来源：http://hz.gotoacloud.top/gtabsnenjr.html

[U52] PHP：箭头函数
来源：http://hz.chenjidiqi.icu/gtwjzgypnl.html

$double = fn($x) => $x * 2;
来源：http://hz.zycfv.cn/gtwxqfwrhu.html

[U53] PHP：空合并运算符
来源：http://hz.ppjwa.cn/gtxnktofyc.html

$v = $a ?? $b ?? "default";
来源：http://hz.yj20258.top/gtfgxpawty.html

[U54] PHP：空安全调用
来源：http://hz.jiagoushi.top/gtvbufqoau.html

$obj?->method()
来源：http://hz.gzhubu.top/gtegwnwfvt.html

[U55] PHP：match 表达式
来源：http://hz.svipenyu.cn/gtwcvvkhsz.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.cashguo.top/gtfuaeqbwk.html

[U56] PHP：命名参数
来源：http://hz.tianlin.xyz/gtwetxalfe.html

f(a: 1, b: 2)
来源：http://hz.smart0.xyz/gtszycjwef.html

[U57] PHP：字符串插值
来源：http://hz.haohaochexian.top/gtrzxqfatc.html

"值: {$a}"
来源：http://hz.wangdashe.top/gtlwzcreyc.html

[U58] PHP：数组三件套
来源：http://hz.yvedp.cn/gtjpjxdzdv.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.jiagoushi.top/gtskgeixet.html

[U59] PHP：自定义排序
来源：http://hz.jiagoushi.top/gtabmbltae.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.bjfxy.top/gtgdxzwdjq.html

[U60] PHP：JSON 编解码
来源：http://hz.redwolf501.top/gteicbvvwq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.gzhubu.top/gtrviwxunq.html

[U61] PHP：正则
来源：http://hz.guowangkeji.top/gtwwdwfpct.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.dashuyun.cn/gtmouqoihq.html

[U62] PHP：日期对象
来源：http://hz.yvedp.cn/gtzoecirga.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.birdmap.top/gtacbroluh.html

[U63] PHP：文件读写
来源：http://hz.ppjwa.cn/gtixnthbyo.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.dianchejie.cn/gtnnoqpprq.html

[U64] PHP：目录遍历
来源：http://hz.ydzc1.top/gtbpljpcfb.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.zhijiandao.cn/gtozrojllw.html

[U65] PHP：会话
来源：http://hz.yj202588.top/gtievjsyvq.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.yj20258.top/gttutbltpa.html

[U66] PHP：设置 Cookie
来源：http://hz.xziqi.cn/gtrasxuakc.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.jlsjyb.cn/gttjojrtxt.html

[U67] PHP：处理文件上传
来源：http://hz.havefunace.top/gtafzkyafz.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.feifeiyinyue.top/gttfwkxusx.html

[U68] PHP：PDO 连接
来源：http://hz.xuetiantiany.cn/gtegsmnovt.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.zhixingplan.top/gtvxvnzpif.html

[U69] PHP：PDO 预处理
来源：http://hz.guannengcc.top/gtsffpphay.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.hnqzz.top/gtcypducqe.html

[U70] PHP：PDO 事务
来源：http://hz.ydjk.org.cn/gtpekggkwn.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.yueranfly.top/gtljdpbmae.html

[U71] PHP：抛出异常
来源：http://hz.nanxinkj.top/gtxwibymzt.html

throw new RuntimeException("失败", 500);
来源：http://hz.nanxinkj.top/gtxpifyvlz.html

[U72] PHP：写错误日志
来源：http://hz.yj20258888.top/gtsadakwiv.html

error_log("失败: " . $e->getMessage());
来源：http://hz.hammf.cn/gtzwliewzi.html

[U73] PHP：读取 ini 配置
来源：http://hz.zhoulong.xyz/gtwsexzuvy.html

parse_ini_file("config.ini", true)
来源：http://hz.yj20258.top/gtaxtitckk.html

[U74] PHP：读取环境变量
来源：http://hz.redwolf501.top/gtfvlxvszp.html

getenv("APP_ENV") ?: "production"
来源：http://hz.jyoumei.cn/gtrrlrkeqc.html

[U75] PHP：依赖注入
来源：http://hz.zhijiandao.cn/gttikqtymh.html

composer require psr/container
来源：http://hz.hnqzz.top/gtinxcefrm.html

[U76] PHP：简单路由
来源：http://hz.shanyushiyangtech.top/gtgcifziua.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.hysaishi.cn/gtuaqpnpsd.html

[U77] PHP：模板渲染
来源：http://hz.xuanzx.com/gtykylhulv.html

composer require twig/twig
来源：http://hz.cheryme.top/gtmlrritol.html

[U78] PHP：单元测试
来源：http://hz.havefunace.top/gtcbokiknv.html

composer require --dev phpunit/phpunit
来源：http://hz.aizwys.cn/gtjwjoahhd.html

[U79] PHP：静态分析
来源：http://hz.tian-w.cn/gtofzphvsd.html

composer require --dev phpstan/phpstan
来源：http://hz.zhiwuduotai.top/gtwdyctade.html

[U80] PHP：代码规范修复
来源：http://hz.xingfuxueyuan.xyz/gthvocvwmx.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.havefunace.top/gtezdwdiqu.html

[U81] JS：初始化项目
来源：http://hz.aibaodan.cn/gtumxfhyma.html

npm init -y;  npm i express
来源：http://hz.daria6918.cn/gtfftwfgpu.html

[U82] JS：package.json 脚本
来源：http://hz.kuanghao11.cn/gtxcwevnbn.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.nanxuanxn.top/gtqdjzkxhq.html

[U83] JS：ES Module 导入导出
来源：http://hz.vqdsnc.cn/gtrmhbmlet.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.meibo888.top/gtoqalkcgx.html

[U84] JS：CommonJS 写法
来源：http://hz.jyoumei.cn/gthhyexwob.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.chenzaomai.com/gthzfigjph.html

[U85] JS：可选链
来源：http://hz.yonumen.top/gtzuwdycju.html

a?.b?.c
来源：http://hz.cucudq.cn/gtewloabwa.html

[U86] JS：空值合并
来源：http://hz.zhixingplan.top/gtgmglvjvu.html

a ?? b
来源：http://hz.zhiwuduotai.top/gttcufxvzr.html

[U87] JS：解构默认值
来源：http://hz.cheryme.top/gthuqsxgmv.html

const { a = 1, b = 2 } = obj;
来源：http://hz.hfpthk.cn/gtufphwijr.html

[U88] JS：对象展开合并
来源：http://hz.jinyuanbaomall.cn/gtyfewqjxw.html

{ ...a, ...b }
来源：http://hz.nanxinkj.top/gtaflaqdwm.html

[U89] JS：数组去重
来源：http://hz.zhiwuduotai.top/gtzmcgryjn.html

[...new Set(arr)]
来源：http://hz.snrcjt.cn/gtymtvtigm.html

[U90] JS：数字数组排序
来源：http://hz.guannengcc.top/gtxcvbodwc.html

[...arr].sort((a, b) => a - b)
来源：http://hz.jqgfzy.top/gtlovtlhzy.html

[U91] JS：对象键值遍历
来源：http://hz.yj20258.top/gttxbwwksh.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.ydjk.org.cn/gtfyhblbke.html

[U92] JS：深拷贝
来源：http://hz.bjfxy.top/gttzvvymic.html

structuredClone(obj)
来源：http://hz.vqdsnc.cn/gtommxtxsb.html

[U93] JS：模板字符串
来源：http://hz.tian-w.cn/gtxhovtfgu.html

`共 ${n} 条`
来源：http://hz.cdnleiting.top/gtywyuwily.html

[U94] JS：箭头函数
来源：http://hz.ivvv.top/gtmmutbjzy.html

const double = x => x * 2;
来源：http://hz.yongpay.top/gtwxehhhjr.html

[U95] JS：Promise 包装
来源：http://hz.nanxuanxn.top/gtgzletvms.html

new Promise((resolve, reject) => {})
来源：http://hz.jinghuilouyu.cn/gteympdcux.html

[U96] JS：async/await 与异常
来源：http://hz.sxryk.cn/gtlxymdimn.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.ydzc1.top/gtqsrqcxoq.html

[U97] JS：并发请求
来源：http://hz.tianlin.xyz/gtrbvvtitq.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shanyushiyangtech.top/gtaytbzwsj.html

[U98] JS：fetch 带 JSON
来源：http://hz.gzhubu.top/gtwjxrxnjd.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.jlsjyb.cn/gtcyeqmsmr.html

[U99] JS：事件监听
来源：http://hz.aizwys.cn/gtzhrdzezb.html

el.addEventListener("click", e => {})
来源：http://hz.guowangkeji.top/gtstpcorhk.html

[U100] JS：DOM 查询
来源：http://hz.guannengcc.top/gtlrpyjhev.html

document.querySelector(".item")
来源：http://hz.nanxinkj.top/gteaeyfcsw.html

[U101] JS：classList 操作
来源：http://hz.daria6918.cn/gtsdcqtoay.html

el.classList.toggle("active")
来源：http://hz.yongpay.top/gtbomcgjoi.html

[U102] JS：本地存储
来源：http://hz.cucudq.cn/gtfdvoghbn.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.nanxinkj.top/gtldlpiafn.html

[U103] JS：定时器
来源：http://hz.c1oappe.top/gtzirgzxmq.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.yj202588.top/gtlnuzxsom.html

[U104] JS：防抖
来源：http://hz.shanyushiyangtech.top/gtcrkkgvnd.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yj20258888.top/gtkausnmrl.html

[U105] JS：节流
来源：http://hz.shanyushiyangkeji.top/gtcojqvlmp.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.yangfankeji.com/gtjnchrcld.html

[U106] JS：日期格式化
来源：http://hz.sxryk.cn/gtasueqdbc.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.havefunace.top/gtlpcgkgpb.html

[U107] JS：数字千分位
来源：http://hz.aizwys.cn/gtcxwiuwem.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.smart0.xyz/gtgljglelm.html

[U108] JS：随机整数
来源：http://hz.tian-w.cn/gtzxcdrelp.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.tian-w.cn/gtphckgpsm.html

[U109] JS：数组分组
来源：http://hz.ppjwa.cn/gtuwvdssod.html

Object.groupBy(arr, x => x.type)
来源：http://hz.xuanzx.com/gtyionrjqy.html

[U110] JS：数组分块
来源：http://hz.jyoumei.cn/gtrssrvhdv.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.nanxuanxn.top/gtxvnbixps.html

[U111] JS：对象转 Map
来源：http://hz.yj20258.top/gtizivgjwh.html

new Map(Object.entries(obj))
来源：http://hz.chenjidiqi.icu/gtysqpezyb.html

[U112] JS：字符串补位
来源：http://hz.dianchejie.cn/gtglzhccfu.html

"7".padStart(3, "0")
来源：http://hz.yvedp.cn/gtbinllizp.html

[U113] JS：正则替换全部
来源：http://hz.xuanzx.com/gtqftgkuda.html

s.replaceAll("a", "b")
来源：http://hz.meibo888.top/gtzngkyrir.html

[U114] JS：JSON 深比较
来源：http://hz.jinghuilouyu.cn/gtpyrwspsq.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yj20258.top/gtvfusluhq.html

[U115] JS：生成 UUID
来源：http://hz.redwolf501.top/gtkdhpgxbs.html

crypto.randomUUID()
来源：http://hz.xylfe.cn/gteboymwor.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.hnqzz.top/gtryqkrblj.html

/** @param {string} name */ function f(name) {}
来源：http://hz.zhiwuduotai.top/gtvnicjaem.html

[U117] JS：单元测试
来源：http://hz.pycfn.com/gtrtaljtra.html

npm i -D vitest;  npx vitest
来源：http://hz.zhoulong.xyz/gttmpljgdr.html

[U118] JS：开发服务器
来源：http://hz.ppjwa.cn/gtlegvmwtt.html

npm i -D vite;  npx vite
来源：http://hz.zycfv.cn/gtappzbsfp.html

[U119] JS：生产构建
来源：http://hz.jianghu66.top/gtqdlfmzsd.html

npx vite build
来源：http://hz.aizwys.cn/gtpgxwoswc.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.shanyushiyangkeji.top/gtkqrewzhp.html

import.meta.env.VITE_API_URL
来源：http://hz.yj20258.top/gtvdfcgwbu.html

================================================================================
来源：http://hz.xziqi.cn/gtiqfvkiyk.html

统计汇总
来源：http://hz.52xcode.cn/gtuuqsdmli.html

================================================================================
来源：http://hz.sxryk.cn/gtfnwqxgvr.html

按语言统计（条）：
来源：http://hz.meibo888.top/gtukvrfopm.html

Python ......... 252
来源：http://hz.sxryk.cn/gtaqjokydf.html

PHP ............ 252
来源：http://hz.meibo888.top/gtqxhzodsd.html

JavaScript ..... 252
来源：http://hz.hnxiangtu.top/gttoachwku.html

TypeScript ..... 212
来源：http://hz.sufxvd.cn/gtqvnljfhf.html

Java ........... 212
来源：http://hz.bjfxy.top/gtnsdwpvge.html

Go ............. 212
来源：http://hz.xuetiantiany.cn/gtgezqvelj.html

Ruby ........... 212
来源：http://hz.52xcode.cn/gtggiarwwm.html

C# ............. 212
来源：http://hz.aizwys.cn/gteymcidaf.html

C .............. 30
来源：http://hz.ehwqpu.com/gtehtgklav.html

C++ ............ 30
来源：http://hz.shanyushiyangkeji.top/gtnehbcnxv.html

SQL ............ 90
来源：http://hz.sweek.top/gtewdpnlex.html

Bash ........... 80
来源：http://hz.chenjidiqi.icu/gthtsameas.html

Kotlin ......... 15
来源：http://hz.aizwys.cn/gtorekyjnf.html

Swift .......... 15
来源：http://hz.52xcode.cn/gtxyxrawxn.html

Lua ............ 10
来源：http://hz.chenzaomai.com/gtdxdktqmo.html

Perl ........... 10
来源：http://hz.hysaishi.cn/gtfhityuea.html

Scala .......... 10
来源：http://hz.tian-w.cn/gtzufrllji.html

------------------------------------
来源：http://hz.yangfankeji.com/gtxhmncgud.html

合计 ........... 2106 条
来源：http://hz.0kj1m.cn/gttmqvjkqi.html

按章节统计：
来源：http://hz.iojbl.cn/gtesjaudmo.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.gotoacloud.top/gtkxuhhldh.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.shanyushiyangkeji.top/gtqtkgpdcz.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.chenlongwang.top/gtekbsqcba.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.cqqwz.cn/gtrvsslacc.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.feifeiyinyue.top/gtemtbbtyp.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.nwbrower.top/gtbddzgyrc.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.andypj.xyz/gtdbkawfch.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.cqqwz.cn/gtpmimqski.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.cashguo.top/gtyqxttcse.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.shanyushiyangtech.top/gtteepfawb.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.gotoacloud.top/gtksoulyqq.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.zdqjudy.top/gtujsytfpf.html


<!-- 参考信息 -->