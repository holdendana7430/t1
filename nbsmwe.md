代发 wailian999

[T47] Perl：正则捕获
来源：http://hz.guannengcc.top/gtycvwtais.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.yuanzhike.top/gttfjdqpzk.html

[T48] Perl：正则替换
来源：http://hz.zhixingplan.top/gttwvcqbvj.html

$s =~ s/old/new/g;
来源：http://hz.0kj1m.cn/gtcznsmwbl.html

[T49] Perl：函数
来源：http://hz.9152youxi.cn/gtvhmsnuik.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.sxryk.cn/gteijmgkmc.html

[T50] Perl：逐行读文件
来源：http://hz.gotoacloud.top/gtruihaeoe.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.jqgfzy.top/gtszukprwf.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.feifeiyinyue.top/gtvbibaxcw.html

[T51] Scala：Hello World
来源：http://hz.wangshuangyany.cn/gtkpcidlyl.html

println("Hello")
来源：http://hz.jinyuanbaomall.cn/gtsmvbgbqf.html

[T52] Scala：变量
来源：http://hz.ivvv.top/gtpkfzpgzz.html

val a = 1;  var b = 2
来源：http://hz.svipenyu.cn/gtnrjuappy.html

[T53] Scala：字符串插值
来源：http://hz.yangfankeji.com/gtxeunstcy.html

s"值: $b"
来源：http://hz.yj20258.top/gtsxpisogs.html

[T54] Scala：集合映射
来源：http://hz.jinghuilouyu.cn/gtybfrrnur.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.wangdashe.top/gtsuhymvbz.html

[T55] Scala：集合过滤
来源：http://hz.yj20258888.top/gtfyxqyzbp.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.wangdashe.top/gtrcksawys.html

[T56] Scala：样例类
来源：http://hz.svipenyu.cn/gtuajluzof.html

case class User(name: String, age: Int)
来源：http://hz.wangshuangyany.cn/gtrettvkmg.html

[T57] Scala：模式匹配
来源：http://hz.shanyushiyangkeji.top/gtwurvhani.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.guannengcc.top/gtzvtisdjf.html

[T58] Scala：函数定义
来源：http://hz.yj20258.top/gtdswxfijg.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.tian-w.cn/gtlbrklttm.html

[T59] Scala：循环
来源：http://hz.pengpengdd.cyou/gtwcovkmsn.html

for (i <- 1 to 10) println(i)
来源：http://hz.zycfv.cn/gtzaxnevqo.html

[T60] Scala：折叠
来源：http://hz.zhiwuduotai.top/gtlduwjhpr.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.ivvv.top/gtsltyxnqj.html

================================================================================
来源：http://hz.haohaochexian.top/gteikggegn.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.ydjk.org.cn/gtqosmbslv.html

================================================================================
来源：http://hz.ydzc1.top/gtggilmcmc.html

[U01] Py：创建虚拟环境
来源：http://hz.jlsjyb.cn/gtttzvhuwi.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.jqgufenzy.top/gtpgxagqab.html

[U02] Py：导出 / 安装依赖
来源：http://hz.cashguo.top/gtvketmftx.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.yonumen.top/gtctjuyedy.html

[U03] Py：加载 .env 配置
来源：http://hz.yj202588.top/gtsdmjkumv.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.hnqzz.top/gtrmxvdtjm.html

[U04] Py：变量调试打印
来源：http://hz.vqdsnc.cn/gtorueirmf.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.zhiwuduotai.top/gtninnment.html

[U05] Py：列表去重且保序
来源：http://hz.yonumen.top/gtwdojrwim.html

list(dict.fromkeys(arr))
来源：http://hz.0kj1m.cn/gthnkagiry.html

[U06] Py：合并两个字典
来源：http://hz.jqgufenzy.top/gthxirhogq.html

{**a, **b}
来源：http://hz.guannengcc.top/gtgqavnjpy.html

