代发 wailian999

[T47] Perl：正则捕获
来源：http://hz.ehwqpu.com/gtxfrdugii.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.fengsongda.top/gthyivuhot.html

[T48] Perl：正则替换
来源：http://hz.shangyingyoupin.top/gtdisqhkeh.html

$s =~ s/old/new/g;
来源：http://hz.shanyushiyangtech.top/gtrmzpeana.html

[T49] Perl：函数
来源：http://hz.ivvv.top/gtfgeinjhc.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.jinqigfzy.top/gtzpokeeao.html

[T50] Perl：逐行读文件
来源：http://hz.meibo888.top/gtoquyhttk.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.jinyuanbaomall.cn/gtxihfsqvj.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.zdqjudy.top/gtjhduxhbu.html

[T51] Scala：Hello World
来源：http://hz.zhoulong.xyz/gtwjkxlbga.html

println("Hello")
来源：http://hz.pengpengdd.cyou/gtojmamvxj.html

[T52] Scala：变量
来源：http://hz.ivvv.top/gtxaismdee.html

val a = 1;  var b = 2
来源：http://hz.svipenyu.cn/gttnssvtaw.html

[T53] Scala：字符串插值
来源：http://hz.pengpengdd.cyou/gtpzaftgag.html

s"值: $b"
来源：http://hz.cdnleiting.top/gtexjnafcn.html

[T54] Scala：集合映射
来源：http://hz.zhongyouzk.top/gtvmbqikpn.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.smart0.xyz/gtakdemzgf.html

[T55] Scala：集合过滤
来源：http://hz.yuxming.cn/gtpdgmswlv.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.aibaodan.cn/gtgsnhbhtm.html

[T56] Scala：样例类
来源：http://hz.gzhubu.top/gteehnadkh.html

case class User(name: String, age: Int)
来源：http://hz.hammf.cn/gtssjqeudv.html

[T57] Scala：模式匹配
来源：http://hz.ivvv.top/gtibqfunkq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.yj202588.top/gtbxyvtezo.html

[T58] Scala：函数定义
来源：http://hz.jinqigfzy.top/gtzfgxkggn.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.ybcxt.top/gtpdakacps.html

[T59] Scala：循环
来源：http://hz.dianchejie.cn/gtebobgdcx.html

for (i <- 1 to 10) println(i)
来源：http://hz.fzhhl.top/gtyhnewjns.html

[T60] Scala：折叠
来源：http://hz.xuanzx.com/gtkizeyyuv.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.kuanghao11.cn/gtfssvqhzc.html

================================================================================
来源：http://hz.chenzaomai.com/gthgagiuve.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.nwbrower.top/gtqsnixzgh.html

================================================================================
来源：http://hz.tianlin.xyz/gtiltsktrn.html

[U01] Py：创建虚拟环境
来源：http://hz.chenjidiqi.icu/gtodhmwmjv.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.yangfankeji.com/gtevuzdxqi.html

[U02] Py：导出 / 安装依赖
来源：http://hz.bjfxy.top/gtchtavxcd.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.jinghuilouyu.cn/gtfvpxmtpo.html

[U03] Py：加载 .env 配置
来源：http://hz.tanke756.top/gttxuxzfbh.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.jinqigufen.top/gthcdlagiz.html

[U04] Py：变量调试打印
来源：http://hz.yonumen.top/gtncebqfha.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.9152youxi.cn/gtwzkhxxzo.html

[U05] Py：列表去重且保序
来源：http://hz.sysykeji.top/gtwidqlxhz.html

list(dict.fromkeys(arr))
来源：http://hz.cdnleiting.top/gttmyyqhfl.html

[U06] Py：合并两个字典
来源：http://hz.zhoulong.xyz/gtlmtmtfpf.html

{**a, **b}
来源：http://hz.tian-w.cn/gtkkkdnnlz.html

[U07] Py：反转字典键值
来源：http://hz.cheryme.top/gtxntkuzby.html

