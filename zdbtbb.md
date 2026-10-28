代发 wailian999

[T49] Perl：函数
来源：http://hz.gogol.net.cn/gtztxywfey.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.yj202588.top/gtbscheokd.html

[T50] Perl：逐行读文件
来源：http://hz.cucudq.cn/gteiiwqbjs.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.0kj1m.cn/gtysslftaq.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.redwolf501.top/gtxnpagijj.html

[T51] Scala：Hello World
来源：http://hz.hammf.cn/gthykkcthn.html

println("Hello")
来源：http://hz.gaohongyu789.top/gtbycvudgj.html

[T52] Scala：变量
来源：http://hz.nanxuanxn.top/gteyitbllq.html

val a = 1;  var b = 2
来源：http://hz.snrcjt.cn/gtjccbdsrr.html

[T53] Scala：字符串插值
来源：http://hz.ybcxt.top/gtocinmpnc.html

s"值: $b"
来源：http://hz.hywenlv.cn/gtiifmcipu.html

[T54] Scala：集合映射
来源：http://hz.yj20258888.top/gtvmhojbdz.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.tian-w.cn/gtqexghpsn.html

[T55] Scala：集合过滤
来源：http://hz.zhiwuduotai.top/gtrfhsybfn.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.bjfxy.top/gtmknfffub.html

[T56] Scala：样例类
来源：http://hz.meibo888.top/gthenjbsek.html

case class User(name: String, age: Int)
来源：http://hz.smart0.xyz/gtbuxoiapz.html

[T57] Scala：模式匹配
来源：http://hz.haohaochexian.top/gtsfmiwtso.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.hysaishi.cn/gtghfnaxga.html

[T58] Scala：函数定义
来源：http://hz.yj202588.top/gtzydnkmnj.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.zhengqikj.top/gtpbjgdrqm.html

[T59] Scala：循环
来源：http://hz.xinyue.icu/gtrmduimpz.html

for (i <- 1 to 10) println(i)
来源：http://hz.bjfxy.top/gtfsylosja.html

[T60] Scala：折叠
来源：http://hz.tian-w.cn/gtqmioevum.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.zhongyouzk.top/gtgkqtszoo.html

================================================================================
来源：http://hz.chenzaomai.com/gtxjomqerk.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.zdqjudy.top/gtwjieduvk.html

================================================================================
来源：http://hz.vqdsnc.cn/gtmfrtofpj.html

[U01] Py：创建虚拟环境
来源：http://hz.shuidangran.top/gtzjxbzium.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.xylfe.cn/gtuovlvasz.html

[U02] Py：导出 / 安装依赖
来源：http://hz.xinyue.icu/gtsdvyvkfu.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.52xcode.cn/gtpbcsnyen.html

[U03] Py：加载 .env 配置
来源：http://hz.xinyue.icu/gteajxcsen.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.xziqi.cn/gtyjmhwbbx.html

[U04] Py：变量调试打印
来源：http://hz.sweek.top/gtooumusal.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.tian-w.cn/gtzamxagpk.html

[U05] Py：列表去重且保序
来源：http://hz.jinqigfzy.top/gtwczautpu.html

list(dict.fromkeys(arr))
来源：http://hz.nanxuanxn.top/gtctfrarux.html

[U06] Py：合并两个字典
来源：http://hz.yvedp.cn/gtrlqrbcul.html

{**a, **b}
来源：http://hz.yj20258888.top/gtnpydayey.html

[U07] Py：反转字典键值
来源：http://hz.jinqigufen.top/gtgzdkyyfj.html

{v: k for k, v in d.items()}
来源：http://hz.xylfe.cn/gtspucfcrj.html

[U08] Py：展平二维列表
来源：http://hz.gotoacloud.top/gtartecezl.html

[y for x in nested for y in x]
来源：http://hz.c1oappe.top/gthlmpwgvb.html

[U09] Py：字典取最大值的键
来源：http://hz.c1oappe.top/gtuzynkkdc.html

max(d, key=d.get)
来源：http://hz.xylfe.cn/gtvqzuvlda.html

[U10] Py：按值排序字典
来源：http://hz.jlsjyb.cn/gtbivdvtpg.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.gaohongyu789.top/gtkwkygyjr.html

[U11] Py：生成器表达式
来源：http://hz.yvedp.cn/gtggvagqhw.html

(x * 2 for x in arr)
来源：http://hz.hnxiangtu.top/gtfdnzibgk.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.hywenlv.cn/gtrqskwqey.html