[U07] Py：反转字典键值
来源：http://hz.gaohongyu789.top/gtmcscepoq.html

{v: k for k, v in d.items()}
来源：http://hz.shuidangran.top/gteqhwaflb.html

[U08] Py：展平二维列表
来源：http://hz.fzhhl.top/gtqtfuehep.html

[y for x in nested for y in x]
来源：http://hz.c1oappe.top/gtxogrnian.html

[U09] Py：字典取最大值的键
来源：http://hz.kuanghao11.cn/gtpssgaypt.html

max(d, key=d.get)
来源：http://hz.tian-w.cn/gtgmiopjns.html

[U10] Py：按值排序字典
来源：http://hz.hfpthk.cn/gtgyhkbzez.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.andypj.xyz/gtfbowasgw.html

[U11] Py：生成器表达式
来源：http://hz.cqqwz.cn/gtldqwhcmj.html

(x * 2 for x in arr)
来源：http://hz.zdqjudy.top/gtqqaugmzt.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.zhaomingkeji.xyz/gtwmkhtsqo.html

Counter(arr).most_common(3)
来源：http://hz.tian-w.cn/gtzswntaja.html

[U13] Py：固定长度队列
来源：http://hz.ydzc1.top/gtkwbjglar.html

deque(maxlen=10)
来源：http://hz.birdmap.top/gtohuxbfzw.html

[U14] Py：分组收集到列表
来源：http://hz.hammf.cn/gtypejzfzp.html

defaultdict(list)
来源：http://hz.jqgfzy.top/gtezbgbdgv.html

[U15] Py：高精度计时
来源：http://hz.cdnleiting.top/gtfrgdmslc.html

t = time.perf_counter()
来源：http://hz.daxiang520.top/gtwfjpujum.html

[U16] Py：命令行参数解析
来源：http://hz.cqqwz.cn/gtpqbqvljx.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.hywenlv.cn/gtaknzsstf.html

[U17] Py：初始化日志
来源：http://hz.zhoulong.xyz/gtsvoakbpp.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.hongshengwenyu.top/gtmlbchxlv.html

[U18] Py：预编译正则
来源：http://hz.dianchejie.cn/gtgdpfgarh.html

pat = re.compile(r"\d+")
来源：http://hz.zhongyouzk.top/gthdciyugl.html

[U19] Py：正则替换带回调
来源：http://hz.yanxiufei.cn/gtdlytqlky.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.dianchejie.cn/gtnwzglpkh.html

[U20] Py：缓存函数结果
来源：http://hz.iojbl.cn/gtjazibykz.html

@functools.lru_cache(maxsize=None)
来源：http://hz.jyoumei.cn/gtctwebnis.html

[U21] Py：自定义上下文管理器
来源：http://hz.tanke756.top/gtfybvnjvy.html

@contextlib.contextmanager
来源：http://hz.daxiang520.top/gtcojpwwju.html

[U22] Py：矩阵转置
来源：http://hz.yj202588.top/gtfokqnlgz.html

list(zip(*m))
来源：http://hz.xingfuxueyuan.xyz/gtwiqkilzj.html

[U23] Py：分块读取大文件
来源：http://hz.cheryme.top/gtqlbmyhaw.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.mhx1999.top/gtvbaxdcwm.html

[U24] Py：路径操作
来源：http://hz.yuanzhike.top/gtjopuppsh.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.guannengcc.top/gtpsveqaoj.html

[U25] Py：CSV 按字典读
来源：http://hz.zycfv.cn/gttjgoyvjg.html

csv.DictReader(f)
来源：http://hz.jyoumei.cn/gtzfdnznrg.html

[U26] Py：并发下载
来源：http://hz.chenlongwang.top/gtylzpogiq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.shanyushiyangkeji.top/gtiucgfziv.html

[U27] Py：异步 HTTP
来源：http://hz.feifeiyinyue.top/gtrkddxtvi.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.316326.xyz/gtnahpchxw.html

