代发 wailian999

[U07] Py：反转字典键值
来源：http://3g.fanxiaobao.xyz/Article/details/gsfboepac.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fanxiaobao.xyz/Article/details/gccecfpes.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gyffjaqnq.sHtML

[y for x in nested for y in x]
来源：http://read.share.fanxiaobao.xyz/Article/details/gidajytgi.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqniucia.sHtML

max(d, key=d.get)
来源：http://wap.fanxiaobao.xyz/Article/details/gtdqoxayu.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitmiccfz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fanxiaobao.xyz/Article/details/gggtmmnzn.sHtML

[U11] Py：生成器表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gbahbiwqb.sHtML

(x * 2 for x in arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gurxcmlos.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fanxiaobao.xyz/Article/details/gafthqhys.sHtML

Counter(arr).most_common(3)
来源：http://wap.fanxiaobao.xyz/Article/details/gyncpbhmv.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtpuhiwbm.sHtML

deque(maxlen=10)
来源：http://baike.fanxiaobao.xyz/Article/details/ghfoliinz.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fanxiaobao.xyz/Article/details/gfhkeydeo.sHtML

defaultdict(list)
来源：http://baike.fanxiaobao.xyz/Article/details/gamfotqdh.sHtML

[U15] Py：高精度计时
来源：http://mobile.fanxiaobao.xyz/Article/details/gfyurlncj.sHtML

t = time.perf_counter()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxyygnao.sHtML

[U16] Py：命令行参数解析
来源：http://3g.fanxiaobao.xyz/Article/details/gygkqgiyj.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkyifyhs.sHtML

[U17] Py：初始化日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzhzmxet.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvigihgfb.sHtML

[U18] Py：预编译正则
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdxvcntd.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjwuquqs.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fanxiaobao.xyz/Article/details/gqcmdnkdh.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwibajwah.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fanxiaobao.xyz/Article/details/gfsneiisu.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fanxiaobao.xyz/Article/details/gnqakzynp.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.fanxiaobao.xyz/Article/details/gvylarrly.sHtML

@contextlib.contextmanager
来源：http://read.share.fanxiaobao.xyz/Article/details/gqgxpkfyv.sHtML

[U22] Py：矩阵转置
来源：http://3g.fanxiaobao.xyz/Article/details/gvmynoxnm.sHtML

list(zip(*m))
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfzsisdu.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwnfjhsv.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fanxiaobao.xyz/Article/details/gcqtpquuf.sHtML

[U24] Py：路径操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlmntogo.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.fanxiaobao.xyz/Article/details/gpmwealxi.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdnzazer.sHtML

csv.DictReader(f)
来源：http://3g.fanxiaobao.xyz/Article/details/gtletlhhe.sHtML

[U26] Py：并发下载
来源：http://www.blog.fanxiaobao.xyz/Article/details/guanhamww.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.fanxiaobao.xyz/Article/details/giotkdarv.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fanxiaobao.xyz/Article/details/glxwyzqau.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fanxiaobao.xyz/Article/details/gmywjkhzq.sHtML

[U28] Py：类型别名
来源：http://wap.fanxiaobao.xyz/Article/details/gubfsstdi.sHtML

UserId = int
来源：http://wap.fanxiaobao.xyz/Article/details/gizciprgg.sHtML

[U29] Py：属性校验
来源：http://3g.fanxiaobao.xyz/Article/details/gixggmmdh.sHtML

@property 与 @x.setter 配合
来源：http://baike.fanxiaobao.xyz/Article/details/gwdvytpne.sHtML

[U30] Py：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/gkncepmha.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzhoqwbo.sHtML

[U31] Py：单测
来源：http://mobile.fanxiaobao.xyz/Article/details/grfycsleg.sHtML

python -m pytest -q
来源：http://blog.fanxiaobao.xyz/Article/details/gxkfshhkf.sHtML

[U32] Py：代码格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gwrcfdxtg.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fanxiaobao.xyz/Article/details/gpxizsghi.sHtML

[U33] Py：打包发布
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxfnucfq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fanxiaobao.xyz/Article/details/gswxtujpr.sHtML

[U34] Py：判断编码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrxubeta.sHtML

chardet.detect(raw)
来源：http://3g.fanxiaobao.xyz/Article/details/gvzuxgdgw.sHtML

[U35] Py：发送邮件
来源：http://wap.fanxiaobao.xyz/Article/details/gayaobvxm.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fanxiaobao.xyz/Article/details/gnuadiuld.sHtML

[U36] Py：定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqrkfnlo.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.fanxiaobao.xyz/Article/details/gqssahbba.sHtML

[U37] Py：读写 Excel
来源：http://www.share.fanxiaobao.xyz/Article/details/gooqitcgb.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.fanxiaobao.xyz/Article/details/gqsmrkrkz.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjiuikpn.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhpipsrq.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwkuzeka.sHtML

sys.stdout.isatty()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gliixlcit.sHtML

[U40] Py：打印到标准错误
来源：http://wap.fanxiaobao.xyz/Article/details/gstmjlsre.sHtML

print("err", file=sys.stderr)
来源：http://wap.fanxiaobao.xyz/Article/details/gvgnijdks.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.fanxiaobao.xyz/Article/details/gzxsnifmi.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.fanxiaobao.xyz/Article/details/gozbgklel.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmjrcowe.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glcamdknt.sHtML

[U43] PHP：声明命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gjteqaqtq.sHtML

namespace App\Http;
来源：http://m.share.fanxiaobao.xyz/Article/details/giwpwcvln.sHtML

[U44] PHP：开启严格类型
来源：http://baike.fanxiaobao.xyz/Article/details/ghsbtvvdy.sHtML

declare(strict_types=1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gobcmfasp.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmgniohi.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/giahwroqm.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyugawesb.sHtML

?string $name = null
来源：http://wap.fanxiaobao.xyz/Article/details/gcnyoiwth.sHtML

[U47] PHP：联合类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/glovyedib.sHtML

int|string $id
来源：http://3g.fanxiaobao.xyz/Article/details/gcaaakxhq.sHtML

[U48] PHP：纯枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gnihpyuli.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gtxsgdtwj.sHtML

[U49] PHP：只读属性
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhmftqun.sHtML

public readonly string $name
来源：http://baike.fanxiaobao.xyz/Article/details/gyxwrhvux.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtazenbw.sHtML

public function __construct(private int $id) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gxtdiurdl.sHtML

[U51] PHP：数组解构
来源：http://m.share.fanxiaobao.xyz/Article/details/gxpxhiozf.sHtML

[$a, $b] = $arr;
来源：http://baike.fanxiaobao.xyz/Article/details/gagdufmrg.sHtML

[U52] PHP：箭头函数
来源：http://wap.fanxiaobao.xyz/Article/details/ggpfkrpso.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.fanxiaobao.xyz/Article/details/gieduvlhc.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowegycil.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmjdocch.sHtML

[U54] PHP：空安全调用
来源：http://baike.fanxiaobao.xyz/Article/details/gfbmzdske.sHtML

$obj?->method()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvrjywbc.sHtML

[U55] PHP：match 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwkrfwlz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.fanxiaobao.xyz/Article/details/gyyekawsi.sHtML

[U56] PHP：命名参数
来源：http://wap.fanxiaobao.xyz/Article/details/gmlpbsukl.sHtML

f(a: 1, b: 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gkzcbshvw.sHtML

[U57] PHP：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/ggiadtxtg.sHtML

"值: {$a}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gctpddmgu.sHtML

[U58] PHP：数组三件套
来源：http://m.share.fanxiaobao.xyz/Article/details/gkaueocoa.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/gsrlslqqf.sHtML

[U59] PHP：自定义排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gaquoyvgr.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/grqrdjoxq.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwbdmvir.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsodmqkod.sHtML

[U61] PHP：正则
来源：http://mobile.fanxiaobao.xyz/Article/details/gyremzjsr.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkrtyihfh.sHtML

[U62] PHP：日期对象
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtoqcxkw.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.fanxiaobao.xyz/Article/details/gncrcklmw.sHtML

[U63] PHP：文件读写
来源：http://mobile.fanxiaobao.xyz/Article/details/gycdxxzax.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzefajwvq.sHtML

[U64] PHP：目录遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfduznds.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfchqxnq.sHtML

[U65] PHP：会话
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtstsnuic.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/giyuokwjr.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guoyveyyo.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.fanxiaobao.xyz/Article/details/gksefqere.sHtML

[U67] PHP：处理文件上传
来源：http://blog.fanxiaobao.xyz/Article/details/gmghkfomm.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjlzcxsij.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxnbwgrxc.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.fanxiaobao.xyz/Article/details/goatbxxlo.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.fanxiaobao.xyz/Article/details/guayglnoa.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.fanxiaobao.xyz/Article/details/ggiicecet.sHtML

[U70] PHP：PDO 事务
来源：http://baike.fanxiaobao.xyz/Article/details/gcseykaaj.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.fanxiaobao.xyz/Article/details/gfbbhpsvq.sHtML

[U71] PHP：抛出异常
来源：http://3g.fanxiaobao.xyz/Article/details/gikttkbwj.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfhglwsy.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gieamlpru.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.fanxiaobao.xyz/Article/details/gojfyjsqt.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwpxbhoz.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.fanxiaobao.xyz/Article/details/gtrmbinxu.sHtML

[U74] PHP：读取环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gqqhvrmvx.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fanxiaobao.xyz/Article/details/grafzzmlb.sHtML

[U75] PHP：依赖注入
来源：http://baike.fanxiaobao.xyz/Article/details/gifnwqbzp.sHtML

composer require psr/container
来源：http://m.share.fanxiaobao.xyz/Article/details/gqsbpxfwb.sHtML

[U76] PHP：简单路由
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmkpixdm.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.fanxiaobao.xyz/Article/details/gbxzutyhb.sHtML

[U77] PHP：模板渲染
来源：http://3g.fanxiaobao.xyz/Article/details/gswydvopk.sHtML

composer require twig/twig
来源：http://wap.fanxiaobao.xyz/Article/details/gpkypufuq.sHtML

[U78] PHP：单元测试
来源：http://mobile.fanxiaobao.xyz/Article/details/gmaknkvgh.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.fanxiaobao.xyz/Article/details/ginvvedck.sHtML

[U79] PHP：静态分析
来源：http://www.share.fanxiaobao.xyz/Article/details/gudvuryvy.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.fanxiaobao.xyz/Article/details/gpgclhfhm.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fanxiaobao.xyz/Article/details/gojymmxen.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxgxvann.sHtML

[U81] JS：初始化项目
来源：http://baike.fanxiaobao.xyz/Article/details/gqtkcsaip.sHtML

npm init -y;  npm i express
来源：http://wap.fanxiaobao.xyz/Article/details/gcsstuxsd.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fanxiaobao.xyz/Article/details/gvbivzzhm.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.fanxiaobao.xyz/Article/details/gzbnesths.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.fanxiaobao.xyz/Article/details/gejqteflr.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.fanxiaobao.xyz/Article/details/glswjovpn.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.fanxiaobao.xyz/Article/details/ghoifjjuv.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.fanxiaobao.xyz/Article/details/gagnyautz.sHtML

[U85] JS：可选链
来源：http://blog.fanxiaobao.xyz/Article/details/gtwxhwyvl.sHtML

a?.b?.c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvxoxxpu.sHtML

[U86] JS：空值合并
来源：http://baike.fanxiaobao.xyz/Article/details/gsvchgfvg.sHtML

a ?? b
来源：http://m.share.fanxiaobao.xyz/Article/details/gudzfjkuo.sHtML

[U87] JS：解构默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqhgrznn.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.fanxiaobao.xyz/Article/details/glmkbqdfq.sHtML

[U88] JS：对象展开合并
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpbghcff.sHtML

{ ...a, ...b }
来源：http://wap.fanxiaobao.xyz/Article/details/gnehblwtb.sHtML

[U89] JS：数组去重
来源：http://mobile.fanxiaobao.xyz/Article/details/gcwramigo.sHtML

[...new Set(arr)]
来源：http://blog.fanxiaobao.xyz/Article/details/gdhntszhf.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gniugbwtx.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqblcrvsx.sHtML

[U91] JS：对象键值遍历
来源：http://3g.fanxiaobao.xyz/Article/details/ggmpykoqs.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.fanxiaobao.xyz/Article/details/gkyemfqby.sHtML

[U92] JS：深拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbzjzltb.sHtML

structuredClone(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfhhmayom.sHtML

[U93] JS：模板字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gqpedtnsh.sHtML

`共 ${n} 条`
来源：http://3g.fanxiaobao.xyz/Article/details/gxeyyvywo.sHtML

[U94] JS：箭头函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtdefmzm.sHtML

const double = x => x * 2;
来源：http://baike.fanxiaobao.xyz/Article/details/gobfhaali.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geuseooxj.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyoddwsip.sHtML

[U96] JS：async/await 与异常
来源：http://3g.fanxiaobao.xyz/Article/details/gdsvmmivo.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjmpqpkf.sHtML

[U97] JS：并发请求
来源：http://blog.fanxiaobao.xyz/Article/details/gycyuvswh.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjpjwghq.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/geqxyczwb.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaudfzimu.sHtML

[U99] JS：事件监听
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghdgxcjkb.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gfppmldhi.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fanxiaobao.xyz/Article/details/ggndbmkzt.sHtML

document.querySelector(".item")
来源：http://blog.fanxiaobao.xyz/Article/details/gantrfhlk.sHtML

[U101] JS：classList 操作
来源：http://3g.fanxiaobao.xyz/Article/details/gctjeaapd.sHtML

el.classList.toggle("active")
来源：http://mobile.fanxiaobao.xyz/Article/details/giouliydk.sHtML

[U102] JS：本地存储
来源：http://baike.fanxiaobao.xyz/Article/details/gdcpnfzhl.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxlwlpxvd.sHtML

[U103] JS：定时器
来源：http://m.share.fanxiaobao.xyz/Article/details/gtyiuedhz.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdafiihzc.sHtML

[U104] JS：防抖
来源：http://baike.fanxiaobao.xyz/Article/details/gevwrjyiy.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtlzrfkl.sHtML

[U105] JS：节流
来源：http://m.share.fanxiaobao.xyz/Article/details/gonglhtpw.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gobkkdjxk.sHtML

[U106] JS：日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/grunfpdqo.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.fanxiaobao.xyz/Article/details/goctdmogv.sHtML

[U107] JS：数字千分位
来源：http://blog.fanxiaobao.xyz/Article/details/gkhzpnbig.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpyidkeeo.sHtML

[U108] JS：随机整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gogshyiha.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfnhbcvq.sHtML

[U109] JS：数组分组
来源：http://m.share.fanxiaobao.xyz/Article/details/gqrtzhbpj.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghfcpkapb.sHtML

[U110] JS：数组分块
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsztsecvn.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fanxiaobao.xyz/Article/details/ghuxqobla.sHtML

[U111] JS：对象转 Map
来源：http://blog.fanxiaobao.xyz/Article/details/gexgfwpbh.sHtML

new Map(Object.entries(obj))
来源：http://m.share.fanxiaobao.xyz/Article/details/gbcfamlgo.sHtML

[U112] JS：字符串补位
来源：http://wap.fanxiaobao.xyz/Article/details/gihtzdccq.sHtML

"7".padStart(3, "0")
来源：http://wap.fanxiaobao.xyz/Article/details/gtvsdmyhd.sHtML

[U113] JS：正则替换全部
来源：http://baike.fanxiaobao.xyz/Article/details/gbownncbj.sHtML

s.replaceAll("a", "b")
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxnkkgyy.sHtML

[U114] JS：JSON 深比较
来源：http://blog.fanxiaobao.xyz/Article/details/glkgysjsh.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxailazd.sHtML

[U115] JS：生成 UUID
来源：http://read.share.fanxiaobao.xyz/Article/details/ggpkaspvp.sHtML

crypto.randomUUID()
来源：http://baike.fanxiaobao.xyz/Article/details/gncvjnuuc.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gougejsby.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fanxiaobao.xyz/Article/details/goxlmeols.sHtML

[U117] JS：单元测试
来源：http://blog.fanxiaobao.xyz/Article/details/grmkcoiwq.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.fanxiaobao.xyz/Article/details/ghqfqtcgz.sHtML

[U118] JS：开发服务器
来源：http://mobile.fanxiaobao.xyz/Article/details/gpteatodr.sHtML

npm i -D vite;  npx vite
来源：http://3g.fanxiaobao.xyz/Article/details/gvxwwpiux.sHtML

[U119] JS：生产构建
来源：http://wap.fanxiaobao.xyz/Article/details/gknihpjfl.sHtML

npx vite build
来源：http://3g.fanxiaobao.xyz/Article/details/gqqwlflqt.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fanxiaobao.xyz/Article/details/gocpwmhvf.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fanxiaobao.xyz/Article/details/glspesxri.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gpozuiafc.sHtML

统计汇总
来源：http://mobile.fanxiaobao.xyz/Article/details/gnluufxxf.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gbofmlkwm.sHtML

按语言统计（条）：
来源：http://wap.fanxiaobao.xyz/Article/details/gzidpshxr.sHtML

Python ......... 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfbebndq.sHtML

PHP ............ 252
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgbhftui.sHtML

JavaScript ..... 252
来源：http://www.share.fanxiaobao.xyz/Article/details/ghsxmetmi.sHtML

TypeScript ..... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geyhhftdm.sHtML

Java ........... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmfdpwbi.sHtML

Go ............. 212
来源：http://blog.fanxiaobao.xyz/Article/details/gqrvvcmqn.sHtML

Ruby ........... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gcuututxs.sHtML

C# ............. 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzqilduc.sHtML

C .............. 30
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofqgwjby.sHtML

C++ ............ 30
来源：http://baike.fanxiaobao.xyz/Article/details/gldkchhxb.sHtML

SQL ............ 90
来源：http://www.share.fanxiaobao.xyz/Article/details/glfmwontx.sHtML

Bash ........... 80
来源：http://wap.fanxiaobao.xyz/Article/details/gomrslisz.sHtML

Kotlin ......... 15
来源：http://baike.fanxiaobao.xyz/Article/details/gvpjwfimj.sHtML

Swift .......... 15
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjmcbxmh.sHtML

Lua ............ 10
来源：http://3g.fanxiaobao.xyz/Article/details/gnnsohjqq.sHtML

Perl ........... 10
来源：http://read.share.fanxiaobao.xyz/Article/details/gbepvyjrx.sHtML

Scala .......... 10
来源：http://m.share.fanxiaobao.xyz/Article/details/grnihcovy.sHtML

------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/giprvgppk.sHtML

合计 ........... 2106 条
来源：http://mobile.fanxiaobao.xyz/Article/details/guvdmqkpj.sHtML

按章节统计：
来源：http://m.share.fanxiaobao.xyz/Article/details/gppbqyzut.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.fanxiaobao.xyz/Article/details/gliqztyal.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/gzyaoocty.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/gkfvlbzxj.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.fanxiaobao.xyz/Article/details/greeemxck.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybqtohdj.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxbmykwn.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/gbpktsyqy.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.fanxiaobao.xyz/Article/details/gppjhaszq.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gqcbthpji.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwyrcaqdi.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gddbtpmai.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gakfdqgno.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/goodrkoai.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfevkkabj.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.fanxiaobao.xyz/Article/details/gdaedfihw.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/givqfqqgh.sHtML

Q SQL 专题                              90
来源：http://3g.fanxiaobao.xyz/Article/details/gydbuawbu.sHtML

R Bash 专题                             80
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbzjssxo.sHtML

S C / C++ 专题                          60
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjrnlvrt.sHtML

T 其他语言补充                          60
来源：http://3g.fanxiaobao.xyz/Article/details/gvvwhulir.sHtML

U 高频实用片段                         120
来源：http://m.share.fanxiaobao.xyz/Article/details/gcybjufuz.sHtML

------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gowncmyel.sHtML

合计                                  2106 条
来源：http://blog.fanxiaobao.xyz/Article/details/ggxelfilx.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gulwdgves.sHtML

使用提醒
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmdsdjkz.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdckvrys.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.fanxiaobao.xyz/Article/details/gxfzykcym.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnljfogmi.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.fanxiaobao.xyz/Article/details/ggwspgypx.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfqqlbvc.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.fanxiaobao.xyz/Article/details/gdelawyed.sHtML

—— 文件结束 ——
来源：http://read.share.fanxiaobao.xyz/Article/details/gitldyazk.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gtayjmycv.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.fanxiaobao.xyz/Article/details/gsundeglj.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyfhohoi.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ggneiaszv.sHtML

【收录内容】
来源：http://wap.fanxiaobao.xyz/Article/details/ggllysfmp.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.fanxiaobao.xyz/Article/details/ginfqmbfx.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.fanxiaobao.xyz/Article/details/gofwfwuwq.sHtML

SQL · Bash · C · C++
来源：http://3g.fanxiaobao.xyz/Article/details/gurvilsjt.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.fanxiaobao.xyz/Article/details/gfvoqogvi.sHtML

【使用说明】
来源：http://read.share.fanxiaobao.xyz/Article/details/gpksuiqdj.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.fanxiaobao.xyz/Article/details/gbjpdltnr.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.fanxiaobao.xyz/Article/details/gxdihqkhl.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.fanxiaobao.xyz/Article/details/gejnqoyri.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.fanxiaobao.xyz/Article/details/grzlcfjre.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfmhgavjp.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.fanxiaobao.xyz/Article/details/gfigcqogf.sHtML


<!-- 参考信息 -->