{v: k for k, v in d.items()}
来源：http://hz.jqgfzy.top/gtkaufycmd.html

[U08] Py：展平二维列表
来源：http://hz.tian-w.cn/gtsfyjdkvm.html

[y for x in nested for y in x]
来源：http://hz.wangdashe.top/gttvcjhoog.html

[U09] Py：字典取最大值的键
来源：http://hz.shanyushiyangtech.top/gtrmdazaxd.html

max(d, key=d.get)
来源：http://hz.jyoumei.cn/gtddrzrvvt.html

[U10] Py：按值排序字典
来源：http://hz.iojbl.cn/gtdqijfbcu.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.9152youxi.cn/gtjwoplxhz.html

[U11] Py：生成器表达式
来源：http://hz.jianghu66.top/gtnspboqsh.html

(x * 2 for x in arr)
来源：http://hz.nanxinkj.top/gtrntnbgwm.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.52xcode.cn/gtppuepknd.html

Counter(arr).most_common(3)
来源：http://hz.hammf.cn/gtztlfnbrw.html

[U13] Py：固定长度队列
来源：http://hz.meibo888.top/gtbzxcnubc.html

deque(maxlen=10)
来源：http://hz.feifeiyinyue.top/gthnqvmwtx.html

[U14] Py：分组收集到列表
来源：http://hz.nanxuanxn.top/gtqsxqrvpi.html

defaultdict(list)
来源：http://hz.aizwys.cn/gtimpeicdh.html

[U15] Py：高精度计时
来源：http://hz.jqgfzy.top/gthlwcjjaw.html

t = time.perf_counter()
来源：http://hz.sysykeji.top/gtdljfzhro.html

[U16] Py：命令行参数解析
来源：http://hz.yj20258888.top/gtkivcjpsc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.ivvv.top/gtagbxxknz.html

[U17] Py：初始化日志
来源：http://hz.tian-w.cn/gtbymfkbrh.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.tanke756.top/gtklqqdwcp.html

[U18] Py：预编译正则
来源：http://hz.guowangkeji.top/gtvcwbhniw.html

pat = re.compile(r"\d+")
来源：http://hz.jianghu66.top/gtrsvqseps.html

[U19] Py：正则替换带回调
来源：http://hz.bjfxy.top/gtfdmiaqle.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.jianghu66.top/gtxtdanpcn.html

[U20] Py：缓存函数结果
来源：http://hz.gaohongyu789.top/gtjxdndsdz.html

@functools.lru_cache(maxsize=None)
来源：http://hz.zhaomingkeji.xyz/gtbucrvppl.html

[U21] Py：自定义上下文管理器
来源：http://hz.tanke756.top/gteuabdqve.html

@contextlib.contextmanager
来源：http://hz.jqgufenzy.top/gtbcmkzxpf.html

[U22] Py：矩阵转置
来源：http://hz.hnxiangtu.top/gtqpooongl.html

list(zip(*m))
来源：http://hz.jianghu66.top/gtcgjjyqeu.html

[U23] Py：分块读取大文件
来源：http://hz.haohaochexian.top/gtaehkwsac.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.jinyuanbaomall.cn/gtxueobuqm.html

[U24] Py：路径操作
来源：http://hz.wangshuangyany.cn/gtezghcsua.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.jinyuanbaomall.cn/gtvuledtlr.html

[U25] Py：CSV 按字典读
来源：http://hz.sxryk.cn/gtknjrtpgb.html

csv.DictReader(f)
来源：http://hz.xingfuxueyuan.xyz/gtmifmowey.html

[U26] Py：并发下载
来源：http://hz.hysaishi.cn/gtypvibhik.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.fengsongda.top/gtlgmlthrd.html

[U27] Py：异步 HTTP
来源：http://hz.yongpay.top/gttdiirsvm.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.yonumen.top/gtyuwigpay.html