[U28] Py：类型别名
来源：http://hz.zdqjudy.top/gtjgtketqj.html

UserId = int
来源：http://hz.kuanghao11.cn/gtdluhroxl.html

[U29] Py：属性校验
来源：http://hz.yanxiufei.cn/gtmutigcvm.html

@property 与 @x.setter 配合
来源：http://hz.daria6918.cn/gtlaycfbhj.html

[U30] Py：数据类
来源：http://hz.yonumen.top/gtlgvimozz.html

@dataclass(slots=True)
来源：http://hz.shanyushiyangtech.top/gtgazpgkty.html

[U31] Py：单测
来源：http://hz.vqdsnc.cn/gtyanjngfk.html

python -m pytest -q
来源：http://hz.yangfankeji.com/gtppstmwnx.html

[U32] Py：代码格式化
来源：http://hz.daria6918.cn/gtejvumyhn.html

ruff format . && ruff check --fix .
来源：http://hz.xylfe.cn/gteqdtsuyt.html

[U33] Py：打包发布
来源：http://hz.ywan-chungtsiang.top/gtalqwncyc.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.sufxvd.cn/gtuwssavji.html

[U34] Py：判断编码
来源：http://hz.aibaodan.cn/gtyghegdjv.html

chardet.detect(raw)
来源：http://hz.yuxming.cn/gthlfbgvtd.html

[U35] Py：发送邮件
来源：http://hz.xuetiantiany.cn/gthlaqxksb.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.yuanzhike.top/gtrvihofzu.html

[U36] Py：定时任务
来源：http://hz.jlsjyb.cn/gtokygrhmx.html

schedule.every(10).minutes.do(job)
来源：http://hz.shangyingyoupin.top/gtyohwjdsq.html

[U37] Py：读写 Excel
来源：http://hz.tianlin.xyz/gtqprhqpqf.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.yongpay.top/gtwsdqzgkb.html

[U38] Py：获取脚本所在目录
来源：http://hz.wangshuangyany.cn/gtmgfufwqw.html

Path(__file__).resolve().parent
来源：http://hz.kuanghao11.cn/gtjkgloncb.html

[U39] Py：判断是否在交互环境
来源：http://hz.bjfxy.top/gthsvdpgmi.html

sys.stdout.isatty()
来源：http://hz.cucudq.cn/gtxlqrowna.html

[U40] Py：打印到标准错误
来源：http://hz.ywan-chungtsiang.top/gtaidmgeee.html

print("err", file=sys.stderr)
来源：http://hz.jinqigufen.top/gtavwxmlzv.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.guannengcc.top/gtubkuipqx.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.shanyushiyangkeji.top/gtdvikzdey.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.yueranfly.top/gtgpqfgpmp.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.9152youxi.cn/gtwcgrdbli.html

[U43] PHP：声明命名空间
来源：http://hz.ydjk.org.cn/gtrruxfdbq.html

namespace App\Http;
来源：http://hz.jqgufenzy.top/gtfibupdxq.html

[U44] PHP：开启严格类型
来源：http://hz.yj20258.top/gtobyezdid.html

declare(strict_types=1);
来源：http://hz.cqqwz.cn/gtyqbxidus.html

[U45] PHP：类型声明与返回类型
来源：http://hz.316326.xyz/gteoatdckq.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yonumen.top/gtcgbycehs.html

[U46] PHP：可空类型
来源：http://hz.yj20258888.top/gtdeffekuk.html

?string $name = null
来源：http://hz.xuanzx.com/gtshvwqain.html

[U47] PHP：联合类型
来源：http://hz.hywenlv.cn/gtybrifytm.html

int|string $id
来源：http://hz.guowangkeji.top/gtnlnfneen.html

[U48] PHP：纯枚举
来源：http://hz.fengsongda.top/gtcjjrukaa.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.guowangkeji.top/gtdvrjcnvy.html

