代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2rfplgkqg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cobhipdd.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2nnmcnnbi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wfnspyld.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2lehwrukn.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2frrqatpt.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2wvfjjgcm.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2armqgmsv.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2osqqxftf.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2qljvnpzh.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2cjuruprz.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2mvnbiftf.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2iyrqisox.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2dqnufrbr.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2apxmfmbs.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2avvldyje.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2qrhgrzep.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2mtxcuulj.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2imztmapm.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2ixgzkxvc.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2ysjvxura.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2lietiflk.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2evqwipdv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2hegqcrni.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ouvrpaux.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2kktgqhvo.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2osaufmgu.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zmdttdor.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2ayipigig.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2fkbvukgt.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2agcegkva.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2yfihqcrk.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2qjsevcwv.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2axclojyk.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2xwfsxqmg.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2wwhovbwq.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2amfbllmn.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2gzqwyqpc.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2tmlgnpnt.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2voacwwsd.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2fextozmn.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2ejfwcpcm.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2tpvtikku.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2ajdmkhyq.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2lvmplpzg.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2whjdshln.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2mhwpqpkv.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2eqvlknel.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2hzkmrpww.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2xkjdthrn.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2jmpxvftt.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2mnvbkwtb.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2mubpdfny.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2mtnxlscp.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2zwsoecox.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2mklfmebl.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2jpkiyguh.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2qonihexd.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2pszrpfbl.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2qlsrcotf.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2sbpjwbcw.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2xviqloxj.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2xejrmlxh.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2aatemumg.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2mdrmhjmc.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2sugjbhsh.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ihssnfkf.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2vfsdkuln.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2leshxwex.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2ooqadrcy.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2tsjzphrb.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2jvqgarxi.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2nqxactfi.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2rrsydndc.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2dluowyxv.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2fhhjhpzq.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2acbkmuen.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2gzxsjsdb.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2depeswor.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2yamtubrg.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2izrvarte.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2tnyrzgjp.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2sjylcsvg.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2akdfiscn.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2omwiathy.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2nywjsifg.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2svwkoxto.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2prqneizc.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2mgtmoxqk.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2vxnlqnmw.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2ccoltlly.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2tdqsxgic.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2tcecdbqz.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2atwkiimw.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2oddcoptp.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2pkelhdnp.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2sjgqmrra.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2xqworgep.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2osltzwku.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2gdxjeqok.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2rizuwhfz.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2ytxwmeyp.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2xuudjnel.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dpogjuqb.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2zxkywczt.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2zqwekftk.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2popamlae.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2mqcjwmtq.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2vxnwnsga.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2xawyukew.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2scypeyks.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2jfuvznuw.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2sapiioqy.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2cccdzmsk.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2koqfhkvl.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2uvobrchm.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2sxxtbqnk.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2ikzkvlpj.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2irieawua.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rograqpz.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2jjsuawof.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2cwiilieu.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2uzlerftu.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2olazvyac.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2lbqsufrs.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2ffzcmhfs.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2lzdayuaf.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2gcmsabpu.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2qdhrulqt.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2legfnwtt.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jukiqlwr.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2ninjahem.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2exhroqgm.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wuawltlb.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2onoxiaip.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2sbnkuotn.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2kakuamdx.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2kvpxpbrd.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2noduuwms.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2zaxerzrf.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2wohzrflw.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2cusvaowg.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2wqtcbksd.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2qdswqjte.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2osywcedz.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2hlwlxncj.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2kpyrizhc.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2lsrjlxgt.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2lslhkwys.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2rewaumgq.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2yfftmqjz.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2sgxdmwod.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2whputqog.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2ovzdxtbo.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2tugvgocj.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2tfeshach.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2dtnfnilm.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2bfsueped.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2xwwrviyw.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2vxhcjemf.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2xjhgpqln.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2xdceqqwx.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2qqrgzqjy.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2ybgvflwz.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2oayepykn.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2ciwgltkc.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2esgnjytx.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2rsrtevfi.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2auxwcypc.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2digxkytv.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2mbmdelro.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2xqbamdxu.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2phsoubxz.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2nbrhakta.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2porkklhu.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2nhjkefrv.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2niuigdji.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2nhkznpbn.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2cjxzkdxo.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2fcsfhoma.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2cdbcqsjl.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2zmtzlkwt.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2sqbjmytz.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2vcqeaqqt.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nsutcpyc.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2qjgxjgog.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2gnnhoukv.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pcsjyyly.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2anbqmzug.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2miklujnp.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2tpawrnbi.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2vzpfmlyr.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2kztgvsyc.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2xalvlonv.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2izcrhdkx.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2umugitzh.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2tbdojqer.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2hgpvmfyw.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2mfzglxaz.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2ljeqcyab.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2aqkdooyz.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2skaflenk.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2dvgvdhdp.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2jksdcwwz.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2dedayplo.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2pdnnauhu.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2fmshkxsy.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2acpzocwp.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2mprtwgep.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2hbqerjbe.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2vpghqazw.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2lquqdkny.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2ukzircpy.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2jaulofry.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2kgmsdgqn.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2jrkvraqz.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2yxgyniyd.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2oejtzyrv.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2epmcgnsa.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2zravhels.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2nqiyctzt.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ezvowsno.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2hyolicih.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2taubijuo.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2hxquwugo.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2wprmfvwz.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2fbyokhdz.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ibqmernm.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2zvdukydu.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2fkijwyus.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2diutmikn.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2zbzllknq.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2wfobkkdq.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ksyppuzl.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2jwmhnphu.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ivfwspob.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2wbosnzqa.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2cchtyzji.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2ryrwpoua.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2rnktrjdy.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2wnzecife.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2flhlmmwa.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2jloysubi.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2rdzoouwv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lruyzwub.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2pwbkpabf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xdlbvgpr.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2jrionjus.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2qjyroqem.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2agasqidg.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2ksujhbgq.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2nanqbpqo.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2wlumvwzz.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2kouksvqs.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2voasfdgo.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2remgvfie.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2vticozsd.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2rcmqicrs.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2dwlxwrhw.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2raiuduyk.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2fcvbfimq.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2wvudrpja.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2xurngggk.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2dptnapzb.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2juphkhpt.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2yhkqcwpx.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2vuusmsca.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2bwjofhcg.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2brdzaude.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2wwbiqajn.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2pnyrlryv.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2optoeval.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2ohgtvbyu.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2sofwxvxt.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2fpqdchkk.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2ajabktef.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2gxxkcwrj.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2anlhowcl.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2fwfdbmlm.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2yodjgwrd.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2kpusmuut.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2eiaiiheu.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2oqqyjqxf.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2jiwumbhg.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2kllkapbi.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2rqmmbztm.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2sfncdpol.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2mkvepqeb.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2qyzxpvrc.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2vbmpquma.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2lzoevwma.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2xsrgukgp.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2doccorrw.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2vrwmyhvt.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2aftzqefb.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2pprfypos.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2odcgaknn.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2jjiciqij.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2aiizyufv.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2ajjsbrhp.html


<!-- 参考信息 -->