代发 wailian999

[T49] Perl：函数
来源：http://hz.xuetiantiany.cn/gtxomoinef.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.snrcjt.cn/gtwuwjlppc.html

[T50] Perl：逐行读文件
来源：http://hz.cashguo.top/gtumfozgvq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.sysykeji.top/gtocscfaxt.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.sxryk.cn/gthmcpemsc.html

[T51] Scala：Hello World
来源：http://hz.xuetiantiany.cn/gtkohimqfm.html

println("Hello")
来源：http://hz.gotoacloud.top/gtyzfiwkgs.html

[T52] Scala：变量
来源：http://hz.havefunace.top/gtgwbnbpjy.html

val a = 1;  var b = 2
来源：http://hz.9152youxi.cn/gtlpzgogun.html

[T53] Scala：字符串插值
来源：http://hz.zhengqikj.top/gtrrbwnbuj.html

s"值: $b"
来源：http://hz.ppjwa.cn/gtapinlseq.html

[T54] Scala：集合映射
来源：http://hz.tanke756.top/gttfvszxcs.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.nwbrower.top/gtbklcojnw.html

[T55] Scala：集合过滤
来源：http://hz.zdqjudy.top/gtgpazzezm.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.feifeiyinyue.top/gtaahmswol.html

[T56] Scala：样例类
来源：http://hz.smart0.xyz/gtmmuuvvqd.html

case class User(name: String, age: Int)
来源：http://hz.nanxinkj.top/gtvafdcntq.html

[T57] Scala：模式匹配
来源：http://hz.yuanzhike.top/gtnhwenmwp.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.c1oappe.top/gtxjjnooca.html

[T58] Scala：函数定义
来源：http://hz.iojbl.cn/gtbunhcwgk.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.zdqjudy.top/gtzgbwnbpz.html

[T59] Scala：循环
来源：http://hz.zhongyouzk.top/gtfzflrfrl.html

for (i <- 1 to 10) println(i)
来源：http://hz.chenzaomai.com/gtmrwrczvt.html

[T60] Scala：折叠
来源：http://hz.52xcode.cn/gtqrkpyjqs.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.ivvv.top/gtelsjocux.html

================================================================================
来源：http://hz.jqgufenzy.top/gtdjxhuozf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.zhixingplan.top/gtlxfrroyq.html

================================================================================
来源：http://hz.pycfn.com/gtofcbbywc.html

[U01] Py：创建虚拟环境
来源：http://hz.zhijiandao.cn/gtqxsqelbl.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.jyoumei.cn/gtlvrszfyb.html

[U02] Py：导出 / 安装依赖
来源：http://hz.aizwys.cn/gtvukavszu.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.ehwqpu.com/gtxcjpipmg.html

[U03] Py：加载 .env 配置
来源：http://hz.zhoulong.xyz/gtnzgahazl.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.bjfxy.top/gtnjvslbuv.html

[U04] Py：变量调试打印
来源：http://hz.jyoumei.cn/gtakgojhug.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.cucudq.cn/gtocjemnjj.html

[U05] Py：列表去重且保序
来源：http://hz.yj202588.top/gtqhwouddt.html

list(dict.fromkeys(arr))
来源：http://hz.hongshengwenyu.top/gtmsmzpxlg.html

[U06] Py：合并两个字典
来源：http://hz.yonumen.top/gtvfycxdwh.html

{**a, **b}
来源：http://hz.ywan-chungtsiang.top/gtknmimxyd.html

[U07] Py：反转字典键值
来源：http://hz.jqgfzy.top/gtksnqhbhn.html

{v: k for k, v in d.items()}
来源：http://hz.yueranfly.top/gtwmrxupgv.html

[U08] Py：展平二维列表
来源：http://hz.jyoumei.cn/gtcfhqezbi.html

[y for x in nested for y in x]
来源：http://hz.yongpay.top/gtqesjdydf.html