[U49] PHP：只读属性
来源：http://hz.tanke756.top/gtbnoxqwbr.html

public readonly string $name
来源：http://hz.nwbrower.top/gtznlrhyhk.html

[U50] PHP：构造器属性提升
来源：http://hz.pycfn.com/gtoatpvmjt.html

public function __construct(private int $id) {}
来源：http://hz.jianghu66.top/gtsolalwdt.html

[U51] PHP：数组解构
来源：http://hz.xingfuxueyuan.xyz/gtmamepeva.html

[$a, $b] = $arr;
来源：http://hz.ydzc1.top/gthxaqfjcd.html

[U52] PHP：箭头函数
来源：http://hz.jinqigufen.top/gtqkjhzcpu.html

$double = fn($x) => $x * 2;
来源：http://hz.shzxlz.cn/gtnjcbkvmy.html

[U53] PHP：空合并运算符
来源：http://hz.9152youxi.cn/gtkqogdaik.html

$v = $a ?? $b ?? "default";
来源：http://hz.zhixingplan.top/gttxyurjdx.html

[U54] PHP：空安全调用
来源：http://hz.chenlongwang.top/gtwqbjwqjl.html

$obj?->method()
来源：http://hz.sysykeji.top/gtbinmygvc.html

[U55] PHP：match 表达式
来源：http://hz.zycfv.cn/gtkklectcf.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.bjfxy.top/gthyogklnx.html

[U56] PHP：命名参数
来源：http://hz.sysykeji.top/gtwwofmpev.html

f(a: 1, b: 2)
来源：http://hz.zhixingplan.top/gtbtucipix.html

[U57] PHP：字符串插值
来源：http://hz.sxryk.cn/gtjbrodluf.html

"值: {$a}"
来源：http://hz.cqqwz.cn/gtecuewjdg.html

[U58] PHP：数组三件套
来源：http://hz.snrcjt.cn/gtxttprxav.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.shzxlz.cn/gtzesqjayg.html

[U59] PHP：自定义排序
来源：http://hz.daria6918.cn/gthysyzavw.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yonumen.top/gtwqiznoqr.html

[U60] PHP：JSON 编解码
来源：http://hz.nwbrower.top/gtmwicemfv.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.jlsjyb.cn/gticlxojef.html

[U61] PHP：正则
来源：http://hz.sufxvd.cn/gtpmcqifmb.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.cqqwz.cn/gtqrhooswl.html

[U62] PHP：日期对象
来源：http://hz.cucudq.cn/gtphfnuwtn.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.jinqigfzy.top/gtnasuuxfa.html

[U63] PHP：文件读写
来源：http://hz.chenjidiqi.icu/gtbgaysico.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.yuxming.cn/gtdiffkfuy.html

[U64] PHP：目录遍历
来源：http://hz.zhijiandao.cn/gtjxxxvvub.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.hnxiangtu.top/gthopidkod.html

[U65] PHP：会话
来源：http://hz.ybcxt.top/gtsrdipyrb.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.iojbl.cn/gtwtkpzddg.html

[U66] PHP：设置 Cookie
来源：http://hz.jinqigfzy.top/gtyqjlzmtg.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.yvedp.cn/gtaovrnkus.html

[U67] PHP：处理文件上传
来源：http://hz.yongpay.top/gtkcofiyvv.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.daria6918.cn/gtqdmywume.html

[U68] PHP：PDO 连接
来源：http://hz.kuanghao11.cn/gtiprzttlq.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.kuanghao11.cn/gtvqowzcde.html

[U69] PHP：PDO 预处理
来源：http://hz.ehwqpu.com/gtemmgvofv.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.jyoumei.cn/gttmayzkzi.html

[U70] PHP：PDO 事务
来源：http://hz.chenzaomai.com/gtbppbcidk.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.dashuyun.cn/gtworqashd.html

[U71] PHP：抛出异常
来源：http://hz.gzhubu.top/gtngilebdl.html

