代发 wailian999

[U05] Py：列表去重且保序
来源：http://read.share.fanxiaobao.xyz/Article/details/gmapptcxo.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fanxiaobao.xyz/Article/details/gtbctewcx.sHtML

[U06] Py：合并两个字典
来源：http://baike.fanxiaobao.xyz/Article/details/grenezsnr.sHtML

{**a, **b}
来源：http://mobile.fanxiaobao.xyz/Article/details/gfigapetk.sHtML

[U07] Py：反转字典键值
来源：http://3g.fanxiaobao.xyz/Article/details/ghfltounl.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fanxiaobao.xyz/Article/details/gyqunwnxr.sHtML

[U08] Py：展平二维列表
来源：http://3g.fanxiaobao.xyz/Article/details/gdiulgrvd.sHtML

[y for x in nested for y in x]
来源：http://www.share.fanxiaobao.xyz/Article/details/gezeqouwz.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fanxiaobao.xyz/Article/details/gxszsnpsm.sHtML

max(d, key=d.get)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghexuxiel.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gzximtvtf.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwfpzmjo.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gmijnxwsi.sHtML

(x * 2 for x in arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gzfoyhaih.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fanxiaobao.xyz/Article/details/gjqyrdatl.sHtML

Counter(arr).most_common(3)
来源：http://blog.fanxiaobao.xyz/Article/details/gnogpjwhe.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkjcyoad.sHtML

deque(maxlen=10)
来源：http://mobile.fanxiaobao.xyz/Article/details/glunefrek.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fanxiaobao.xyz/Article/details/gdohajhgp.sHtML

defaultdict(list)
来源：http://3g.fanxiaobao.xyz/Article/details/gohjepkzs.sHtML

[U15] Py：高精度计时
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqacbjbj.sHtML

t = time.perf_counter()
来源：http://wap.fanxiaobao.xyz/Article/details/gttbjliff.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fanxiaobao.xyz/Article/details/glveuodcu.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fanxiaobao.xyz/Article/details/gyebblldq.sHtML

[U17] Py：初始化日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gnawawskw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fanxiaobao.xyz/Article/details/gljhzjkyu.sHtML

[U18] Py：预编译正则
来源：http://mobile.fanxiaobao.xyz/Article/details/ghrhyazws.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/givyqhzfz.sHtML

[U19] Py：正则替换带回调
来源：http://3g.fanxiaobao.xyz/Article/details/gspjpwxfw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fanxiaobao.xyz/Article/details/gsvjloxqr.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fanxiaobao.xyz/Article/details/gyzzalgnt.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fanxiaobao.xyz/Article/details/gebzsahgo.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.fanxiaobao.xyz/Article/details/gckvapsrc.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvenzbdd.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtsenffq.sHtML

list(zip(*m))
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjqlpdul.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fanxiaobao.xyz/Article/details/golxfteaa.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.fanxiaobao.xyz/Article/details/grzkfkggb.sHtML

[U24] Py：路径操作
来源：http://wap.fanxiaobao.xyz/Article/details/guwmgswxs.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxuhtvcq.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gancavrmr.sHtML

csv.DictReader(f)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcztsouwd.sHtML

[U26] Py：并发下载
来源：http://m.share.fanxiaobao.xyz/Article/details/gyerzwryn.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzkxptjn.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjyxposp.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fanxiaobao.xyz/Article/details/gpjlyrhbf.sHtML

[U28] Py：类型别名
来源：http://blog.fanxiaobao.xyz/Article/details/gwnyxhziz.sHtML

UserId = int
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfbynpub.sHtML

[U29] Py：属性校验
来源：http://3g.fanxiaobao.xyz/Article/details/gnwyxbxnf.sHtML

@property 与 @x.setter 配合
来源：http://baike.fanxiaobao.xyz/Article/details/gahjnqfxw.sHtML

[U30] Py：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtqqamce.sHtML

@dataclass(slots=True)
来源：http://baike.fanxiaobao.xyz/Article/details/gskuexsxq.sHtML

[U31] Py：单测
来源：http://blog.fanxiaobao.xyz/Article/details/gbweijpzt.sHtML

python -m pytest -q
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyivrtnhg.sHtML

[U32] Py：代码格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gldkyiopy.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fanxiaobao.xyz/Article/details/gizabhdlk.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqxtarpd.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fanxiaobao.xyz/Article/details/gmmgwxgru.sHtML

[U34] Py：判断编码
来源：http://wap.fanxiaobao.xyz/Article/details/ggagskaon.sHtML

chardet.detect(raw)
来源：http://m.share.fanxiaobao.xyz/Article/details/glfujjaks.sHtML

[U35] Py：发送邮件
来源：http://m.share.fanxiaobao.xyz/Article/details/gljacabsh.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.fanxiaobao.xyz/Article/details/griklhmog.sHtML

[U36] Py：定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gbcejdlrj.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzpuwwbg.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjbujhsc.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.fanxiaobao.xyz/Article/details/gdokdsqnv.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fanxiaobao.xyz/Article/details/gjseafqdz.sHtML

Path(__file__).resolve().parent
来源：http://www.share.fanxiaobao.xyz/Article/details/giibtrmtr.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.fanxiaobao.xyz/Article/details/gacjlwbgj.sHtML

sys.stdout.isatty()
来源：http://www.share.fanxiaobao.xyz/Article/details/gnblkqbdb.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fanxiaobao.xyz/Article/details/guzxlwpbb.sHtML

print("err", file=sys.stderr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtdtgcjg.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.fanxiaobao.xyz/Article/details/gxhrtyrsq.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fanxiaobao.xyz/Article/details/ghborlcgo.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbyehlbz.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmgjwgxu.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/glctfurrg.sHtML

namespace App\Http;
来源：http://blog.fanxiaobao.xyz/Article/details/glcxtyyfc.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvjblfkt.sHtML

declare(strict_types=1);
来源：http://baike.fanxiaobao.xyz/Article/details/gjeunepxo.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkkcjlij.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbgbmzhl.sHtML

[U46] PHP：可空类型
来源：http://blog.fanxiaobao.xyz/Article/details/gahbkwais.sHtML

?string $name = null
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbymzjtd.sHtML

[U47] PHP：联合类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshtapotz.sHtML

int|string $id
来源：http://mobile.fanxiaobao.xyz/Article/details/gpgdhgjpg.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobuzmykl.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjdotqcy.sHtML

[U49] PHP：只读属性
来源：http://wap.fanxiaobao.xyz/Article/details/gxhtxzndz.sHtML

public readonly string $name
来源：http://baike.fanxiaobao.xyz/Article/details/gwxndqdbw.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.fanxiaobao.xyz/Article/details/gjnhwneuz.sHtML

public function __construct(private int $id) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gaymqjfmx.sHtML

[U51] PHP：数组解构
来源：http://mobile.fanxiaobao.xyz/Article/details/gkyyttbjn.sHtML

[$a, $b] = $arr;
来源：http://wap.fanxiaobao.xyz/Article/details/gospmdtur.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvetychci.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvcgibve.sHtML

[U53] PHP：空合并运算符
来源：http://blog.fanxiaobao.xyz/Article/details/glcvmthoy.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.fanxiaobao.xyz/Article/details/gezcyjkkk.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwkzqghdu.sHtML

$obj?->method()
来源：http://www.share.fanxiaobao.xyz/Article/details/gewbqezpk.sHtML

[U55] PHP：match 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgeecdvj.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.fanxiaobao.xyz/Article/details/gcebunoug.sHtML

[U56] PHP：命名参数
来源：http://blog.fanxiaobao.xyz/Article/details/gzhcttqit.sHtML

f(a: 1, b: 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gvskpatmz.sHtML

[U57] PHP：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gzosbzbzl.sHtML

"值: {$a}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gepgnlkzh.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fanxiaobao.xyz/Article/details/gufpgkagc.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/gyaorsmgj.sHtML

[U59] PHP：自定义排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrobwahz.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwswofle.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fanxiaobao.xyz/Article/details/gjrnokcyn.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftozctar.sHtML

[U61] PHP：正则
来源：http://wap.fanxiaobao.xyz/Article/details/godwqszki.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.fanxiaobao.xyz/Article/details/gfmxaocxj.sHtML

[U62] PHP：日期对象
来源：http://mobile.fanxiaobao.xyz/Article/details/gvojcqfvh.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.fanxiaobao.xyz/Article/details/gauyocpod.sHtML

[U63] PHP：文件读写
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdqsmdcil.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.fanxiaobao.xyz/Article/details/gbrrttqip.sHtML

[U64] PHP：目录遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gylsyqynv.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbvkxdag.sHtML

[U65] PHP：会话
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdxgowjp.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdojqfoji.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.fanxiaobao.xyz/Article/details/glcskdryx.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.fanxiaobao.xyz/Article/details/gbjtjbpop.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.fanxiaobao.xyz/Article/details/gstdhuloz.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.fanxiaobao.xyz/Article/details/gazgwojho.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gxyvfvekf.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.fanxiaobao.xyz/Article/details/grmkphcru.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gvnmqwbdr.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjgytdool.sHtML

[U70] PHP：PDO 事务
来源：http://baike.fanxiaobao.xyz/Article/details/gltiacdhj.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjfkzhve.sHtML

[U71] PHP：抛出异常
来源：http://blog.fanxiaobao.xyz/Article/details/gzwigxkhf.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.fanxiaobao.xyz/Article/details/gfllqzuis.sHtML

[U72] PHP：写错误日志
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwjwjqew.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwafiaqkt.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gocirfrmc.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.fanxiaobao.xyz/Article/details/gekhflozj.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/ghikbnslt.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.fanxiaobao.xyz/Article/details/gvdzqjkhg.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfoedqttu.sHtML

composer require psr/container
来源：http://www.share.fanxiaobao.xyz/Article/details/gpszgeigt.sHtML

[U76] PHP：简单路由
来源：http://baike.fanxiaobao.xyz/Article/details/gmjufrtyf.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpejidbv.sHtML

[U77] PHP：模板渲染
来源：http://m.share.fanxiaobao.xyz/Article/details/godnvexih.sHtML

composer require twig/twig
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwticapb.sHtML

[U78] PHP：单元测试
来源：http://blog.fanxiaobao.xyz/Article/details/gnfsmgzvh.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.fanxiaobao.xyz/Article/details/gfugkbohs.sHtML

[U79] PHP：静态分析
来源：http://wap.fanxiaobao.xyz/Article/details/goxzmgjzu.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.fanxiaobao.xyz/Article/details/gtwwmwagu.sHtML

[U80] PHP：代码规范修复
来源：http://baike.fanxiaobao.xyz/Article/details/gdcxpbjfv.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fanxiaobao.xyz/Article/details/gsbujcurj.sHtML

[U81] JS：初始化项目
来源：http://blog.fanxiaobao.xyz/Article/details/gmccxtwwn.sHtML

npm init -y;  npm i express
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimcfudug.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fanxiaobao.xyz/Article/details/gauvxfmwu.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.fanxiaobao.xyz/Article/details/gdubvwqmu.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwedvfqbj.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyqjvxsmq.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.fanxiaobao.xyz/Article/details/gunlxwptf.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzifyvhke.sHtML

[U85] JS：可选链
来源：http://3g.fanxiaobao.xyz/Article/details/gejrnnsum.sHtML

a?.b?.c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztnvongx.sHtML

[U86] JS：空值合并
来源：http://wap.fanxiaobao.xyz/Article/details/gomzhjizd.sHtML

a ?? b
来源：http://3g.fanxiaobao.xyz/Article/details/gotdwxxgm.sHtML

[U87] JS：解构默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzfsweei.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzgzkkis.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fanxiaobao.xyz/Article/details/grvomzsbz.sHtML

{ ...a, ...b }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpxrjpsp.sHtML

[U89] JS：数组去重
来源：http://m.share.fanxiaobao.xyz/Article/details/giifstquq.sHtML

[...new Set(arr)]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaixowwve.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxbprnaz.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gatzjnrzy.sHtML

[U91] JS：对象键值遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gusuqvpnp.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.fanxiaobao.xyz/Article/details/gushsjeym.sHtML

[U92] JS：深拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqgsvugl.sHtML

structuredClone(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gimedfdne.sHtML

[U93] JS：模板字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gvzpgmyxq.sHtML

`共 ${n} 条`
来源：http://3g.fanxiaobao.xyz/Article/details/gryoirrvo.sHtML

[U94] JS：箭头函数
来源：http://wap.fanxiaobao.xyz/Article/details/gmglwshqd.sHtML

const double = x => x * 2;
来源：http://blog.fanxiaobao.xyz/Article/details/gaczmkysu.sHtML

[U95] JS：Promise 包装
来源：http://blog.fanxiaobao.xyz/Article/details/guyoauiac.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfkjnrvr.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fanxiaobao.xyz/Article/details/gxirysive.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqomzqwan.sHtML

[U97] JS：并发请求
来源：http://blog.fanxiaobao.xyz/Article/details/gcejpeviz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvvmbrgq.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gzpyqqyub.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.fanxiaobao.xyz/Article/details/gsrkbuuxc.sHtML

[U99] JS：事件监听
来源：http://wap.fanxiaobao.xyz/Article/details/gzgzqtaur.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goyrhyqlo.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkfcjjtsd.sHtML

document.querySelector(".item")
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvritwha.sHtML

[U101] JS：classList 操作
来源：http://wap.fanxiaobao.xyz/Article/details/gwhsvgmvy.sHtML

el.classList.toggle("active")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxpyhmbs.sHtML

[U102] JS：本地存储
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjtnywde.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.fanxiaobao.xyz/Article/details/gjdwvrlen.sHtML

[U103] JS：定时器
来源：http://wap.fanxiaobao.xyz/Article/details/gvvxzksaw.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gapycgzgw.sHtML

[U104] JS：防抖
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohwuwmvw.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fanxiaobao.xyz/Article/details/giqgiryrl.sHtML

[U105] JS：节流
来源：http://blog.fanxiaobao.xyz/Article/details/gogfmbwyn.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.fanxiaobao.xyz/Article/details/ggtgojgau.sHtML

[U106] JS：日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gqqqecald.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fanxiaobao.xyz/Article/details/glflfwjlv.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxhyccvm.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzffkbic.sHtML

[U108] JS：随机整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gypbecjvj.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnlpjanxx.sHtML

[U109] JS：数组分组
来源：http://mobile.fanxiaobao.xyz/Article/details/gckxloyvm.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fanxiaobao.xyz/Article/details/gflcyniao.sHtML

[U110] JS：数组分块
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyshzdogf.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fanxiaobao.xyz/Article/details/glwjiulfv.sHtML

[U111] JS：对象转 Map
来源：http://3g.fanxiaobao.xyz/Article/details/gmmsafoii.sHtML

new Map(Object.entries(obj))
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmldcnji.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gizjmpwba.sHtML

"7".padStart(3, "0")
来源：http://3g.fanxiaobao.xyz/Article/details/grebkuboc.sHtML

[U113] JS：正则替换全部
来源：http://baike.fanxiaobao.xyz/Article/details/grlcgslwf.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gucrzvdiy.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.fanxiaobao.xyz/Article/details/giopggyty.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdemgytn.sHtML

[U115] JS：生成 UUID
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhdgcpke.sHtML

crypto.randomUUID()
来源：http://baike.fanxiaobao.xyz/Article/details/gomupwumt.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.fanxiaobao.xyz/Article/details/gmgtwxmkn.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gfoocrnog.sHtML

[U117] JS：单元测试
来源：http://blog.fanxiaobao.xyz/Article/details/ggsywicmb.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxylfkcw.sHtML

[U118] JS：开发服务器
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjpkkrho.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gheevlogt.sHtML

[U119] JS：生产构建
来源：http://wap.fanxiaobao.xyz/Article/details/gbgjgtjdj.sHtML

npx vite build
来源：http://baike.fanxiaobao.xyz/Article/details/gzdylobuc.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gquzxeibd.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fanxiaobao.xyz/Article/details/gwuzgvmqg.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gtoxpzriu.sHtML

统计汇总
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvodnary.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gbkjbpsxf.sHtML

按语言统计（条）：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxqwgjhp.sHtML

Python ......... 252
来源：http://mobile.fanxiaobao.xyz/Article/details/ggnequlgg.sHtML

PHP ............ 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfinuaxri.sHtML

JavaScript ..... 252
来源：http://blog.fanxiaobao.xyz/Article/details/gxbfzkpds.sHtML

TypeScript ..... 212
来源：http://baike.fanxiaobao.xyz/Article/details/gcwgtjlfp.sHtML

Java ........... 212
来源：http://blog.fanxiaobao.xyz/Article/details/gahkagmjd.sHtML

Go ............. 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqckezlv.sHtML

Ruby ........... 212
来源：http://www.share.fanxiaobao.xyz/Article/details/ghafztmlk.sHtML

C# ............. 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gofsslyyn.sHtML

C .............. 30
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgllarnz.sHtML

C++ ............ 30
来源：http://3g.fanxiaobao.xyz/Article/details/ggobjfhpn.sHtML

SQL ............ 90
来源：http://baike.fanxiaobao.xyz/Article/details/glgiwioko.sHtML

Bash ........... 80
来源：http://wap.fanxiaobao.xyz/Article/details/gsxzghvff.sHtML

Kotlin ......... 15
来源：http://mobile.fanxiaobao.xyz/Article/details/gxahlvngu.sHtML

Swift .......... 15
来源：http://baike.fanxiaobao.xyz/Article/details/geflgxwmm.sHtML

Lua ............ 10
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbkejidh.sHtML

Perl ........... 10
来源：http://wap.fanxiaobao.xyz/Article/details/gwsrqsjki.sHtML

Scala .......... 10
来源：http://blog.fanxiaobao.xyz/Article/details/ghwtsdlbg.sHtML

------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvtretsf.sHtML

合计 ........... 2106 条
来源：http://3g.fanxiaobao.xyz/Article/details/gbtvweeoj.sHtML

按章节统计：
来源：http://wap.fanxiaobao.xyz/Article/details/gxoagvlxg.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.fanxiaobao.xyz/Article/details/gefjxwcdv.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gziarlnnt.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.fanxiaobao.xyz/Article/details/gaiqxogtm.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwtqgmgvo.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmcylgeb.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxbdbbcv.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/gnfxmfmgj.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.fanxiaobao.xyz/Article/details/gsufdubwn.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gbaswxzsq.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.fanxiaobao.xyz/Article/details/geimmroyg.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunigqhfq.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjkxcdwn.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/guazkwfmg.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.fanxiaobao.xyz/Article/details/guxthvobc.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.fanxiaobao.xyz/Article/details/gvfaiwyxv.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gixgaecfq.sHtML

Q SQL 专题                              90
来源：http://3g.fanxiaobao.xyz/Article/details/gaqmsnuph.sHtML

R Bash 专题                             80
来源：http://3g.fanxiaobao.xyz/Article/details/ggxqdumzz.sHtML

S C / C++ 专题                          60
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbxvsohh.sHtML

T 其他语言补充                          60
来源：http://3g.fanxiaobao.xyz/Article/details/gjrnqnrvd.sHtML

U 高频实用片段                         120
来源：http://www.blog.fanxiaobao.xyz/Article/details/grolppbuj.sHtML

------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/glmffdyhl.sHtML

合计                                  2106 条
来源：http://blog.fanxiaobao.xyz/Article/details/geuhshsan.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/ghhfwapgk.sHtML

使用提醒
来源：http://wap.fanxiaobao.xyz/Article/details/gpajojgem.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gvqobmmbg.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.fanxiaobao.xyz/Article/details/gfbiziake.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.fanxiaobao.xyz/Article/details/glcthsfki.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.fanxiaobao.xyz/Article/details/gvknwvadp.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.fanxiaobao.xyz/Article/details/gvxnujtao.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.fanxiaobao.xyz/Article/details/gnduebjja.sHtML

—— 文件结束 ——
来源：http://mobile.fanxiaobao.xyz/Article/details/gpqybeuxy.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbdafsul.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwjxhigd.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.fanxiaobao.xyz/Article/details/gttjwpwui.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkpgypqcf.sHtML

【收录内容】
来源：http://wap.fanxiaobao.xyz/Article/details/gkdhsrhnw.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.fanxiaobao.xyz/Article/details/gbdejiljo.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.fanxiaobao.xyz/Article/details/gvjcytnkz.sHtML

SQL · Bash · C · C++
来源：http://wap.fanxiaobao.xyz/Article/details/gawqzpzlu.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.fanxiaobao.xyz/Article/details/gyxrkkpwy.sHtML

【使用说明】
来源：http://read.share.fanxiaobao.xyz/Article/details/gavdxegkp.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsnfqylgd.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.fanxiaobao.xyz/Article/details/grkbfqsrq.sHtML


<!-- 参考信息 -->