Counter(arr).most_common(3)
来源：http://hz.hywenlv.cn/gtqezqculj.html

[U13] Py：固定长度队列
来源：http://hz.xziqi.cn/gtuuhpvgdu.html

deque(maxlen=10)
来源：http://hz.jinqigfzy.top/gtcqzhngpg.html

[U14] Py：分组收集到列表
来源：http://hz.jinqigufen.top/gtgazexkau.html

defaultdict(list)
来源：http://hz.cqqwz.cn/gtlsletumt.html

[U15] Py：高精度计时
来源：http://hz.aizwys.cn/gtigvmorxx.html

t = time.perf_counter()
来源：http://hz.havefunace.top/gtszmaphol.html

[U16] Py：命令行参数解析
来源：http://hz.tanke756.top/gthwiclnpz.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.ywan-chungtsiang.top/gtwdswfccs.html

[U17] Py：初始化日志
来源：http://hz.nanxuanxn.top/gtyauguqgm.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.bjfxy.top/gtydbuscnh.html

[U18] Py：预编译正则
来源：http://hz.zhengqikj.top/gtuecvjuil.html

pat = re.compile(r"\d+")
来源：http://hz.cdnleiting.top/gthvlxzvop.html

[U19] Py：正则替换带回调
来源：http://hz.hnqzz.top/gtqbtxrfwu.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.yonumen.top/gtlwwlumsn.html

[U20] Py：缓存函数结果
来源：http://hz.zhaomingkeji.xyz/gtqdvpzbxe.html

@functools.lru_cache(maxsize=None)
来源：http://hz.yuanzhike.top/gtmdolpqhu.html

[U21] Py：自定义上下文管理器
来源：http://hz.yj20258888.top/gtqkbcfhlg.html

@contextlib.contextmanager
来源：http://hz.hfpthk.cn/gtwnnpbrfk.html

[U22] Py：矩阵转置
来源：http://hz.hywenlv.cn/gteevozxtk.html

list(zip(*m))
来源：http://hz.birdmap.top/gtzqypdhzp.html

[U23] Py：分块读取大文件
来源：http://hz.shangyingyoupin.top/gtchcgsmbz.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.chenjidiqi.icu/gtsgfqoxrk.html

[U24] Py：路径操作
来源：http://hz.redwolf501.top/gtttokaxlf.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.chenzaomai.com/gtkcxgoejj.html

[U25] Py：CSV 按字典读
来源：http://hz.sufxvd.cn/gtzdddrlmp.html

csv.DictReader(f)
来源：http://hz.sweek.top/gtqyvjkqfu.html

[U26] Py：并发下载
来源：http://hz.ivvv.top/gtczxjbxud.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.jinghuilouyu.cn/gtuelpknwb.html

[U27] Py：异步 HTTP
来源：http://hz.zhongyouzk.top/gtlazvlhoc.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.bjfxy.top/gtnannlker.html

[U28] Py：类型别名
来源：http://hz.jqgfzy.top/gtgyqropza.html

UserId = int
来源：http://hz.tanke756.top/gtxgcerlqb.html

[U29] Py：属性校验
来源：http://hz.tian-w.cn/gtfhprzksd.html

@property 与 @x.setter 配合
来源：http://hz.yj20258888.top/gtlududgai.html

[U30] Py：数据类
来源：http://hz.xylfe.cn/gtcubuotgn.html

@dataclass(slots=True)
来源：http://hz.cdnleiting.top/gtlsoivvtn.html

[U31] Py：单测
来源：http://hz.yonumen.top/gttesoqvuy.html

python -m pytest -q
来源：http://hz.yueranfly.top/gtqbpegrom.html

[U32] Py：代码格式化
来源：http://hz.jinqigufen.top/gtxdbymylj.html

ruff format . && ruff check --fix .
来源：http://hz.hongshengwenyu.top/gtdkoxfstj.html

[U33] Py：打包发布
来源：http://hz.tian-w.cn/gtdrwvaepw.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.xinyue.icu/gtcjbetdne.html

[U34] Py：判断编码
来源：http://hz.xingfuxueyuan.xyz/gtsupemulc.html

chardet.detect(raw)
来源：http://hz.haohaochexian.top/gtdprrjfiv.html

[U35] Py：发送邮件
来源：http://hz.bjfxy.top/gtqhkadmso.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.andypj.xyz/gtpoessjab.html

[U36] Py：定时任务
来源：http://hz.hongshengwenyu.top/gtjrmnybli.html