[U28] Py：类型别名
来源：http://hz.tanke756.top/gtgwpfxvno.html

UserId = int
来源：http://hz.aibaodan.cn/gtxzcalcxh.html

[U29] Py：属性校验
来源：http://hz.xuetiantiany.cn/gtabaazkna.html

@property 与 @x.setter 配合
来源：http://hz.tianlin.xyz/gtlzpgnatu.html

[U30] Py：数据类
来源：http://hz.ppjwa.cn/gtxtrypurk.html

@dataclass(slots=True)
来源：http://hz.xingfuxueyuan.xyz/gtlcvcqmgo.html

[U31] Py：单测
来源：http://hz.cdnleiting.top/gtnnpfqmnw.html

python -m pytest -q
来源：http://hz.9152youxi.cn/gtkippuhbe.html

[U32] Py：代码格式化
来源：http://hz.9152youxi.cn/gthmhcslyj.html

ruff format . && ruff check --fix .
来源：http://hz.bjfxy.top/gtpobewvhd.html

[U33] Py：打包发布
来源：http://hz.chenjidiqi.icu/gtykfmvwlf.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.pengpengdd.cyou/gtsodgyzxn.html

[U34] Py：判断编码
来源：http://hz.wangshuangyany.cn/gtttrazloh.html

chardet.detect(raw)
来源：http://hz.jianghu66.top/gtzhkfgrct.html

[U35] Py：发送邮件
来源：http://hz.xingfuxueyuan.xyz/gtxtvaelhi.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.jinqigfzy.top/gtcruifyev.html

[U36] Py：定时任务
来源：http://hz.yj202588.top/gtlbfzcedf.html

schedule.every(10).minutes.do(job)
来源：http://hz.cdnleiting.top/gtwashekul.html

[U37] Py：读写 Excel
来源：http://hz.gaohongyu789.top/gtqhihlfip.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.shanyushiyangkeji.top/gtkkhpceuw.html

[U38] Py：获取脚本所在目录
来源：http://hz.haohaochexian.top/gtiuparokv.html

Path(__file__).resolve().parent
来源：http://hz.zhoulong.xyz/gticltfqxd.html

[U39] Py：判断是否在交互环境
来源：http://hz.xingfuxueyuan.xyz/gtfmbfqguw.html

sys.stdout.isatty()
来源：http://hz.sxryk.cn/gtliyrqmjb.html

[U40] Py：打印到标准错误
来源：http://hz.hammf.cn/gtddxdvobn.html

print("err", file=sys.stderr)
来源：http://hz.zdqjudy.top/gtpzdvmqmc.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.yj20258.top/gtegxjprbz.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.xinyue.icu/gtkfbziryh.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.redwolf501.top/gtodaicaob.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.yanxiufei.cn/gtrgghclup.html

[U43] PHP：声明命名空间
来源：http://hz.fengsongda.top/gtjwvhzmir.html

namespace App\Http;
来源：http://hz.zhongyouzk.top/gtbfqddjph.html

[U44] PHP：开启严格类型
来源：http://hz.zhongyouzk.top/gtxpjogmmx.html

declare(strict_types=1);
来源：http://hz.yuxming.cn/gtkltgtall.html

[U45] PHP：类型声明与返回类型
来源：http://hz.snrcjt.cn/gtnyvyhdoo.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.52xcode.cn/gtfkztzswq.html

[U46] PHP：可空类型
来源：http://hz.yuxming.cn/gtrbatkret.html

?string $name = null
来源：http://hz.jiagoushi.top/gtphyfszoj.html

[U47] PHP：联合类型
来源：http://hz.jianghu66.top/gtgbnbnmpv.html

int|string $id
来源：http://hz.hysaishi.cn/gtwfyhdipu.html

[U48] PHP：纯枚举
来源：http://hz.xinyue.icu/gtyrdxwpld.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.jyoumei.cn/gtzjjduqnz.html

[U49] PHP：只读属性
来源：http://hz.chenjidiqi.icu/gtleaxwpts.html

