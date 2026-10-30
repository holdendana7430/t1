代发 wailian999

[U09] Py：字典取最大值的键
来源：http://wap.fanxiaobao.xyz/Article/details/gwrevppvc.sHtML

max(d, key=d.get)
来源：http://3g.fanxiaobao.xyz/Article/details/gaahfywst.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqayovuh.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fanxiaobao.xyz/Article/details/gjmjolbbo.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grthmdtgq.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbxhauxa.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fanxiaobao.xyz/Article/details/glgovotsq.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtgrffqkj.sHtML

[U13] Py：固定长度队列
来源：http://3g.fanxiaobao.xyz/Article/details/gtvgssjbe.sHtML

deque(maxlen=10)
来源：http://blog.fanxiaobao.xyz/Article/details/gympupzwc.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtbhubox.sHtML

defaultdict(list)
来源：http://3g.fanxiaobao.xyz/Article/details/gvncrjzqn.sHtML

[U15] Py：高精度计时
来源：http://wap.fanxiaobao.xyz/Article/details/gfgbrfihj.sHtML

t = time.perf_counter()
来源：http://mobile.fanxiaobao.xyz/Article/details/grpuffgvg.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnoerbwav.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fanxiaobao.xyz/Article/details/grizbxhdr.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmgxotomo.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.fanxiaobao.xyz/Article/details/gqtoixhez.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghidpnpgq.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdachumr.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fanxiaobao.xyz/Article/details/gjdzgulia.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.fanxiaobao.xyz/Article/details/glufzwxmp.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fanxiaobao.xyz/Article/details/giupnokmg.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhzgnmhi.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fanxiaobao.xyz/Article/details/gjeunyoti.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjicrkret.sHtML

[U22] Py：矩阵转置
来源：http://baike.fanxiaobao.xyz/Article/details/gkewwxmtl.sHtML

list(zip(*m))
来源：http://3g.fanxiaobao.xyz/Article/details/grzssgxyy.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fanxiaobao.xyz/Article/details/gluorijyj.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fanxiaobao.xyz/Article/details/gswgsbxyr.sHtML

[U24] Py：路径操作
来源：http://wap.fanxiaobao.xyz/Article/details/glqntlkog.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fanxiaobao.xyz/Article/details/gipzzyfex.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.fanxiaobao.xyz/Article/details/gzatbqgol.sHtML

csv.DictReader(f)
来源：http://www.share.fanxiaobao.xyz/Article/details/grkcbfxbt.sHtML

[U26] Py：并发下载
来源：http://www.share.fanxiaobao.xyz/Article/details/gwcjbmunf.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzygurbzm.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxjhdzoj.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.fanxiaobao.xyz/Article/details/gskpvktso.sHtML

[U28] Py：类型别名
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqpeknqk.sHtML

UserId = int
来源：http://m.share.fanxiaobao.xyz/Article/details/grnjbzklk.sHtML

[U29] Py：属性校验
来源：http://blog.fanxiaobao.xyz/Article/details/gprubjtpb.sHtML

@property 与 @x.setter 配合
来源：http://baike.fanxiaobao.xyz/Article/details/gscvufaiu.sHtML

[U30] Py：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/gsfvmbujk.sHtML