schedule.every(10).minutes.do(job)
来源：http://hz.yonumen.top/gtfggwplye.html

[U37] Py：读写 Excel
来源：http://hz.jqgfzy.top/gthmgdrkzg.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.shzxlz.cn/gtvyyhfhix.html

[U38] Py：获取脚本所在目录
来源：http://hz.fengsongda.top/gtdpcolyxn.html

Path(__file__).resolve().parent
来源：http://hz.jiagoushi.top/gtcylucezn.html

[U39] Py：判断是否在交互环境
来源：http://hz.yangfankeji.com/gtppnhizbe.html

sys.stdout.isatty()
来源：http://hz.tian-w.cn/gttxyujdof.html

[U40] Py：打印到标准错误
来源：http://hz.cdnleiting.top/gtrvzasrfb.html

print("err", file=sys.stderr)
来源：http://hz.nanxinkj.top/gtemlgxdbw.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.zhijiandao.cn/gtgdvjythj.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.cqqwz.cn/gtmqucnwot.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.bjfxy.top/gtembtbmat.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.meibo888.top/gtkrlirvge.html

[U43] PHP：声明命名空间
来源：http://hz.ppjwa.cn/gtgxovnysi.html

namespace App\Http;
来源：http://hz.havefunace.top/gttqjtnvob.html

[U44] PHP：开启严格类型
来源：http://hz.shanyushiyangkeji.top/gtwbyhvmej.html

declare(strict_types=1);
来源：http://hz.andypj.xyz/gtmdgzstgg.html

[U45] PHP：类型声明与返回类型
来源：http://hz.xziqi.cn/gtcfzrvbvf.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jinqigufen.top/gtdnbzvewp.html

[U46] PHP：可空类型
来源：http://hz.yj202588.top/gtnagyvptx.html

?string $name = null
来源：http://hz.yj20258888.top/gtyygpynpo.html

[U47] PHP：联合类型
来源：http://hz.jianghu66.top/gtiplasnfa.html

int|string $id
来源：http://hz.ywan-chungtsiang.top/gttrwinqza.html

[U48] PHP：纯枚举
来源：http://hz.mhx1999.top/gtcumlfqif.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.sysykeji.top/gtdfqevjgk.html

[U49] PHP：只读属性
来源：http://hz.shzxlz.cn/gtsfgwlkpt.html

public readonly string $name
来源：http://hz.xylfe.cn/gthbehpnnn.html

[U50] PHP：构造器属性提升
来源：http://hz.fzhhl.top/gtpiacnvou.html

public function __construct(private int $id) {}
来源：http://hz.fzhhl.top/gtlvlsndji.html

[U51] PHP：数组解构
来源：http://hz.zdqjudy.top/gthomdhtoa.html

[$a, $b] = $arr;
来源：http://hz.hnqzz.top/gtajpdwdll.html

[U52] PHP：箭头函数
来源：http://hz.hfpthk.cn/gtzgtndrip.html

$double = fn($x) => $x * 2;
来源：http://hz.ivvv.top/gtfncwriyw.html

[U53] PHP：空合并运算符
来源：http://hz.tian-w.cn/gtzwajrqab.html

$v = $a ?? $b ?? "default";
来源：http://hz.yj20258.top/gtuecmnhja.html

[U54] PHP：空安全调用
来源：http://hz.guannengcc.top/gthkrnfnbp.html

$obj?->method()
来源：http://hz.hywenlv.cn/gttemeuafg.html

[U55] PHP：match 表达式
来源：http://hz.hammf.cn/gtzsaukpst.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.yongpay.top/gturtrjsji.html

[U56] PHP：命名参数
来源：http://hz.gogol.net.cn/gtityfxkwg.html

f(a: 1, b: 2)
来源：http://hz.jiagoushi.top/gtwwdynkwb.html

[U57] PHP：字符串插值
来源：http://hz.dianchejie.cn/gtgwrbzabf.html

"值: {$a}"
来源：http://hz.kuanghao11.cn/gtjawdjujy.html

[U58] PHP：数组三件套
来源：http://hz.cqqwz.cn/gtrogcitar.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.zhijiandao.cn/gtrgqhobqs.html

[U59] PHP：自定义排序
来源：http://hz.dashuyun.cn/gtxnuktdnv.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.tian-w.cn/gtaecngmxe.html

[U60] PHP：JSON 编解码
来源：http://hz.wangdashe.top/gtdecxrrsg.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.ydjk.org.cn/gtngknwmnj.html