[U09] Py：字典取最大值的键
来源：http://hz.shanyushiyangkeji.top/gtgqaajcqt.html

max(d, key=d.get)
来源：http://hz.yangfankeji.com/gtpiwczadw.html

[U10] Py：按值排序字典
来源：http://hz.fengsongda.top/gtwpxwwyvb.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.316326.xyz/gtdsxvaicy.html

[U11] Py：生成器表达式
来源：http://hz.sweek.top/gtsmdithus.html

(x * 2 for x in arr)
来源：http://hz.52xcode.cn/gtssvbntcl.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.yangfankeji.com/gtwlqauwyt.html

Counter(arr).most_common(3)
来源：http://hz.ehwqpu.com/gtpnfxrijs.html

[U13] Py：固定长度队列
来源：http://hz.daria6918.cn/gtidzguotu.html

deque(maxlen=10)
来源：http://hz.tianlin.xyz/gtmvodugfo.html

[U14] Py：分组收集到列表
来源：http://hz.bjfxy.top/gtgfzoxemb.html

defaultdict(list)
来源：http://hz.yj20258888.top/gttszxfakh.html

[U15] Py：高精度计时
来源：http://hz.xziqi.cn/gtktyhezom.html

t = time.perf_counter()
来源：http://hz.9152youxi.cn/gtlsygknlx.html

[U16] Py：命令行参数解析
来源：http://hz.shanyushiyangtech.top/gtvvtxhsrb.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.sysykeji.top/gtjcoqhgiz.html

[U17] Py：初始化日志
来源：http://hz.iojbl.cn/gtorskdujc.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.yj202588.top/gtnwmppgoq.html

[U18] Py：预编译正则
来源：http://hz.gogol.net.cn/gtcuffsbxo.html

pat = re.compile(r"\d+")
来源：http://hz.smart0.xyz/gtdjpavlgl.html

[U19] Py：正则替换带回调
来源：http://hz.xuetiantiany.cn/gtufwoceew.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.cdnleiting.top/gtcglhlgmh.html

[U20] Py：缓存函数结果
来源：http://hz.jinqigfzy.top/gtxwaqignc.html

@functools.lru_cache(maxsize=None)
来源：http://hz.0kj1m.cn/gtfylbuyvs.html

[U21] Py：自定义上下文管理器
来源：http://hz.jyoumei.cn/gtojkjxizr.html

@contextlib.contextmanager
来源：http://hz.jinqigufen.top/gtjeavqfsu.html

[U22] Py：矩阵转置
来源：http://hz.cqqwz.cn/gtaituevfu.html

list(zip(*m))
来源：http://hz.52xcode.cn/gtfnyuefnm.html

[U23] Py：分块读取大文件
来源：http://hz.ywan-chungtsiang.top/gtszzirgvo.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.shzxlz.cn/gtdoftuacr.html

[U24] Py：路径操作
来源：http://hz.jlsjyb.cn/gtragprkmb.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.ydjk.org.cn/gtdbozzrmf.html

[U25] Py：CSV 按字典读
来源：http://hz.tian-w.cn/gtdfwwmjqt.html

csv.DictReader(f)
来源：http://hz.xuanzx.com/gtrwaxdlll.html

[U26] Py：并发下载
来源：http://hz.jinqigufen.top/gtadjfhaql.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.shanyushiyangkeji.top/gtsigzppqw.html

[U27] Py：异步 HTTP
来源：http://hz.xingfuxueyuan.xyz/gtqyupossd.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.sysykeji.top/gtytdcyvoj.html

[U28] Py：类型别名
来源：http://hz.tianlin.xyz/gtmxcjmqwo.html

UserId = int
来源：http://hz.ehwqpu.com/gtgzomcuha.html

[U29] Py：属性校验
来源：http://hz.tanke756.top/gtyufjxdbi.html

@property 与 @x.setter 配合
来源：http://hz.gotoacloud.top/gtvwprhsgu.html

