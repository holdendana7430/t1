代发 wailian999

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2xnwqtzsd.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2qpoktuju.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2tqymrqtc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2njxpkvgg.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2bdvbgadh.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zbumkwnk.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2eaniiiqi.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2kwothxyf.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2bfkuzlvi.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ymqqffum.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2lissbijd.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2ggotojqd.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2puxelzmc.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2mvexmiip.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2rhefmpup.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2aeefklwd.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2zfqynwzz.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ihnzwuvk.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2uajnbhbg.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2iovbxcpi.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2zvokijeg.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2qtimwped.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2bvkyzgov.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2mdiqgoti.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2ttycvnrz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cfcdrumq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bmciczaq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wvrixhhw.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2tedsufpf.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2iikoijug.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2bzivbrwx.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2mkcbqqpe.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2rkjqrziv.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2rufvfhpu.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2bpjfvdhx.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2hldrmohd.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2ajmqnatn.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2odrfiajg.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2chnkttds.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2makgftdc.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2kjfzkrme.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2htoutobs.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2uxuanmrl.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2vaqucgmo.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2ssvzyhbj.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2usihnlpz.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2gtjgzqhn.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2fuspjwva.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2sjwrmyxg.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dpgqggkz.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2ukbmjrvm.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2mpqdeitu.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2bjtkugvg.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2eiyfpmih.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2cwfrxbxm.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2doapgzpz.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2psorrolz.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2nwfwnyye.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2brfxqtth.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2ebdiqobr.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2ylhwkrzl.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2wirqllqt.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2lzazugki.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2npngwvqk.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2gcqgxcok.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2uicuggbk.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2kjqfpuvf.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2vzukxvrc.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2hujjfbmq.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2oufaaqex.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2cdqzaqbu.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2vugveisf.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2tqlwexxk.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2autigkls.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2zlczaqem.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2qktvqtnx.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2yjpguszu.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2kqtbytpl.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2ozqadtob.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2jetdkjro.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2unlilmjs.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2fyfwxkjr.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2wucettrg.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2heclyple.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2wgrvrmhw.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2mrfkridc.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2cqicknjt.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2wawrivyt.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2xfqhfykj.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2zpgievrj.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2kwaogknn.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2azxmfvld.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2hzsztyrp.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2zyegbggc.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2vfzuvgcx.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2jhtftlnl.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2sjtzbbjz.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2qxslxsee.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2drifnuoa.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2ttprotbb.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2kqsjpcff.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2doxnmufv.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2bprmhaos.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2kdxxhkzx.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2gaivdajo.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2pseemniz.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2eumtzfqv.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ukfnubgs.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2iutdhbua.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2ggknmrfi.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2xfeagfdn.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2lxnvofzc.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2texnvfzn.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2oyzzxrbx.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2juufaxfl.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2uamqnhln.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2kxfjbmmn.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2pzcfasch.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2jnbukrdu.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2dgougfjs.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2fiqxnddp.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2znbanrhk.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2kqkgzrip.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xzzepcoa.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2lxlcuemp.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2flltbnmk.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2cyephumk.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2fdukqvph.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2pbcapbdy.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2shrlxzwr.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2vtrgnxhy.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ttneoioc.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2jkzwmqvr.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2abmaovvh.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2yegicate.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2bnlwptfl.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2lbhikkvg.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2dqnwuukv.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2pcjzqeve.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2gbvyedxo.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2cbkyaccd.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2afesbptd.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2twoiebgs.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2qecufwyv.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2toopleud.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2igjzmkbc.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2juedrmty.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2athjbcbt.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2lzpuaoom.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2punvhfho.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2bacpvlll.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2faaayqgg.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2wpzqvthe.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2cvdzqvay.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2ehktwodb.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2yienhele.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2seazdkcc.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2epcdgavz.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2xcmdtvnj.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2fstmjqof.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2pjodfbrp.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2igyquarm.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2qmrryozf.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2hnpyddxx.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2aczyomnp.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2voejkgiu.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2qmoniocb.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2fllappjn.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2xgveazga.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2vkohzjsy.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2bjxyoxyt.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2woxqrquo.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2crobtoyj.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2xyzpkoim.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2ijqpblhl.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2kflgegix.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2auvkilah.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2zrxwoslj.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2unupqoov.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2fgclsrrg.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2otyuxdfp.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2idtffrcp.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2ipcofdtt.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2gzqduarc.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2ekeunpod.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2ekxkpmmr.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2segqluzg.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2gjxyixhy.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2djxiukou.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2wwotgdjm.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2rgsaqgru.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2lbjcoxsg.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2ecpnjozf.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2xrxqhdlb.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2nxygekza.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2nhavqjvw.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2xdwxnvyc.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2hovqmdza.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2kslnmhfl.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2kcjibojg.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2eejzbazc.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2ljphnafc.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2nsxblepq.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2phyjsnbr.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2fxlajpgq.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ymzwogxn.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2smdklmqv.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2vtxdtqog.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2fltaidcw.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2rntiswle.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2rsakqwbk.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2pwwnfsgs.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2thwjzjes.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2gyxybtsg.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2zjhthbty.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2zstyxjzb.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2zedvqizf.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2nibtxxaj.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2sxemmnao.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2beiwepxr.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2licwrxsw.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2tfoaoggp.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2byhdwfmz.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2ghuusdzs.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2gncrcgff.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2vzsdilgi.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2kkorhvpf.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2thxuewaw.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2spdzortq.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2niubkjck.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2nwwnskbb.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2gmfgzjwp.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2kxyixaef.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2yqwbphwk.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2pmdrjibd.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2mwppjwlu.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2tjuhdsae.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2wyfsuwuz.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2bbtnlnwb.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2fzwzcscf.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2xocotjdo.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2onmvhpcp.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2tihbbhgu.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2wffdjtif.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2wknstwmm.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2xlzbnfol.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2vladazhg.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2vrsxwptm.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2ubmavulu.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2hmisichk.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2beglnpfn.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ewyehoqa.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2bnmsuovh.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ndttrokd.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2tjqlwvkd.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2crglwkoj.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2czfzvujy.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2xdogmsqr.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2syebaebd.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2byusdcjg.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2owduqiyz.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2mfieibqd.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2bfzxlpgo.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2dcalklos.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2hyxleyka.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2cjatemsj.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2rcsvfoah.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2kdpbpevi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ykvxhwjm.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2ywgwvdqf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mhfqzawu.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2wrrinxnc.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2salhwuvs.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2uqcaqagq.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2keramwdh.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2qclbolom.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2aloopeyl.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2pcnyelwu.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2xvpzqtbq.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2kqlexrom.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2sosgfjze.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2gtzsdcsj.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2buvwqsce.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2quupdtzw.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2auxnkbfd.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2jfwbpwgc.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2aqgqcagl.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2ibuzlnqg.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2jhblebva.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2amejihwu.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2iucdvevd.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2unykmsqg.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2uatvfjsk.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2edallkxo.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ferzjmro.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2gdzjnfnc.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2bwhdifud.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2hqfundwi.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2rcepwbmj.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2owetfyui.html


<!-- 参考信息 -->