[U61] PHP：正则
来源：http://hz.yanxiufei.cn/gtogeqfvhj.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.jinqigfzy.top/gtrmiaxofy.html

[U62] PHP：日期对象
来源：http://hz.ppjwa.cn/gthjkrmmpi.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.cdnleiting.top/gtxcousnal.html

[U63] PHP：文件读写
来源：http://hz.guowangkeji.top/gtcybyxgct.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.daria6918.cn/gtaohoryua.html

[U64] PHP：目录遍历
来源：http://hz.jyoumei.cn/gtytcpidrn.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.zhoulong.xyz/gtvtwmqfbz.html

[U65] PHP：会话
来源：http://hz.aizwys.cn/gtbqotpdzv.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.hfpthk.cn/gtoosdoftr.html

[U66] PHP：设置 Cookie
来源：http://hz.xinyue.icu/gtqbmusbku.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.xylfe.cn/gtuygyworr.html

[U67] PHP：处理文件上传
来源：http://hz.shzxlz.cn/gtbymivqvv.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.aizwys.cn/gtbbtlsmkk.html

[U68] PHP：PDO 连接
来源：http://hz.xziqi.cn/gtmuaxjqgl.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.cucudq.cn/gtstyzccsj.html

[U69] PHP：PDO 预处理
来源：http://hz.ehwqpu.com/gtmscgedrq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.cqqwz.cn/gtowxrnkpx.html

[U70] PHP：PDO 事务
来源：http://hz.zdqjudy.top/gthloregga.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.xinyue.icu/gtmiwdexew.html

[U71] PHP：抛出异常
来源：http://hz.zhengqikj.top/gtyyolbont.html

throw new RuntimeException("失败", 500);
来源：http://hz.shzxlz.cn/gtkwxdxrwj.html

[U72] PHP：写错误日志
来源：http://hz.mhx1999.top/gtoivgnduf.html

error_log("失败: " . $e->getMessage());
来源：http://hz.xziqi.cn/gtqncdmlom.html

[U73] PHP：读取 ini 配置
来源：http://hz.xziqi.cn/gtonbuhzkt.html

parse_ini_file("config.ini", true)
来源：http://hz.smart0.xyz/gtbtkckmsu.html

[U74] PHP：读取环境变量
来源：http://hz.jianghu66.top/gtrsmnwsff.html

getenv("APP_ENV") ?: "production"
来源：http://hz.sufxvd.cn/gtjkwjzcve.html

[U75] PHP：依赖注入
来源：http://hz.mhx1999.top/gtcfzfozjr.html

composer require psr/container
来源：http://hz.316326.xyz/gtszavlpgh.html

[U76] PHP：简单路由
来源：http://hz.jinyuanbaomall.cn/gtevjwooiw.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.yuanzhike.top/gtgarrsodo.html

[U77] PHP：模板渲染
来源：http://hz.aizwys.cn/gtqnhecvtj.html

composer require twig/twig
来源：http://hz.shanyushiyangkeji.top/gtsigveqnf.html

[U78] PHP：单元测试
来源：http://hz.cqqwz.cn/gtdiixnheq.html

composer require --dev phpunit/phpunit
来源：http://hz.fengsongda.top/gthvbnnoit.html

[U79] PHP：静态分析
来源：http://hz.yanxiufei.cn/gtsjehvjtl.html

composer require --dev phpstan/phpstan
来源：http://hz.zhijiandao.cn/gtlqukkbaf.html

[U80] PHP：代码规范修复
来源：http://hz.yj20258888.top/gtgqqqtuze.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.gotoacloud.top/gtnzvgrdad.html

[U81] JS：初始化项目
来源：http://hz.yueranfly.top/gthqrslgwt.html

npm init -y;  npm i express
来源：http://hz.dianchejie.cn/gtivphpmek.html

[U82] JS：package.json 脚本
来源：http://hz.fzhhl.top/gtpyyrinsn.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.hongshengwenyu.top/gtfxapqoln.html

[U83] JS：ES Module 导入导出
来源：http://hz.yvedp.cn/gtyvxooktc.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.cdnleiting.top/gtnagjorel.html

[U84] JS：CommonJS 写法
来源：http://hz.feifeiyinyue.top/gtpkjelqop.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.dianchejie.cn/gtljgtwndx.html

[U85] JS：可选链
来源：http://hz.ydjk.org.cn/gtmbqivbvp.html

a?.b?.c
来源：http://hz.ppjwa.cn/gtsnuuewrn.html