[U30] Py：数据类
来源：http://hz.cdnleiting.top/gtstymxfxw.html

@dataclass(slots=True)
来源：http://hz.nanxinkj.top/gtmrnsyiav.html

[U31] Py：单测
来源：http://hz.zhiwuduotai.top/gtyyqluhsa.html

python -m pytest -q
来源：http://hz.aibaodan.cn/gtulawjwaz.html

[U32] Py：代码格式化
来源：http://hz.chenjidiqi.icu/gtqvjfpnmv.html

ruff format . && ruff check --fix .
来源：http://hz.cdnleiting.top/gtnxthkmib.html

[U33] Py：打包发布
来源：http://hz.yueranfly.top/gtjqzhijmx.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.andypj.xyz/gtkdzbukrq.html

[U34] Py：判断编码
来源：http://hz.cucudq.cn/gthobphzom.html

chardet.detect(raw)
来源：http://hz.sufxvd.cn/gtdhfvgoqd.html

[U35] Py：发送邮件
来源：http://hz.sysykeji.top/gtozhdsfvv.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.havefunace.top/gtpuzhjiki.html

[U36] Py：定时任务
来源：http://hz.yuanzhike.top/gtgynmdfrk.html

schedule.every(10).minutes.do(job)
来源：http://hz.xingfuxueyuan.xyz/gtjuhzzkka.html

[U37] Py：读写 Excel
来源：http://hz.tanke756.top/gtpqkazuig.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.chenlongwang.top/gtxoozdsme.html

[U38] Py：获取脚本所在目录
来源：http://hz.tanke756.top/gtrybetsfd.html

Path(__file__).resolve().parent
来源：http://hz.0kj1m.cn/gtjewqbcqb.html

[U39] Py：判断是否在交互环境
来源：http://hz.316326.xyz/gtxhwfmeev.html

sys.stdout.isatty()
来源：http://hz.zhiwuduotai.top/gtknozzlvo.html

[U40] Py：打印到标准错误
来源：http://hz.hongshengwenyu.top/gttahniibq.html

print("err", file=sys.stderr)
来源：http://hz.sxryk.cn/gthqtwvbde.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.ivvv.top/gtosopjjuo.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.yangfankeji.com/gtsqqzofpi.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.cashguo.top/gtbwzhomzl.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.c1oappe.top/gtrfmdesvh.html

[U43] PHP：声明命名空间
来源：http://hz.chenjidiqi.icu/gtcjwdmjoi.html

namespace App\Http;
来源：http://hz.sufxvd.cn/gtiaqscixn.html

[U44] PHP：开启严格类型
来源：http://hz.daxiang520.top/gtdhoeflgw.html

declare(strict_types=1);
来源：http://hz.xuanzx.com/gtvmdaoumo.html

[U45] PHP：类型声明与返回类型
来源：http://hz.ydzc1.top/gtwgiskthw.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.c1oappe.top/gtaaivnbap.html

[U46] PHP：可空类型
来源：http://hz.ybcxt.top/gtgrzfmsof.html

?string $name = null
来源：http://hz.hywenlv.cn/gtxhfgffvy.html

[U47] PHP：联合类型
来源：http://hz.cdnleiting.top/gtsovaqrlo.html

int|string $id
来源：http://hz.yuxming.cn/gtnnwgsqfe.html

[U48] PHP：纯枚举
来源：http://hz.jqgfzy.top/gteqgvkiqa.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.tian-w.cn/gtsitvctic.html

[U49] PHP：只读属性
来源：http://hz.sxryk.cn/gtbqccdnbd.html

public readonly string $name
来源：http://hz.xinyue.icu/gtsycudqys.html

[U50] PHP：构造器属性提升
来源：http://hz.yvedp.cn/gtnjwtsbtc.html

public function __construct(private int $id) {}
来源：http://hz.tian-w.cn/gtpkjrlolx.html