@dataclass(slots=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmazsuctk.sHtML

[U31] Py：单测
来源：http://wap.fanxiaobao.xyz/Article/details/guaigxlai.sHtML

python -m pytest -q
来源：http://blog.fanxiaobao.xyz/Article/details/gmvagazkr.sHtML

[U32] Py：代码格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gobguezkf.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmaptdop.sHtML

[U33] Py：打包发布
来源：http://baike.fanxiaobao.xyz/Article/details/gxgjxdmna.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fanxiaobao.xyz/Article/details/gqfqvtkpv.sHtML

[U34] Py：判断编码
来源：http://3g.fanxiaobao.xyz/Article/details/gxvsdtqxf.sHtML

chardet.detect(raw)
来源：http://blog.fanxiaobao.xyz/Article/details/gerprofok.sHtML

[U35] Py：发送邮件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjsveqvyg.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcipjipsx.sHtML

[U36] Py：定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gnofuhpte.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbaogghi.sHtML

[U37] Py：读写 Excel
来源：http://blog.fanxiaobao.xyz/Article/details/ghtnmqedz.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhwiimvv.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqftfcfi.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtcnetaua.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmkqnafb.sHtML

sys.stdout.isatty()
来源：http://read.share.fanxiaobao.xyz/Article/details/gdkoyquun.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrkadtfa.sHtML

print("err", file=sys.stderr)
来源：http://wap.fanxiaobao.xyz/Article/details/gzdvsnaeu.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrxkoxxg.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffxynlco.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.fanxiaobao.xyz/Article/details/gnmriptxv.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxiozgiuu.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbgrgxcdd.sHtML

namespace App\Http;
来源：http://m.share.fanxiaobao.xyz/Article/details/gznpdnmhm.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gmhqtnqst.sHtML

declare(strict_types=1);
来源：http://3g.fanxiaobao.xyz/Article/details/gcfwdzluf.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.fanxiaobao.xyz/Article/details/guenfjtsa.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwnqdelv.sHtML

[U46] PHP：可空类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjtgewfu.sHtML

?string $name = null
来源：http://baike.fanxiaobao.xyz/Article/details/gsknsvbhe.sHtML

[U47] PHP：联合类型
来源：http://wap.fanxiaobao.xyz/Article/details/gdhvmiekf.sHtML

int|string $id
来源：http://baike.fanxiaobao.xyz/Article/details/gqzhkghtq.sHtML

[U48] PHP：纯枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gumdmljib.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/georrnfdv.sHtML

[U49] PHP：只读属性
来源：http://blog.fanxiaobao.xyz/Article/details/gyegduksu.sHtML

public readonly string $name
来源：http://www.share.fanxiaobao.xyz/Article/details/gsiaunxgj.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.fanxiaobao.xyz/Article/details/gizwsdhkv.sHtML

public function __construct(private int $id) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gkwpbegpx.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqckmtge.sHtML

[$a, $b] = $arr;
来源：http://baike.fanxiaobao.xyz/Article/details/gdkurcaxn.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdylrqyqn.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnznxqiuy.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fanxiaobao.xyz/Article/details/gujplnofk.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.fanxiaobao.xyz/Article/details/gygsmhmtw.sHtML

[U54] PHP：空安全调用
来源：http://wap.fanxiaobao.xyz/Article/details/gxjdtoflt.sHtML

$obj?->method()
来源：http://www.share.fanxiaobao.xyz/Article/details/gatlwfsuh.sHtML

[U55] PHP：match 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwuxmdxs.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.fanxiaobao.xyz/Article/details/gcqaqxiec.sHtML

[U56] PHP：命名参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gjokqiiwh.sHtML

f(a: 1, b: 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdkoxlia.sHtML

[U57] PHP：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqyqyalz.sHtML

"值: {$a}"
来源：http://baike.fanxiaobao.xyz/Article/details/ggmjtwjtl.sHtML

[U58] PHP：数组三件套
来源：http://www.share.fanxiaobao.xyz/Article/details/grndkawcf.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitwtpekc.sHtML

[U59] PHP：自定义排序
来源：http://3g.fanxiaobao.xyz/Article/details/gcnpyopsi.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/govbmjtvh.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlqlluxv.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.fanxiaobao.xyz/Article/details/gldbzdeao.sHtML

[U61] PHP：正则
来源：http://read.share.fanxiaobao.xyz/Article/details/gkykrziza.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqkyymye.sHtML

[U62] PHP：日期对象
来源：http://baike.fanxiaobao.xyz/Article/details/gbgifqqjm.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.fanxiaobao.xyz/Article/details/grlsagcmd.sHtML

[U63] PHP：文件读写
来源：http://wap.fanxiaobao.xyz/Article/details/gujypbqdi.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjtiyxio.sHtML

[U64] PHP：目录遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/grbcuqwxi.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fanxiaobao.xyz/Article/details/gajlgogsa.sHtML

[U65] PHP：会话
来源：http://m.share.fanxiaobao.xyz/Article/details/gllvyvhew.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzhkfpxt.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.fanxiaobao.xyz/Article/details/gwcnxtpkj.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmztmajk.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbonuwsc.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwapxuzp.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fanxiaobao.xyz/Article/details/genqvrbhq.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.fanxiaobao.xyz/Article/details/ggvqjckbk.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.fanxiaobao.xyz/Article/details/gslbqisdt.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fanxiaobao.xyz/Article/details/gqmqyxenm.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givvdhgoq.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.fanxiaobao.xyz/Article/details/gzesvotzi.sHtML

[U71] PHP：抛出异常
来源：http://www.share.fanxiaobao.xyz/Article/details/gvcettgnm.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkiawhqem.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grepicjmv.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.fanxiaobao.xyz/Article/details/gqgxwaeod.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.fanxiaobao.xyz/Article/details/gfgfrbeju.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.fanxiaobao.xyz/Article/details/gasfnfmod.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gcekqmgwa.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfchvqacf.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqcqrowp.sHtML

composer require psr/container
来源：http://blog.fanxiaobao.xyz/Article/details/gyrxzigqh.sHtML

[U76] PHP：简单路由
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxvtmmmw.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.fanxiaobao.xyz/Article/details/gvmexkljn.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fanxiaobao.xyz/Article/details/giyjnhuxw.sHtML

composer require twig/twig
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzidfpnx.sHtML

[U78] PHP：单元测试
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqfpfpsr.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.fanxiaobao.xyz/Article/details/gslcrmgva.sHtML

[U79] PHP：静态分析
来源：http://wap.fanxiaobao.xyz/Article/details/gnkogajvq.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.fanxiaobao.xyz/Article/details/gdvfetqsy.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gotpymnru.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.fanxiaobao.xyz/Article/details/gacaqhxxw.sHtML

[U81] JS：初始化项目
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfstpnqj.sHtML

npm init -y;  npm i express
来源：http://wap.fanxiaobao.xyz/Article/details/glmrawywv.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.fanxiaobao.xyz/Article/details/gbgsfphjc.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvcmzovi.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.fanxiaobao.xyz/Article/details/gaethqroa.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.fanxiaobao.xyz/Article/details/gelbpgajs.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.fanxiaobao.xyz/Article/details/gnpwivjln.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fanxiaobao.xyz/Article/details/glxsqdlqv.sHtML

[U85] JS：可选链
来源：http://3g.fanxiaobao.xyz/Article/details/gudhqfcvg.sHtML

a?.b?.c
来源：http://read.share.fanxiaobao.xyz/Article/details/gqzyycfxb.sHtML

[U86] JS：空值合并
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjkqgkyd.sHtML

a ?? b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfcapttpq.sHtML

[U87] JS：解构默认值
来源：http://blog.fanxiaobao.xyz/Article/details/gmshoveby.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.fanxiaobao.xyz/Article/details/gjjjfmjdy.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbsvumqtn.sHtML

{ ...a, ...b }
来源：http://baike.fanxiaobao.xyz/Article/details/gaflotttz.sHtML

[U89] JS：数组去重
来源：http://wap.fanxiaobao.xyz/Article/details/gbjyulqyi.sHtML

[...new Set(arr)]
来源：http://3g.fanxiaobao.xyz/Article/details/gghokjnmt.sHtML

[U90] JS：数字数组排序
来源：http://baike.fanxiaobao.xyz/Article/details/goobqzvzg.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxktdtdao.sHtML

[U91] JS：对象键值遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gagecbwqg.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbeuyfhl.sHtML

[U92] JS：深拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjylzjvt.sHtML

structuredClone(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfxqjcyq.sHtML

[U93] JS：模板字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gmbznavse.sHtML

`共 ${n} 条`
来源：http://wap.fanxiaobao.xyz/Article/details/gipuxqctk.sHtML

[U94] JS：箭头函数
来源：http://3g.fanxiaobao.xyz/Article/details/gubahrigs.sHtML

const double = x => x * 2;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxifuroh.sHtML

[U95] JS：Promise 包装
来源：http://baike.fanxiaobao.xyz/Article/details/gjtncadol.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.fanxiaobao.xyz/Article/details/gpouidevy.sHtML

[U96] JS：async/await 与异常
来源：http://3g.fanxiaobao.xyz/Article/details/guquzjfgy.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.fanxiaobao.xyz/Article/details/gvspsjkyt.sHtML

[U97] JS：并发请求
来源：http://3g.fanxiaobao.xyz/Article/details/gzvdwtves.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdgtwhpu.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gnjitozbp.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzccllhke.sHtML

[U99] JS：事件监听
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjsmhkxox.sHtML

el.addEventListener("click", e => {})
来源：http://blog.fanxiaobao.xyz/Article/details/gmgmvrzef.sHtML

[U100] JS：DOM 查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gidwqhlgt.sHtML

document.querySelector(".item")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtsahvkm.sHtML

[U101] JS：classList 操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gqraxrtkt.sHtML

el.classList.toggle("active")
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhgoliai.sHtML

[U102] JS：本地存储
来源：http://blog.fanxiaobao.xyz/Article/details/grywtsvip.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.fanxiaobao.xyz/Article/details/gasmyuwrz.sHtML

[U103] JS：定时器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmfrkkji.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fanxiaobao.xyz/Article/details/gocuywque.sHtML

[U104] JS：防抖
来源：http://mobile.fanxiaobao.xyz/Article/details/gchkpolja.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gilxszxfx.sHtML

[U105] JS：节流
来源：http://baike.fanxiaobao.xyz/Article/details/gckudowlo.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fanxiaobao.xyz/Article/details/gpzbvhmnj.sHtML

[U106] JS：日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/grojfbzqs.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.fanxiaobao.xyz/Article/details/gskvvaeor.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcejeyhew.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.fanxiaobao.xyz/Article/details/giodffqmy.sHtML

[U108] JS：随机整数
来源：http://www.share.fanxiaobao.xyz/Article/details/guyxbvktv.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.fanxiaobao.xyz/Article/details/gfgpxrxvm.sHtML

[U109] JS：数组分组
来源：http://www.share.fanxiaobao.xyz/Article/details/glzcnumxn.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.fanxiaobao.xyz/Article/details/gammfxntg.sHtML

[U110] JS：数组分块
来源：http://mobile.fanxiaobao.xyz/Article/details/gadwraqvl.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grnmvnhiy.sHtML

[U111] JS：对象转 Map
来源：http://3g.fanxiaobao.xyz/Article/details/gajhybjif.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrmkqkbu.sHtML

[U112] JS：字符串补位
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlbqzxvb.sHtML

"7".padStart(3, "0")
来源：http://baike.fanxiaobao.xyz/Article/details/gcnsaazlp.sHtML

[U113] JS：正则替换全部
来源：http://blog.fanxiaobao.xyz/Article/details/grzcgorvs.sHtML

s.replaceAll("a", "b")
来源：http://m.share.fanxiaobao.xyz/Article/details/gifabykxx.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fanxiaobao.xyz/Article/details/gvqabywtk.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fanxiaobao.xyz/Article/details/goggetbqv.sHtML

[U115] JS：生成 UUID
来源：http://3g.fanxiaobao.xyz/Article/details/gqhtguudw.sHtML

crypto.randomUUID()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmadmmchc.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdflaugx.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.fanxiaobao.xyz/Article/details/ghlrijvhc.sHtML

[U117] JS：单元测试
来源：http://3g.fanxiaobao.xyz/Article/details/gnitipsfo.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.fanxiaobao.xyz/Article/details/gihilgdto.sHtML

[U118] JS：开发服务器
来源：http://blog.fanxiaobao.xyz/Article/details/greqyjtey.sHtML

npm i -D vite;  npx vite
来源：http://read.share.fanxiaobao.xyz/Article/details/gqnsqmzer.sHtML

[U119] JS：生产构建
来源：http://blog.fanxiaobao.xyz/Article/details/gfymruiaz.sHtML

npx vite build
来源：http://m.share.fanxiaobao.xyz/Article/details/gitunlbps.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqwrygkk.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvlzxmof.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gerfiijzy.sHtML

统计汇总
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqdpakqz.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkyfbcwp.sHtML

按语言统计（条）：
来源：http://www.share.fanxiaobao.xyz/Article/details/gwehnwicm.sHtML

Python ......... 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glcfodhat.sHtML

PHP ............ 252
来源：http://wap.fanxiaobao.xyz/Article/details/gxnjvweyp.sHtML

JavaScript ..... 252
来源：http://wap.fanxiaobao.xyz/Article/details/gjmighvqb.sHtML

TypeScript ..... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gzaqcbdlc.sHtML

Java ........... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gufryutoa.sHtML

Go ............. 212
来源：http://wap.fanxiaobao.xyz/Article/details/gmbuyfvdd.sHtML

Ruby ........... 212
来源：http://blog.fanxiaobao.xyz/Article/details/gwelizdgd.sHtML

C# ............. 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwfjtbbcl.sHtML

C .............. 30
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkiwrwsme.sHtML

C++ ............ 30
来源：http://baike.fanxiaobao.xyz/Article/details/ggycgotak.sHtML

SQL ............ 90
来源：http://3g.fanxiaobao.xyz/Article/details/gdigslmgr.sHtML

Bash ........... 80
来源：http://read.share.fanxiaobao.xyz/Article/details/gbevdqlqj.sHtML

Kotlin ......... 15
来源：http://www.share.fanxiaobao.xyz/Article/details/gmspguxyo.sHtML

Swift .......... 15
来源：http://www.share.fanxiaobao.xyz/Article/details/gacmpvrfv.sHtML

Lua ............ 10
来源：http://3g.fanxiaobao.xyz/Article/details/gimitsjty.sHtML

Perl ........... 10
来源：http://3g.fanxiaobao.xyz/Article/details/gpubexhwa.sHtML

Scala .......... 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxxqtbwo.sHtML

------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggbvkmsbd.sHtML

合计 ........... 2106 条
来源：http://baike.fanxiaobao.xyz/Article/details/gcqchfbek.sHtML

按章节统计：
来源：http://wap.fanxiaobao.xyz/Article/details/gppfqasbi.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.fanxiaobao.xyz/Article/details/gfusfjipz.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.fanxiaobao.xyz/Article/details/gpszqblvo.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.fanxiaobao.xyz/Article/details/gbyymlgvp.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.fanxiaobao.xyz/Article/details/gftxlkjon.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fanxiaobao.xyz/Article/details/gtsqedmna.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gixargieb.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpltbppl.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.fanxiaobao.xyz/Article/details/gpuygfjco.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvlomqgu.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.fanxiaobao.xyz/Article/details/gstcnottu.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrpvraro.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gxujkskjq.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gtudoxviq.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.fanxiaobao.xyz/Article/details/gepkmqqda.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.fanxiaobao.xyz/Article/details/grpkgxgbe.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbghvnjz.sHtML

Q SQL 专题                              90
来源：http://mobile.fanxiaobao.xyz/Article/details/gadkcjgpx.sHtML

R Bash 专题                             80
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhdsmczy.sHtML

S C / C++ 专题                          60
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxmzcrjz.sHtML

T 其他语言补充                          60
来源：http://3g.fanxiaobao.xyz/Article/details/gvybrwnbb.sHtML

U 高频实用片段                         120
来源：http://wap.fanxiaobao.xyz/Article/details/gwipwnckb.sHtML

------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gwazejdwn.sHtML

合计                                  2106 条
来源：http://read.share.fanxiaobao.xyz/Article/details/gryqspdvf.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gzzredmob.sHtML

使用提醒
来源：http://www.share.fanxiaobao.xyz/Article/details/giwoyqiys.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/glxctarta.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjuhhunn.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glivvbnyy.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.fanxiaobao.xyz/Article/details/gkocbcvcm.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsepsllvf.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.fanxiaobao.xyz/Article/details/gtijqnham.sHtML

—— 文件结束 ——
来源：http://www.share.fanxiaobao.xyz/Article/details/gkuoxnvbz.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gdrmzjqvg.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghdvdhug.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.fanxiaobao.xyz/Article/details/govjuvbaj.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gfurbklut.sHtML

【收录内容】
来源：http://baike.fanxiaobao.xyz/Article/details/gfnoyqnge.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.fanxiaobao.xyz/Article/details/gpqcgzspj.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.fanxiaobao.xyz/Article/details/gvldhodtx.sHtML

SQL · Bash · C · C++
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtprrfit.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.fanxiaobao.xyz/Article/details/gaaaiistt.sHtML

【使用说明】
来源：http://read.share.fanxiaobao.xyz/Article/details/gwekkfwpu.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.fanxiaobao.xyz/Article/details/gensxduzb.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.fanxiaobao.xyz/Article/details/gvahtnzcp.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.fanxiaobao.xyz/Article/details/gxhtsvpwz.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzpkyhca.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.fanxiaobao.xyz/Article/details/graphnihs.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.fanxiaobao.xyz/Article/details/gghrjcqpm.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.fanxiaobao.xyz/Article/details/gviklsgqe.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glraetzea.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.fanxiaobao.xyz/Article/details/gvcwaxjbz.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.fanxiaobao.xyz/Article/details/gudlclxmq.sHtML


<!-- 参考信息 -->