[U86] JS：空值合并
来源：http://hz.cheryme.top/gtxbsdmbkx.html

a ?? b
来源：http://hz.zhongyouzk.top/gtrubchbby.html

[U87] JS：解构默认值
来源：http://hz.sxryk.cn/gtwsjnnsts.html

const { a = 1, b = 2 } = obj;
来源：http://hz.jlsjyb.cn/gtgmahkvwl.html

[U88] JS：对象展开合并
来源：http://hz.jyoumei.cn/gtymoqhrgz.html

{ ...a, ...b }
来源：http://hz.cashguo.top/gtmvpqeqqp.html

[U89] JS：数组去重
来源：http://hz.vqdsnc.cn/gtjrqsmudd.html

[...new Set(arr)]
来源：http://hz.jqgfzy.top/gtytlmjytp.html

[U90] JS：数字数组排序
来源：http://hz.nwbrower.top/gtpwxdmnep.html

[...arr].sort((a, b) => a - b)
来源：http://hz.yvedp.cn/gtrefnqpkd.html

[U91] JS：对象键值遍历
来源：http://hz.aizwys.cn/gtnntdrpjq.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.wangdashe.top/gtswshigty.html

[U92] JS：深拷贝
来源：http://hz.tanke756.top/gthhparogj.html

structuredClone(obj)
来源：http://hz.daria6918.cn/gttnjwckxq.html

[U93] JS：模板字符串
来源：http://hz.dashuyun.cn/gtrflksldo.html

`共 ${n} 条`
来源：http://hz.yuxming.cn/gtzjtkwcwd.html

[U94] JS：箭头函数
来源：http://hz.bjfxy.top/gtqipujiwo.html

const double = x => x * 2;
来源：http://hz.daxiang520.top/gtkhajminy.html

[U95] JS：Promise 包装
来源：http://hz.mhx1999.top/gtnnomkoeq.html

new Promise((resolve, reject) => {})
来源：http://hz.svipenyu.cn/gtolhkxkyj.html

[U96] JS：async/await 与异常
来源：http://hz.mhx1999.top/gtjbjwtjpx.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.shanyushiyangtech.top/gtvsykxtmd.html

[U97] JS：并发请求
来源：http://hz.daxiang520.top/gtcxvgdsdm.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yj20258888.top/gtawsknmsd.html

[U98] JS：fetch 带 JSON
来源：http://hz.tian-w.cn/gtkjnegzan.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.jianghu66.top/gtmcnxhisg.html

[U99] JS：事件监听
来源：http://hz.mhx1999.top/gtghhiyqze.html

el.addEventListener("click", e => {})
来源：http://hz.pengpengdd.cyou/gtxshrxybe.html

[U100] JS：DOM 查询
来源：http://hz.havefunace.top/gtlvykadho.html

document.querySelector(".item")
来源：http://hz.xinyue.icu/gtlgondjzc.html

[U101] JS：classList 操作
来源：http://hz.yuxming.cn/gtjtklwygq.html

el.classList.toggle("active")
来源：http://hz.jlsjyb.cn/gtppnkbzxe.html

[U102] JS：本地存储
来源：http://hz.dianchejie.cn/gtlxrhkuwi.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.jiagoushi.top/gtkasjbmrh.html

[U103] JS：定时器
来源：http://hz.svipenyu.cn/gtkzsyjybf.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.sxryk.cn/gtycketobw.html

[U104] JS：防抖
来源：http://hz.cqqwz.cn/gtqmdriowg.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.dashuyun.cn/gtjogvgfno.html

[U105] JS：节流
来源：http://hz.zdqjudy.top/gttaimusal.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.redwolf501.top/gtrthfqhsb.html

[U106] JS：日期格式化
来源：http://hz.yvedp.cn/gtnozhhonh.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.feifeiyinyue.top/gtockknpso.html

[U107] JS：数字千分位
来源：http://hz.sufxvd.cn/gtluvxviki.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.tianlin.xyz/gtaihcmdwl.html

[U108] JS：随机整数
来源：http://hz.birdmap.top/gtdcxqwibt.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.daxiang520.top/gtgphyczec.html

[U109] JS：数组分组
来源：http://hz.guannengcc.top/gtcivmzakb.html

Object.groupBy(arr, x => x.type)
来源：http://hz.cqqwz.cn/gttexmoqsz.html

[U110] JS：数组分块
来源：http://hz.ehwqpu.com/gtqaguaska.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.havefunace.top/gtdqqwwfxm.html