throw new RuntimeException("失败", 500);
来源：http://hz.ehwqpu.com/gtfrguezjg.html

[U72] PHP：写错误日志
来源：http://hz.gotoacloud.top/gtrqmqwxep.html

error_log("失败: " . $e->getMessage());
来源：http://hz.xuanzx.com/gtpfoptskx.html

[U73] PHP：读取 ini 配置
来源：http://hz.ppjwa.cn/gtmyslhrkj.html

parse_ini_file("config.ini", true)
来源：http://hz.zdqjudy.top/gtrzbqrqns.html

[U74] PHP：读取环境变量
来源：http://hz.hongshengwenyu.top/gtmqrowakp.html

getenv("APP_ENV") ?: "production"
来源：http://hz.52xcode.cn/gtemifkbpa.html

[U75] PHP：依赖注入
来源：http://hz.zycfv.cn/gtrvowhsvi.html

composer require psr/container
来源：http://hz.yanxiufei.cn/gtahxoyehz.html

[U76] PHP：简单路由
来源：http://hz.cashguo.top/gtocjxhzgd.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.vqdsnc.cn/gtivlenuvv.html

[U77] PHP：模板渲染
来源：http://hz.haohaochexian.top/gtznewmfkf.html

composer require twig/twig
来源：http://hz.shangyingyoupin.top/gtmdmsqmal.html

[U78] PHP：单元测试
来源：http://hz.jiagoushi.top/gtwjonklar.html

composer require --dev phpunit/phpunit
来源：http://hz.ybcxt.top/gtsdqbcehq.html

[U79] PHP：静态分析
来源：http://hz.aibaodan.cn/gtpkwbmqwb.html

composer require --dev phpstan/phpstan
来源：http://hz.yonumen.top/gtgandphin.html

[U80] PHP：代码规范修复
来源：http://hz.dashuyun.cn/gtbzcpluum.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.smart0.xyz/gtozesergl.html

[U81] JS：初始化项目
来源：http://hz.vqdsnc.cn/gthogrzhbi.html

npm init -y;  npm i express
来源：http://hz.ivvv.top/gtzvquxsgz.html

[U82] JS：package.json 脚本
来源：http://hz.xylfe.cn/gtkvpjkhqv.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.hysaishi.cn/gtoyborhjl.html

[U83] JS：ES Module 导入导出
来源：http://hz.wangdashe.top/gtqwhhmukr.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.zhoulong.xyz/gtlewxuzgt.html

[U84] JS：CommonJS 写法
来源：http://hz.aizwys.cn/gtynvbufrs.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.sxryk.cn/gtzkkhlnjo.html

[U85] JS：可选链
来源：http://hz.kuanghao11.cn/gteipbxbqm.html

a?.b?.c
来源：http://hz.sweek.top/gtyfqvvmoh.html

[U86] JS：空值合并
来源：http://hz.ydjk.org.cn/gtklslymgo.html

a ?? b
来源：http://hz.52xcode.cn/gtlcviyiis.html

[U87] JS：解构默认值
来源：http://hz.ivvv.top/gtjxxgpefm.html

const { a = 1, b = 2 } = obj;
来源：http://hz.haohaochexian.top/gthpqsojdd.html

[U88] JS：对象展开合并
来源：http://hz.shanyushiyangtech.top/gtskhcsdbl.html

{ ...a, ...b }
来源：http://hz.hfpthk.cn/gtdzafioyo.html

[U89] JS：数组去重
来源：http://hz.andypj.xyz/gtctzguywe.html

[...new Set(arr)]
来源：http://hz.xziqi.cn/gtffxljzdo.html

[U90] JS：数字数组排序
来源：http://hz.ybcxt.top/gtyhbywlod.html

[...arr].sort((a, b) => a - b)
来源：http://hz.chenlongwang.top/gtfoeajaha.html

[U91] JS：对象键值遍历
来源：http://hz.wangdashe.top/gtpatxpfcj.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.guannengcc.top/gtbfnipuui.html