[U51] PHP：数组解构
来源：http://hz.316326.xyz/gtdbvqoimv.html

[$a, $b] = $arr;
来源：http://hz.yvedp.cn/gtmrrtdrea.html

[U52] PHP：箭头函数
来源：http://hz.c1oappe.top/gtohxzuvlo.html

$double = fn($x) => $x * 2;
来源：http://hz.ybcxt.top/gtcdheoxvx.html

[U53] PHP：空合并运算符
来源：http://hz.sweek.top/gtvhygvksi.html

$v = $a ?? $b ?? "default";
来源：http://hz.nanxinkj.top/gtfkrewmmz.html

[U54] PHP：空安全调用
来源：http://hz.cqqwz.cn/gtvccxchsr.html

$obj?->method()
来源：http://hz.9152youxi.cn/gtilvykkgw.html

[U55] PHP：match 表达式
来源：http://hz.ppjwa.cn/gtoukqjdbu.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.yj20258.top/gtgjlckjfs.html

[U56] PHP：命名参数
来源：http://hz.hnxiangtu.top/gtwwisjbxu.html

f(a: 1, b: 2)
来源：http://hz.jqgfzy.top/gthhiobrrc.html

[U57] PHP：字符串插值
来源：http://hz.jinyuanbaomall.cn/gtqcuaiuhx.html

"值: {$a}"
来源：http://hz.xuanzx.com/gtbazanpkz.html

[U58] PHP：数组三件套
来源：http://hz.zhixingplan.top/gtllfbkdjn.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.aizwys.cn/gtmlmczwjc.html

[U59] PHP：自定义排序
来源：http://hz.jiagoushi.top/gtvbxmhufd.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yuxming.cn/gtwsveglcm.html

[U60] PHP：JSON 编解码
来源：http://hz.c1oappe.top/gtreieeftx.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.pengpengdd.cyou/gtykcssdmx.html

[U61] PHP：正则
来源：http://hz.gotoacloud.top/gtxzzapibu.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.daria6918.cn/gtltpswwts.html

[U62] PHP：日期对象
来源：http://hz.fengsongda.top/gtriekbxsc.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.shuidangran.top/gtrrviadrg.html

[U63] PHP：文件读写
来源：http://hz.shuidangran.top/gtjjdxaonw.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.hongshengwenyu.top/gturtojnlb.html

[U64] PHP：目录遍历
来源：http://hz.cqqwz.cn/gtukzcxtuo.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.cashguo.top/gtxlqjqhpo.html

[U65] PHP：会话
来源：http://hz.fzhhl.top/gtirosswtx.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.ydjk.org.cn/gtpflzzgtl.html

[U66] PHP：设置 Cookie
来源：http://hz.fengsongda.top/gtylyzidph.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.bjfxy.top/gtaknoobbg.html

[U67] PHP：处理文件上传
来源：http://hz.andypj.xyz/gtgzgzrxhq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.zhiwuduotai.top/gtwhggmduy.html

[U68] PHP：PDO 连接
来源：http://hz.ydjk.org.cn/gtpjjteass.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.cdnleiting.top/gtgkpxpfdp.html

[U69] PHP：PDO 预处理
来源：http://hz.nanxinkj.top/gtmccbktkf.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.hammf.cn/gtidomoekj.html

[U70] PHP：PDO 事务
来源：http://hz.chenjidiqi.icu/gtyvwhcjof.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.ydzc1.top/gtieertabo.html

[U71] PHP：抛出异常
来源：http://hz.yuanzhike.top/gtdmpqcvfs.html

throw new RuntimeException("失败", 500);
来源：http://hz.hongshengwenyu.top/gtcjbsqwas.html

[U72] PHP：写错误日志
来源：http://hz.hongshengwenyu.top/gttpmkocxx.html

error_log("失败: " . $e->getMessage());
来源：http://hz.dianchejie.cn/gtrnmnnfze.html