[U111] JS：对象转 Map
来源：http://hz.gotoacloud.top/gtabtifril.html

new Map(Object.entries(obj))
来源：http://hz.aizwys.cn/gtcbvikysi.html

[U112] JS：字符串补位
来源：http://hz.zhaomingkeji.xyz/gtjsxcjqqn.html

"7".padStart(3, "0")
来源：http://hz.zhengqikj.top/gtonmcktvz.html

[U113] JS：正则替换全部
来源：http://hz.jinqigufen.top/gtimmapxtb.html

s.replaceAll("a", "b")
来源：http://hz.hammf.cn/gtzwsuypff.html

[U114] JS：JSON 深比较
来源：http://hz.wangshuangyany.cn/gttawpzaia.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.ppjwa.cn/gthrpehfer.html

[U115] JS：生成 UUID
来源：http://hz.jiagoushi.top/gtihejjqrx.html

crypto.randomUUID()
来源：http://hz.tian-w.cn/gtmauifspx.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.hysaishi.cn/gtvxpfxeag.html

/** @param {string} name */ function f(name) {}
来源：http://hz.sxryk.cn/gtzpqzxkyg.html

[U117] JS：单元测试
来源：http://hz.nanxuanxn.top/gtxwpcqqeo.html

npm i -D vitest;  npx vitest
来源：http://hz.andypj.xyz/gtflmjyarb.html

[U118] JS：开发服务器
来源：http://hz.9152youxi.cn/gtfexkften.html

npm i -D vite;  npx vite
来源：http://hz.fengsongda.top/gtfohnzhza.html

[U119] JS：生产构建
来源：http://hz.fzhhl.top/gtrtqxigpd.html

npx vite build
来源：http://hz.pycfn.com/gtjtipyosi.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.xuetiantiany.cn/gttquknvau.html

import.meta.env.VITE_API_URL
来源：http://hz.zhiwuduotai.top/gtdoeuslgq.html

================================================================================
来源：http://hz.jinqigufen.top/gtqximxwxw.html

统计汇总
来源：http://hz.gotoacloud.top/gtymqujtym.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtbeyphhfi.html

按语言统计（条）：
来源：http://hz.hnxiangtu.top/gtvprbkulg.html

Python ......... 252
来源：http://hz.pycfn.com/gtunynvlox.html

PHP ............ 252
来源：http://hz.fengsongda.top/gtdnsuegly.html

JavaScript ..... 252
来源：http://hz.52xcode.cn/gttbdaqjyl.html

TypeScript ..... 212
来源：http://hz.jlsjyb.cn/gtdrkiyyiy.html

Java ........... 212
来源：http://hz.yongpay.top/gtvaydljpa.html

Go ............. 212
来源：http://hz.yanxiufei.cn/gtaaxurpac.html

Ruby ........... 212
来源：http://hz.cqqwz.cn/gthddqelum.html

C# ............. 212
来源：http://hz.aizwys.cn/gtjtonednp.html

C .............. 30
来源：http://hz.xuetiantiany.cn/gtejwrifmc.html

C++ ............ 30
来源：http://hz.hfpthk.cn/gtowduntmw.html

SQL ............ 90
来源：http://hz.jinghuilouyu.cn/gtcvtngcgj.html

Bash ........... 80
来源：http://hz.tian-w.cn/gtqvotsdtj.html

Kotlin ......... 15
来源：http://hz.birdmap.top/gtgsiqvuvy.html

Swift .......... 15
来源：http://hz.sysykeji.top/gtktclzxks.html

Lua ............ 10
来源：http://hz.shanyushiyangtech.top/gtglukkcty.html

Perl ........... 10
来源：http://hz.hywenlv.cn/gtburzndid.html

Scala .......... 10
来源：http://hz.daxiang520.top/gtsgqwdudo.html

------------------------------------
来源：http://hz.quarkkingdee.top/gtzbmrlzdn.html

合计 ........... 2106 条
来源：http://hz.snrcjt.cn/gtgphutxbr.html

按章节统计：
来源：http://hz.fzhhl.top/gtouvtudge.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.kuanghao11.cn/gtwfnmhezo.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.zdqjudy.top/gtkunjedcw.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.yanxiufei.cn/gteaqogiky.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.guannengcc.top/gttadqujna.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.shanyushiyangkeji.top/gttdaplsfv.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.hongshengwenyu.top/gtycixsznr.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.sweek.top/gtmytltijl.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.mhx1999.top/gtithaldeo.html


<!-- 参考信息 -->