[U92] JS：深拷贝
来源：http://hz.yuanzhike.top/gthcwxjhlu.html

structuredClone(obj)
来源：http://hz.0kj1m.cn/gtuozhycvw.html

[U93] JS：模板字符串
来源：http://hz.hongshengwenyu.top/gtnexjtnnt.html

`共 ${n} 条`
来源：http://hz.zhoulong.xyz/gtbvdvowmp.html

[U94] JS：箭头函数
来源：http://hz.daria6918.cn/gtczempezp.html

const double = x => x * 2;
来源：http://hz.vqdsnc.cn/gtiofjregn.html

[U95] JS：Promise 包装
来源：http://hz.guowangkeji.top/gtqorxyzze.html

new Promise((resolve, reject) => {})
来源：http://hz.tian-w.cn/gtejrnyrot.html

[U96] JS：async/await 与异常
来源：http://hz.yongpay.top/gtsimiwmrz.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.hfpthk.cn/gtsbcseadc.html

[U97] JS：并发请求
来源：http://hz.quarkkingdee.top/gtzxhgccza.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shangyingyoupin.top/gtkyqvmaem.html

[U98] JS：fetch 带 JSON
来源：http://hz.hongshengwenyu.top/gtfsuwhbgm.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.pengpengdd.cyou/gtmwvvbhfq.html

[U99] JS：事件监听
来源：http://hz.zhijiandao.cn/gtnzbdxayt.html

el.addEventListener("click", e => {})
来源：http://hz.xziqi.cn/gtstwmudkf.html

[U100] JS：DOM 查询
来源：http://hz.yonumen.top/gtkitvitkr.html

document.querySelector(".item")
来源：http://hz.haohaochexian.top/gtmxfpzxbp.html

[U101] JS：classList 操作
来源：http://hz.jqgfzy.top/gtludiupwz.html

el.classList.toggle("active")
来源：http://hz.ppjwa.cn/gtsbmpcnay.html

[U102] JS：本地存储
来源：http://hz.yongpay.top/gtdabefgfs.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.svipenyu.cn/gtgqtkbsvj.html

[U103] JS：定时器
来源：http://hz.cheryme.top/gtdknadkmy.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.quarkkingdee.top/gtzxqyeaxe.html

[U104] JS：防抖
来源：http://hz.shzxlz.cn/gtyubgtmxr.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hammf.cn/gtkvsdltwz.html

[U105] JS：节流
来源：http://hz.xylfe.cn/gtzdrocwsj.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.shanyushiyangkeji.top/gtpdczzgwx.html

[U106] JS：日期格式化
来源：http://hz.fzhhl.top/gterpritjx.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.jiagoushi.top/gtjmvozkfi.html

[U107] JS：数字千分位
来源：http://hz.kuanghao11.cn/gtwjasrpzk.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.zhixingplan.top/gtejnojqnf.html

[U108] JS：随机整数
来源：http://hz.0kj1m.cn/gtcapwzrbl.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.aizwys.cn/gtmuzpatyi.html

[U109] JS：数组分组
来源：http://hz.birdmap.top/gtdvkydibx.html

Object.groupBy(arr, x => x.type)
来源：http://hz.jlsjyb.cn/gtdpxsqmkt.html

[U110] JS：数组分块
来源：http://hz.zhixingplan.top/gtzgqztvsb.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.gaohongyu789.top/gtjwweyxdu.html

[U111] JS：对象转 Map
来源：http://hz.svipenyu.cn/gtvlbuejaj.html

new Map(Object.entries(obj))
来源：http://hz.jyoumei.cn/gtsvckcstc.html

[U112] JS：字符串补位
来源：http://hz.daria6918.cn/gtalkzlgxz.html

"7".padStart(3, "0")
来源：http://hz.shuidangran.top/gtsknvlmgs.html

[U113] JS：正则替换全部
来源：http://hz.yongpay.top/gtyfxqufor.html