public readonly string $name
来源：http://hz.gogol.net.cn/gteadukrpm.html

[U50] PHP：构造器属性提升
来源：http://hz.aizwys.cn/gtfiibsrsw.html

public function __construct(private int $id) {}
来源：http://hz.yonumen.top/gtbsbqxuxm.html

[U51] PHP：数组解构
来源：http://hz.smart0.xyz/gteyhysqic.html

[$a, $b] = $arr;
来源：http://hz.ehwqpu.com/gtawuinnsa.html

[U52] PHP：箭头函数
来源：http://hz.ivvv.top/gthcnnpktd.html

$double = fn($x) => $x * 2;
来源：http://hz.jinqigfzy.top/gtznvpuoml.html

[U53] PHP：空合并运算符
来源：http://hz.hongshengwenyu.top/gtrkwjfdpl.html

$v = $a ?? $b ?? "default";
来源：http://hz.ybcxt.top/gtadaqmzxl.html

[U54] PHP：空安全调用
来源：http://hz.zhiwuduotai.top/gtllfcfyep.html

$obj?->method()
来源：http://hz.zhaomingkeji.xyz/gttfgxejhz.html

[U55] PHP：match 表达式
来源：http://hz.xingfuxueyuan.xyz/gtzlwrmyae.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.xziqi.cn/gthkvratsn.html

[U56] PHP：命名参数
来源：http://hz.zhixingplan.top/gtolvllkkg.html

f(a: 1, b: 2)
来源：http://hz.jinghuilouyu.cn/gtuiokwqdz.html

[U57] PHP：字符串插值
来源：http://hz.52xcode.cn/gtjgqardpf.html

"值: {$a}"
来源：http://hz.feifeiyinyue.top/gtmsmahedn.html

[U58] PHP：数组三件套
来源：http://hz.sweek.top/gtueftydpp.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.cheryme.top/gtaovlhtaq.html

[U59] PHP：自定义排序
来源：http://hz.pycfn.com/gtzijbcsoc.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.ivvv.top/gttgdjqirz.html

[U60] PHP：JSON 编解码
来源：http://hz.jqgfzy.top/gtphpjcaay.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.xylfe.cn/gtawvzslzj.html

[U61] PHP：正则
来源：http://hz.xingfuxueyuan.xyz/gtvrydjpht.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.smart0.xyz/gtkqlckfae.html

[U62] PHP：日期对象
来源：http://hz.redwolf501.top/gtfqekckrk.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.gaohongyu789.top/gtrlaujyrp.html

[U63] PHP：文件读写
来源：http://hz.nanxuanxn.top/gtqwuvlvpx.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.yj20258888.top/gtfzdtnber.html

[U64] PHP：目录遍历
来源：http://hz.jqgfzy.top/gtambhzgxw.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.birdmap.top/gteovrcfnt.html

[U65] PHP：会话
来源：http://hz.shanyushiyangkeji.top/gtidqloogn.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.xziqi.cn/gtvjsqynpn.html

[U66] PHP：设置 Cookie
来源：http://hz.cheryme.top/gtacydmfbr.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.ydjk.org.cn/gtnvrkqkah.html

[U67] PHP：处理文件上传
来源：http://hz.xinyue.icu/gtegpwriwh.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.xuanzx.com/gthlwmvdpi.html

[U68] PHP：PDO 连接
来源：http://hz.yongpay.top/gthftkfexd.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.jqgfzy.top/gtbwevamjo.html

[U69] PHP：PDO 预处理
来源：http://hz.kuanghao11.cn/gthqhmcefm.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.haohaochexian.top/gtegnidroj.html

[U70] PHP：PDO 事务
来源：http://hz.andypj.xyz/gtwhgrkhqh.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.xuetiantiany.cn/gtylufdmwk.html

[U71] PHP：抛出异常
来源：http://hz.nanxinkj.top/gtshuustzr.html