[U73] PHP：读取 ini 配置
来源：http://hz.sysykeji.top/gtuzgpejpn.html

parse_ini_file("config.ini", true)
来源：http://hz.yvedp.cn/gtrdofapss.html

[U74] PHP：读取环境变量
来源：http://hz.pycfn.com/gtcawvnjyy.html

getenv("APP_ENV") ?: "production"
来源：http://hz.yj20258.top/gtmevckkae.html

[U75] PHP：依赖注入
来源：http://hz.jyoumei.cn/gtcbqbwqrp.html

composer require psr/container
来源：http://hz.zhixingplan.top/gtxodqleio.html

[U76] PHP：简单路由
来源：http://hz.shuidangran.top/gtkraeewwa.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.mhx1999.top/gtdgdgqcmy.html

[U77] PHP：模板渲染
来源：http://hz.sweek.top/gtzusygxbq.html

composer require twig/twig
来源：http://hz.hongshengwenyu.top/gteglvzlme.html

[U78] PHP：单元测试
来源：http://hz.ehwqpu.com/gteuaagmtx.html

composer require --dev phpunit/phpunit
来源：http://hz.gaohongyu789.top/gtfrumklfo.html

[U79] PHP：静态分析
来源：http://hz.shanyushiyangkeji.top/gthwaoelvl.html

composer require --dev phpstan/phpstan
来源：http://hz.cashguo.top/gtqsmmbrvv.html

[U80] PHP：代码规范修复
来源：http://hz.shuidangran.top/gtgdlvkefj.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.hywenlv.cn/gtaccqfmab.html

[U81] JS：初始化项目
来源：http://hz.hysaishi.cn/gtqaoemvsi.html

npm init -y;  npm i express
来源：http://hz.nanxinkj.top/gtorgoshja.html

[U82] JS：package.json 脚本
来源：http://hz.jianghu66.top/gtpbknqkot.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.yonumen.top/gtvoporaii.html

[U83] JS：ES Module 导入导出
来源：http://hz.dianchejie.cn/gtucbmwljc.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.daria6918.cn/gttueqqxuu.html

[U84] JS：CommonJS 写法
来源：http://hz.xinyue.icu/gtttiwpfox.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.vqdsnc.cn/gtbkkintlc.html

[U85] JS：可选链
来源：http://hz.pengpengdd.cyou/gtfdsbxjuz.html

a?.b?.c
来源：http://hz.nanxinkj.top/gtzixlhlsx.html

[U86] JS：空值合并
来源：http://hz.aibaodan.cn/gtkrowpjng.html

a ?? b
来源：http://hz.daxiang520.top/gtqdklcbwr.html

[U87] JS：解构默认值
来源：http://hz.shzxlz.cn/gtuvukkaec.html

const { a = 1, b = 2 } = obj;
来源：http://hz.jinghuilouyu.cn/gtrdoswugc.html

[U88] JS：对象展开合并
来源：http://hz.vqdsnc.cn/gtczzolwri.html

{ ...a, ...b }
来源：http://hz.jianghu66.top/gthsulotkp.html

[U89] JS：数组去重
来源：http://hz.xylfe.cn/gtmbkpcmvn.html

[...new Set(arr)]
来源：http://hz.xuetiantiany.cn/gtlmkbwrub.html

[U90] JS：数字数组排序
来源：http://hz.yj20258.top/gtrcheekma.html

[...arr].sort((a, b) => a - b)
来源：http://hz.hammf.cn/gtpdclchun.html

[U91] JS：对象键值遍历
来源：http://hz.quarkkingdee.top/gtkubvmexp.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.zhixingplan.top/gtxvnehplx.html

[U92] JS：深拷贝
来源：http://hz.bjfxy.top/gtrygizsje.html

structuredClone(obj)
来源：http://hz.wangshuangyany.cn/gtdesxbdvw.html