s.replaceAll("a", "b")
来源：http://hz.52xcode.cn/gtfxtylblf.html

[U114] JS：JSON 深比较
来源：http://hz.chenzaomai.com/gtbnsigsgu.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.ydzc1.top/gthalsezcf.html

[U115] JS：生成 UUID
来源：http://hz.cashguo.top/gtbsgvfyju.html

crypto.randomUUID()
来源：http://hz.zhongyouzk.top/gtxcsnzwlz.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.tianlin.xyz/gtnnnqvpvx.html

/** @param {string} name */ function f(name) {}
来源：http://hz.smart0.xyz/gtgbdbvdmj.html

[U117] JS：单元测试
来源：http://hz.cashguo.top/gthkuwwgyp.html

npm i -D vitest;  npx vitest
来源：http://hz.zhijiandao.cn/gttwyrujze.html

[U118] JS：开发服务器
来源：http://hz.hywenlv.cn/gtqtqepqdu.html

npm i -D vite;  npx vite
来源：http://hz.nanxuanxn.top/gtqfqrhcvz.html

[U119] JS：生产构建
来源：http://hz.jinyuanbaomall.cn/gtuftqljau.html

npx vite build
来源：http://hz.cqqwz.cn/gtudrdtcoi.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.tian-w.cn/gtfszqmqau.html

import.meta.env.VITE_API_URL
来源：http://hz.pycfn.com/gtljlelfar.html

================================================================================
来源：http://hz.chenzaomai.com/gtgsytolkk.html

统计汇总
来源：http://hz.birdmap.top/gtpnozujqj.html

================================================================================
来源：http://hz.havefunace.top/gtjophqwbs.html

按语言统计（条）：
来源：http://hz.feifeiyinyue.top/gtavfovnji.html

Python ......... 252
来源：http://hz.wangdashe.top/gthybuoeek.html

PHP ............ 252
来源：http://hz.jinqigfzy.top/gtcvhcqsge.html

JavaScript ..... 252
来源：http://hz.ydzc1.top/gtaettazxn.html

TypeScript ..... 212
来源：http://hz.zdqjudy.top/gtvmykzyjr.html

Java ........... 212
来源：http://hz.havefunace.top/gttayrlast.html

Go ............. 212
来源：http://hz.jianghu66.top/gtsexnsdfx.html

Ruby ........... 212
来源：http://hz.haohaochexian.top/gtulpkdirc.html

C# ............. 212
来源：http://hz.cucudq.cn/gtqyuqdtmf.html

C .............. 30
来源：http://hz.daria6918.cn/gttsqabvtj.html

C++ ............ 30
来源：http://hz.zycfv.cn/gtrzdbcbix.html

SQL ............ 90
来源：http://hz.zhixingplan.top/gtpesluqhr.html

Bash ........... 80
来源：http://hz.guannengcc.top/gtjwgbqxkb.html

Kotlin ......... 15
来源：http://hz.andypj.xyz/gtbjqxrxqb.html

Swift .......... 15
来源：http://hz.iojbl.cn/gtjjydmmfg.html

Lua ............ 10
来源：http://hz.sxryk.cn/gtuzyemzbq.html

Perl ........... 10
来源：http://hz.guannengcc.top/gtamraceco.html

Scala .......... 10
来源：http://hz.guannengcc.top/gtoxljvbdt.html

------------------------------------
来源：http://hz.zhaomingkeji.xyz/gtpohhdwwc.html

合计 ........... 2106 条
来源：http://hz.aibaodan.cn/gtrcpvikeu.html

按章节统计：
来源：http://hz.zhoulong.xyz/gtlzkoiwlk.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.snrcjt.cn/gtggfesfft.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.xinyue.icu/gtdcuvylhh.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.kuanghao11.cn/gthbejlxpc.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.9152youxi.cn/gtdnvjyhye.html


<!-- 参考信息 -->