throw new RuntimeException("失败", 500);
来源：http://hz.chenzaomai.com/gtqjarfydy.html

[U72] PHP：写错误日志
来源：http://hz.chenzaomai.com/gtdxfdxprr.html

error_log("失败: " . $e->getMessage());
来源：http://hz.gogol.net.cn/gtptmrttvw.html

[U73] PHP：读取 ini 配置
来源：http://hz.yongpay.top/gtvlgdqovk.html

parse_ini_file("config.ini", true)
来源：http://hz.tianlin.xyz/gtvwuojaqw.html

[U74] PHP：读取环境变量
来源：http://hz.yanxiufei.cn/gtapcwdxki.html

getenv("APP_ENV") ?: "production"
来源：http://hz.gzhubu.top/gtegdxxntp.html

[U75] PHP：依赖注入
来源：http://hz.daria6918.cn/gttrpmgszb.html

composer require psr/container
来源：http://hz.daria6918.cn/gtbhvwvflm.html

[U76] PHP：简单路由
来源：http://hz.jqgfzy.top/gtzivjfqfs.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.shangyingyoupin.top/gtalnrjifr.html

[U77] PHP：模板渲染
来源：http://hz.andypj.xyz/gtblxniikt.html

composer require twig/twig
来源：http://hz.jiagoushi.top/gtdlgkuuog.html

[U78] PHP：单元测试
来源：http://hz.cashguo.top/gtkwyrvjfk.html

composer require --dev phpunit/phpunit
来源：http://hz.nwbrower.top/gteuoxeack.html

[U79] PHP：静态分析
来源：http://hz.yongpay.top/gtqtfnxuyy.html

composer require --dev phpstan/phpstan
来源：http://hz.iojbl.cn/gtouphkpur.html

[U80] PHP：代码规范修复
来源：http://hz.zycfv.cn/gtknclrlpw.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.9152youxi.cn/gtxfajzoht.html

[U81] JS：初始化项目
来源：http://hz.xziqi.cn/gtlvxnrtri.html

npm init -y;  npm i express
来源：http://hz.haohaochexian.top/gtitbzonsh.html

[U82] JS：package.json 脚本
来源：http://hz.dashuyun.cn/gtxmhpcoov.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.ywan-chungtsiang.top/gtmieusdtc.html

[U83] JS：ES Module 导入导出
来源：http://hz.hongshengwenyu.top/gtatpfrjpt.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.hfpthk.cn/gtdltaqdzu.html

[U84] JS：CommonJS 写法
来源：http://hz.jinqigfzy.top/gtqiyzupwj.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.wangdashe.top/gttgzdtdrr.html

[U85] JS：可选链
来源：http://hz.smart0.xyz/gtinazerpi.html

a?.b?.c
来源：http://hz.yj20258888.top/gtamzuhwjs.html

[U86] JS：空值合并
来源：http://hz.gogol.net.cn/gtpltrjzdc.html

a ?? b
来源：http://hz.cheryme.top/gtdrzzuxbk.html

[U87] JS：解构默认值
来源：http://hz.nanxuanxn.top/gtskirktsu.html

const { a = 1, b = 2 } = obj;
来源：http://hz.yj20258888.top/gtewpqryjm.html

[U88] JS：对象展开合并
来源：http://hz.hammf.cn/gtpqdevzni.html

{ ...a, ...b }
来源：http://hz.iojbl.cn/gtwpkwmsac.html

[U89] JS：数组去重
来源：http://hz.redwolf501.top/gtyxxsywmq.html

[...new Set(arr)]
来源：http://hz.sysykeji.top/gtrbpywrir.html

[U90] JS：数字数组排序
来源：http://hz.cucudq.cn/gttlojyoml.html

[...arr].sort((a, b) => a - b)
来源：http://hz.daxiang520.top/gtncgjqstu.html

[U91] JS：对象键值遍历
来源：http://hz.snrcjt.cn/gtwvaaammr.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.yongpay.top/gtchdisodo.html