[U93] JS：模板字符串
来源：http://hz.yj202588.top/gtaeukruul.html

`共 ${n} 条`
来源：http://hz.9152youxi.cn/gtqpiaazjy.html

[U94] JS：箭头函数
来源：http://hz.0kj1m.cn/gtxgzzhqow.html

const double = x => x * 2;
来源：http://hz.sysykeji.top/gtkyxghegu.html

[U95] JS：Promise 包装
来源：http://hz.tianlin.xyz/gtmuzwgfkr.html

new Promise((resolve, reject) => {})
来源：http://hz.jinqigufen.top/gtefilntbi.html

[U96] JS：async/await 与异常
来源：http://hz.birdmap.top/gtykldxixg.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.gaohongyu789.top/gtgktkanvx.html

[U97] JS：并发请求
来源：http://hz.fzhhl.top/gtrblkmypf.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xinyue.icu/gtvpbzanpy.html

[U98] JS：fetch 带 JSON
来源：http://hz.cheryme.top/gtirvwbvmz.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.yonumen.top/gtswwiiuwk.html

[U99] JS：事件监听
来源：http://hz.gzhubu.top/gtwbwrtruk.html

el.addEventListener("click", e => {})
来源：http://hz.jinyuanbaomall.cn/gtrbgeekjf.html

[U100] JS：DOM 查询
来源：http://hz.nanxuanxn.top/gtqpvwfizq.html

document.querySelector(".item")
来源：http://hz.yangfankeji.com/gtovexffzb.html

[U101] JS：classList 操作
来源：http://hz.0kj1m.cn/gtzcdjqmvo.html

el.classList.toggle("active")
来源：http://hz.zhengqikj.top/gtwsclqwhd.html

[U102] JS：本地存储
来源：http://hz.yangfankeji.com/gtlntltbdv.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.ywan-chungtsiang.top/gtdgzfuwpx.html

[U103] JS：定时器
来源：http://hz.meibo888.top/gteanwfwxq.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.zhaomingkeji.xyz/gtqbfilwwj.html

[U104] JS：防抖
来源：http://hz.pengpengdd.cyou/gtnbdztjos.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jyoumei.cn/gtjyzxdwrb.html

[U105] JS：节流
来源：http://hz.zhongyouzk.top/gttthfkymx.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.havefunace.top/gthanfjpwz.html

[U106] JS：日期格式化
来源：http://hz.mhx1999.top/gtqkatvsoh.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.yj20258.top/gtauephisl.html

[U107] JS：数字千分位
来源：http://hz.jqgfzy.top/gtjiqsrwpv.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.cqqwz.cn/gtjrkaapdu.html

[U108] JS：随机整数
来源：http://hz.chenjidiqi.icu/gtmtyozjgg.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.sufxvd.cn/gtsquycejy.html

[U109] JS：数组分组
来源：http://hz.xziqi.cn/gtygitbfzt.html

Object.groupBy(arr, x => x.type)
来源：http://hz.hywenlv.cn/gtxuahybrt.html

[U110] JS：数组分块
来源：http://hz.jqgufenzy.top/gtarmizonp.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.cdnleiting.top/gtbzmdvrxr.html

[U111] JS：对象转 Map
来源：http://hz.xuanzx.com/gtggphcguf.html

new Map(Object.entries(obj))
来源：http://hz.xinyue.icu/gtcpmjdowh.html

[U112] JS：字符串补位
来源：http://hz.xuetiantiany.cn/gtyqadgwdb.html

"7".padStart(3, "0")
来源：http://hz.bjfxy.top/gtquokfmcc.html

[U113] JS：正则替换全部
来源：http://hz.yueranfly.top/gthbfgarsc.html

s.replaceAll("a", "b")
来源：http://hz.zhaomingkeji.xyz/gtkbjuxots.html