[U92] JS：深拷贝
来源：http://hz.c1oappe.top/gtzbdalcvj.html

structuredClone(obj)
来源：http://hz.xuanzx.com/gtrgmkiehe.html

[U93] JS：模板字符串
来源：http://hz.hongshengwenyu.top/gtmrnaqdjd.html

`共 ${n} 条`
来源：http://hz.hfpthk.cn/gtytnzntzv.html

[U94] JS：箭头函数
来源：http://hz.hfpthk.cn/gthejzlcvx.html

const double = x => x * 2;
来源：http://hz.feifeiyinyue.top/gtkzosyghe.html

[U95] JS：Promise 包装
来源：http://hz.jinqigfzy.top/gtacrypujk.html

new Promise((resolve, reject) => {})
来源：http://hz.9152youxi.cn/gtsjqnlufh.html

[U96] JS：async/await 与异常
来源：http://hz.xylfe.cn/gtvikfkmue.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.fengsongda.top/gttpsupiur.html

[U97] JS：并发请求
来源：http://hz.yuanzhike.top/gtkxeaopzo.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.guowangkeji.top/gtlvtubklo.html

[U98] JS：fetch 带 JSON
来源：http://hz.pycfn.com/gtrfhrkxhy.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.yuxming.cn/gtdlcicnnp.html

[U99] JS：事件监听
来源：http://hz.yonumen.top/gthxpwflur.html

el.addEventListener("click", e => {})
来源：http://hz.jiagoushi.top/gtcsehbzdm.html

[U100] JS：DOM 查询
来源：http://hz.jiagoushi.top/gtbopiyaiz.html

document.querySelector(".item")
来源：http://hz.quarkkingdee.top/gteuwwdxoi.html

[U101] JS：classList 操作
来源：http://hz.cheryme.top/gtbjlfffmm.html

el.classList.toggle("active")
来源：http://hz.vqdsnc.cn/gthdditwwr.html

[U102] JS：本地存储
来源：http://hz.redwolf501.top/gtgyvcozzv.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.aizwys.cn/gteclezfii.html

[U103] JS：定时器
来源：http://hz.zhongyouzk.top/gtdvljnsdx.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.yuxming.cn/gtsraibngz.html

[U104] JS：防抖
来源：http://hz.bjfxy.top/gttbnuzcmi.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.feifeiyinyue.top/gtlkilvrpe.html

[U105] JS：节流
来源：http://hz.daria6918.cn/gtcxmpbcvl.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.gogol.net.cn/gtkfvwemxr.html

[U106] JS：日期格式化
来源：http://hz.gogol.net.cn/gtavxzqcdq.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.zycfv.cn/gterixgxds.html

[U107] JS：数字千分位
来源：http://hz.sxryk.cn/gtfdthwhly.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.chenjidiqi.icu/gtjmqrtoum.html

[U108] JS：随机整数
来源：http://hz.pengpengdd.cyou/gtmwhdqijw.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.316326.xyz/gtokorqfjb.html

[U109] JS：数组分组
来源：http://hz.dianchejie.cn/gtvoizfrvk.html

Object.groupBy(arr, x => x.type)
来源：http://hz.andypj.xyz/gtfokmbmtp.html

[U110] JS：数组分块
来源：http://hz.quarkkingdee.top/gtldlhmyyd.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.jlsjyb.cn/gtktsacwgg.html

[U111] JS：对象转 Map
来源：http://hz.vqdsnc.cn/gtqcnfwutj.html

new Map(Object.entries(obj))
来源：http://hz.ybcxt.top/gtjqcvhsqm.html

[U112] JS：字符串补位
来源：http://hz.xuanzx.com/gtwepgdlsn.html

"7".padStart(3, "0")
来源：http://hz.zhoulong.xyz/gtxyuoqhgu.html

[U113] JS：正则替换全部
来源：http://hz.zhaomingkeji.xyz/gtfszmgxcu.html