[U114] JS：JSON 深比较
来源：http://hz.jinqigfzy.top/gtficxbfog.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.sxryk.cn/gtqslvviis.html

[U115] JS：生成 UUID
来源：http://hz.smart0.xyz/gtmrnbsfld.html

crypto.randomUUID()
来源：http://hz.yonumen.top/gttuoxnxpx.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.cqqwz.cn/gthuyyxtrt.html

/** @param {string} name */ function f(name) {}
来源：http://hz.snrcjt.cn/gtopegqnkv.html

[U117] JS：单元测试
来源：http://hz.0kj1m.cn/gtstehmlvr.html

npm i -D vitest;  npx vitest
来源：http://hz.c1oappe.top/gtqtlrchht.html

[U118] JS：开发服务器
来源：http://hz.daxiang520.top/gtlqdmgmgz.html

npm i -D vite;  npx vite
来源：http://hz.shangyingyoupin.top/gtftjbezlc.html

[U119] JS：生产构建
来源：http://hz.shzxlz.cn/gthszckhyx.html

npx vite build
来源：http://hz.yanxiufei.cn/gtgzkrykjx.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.xinyue.icu/gtuxeofjrh.html

import.meta.env.VITE_API_URL
来源：http://hz.wangdashe.top/gtvmbvxqqs.html

================================================================================
来源：http://hz.guannengcc.top/gthwvrsamu.html

统计汇总
来源：http://hz.pycfn.com/gtukmgortb.html

================================================================================
来源：http://hz.zhijiandao.cn/gttfkofpks.html

按语言统计（条）：
来源：http://hz.mhx1999.top/gtjfrpjrrx.html

Python ......... 252
来源：http://hz.pycfn.com/gthqttukcx.html

PHP ............ 252
来源：http://hz.daxiang520.top/gtqbncydip.html

JavaScript ..... 252
来源：http://hz.haohaochexian.top/gtpxfidknm.html

TypeScript ..... 212
来源：http://hz.cqqwz.cn/gtnadfvwvw.html

Java ........... 212
来源：http://hz.fengsongda.top/gtcwyyyxnv.html

Go ............. 212
来源：http://hz.gogol.net.cn/gtpgczhoen.html

Ruby ........... 212
来源：http://hz.nwbrower.top/gtvxwfmzxk.html

C# ............. 212
来源：http://hz.ybcxt.top/gtqjsbruwj.html

C .............. 30
来源：http://hz.pycfn.com/gtmyfmxjzn.html

C++ ............ 30
来源：http://hz.gogol.net.cn/gtvugrcewn.html

SQL ............ 90
来源：http://hz.52xcode.cn/gtlaunhoxr.html

Bash ........... 80
来源：http://hz.guannengcc.top/gtnjnimyze.html

Kotlin ......... 15
来源：http://hz.svipenyu.cn/gtlnumrirw.html

Swift .......... 15
来源：http://hz.zhongyouzk.top/gtvuataiwx.html

Lua ............ 10
来源：http://hz.sweek.top/gthtsvlmeh.html

Perl ........... 10
来源：http://hz.gzhubu.top/gtagazafwx.html

Scala .......... 10
来源：http://hz.yj202588.top/gtbnesmzaw.html

------------------------------------
来源：http://hz.zhongyouzk.top/gtzxgkarki.html

合计 ........... 2106 条
来源：http://hz.feifeiyinyue.top/gthdvakxzr.html

按章节统计：
来源：http://hz.hywenlv.cn/gtijdqzpxn.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.hysaishi.cn/gtvpcjrhbr.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.ywan-chungtsiang.top/gtimkomxkl.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.tanke756.top/gtmywgtikq.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.snrcjt.cn/gtjiwxuqmi.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.jianghu66.top/gtgeawaqje.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.cheryme.top/gtoioddcsc.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.haohaochexian.top/gthhtqwgls.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.zhijiandao.cn/gttmdbpzwx.html


<!-- 参考信息 -->