s.replaceAll("a", "b")
来源：http://hz.shanyushiyangkeji.top/gtfwugrhyx.html

[U114] JS：JSON 深比较
来源：http://hz.nanxinkj.top/gtvdbvqdji.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.hnqzz.top/gteuqhhgno.html

[U115] JS：生成 UUID
来源：http://hz.tanke756.top/gtctydomlm.html

crypto.randomUUID()
来源：http://hz.fzhhl.top/gtiuxmrpbl.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.ppjwa.cn/gtetxmacjf.html

/** @param {string} name */ function f(name) {}
来源：http://hz.jinghuilouyu.cn/gtkdnpmuix.html

[U117] JS：单元测试
来源：http://hz.zhiwuduotai.top/gtmzalqtbw.html

npm i -D vitest;  npx vitest
来源：http://hz.redwolf501.top/gtncujyrfp.html

[U118] JS：开发服务器
来源：http://hz.shuidangran.top/gthkdaujmx.html

npm i -D vite;  npx vite
来源：http://hz.nanxinkj.top/gtgdntmdvm.html

[U119] JS：生产构建
来源：http://hz.jqgfzy.top/gtndhgnfgf.html

npx vite build
来源：http://hz.feifeiyinyue.top/gtwilunjdx.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.redwolf501.top/gtsgaprcuv.html

import.meta.env.VITE_API_URL
来源：http://hz.pengpengdd.cyou/gtolppstbe.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtmmkpwuqa.html

统计汇总
来源：http://hz.zdqjudy.top/gtlydxocrj.html

================================================================================
来源：http://hz.gaohongyu789.top/gtszuibter.html

按语言统计（条）：
来源：http://hz.xuanzx.com/gtsniwrrnr.html

Python ......... 252
来源：http://hz.snrcjt.cn/gtfwjahmjp.html

PHP ............ 252
来源：http://hz.ydjk.org.cn/gtklaqjvvs.html

JavaScript ..... 252
来源：http://hz.zhoulong.xyz/gtgxbextvj.html

TypeScript ..... 212
来源：http://hz.cucudq.cn/gtetmlqvix.html

Java ........... 212
来源：http://hz.hysaishi.cn/gtceaeysji.html

Go ............. 212
来源：http://hz.zycfv.cn/gtsvvmlefd.html

Ruby ........... 212
来源：http://hz.jinqigufen.top/gtaizhdfnt.html

C# ............. 212
来源：http://hz.shangyingyoupin.top/gtdlfyagfm.html

C .............. 30
来源：http://hz.birdmap.top/gtfxhueuqq.html

C++ ............ 30
来源：http://hz.ywan-chungtsiang.top/gtfmkoulkf.html

SQL ............ 90
来源：http://hz.quarkkingdee.top/gtflfnpcoj.html

Bash ........... 80
来源：http://hz.nanxinkj.top/gtsrurehiy.html

Kotlin ......... 15
来源：http://hz.xuetiantiany.cn/gtmmpgkxmi.html

Swift .......... 15
来源：http://hz.fzhhl.top/gtwwubnsxy.html

Lua ............ 10
来源：http://hz.chenlongwang.top/gtpiozhgyt.html

Perl ........... 10
来源：http://hz.zhongyouzk.top/gtxsvwyfvb.html

Scala .......... 10
来源：http://hz.52xcode.cn/gtfsizpuya.html

------------------------------------
来源：http://hz.nwbrower.top/gtprnzsjat.html

合计 ........... 2106 条
来源：http://hz.zhongyouzk.top/gtapcqpkbq.html

按章节统计：
来源：http://hz.dashuyun.cn/gtytobcjnv.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.ppjwa.cn/gtoemfcepk.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.sweek.top/gtyhtkphxb.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.cqqwz.cn/gttztfatgt.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.nanxuanxn.top/gtuzfrtxzl.html


<!-- 参考信息 -->