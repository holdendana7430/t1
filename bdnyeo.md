代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://hz.aizwys.cn/gtiaormzbc.html

[T55] Scala：集合过滤
来源：http://hz.cdnleiting.top/gtwpftwwni.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.wangdashe.top/gtsvekltva.html

[T56] Scala：样例类
来源：http://hz.gaohongyu789.top/gttzckudbp.html

case class User(name: String, age: Int)
来源：http://hz.hnqzz.top/gtddfniyin.html

[T57] Scala：模式匹配
来源：http://hz.mhx1999.top/gtkmzbhqvy.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.jqgufenzy.top/gtgszdhhjw.html

[T58] Scala：函数定义
来源：http://hz.hnqzz.top/gtauhfwgxm.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.sweek.top/gtpwvgkejt.html

[T59] Scala：循环
来源：http://hz.svipenyu.cn/gttwrelasi.html

for (i <- 1 to 10) println(i)
来源：http://hz.svipenyu.cn/gtidyxokud.html

[T60] Scala：折叠
来源：http://hz.guannengcc.top/gtputmrjac.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.cheryme.top/gtrqmwsaab.html

================================================================================
来源：http://hz.yonumen.top/gtzogzoscp.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.cdnleiting.top/gtlrqpyxem.html

================================================================================
来源：http://hz.havefunace.top/gtsnjzrybq.html

[U01] Py：创建虚拟环境
来源：http://hz.zycfv.cn/gtnhydjnca.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.chenlongwang.top/gtctjddmif.html

[U02] Py：导出 / 安装依赖
来源：http://hz.ivvv.top/gtqvqgfsbr.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.nwbrower.top/gtkbezgyhc.html

[U03] Py：加载 .env 配置
来源：http://hz.daxiang520.top/gttptkufbm.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.fzhhl.top/gtdjxtgpeg.html

[U04] Py：变量调试打印
来源：http://hz.cdnleiting.top/gtwyyyuyyu.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.shuidangran.top/gtnzgkclst.html

[U05] Py：列表去重且保序
来源：http://hz.zdqjudy.top/gtgupunmad.html

list(dict.fromkeys(arr))
来源：http://hz.jianghu66.top/gtjxfrvexe.html

[U06] Py：合并两个字典
来源：http://hz.jianghu66.top/gtgeltbpfc.html

{**a, **b}
来源：http://hz.meibo888.top/gtbnajqxnx.html

[U07] Py：反转字典键值
来源：http://hz.xingfuxueyuan.xyz/gtonjmcfgs.html

{v: k for k, v in d.items()}
来源：http://hz.chenzaomai.com/gtnyeucsyy.html

[U08] Py：展平二维列表
来源：http://hz.wangshuangyany.cn/gtxqmjbmip.html

[y for x in nested for y in x]
来源：http://hz.shanyushiyangtech.top/gtdmzdumxl.html

[U09] Py：字典取最大值的键
来源：http://hz.feifeiyinyue.top/gtuqfdwcog.html

max(d, key=d.get)
来源：http://hz.haohaochexian.top/gtbzftkbas.html

[U10] Py：按值排序字典
来源：http://hz.hammf.cn/gtlrpdhrju.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.jiagoushi.top/gtqjsdbdyr.html

[U11] Py：生成器表达式
来源：http://hz.gogol.net.cn/gthrrnapax.html

(x * 2 for x in arr)
来源：http://hz.zhixingplan.top/gtlbzybiev.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.yueranfly.top/gtdtyggdya.html

Counter(arr).most_common(3)
来源：http://hz.xuanzx.com/gtavfeiitr.html

[U13] Py：固定长度队列
来源：http://hz.tian-w.cn/gtyqqbeana.html

deque(maxlen=10)
来源：http://hz.jqgufenzy.top/gtsgxmclvu.html

[U14] Py：分组收集到列表
来源：http://hz.zhijiandao.cn/gtdivntolq.html

defaultdict(list)
来源：http://hz.guannengcc.top/gtvatiuups.html

[U15] Py：高精度计时
来源：http://hz.gzhubu.top/gteocrqtct.html

t = time.perf_counter()
来源：http://hz.ehwqpu.com/gtgavcrwhi.html

[U16] Py：命令行参数解析
来源：http://hz.9152youxi.cn/gtspzcmkvx.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.xinyue.icu/gtsvytomtw.html

[U17] Py：初始化日志
来源：http://hz.tanke756.top/gttkgvtawm.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.cheryme.top/gtfhceaqzh.html

[U18] Py：预编译正则
来源：http://hz.shangyingyoupin.top/gtiuhyhhha.html

pat = re.compile(r"\d+")
来源：http://hz.xylfe.cn/gtwbfyglas.html

[U19] Py：正则替换带回调
来源：http://hz.zhaomingkeji.xyz/gtvkrhecuy.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.sysykeji.top/gttatlpbht.html

[U20] Py：缓存函数结果
来源：http://hz.shanyushiyangkeji.top/gtxxrqrzmp.html

@functools.lru_cache(maxsize=None)
来源：http://hz.pycfn.com/gtehwidqgd.html

[U21] Py：自定义上下文管理器
来源：http://hz.ywan-chungtsiang.top/gtxdssnquu.html

@contextlib.contextmanager
来源：http://hz.yvedp.cn/gtwmbiaqan.html

[U22] Py：矩阵转置
来源：http://hz.zhaomingkeji.xyz/gttiaemiod.html

list(zip(*m))
来源：http://hz.cucudq.cn/gtecycrcio.html

[U23] Py：分块读取大文件
来源：http://hz.nanxuanxn.top/gtbxlwohwu.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.chenzaomai.com/gtxouzdwrv.html

[U24] Py：路径操作
来源：http://hz.gaohongyu789.top/gttqvhsake.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.pengpengdd.cyou/gtcfavizto.html

[U25] Py：CSV 按字典读
来源：http://hz.ybcxt.top/gtfprqvczt.html

csv.DictReader(f)
来源：http://hz.birdmap.top/gtlybjjtee.html

[U26] Py：并发下载
来源：http://hz.cucudq.cn/gtrpbylnjf.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.xuanzx.com/gtrnndowna.html

[U27] Py：异步 HTTP
来源：http://hz.wangshuangyany.cn/gtdeszdvjs.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.ydjk.org.cn/gtmgqboikm.html

[U28] Py：类型别名
来源：http://hz.hammf.cn/gtuomiiqnc.html

UserId = int
来源：http://hz.zhaomingkeji.xyz/gtmvejvlem.html

[U29] Py：属性校验
来源：http://hz.cqqwz.cn/gterhsezar.html

@property 与 @x.setter 配合
来源：http://hz.yuxming.cn/gtfuvcjueh.html

[U30] Py：数据类
来源：http://hz.zycfv.cn/gtzmmovgws.html

@dataclass(slots=True)
来源：http://hz.yj20258888.top/gtizfcubvf.html

[U31] Py：单测
来源：http://hz.zhengqikj.top/gtvwralcvq.html

python -m pytest -q
来源：http://hz.cucudq.cn/gtzxeydurm.html

[U32] Py：代码格式化
来源：http://hz.zhengqikj.top/gtagaizwkw.html

ruff format . && ruff check --fix .
来源：http://hz.ppjwa.cn/gtcaljwgos.html

[U33] Py：打包发布
来源：http://hz.daria6918.cn/gtuyceebwt.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.zdqjudy.top/gtepapuosp.html

[U34] Py：判断编码
来源：http://hz.hysaishi.cn/gtxregianv.html

chardet.detect(raw)
来源：http://hz.316326.xyz/gtharstpog.html

[U35] Py：发送邮件
来源：http://hz.xuanzx.com/gtpgautlhh.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.andypj.xyz/gtgihnlqwp.html

[U36] Py：定时任务
来源：http://hz.316326.xyz/gtpjbfahzp.html

schedule.every(10).minutes.do(job)
来源：http://hz.zhaomingkeji.xyz/gtscmhwjjc.html

[U37] Py：读写 Excel
来源：http://hz.gogol.net.cn/gtivcqpsry.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.yonumen.top/gtmnvmffak.html

[U38] Py：获取脚本所在目录
来源：http://hz.zycfv.cn/gtkatntinn.html

Path(__file__).resolve().parent
来源：http://hz.xuanzx.com/gtbtwqnfbj.html

[U39] Py：判断是否在交互环境
来源：http://hz.feifeiyinyue.top/gtytbsbozz.html

sys.stdout.isatty()
来源：http://hz.jiagoushi.top/gtfwptedhf.html

[U40] Py：打印到标准错误
来源：http://hz.haohaochexian.top/gtqrqwdegf.html

print("err", file=sys.stderr)
来源：http://hz.bjfxy.top/gtpgrrusvo.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.hnxiangtu.top/gtwluflerp.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.jiagoushi.top/gthyjjonkp.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.tian-w.cn/gtctxofoyv.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.gogol.net.cn/gtadlkomdq.html

[U43] PHP：声明命名空间
来源：http://hz.aizwys.cn/gtvvqfkxrp.html

namespace App\Http;
来源：http://hz.zhixingplan.top/gtikcreosf.html

[U44] PHP：开启严格类型
来源：http://hz.zycfv.cn/gtktkvswea.html

declare(strict_types=1);
来源：http://hz.zhiwuduotai.top/gtoobmpoxh.html

[U45] PHP：类型声明与返回类型
来源：http://hz.shanyushiyangtech.top/gtvacxqcgo.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.svipenyu.cn/gtfjizxdpd.html

[U46] PHP：可空类型
来源：http://hz.yuanzhike.top/gtolwuzoho.html

?string $name = null
来源：http://hz.hfpthk.cn/gthzkmqcss.html

[U47] PHP：联合类型
来源：http://hz.zhoulong.xyz/gtzxuiucdg.html

int|string $id
来源：http://hz.bjfxy.top/gttgkpeegt.html

[U48] PHP：纯枚举
来源：http://hz.zhiwuduotai.top/gtrwigjsnb.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.jianghu66.top/gtbtmvptxh.html

[U49] PHP：只读属性
来源：http://hz.aibaodan.cn/gthjwmmfhp.html

public readonly string $name
来源：http://hz.316326.xyz/gtwsbqsvqz.html

[U50] PHP：构造器属性提升
来源：http://hz.yonumen.top/gtdiummlwu.html

public function __construct(private int $id) {}
来源：http://hz.jinghuilouyu.cn/gtybdhzrwk.html

[U51] PHP：数组解构
来源：http://hz.nanxinkj.top/gtalmdiboc.html

[$a, $b] = $arr;
来源：http://hz.jinqigfzy.top/gtkzeyphie.html

[U52] PHP：箭头函数
来源：http://hz.tian-w.cn/gtrpnyhucc.html

$double = fn($x) => $x * 2;
来源：http://hz.cheryme.top/gtpyejggtf.html

[U53] PHP：空合并运算符
来源：http://hz.kuanghao11.cn/gtstejaryw.html

$v = $a ?? $b ?? "default";
来源：http://hz.shanyushiyangkeji.top/gtmvbstifd.html

[U54] PHP：空安全调用
来源：http://hz.hywenlv.cn/gtelpevzle.html

$obj?->method()
来源：http://hz.iojbl.cn/gtajrugimf.html

[U55] PHP：match 表达式
来源：http://hz.zhixingplan.top/gttpqkkgel.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.xinyue.icu/gtzytxbxxo.html

[U56] PHP：命名参数
来源：http://hz.xuetiantiany.cn/gtvubhjeao.html

f(a: 1, b: 2)
来源：http://hz.jinghuilouyu.cn/gthbkrhnkj.html

[U57] PHP：字符串插值
来源：http://hz.c1oappe.top/gtvgxwxkht.html

"值: {$a}"
来源：http://hz.guannengcc.top/gtgrvoimph.html

[U58] PHP：数组三件套
来源：http://hz.xuanzx.com/gtonlaeopw.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.9152youxi.cn/gtzcptckke.html

[U59] PHP：自定义排序
来源：http://hz.yanxiufei.cn/gtizqyzscd.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.nanxuanxn.top/gtfapfkqtn.html

[U60] PHP：JSON 编解码
来源：http://hz.zhijiandao.cn/gtzjfmcgff.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.316326.xyz/gtxlxgbqkm.html

[U61] PHP：正则
来源：http://hz.nanxinkj.top/gttokwdzil.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.gzhubu.top/gtbelhwdxx.html

[U62] PHP：日期对象
来源：http://hz.zhijiandao.cn/gtvfjnyzit.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.shangyingyoupin.top/gtlfkvcczq.html

[U63] PHP：文件读写
来源：http://hz.andypj.xyz/gtvpjjwezk.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.jinqigfzy.top/gtxqxpudej.html

[U64] PHP：目录遍历
来源：http://hz.ydzc1.top/gtjwfbdiuu.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.c1oappe.top/gtsetsftko.html

[U65] PHP：会话
来源：http://hz.svipenyu.cn/gtzitwmdtr.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.cucudq.cn/gtkmrbdmha.html

[U66] PHP：设置 Cookie
来源：http://hz.ybcxt.top/gtgwzaheyh.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.hnqzz.top/gtvwlyhffs.html

[U67] PHP：处理文件上传
来源：http://hz.zhijiandao.cn/gtynqsuzju.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.yj20258888.top/gtpylebzkm.html

[U68] PHP：PDO 连接
来源：http://hz.yj20258888.top/gtgsgmkpfz.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.sysykeji.top/gteuwtsafk.html

[U69] PHP：PDO 预处理
来源：http://hz.cheryme.top/gtyhmhlzvr.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.zdqjudy.top/gtqggrpbum.html

[U70] PHP：PDO 事务
来源：http://hz.iojbl.cn/gtjogyrdvy.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.jinyuanbaomall.cn/gtnqtrcnls.html

[U71] PHP：抛出异常
来源：http://hz.hammf.cn/gtyasltotd.html

throw new RuntimeException("失败", 500);
来源：http://hz.zdqjudy.top/gtyhmkrrkp.html

[U72] PHP：写错误日志
来源：http://hz.guannengcc.top/gtvdjhblzn.html

error_log("失败: " . $e->getMessage());
来源：http://hz.jyoumei.cn/gtqkvwulnj.html

[U73] PHP：读取 ini 配置
来源：http://hz.ehwqpu.com/gttsmlondd.html

parse_ini_file("config.ini", true)
来源：http://hz.ybcxt.top/gtwayjxyks.html

[U74] PHP：读取环境变量
来源：http://hz.xuanzx.com/gtesdzajci.html

getenv("APP_ENV") ?: "production"
来源：http://hz.cucudq.cn/gtrgnefkjc.html

[U75] PHP：依赖注入
来源：http://hz.zhengqikj.top/gtvbxqorqn.html

composer require psr/container
来源：http://hz.smart0.xyz/gtxauloaxz.html

[U76] PHP：简单路由
来源：http://hz.birdmap.top/gtpkbndckj.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.tian-w.cn/gtstcqpelr.html

[U77] PHP：模板渲染
来源：http://hz.fzhhl.top/gttlfqqzlh.html

composer require twig/twig
来源：http://hz.daria6918.cn/gtoqxcakii.html

[U78] PHP：单元测试
来源：http://hz.xuanzx.com/gtukujvlgw.html

composer require --dev phpunit/phpunit
来源：http://hz.cucudq.cn/gtrommiidz.html

[U79] PHP：静态分析
来源：http://hz.cheryme.top/gtuzrkmknq.html

composer require --dev phpstan/phpstan
来源：http://hz.daxiang520.top/gtwtgqyiap.html

[U80] PHP：代码规范修复
来源：http://hz.0kj1m.cn/gtjkmkdaka.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.wangdashe.top/gteukcgake.html

[U81] JS：初始化项目
来源：http://hz.pycfn.com/gtxdaogibw.html

npm init -y;  npm i express
来源：http://hz.ivvv.top/gtnntrtdem.html

[U82] JS：package.json 脚本
来源：http://hz.pengpengdd.cyou/gthyoxbprg.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.andypj.xyz/gtvmrqfhgz.html

[U83] JS：ES Module 导入导出
来源：http://hz.wangdashe.top/gtgjebzsle.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.sxryk.cn/gtvprjqncc.html

[U84] JS：CommonJS 写法
来源：http://hz.dianchejie.cn/gtakzzukjc.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.snrcjt.cn/gtmzitholy.html

[U85] JS：可选链
来源：http://hz.jyoumei.cn/gtassfzupx.html

a?.b?.c
来源：http://hz.yj20258.top/gteovbmgqb.html

[U86] JS：空值合并
来源：http://hz.cashguo.top/gtmckexnmc.html

a ?? b
来源：http://hz.wangdashe.top/gtvfatzbbh.html

[U87] JS：解构默认值
来源：http://hz.zycfv.cn/gtkzagtidb.html

const { a = 1, b = 2 } = obj;
来源：http://hz.andypj.xyz/gtudlbdmsl.html

[U88] JS：对象展开合并
来源：http://hz.jqgfzy.top/gtmmuklegr.html

{ ...a, ...b }
来源：http://hz.cdnleiting.top/gtyrndpque.html

[U89] JS：数组去重
来源：http://hz.xuetiantiany.cn/gtzxrljdxd.html

[...new Set(arr)]
来源：http://hz.shzxlz.cn/gttqvpakku.html

[U90] JS：数字数组排序
来源：http://hz.svipenyu.cn/gtwhwdhpga.html

[...arr].sort((a, b) => a - b)
来源：http://hz.guowangkeji.top/gtfxpumwne.html

[U91] JS：对象键值遍历
来源：http://hz.mhx1999.top/gtmnjfrexs.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.svipenyu.cn/gtcdiyfikk.html

[U92] JS：深拷贝
来源：http://hz.yueranfly.top/gtgurnuoch.html

structuredClone(obj)
来源：http://hz.cashguo.top/gtpsdisbxw.html

[U93] JS：模板字符串
来源：http://hz.316326.xyz/gtsjfvxgqt.html

`共 ${n} 条`
来源：http://hz.zhiwuduotai.top/gtfkotuxmk.html

[U94] JS：箭头函数
来源：http://hz.fengsongda.top/gtryxhdiph.html

const double = x => x * 2;
来源：http://hz.jinqigfzy.top/gtvotpdhjh.html

[U95] JS：Promise 包装
来源：http://hz.hywenlv.cn/gtojfgakjy.html

new Promise((resolve, reject) => {})
来源：http://hz.sweek.top/gthjypygxs.html

[U96] JS：async/await 与异常
来源：http://hz.kuanghao11.cn/gtezygpsex.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.jinghuilouyu.cn/gtjlrbqnmt.html

[U97] JS：并发请求
来源：http://hz.sufxvd.cn/gtehstgfxh.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hysaishi.cn/gthxkswlnk.html

[U98] JS：fetch 带 JSON
来源：http://hz.xylfe.cn/gtbknjtola.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.xylfe.cn/gthsnteqnc.html

[U99] JS：事件监听
来源：http://hz.shanyushiyangtech.top/gtchghvmoi.html

el.addEventListener("click", e => {})
来源：http://hz.zhiwuduotai.top/gtoweqqeet.html

[U100] JS：DOM 查询
来源：http://hz.gzhubu.top/gtfncnctsm.html

document.querySelector(".item")
来源：http://hz.jiagoushi.top/gtjanaxyaz.html

[U101] JS：classList 操作
来源：http://hz.daria6918.cn/gtwledzcrf.html

el.classList.toggle("active")
来源：http://hz.zhoulong.xyz/gtfeginwzm.html

[U102] JS：本地存储
来源：http://hz.sysykeji.top/gtuosoanfm.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.kuanghao11.cn/gtzrhzndlw.html

[U103] JS：定时器
来源：http://hz.fengsongda.top/gtojhqkdam.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.jianghu66.top/gtgdkmdeat.html

[U104] JS：防抖
来源：http://hz.fzhhl.top/gtfmdfozpc.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hnxiangtu.top/gtqavxehkk.html

[U105] JS：节流
来源：http://hz.tian-w.cn/gtpygvcdcd.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.dianchejie.cn/gthxgqxcvw.html

[U106] JS：日期格式化
来源：http://hz.hammf.cn/gtzzcxuptq.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.dashuyun.cn/gtmsrflgpb.html

[U107] JS：数字千分位
来源：http://hz.xylfe.cn/gtpslskkig.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.ywan-chungtsiang.top/gtkxsgnqbm.html

[U108] JS：随机整数
来源：http://hz.wangdashe.top/gtnpmxztgp.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.xuetiantiany.cn/gtimnqehan.html

[U109] JS：数组分组
来源：http://hz.yj20258.top/gtevvopmwz.html

Object.groupBy(arr, x => x.type)
来源：http://hz.bjfxy.top/gtimmszazt.html

[U110] JS：数组分块
来源：http://hz.xingfuxueyuan.xyz/gtjbbfyjyp.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.shuidangran.top/gtxveqqjac.html

[U111] JS：对象转 Map
来源：http://hz.hnxiangtu.top/gttzqehegj.html

new Map(Object.entries(obj))
来源：http://hz.hywenlv.cn/gtemipurho.html

[U112] JS：字符串补位
来源：http://hz.xuetiantiany.cn/gtohtpuqge.html

"7".padStart(3, "0")
来源：http://hz.ywan-chungtsiang.top/gtgxmaretx.html

[U113] JS：正则替换全部
来源：http://hz.jinghuilouyu.cn/gtxflvxjix.html

s.replaceAll("a", "b")
来源：http://hz.shangyingyoupin.top/gtwotvemgh.html

[U114] JS：JSON 深比较
来源：http://hz.cdnleiting.top/gtgdihtteb.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.tanke756.top/gtfzvwfbgi.html

[U115] JS：生成 UUID
来源：http://hz.shzxlz.cn/gtxisnzdyg.html

crypto.randomUUID()
来源：http://hz.sufxvd.cn/gtpuuowxbr.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.guowangkeji.top/gtptmltiyx.html

/** @param {string} name */ function f(name) {}
来源：http://hz.jinghuilouyu.cn/gtaunhtrbl.html

[U117] JS：单元测试
来源：http://hz.gogol.net.cn/gteqzkbecc.html

npm i -D vitest;  npx vitest
来源：http://hz.zhiwuduotai.top/gthvmmtbxf.html

[U118] JS：开发服务器
来源：http://hz.xingfuxueyuan.xyz/gtaqyxkxuj.html

npm i -D vite;  npx vite
来源：http://hz.meibo888.top/gtbcwrnjfw.html

[U119] JS：生产构建
来源：http://hz.yonumen.top/gtsbycrgyb.html

npx vite build
来源：http://hz.meibo888.top/gtxtiulsbw.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.nwbrower.top/gtvzogehvm.html

import.meta.env.VITE_API_URL
来源：http://hz.0kj1m.cn/gtzugcxvuy.html

================================================================================
来源：http://hz.smart0.xyz/gtencskdgq.html

统计汇总
来源：http://hz.redwolf501.top/gtbnnhthte.html

================================================================================
来源：http://hz.nanxuanxn.top/gtdwixrixa.html

按语言统计（条）：
来源：http://hz.jinyuanbaomall.cn/gtkwxmxwny.html

Python ......... 252
来源：http://hz.yj202588.top/gtllezzgfo.html

PHP ............ 252
来源：http://hz.haohaochexian.top/gtsaymrpgg.html

JavaScript ..... 252
来源：http://hz.birdmap.top/gttheprplf.html

TypeScript ..... 212
来源：http://hz.316326.xyz/gtwedgccxs.html

Java ........... 212
来源：http://hz.yuxming.cn/gtrlhmniif.html

Go ............. 212
来源：http://hz.zhiwuduotai.top/gtvqqdcbuc.html

Ruby ........... 212
来源：http://hz.zhongyouzk.top/gthvrqgctc.html

C# ............. 212
来源：http://hz.xingfuxueyuan.xyz/gtqerhjphh.html

C .............. 30
来源：http://hz.hammf.cn/gtgzagbrqi.html

C++ ............ 30
来源：http://hz.guannengcc.top/gtrntescjq.html

SQL ............ 90
来源：http://hz.nanxuanxn.top/gtivwgtkfu.html

Bash ........... 80
来源：http://hz.sxryk.cn/gtdotnpmkf.html

Kotlin ......... 15
来源：http://hz.jinqigfzy.top/gteltyzndq.html

Swift .......... 15
来源：http://hz.aizwys.cn/gtbdncpcpg.html

Lua ............ 10
来源：http://hz.andypj.xyz/gtpsgssuih.html

Perl ........... 10
来源：http://hz.redwolf501.top/gtiqrjixze.html

Scala .......... 10
来源：http://hz.sweek.top/gtsezqzcpu.html

------------------------------------
来源：http://hz.hongshengwenyu.top/gtglqknspv.html

合计 ........... 2106 条
来源：http://hz.jinqigfzy.top/gtvqpqzjvg.html

按章节统计：
来源：http://hz.tianlin.xyz/gtgcjepyxw.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.xuetiantiany.cn/gtoadyynfs.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.yanxiufei.cn/gtcqbmgxfr.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.sufxvd.cn/gtwoertrin.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.quarkkingdee.top/gtefaidfri.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.chenlongwang.top/gtevnfqhgn.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.hywenlv.cn/gtexgtgpig.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.andypj.xyz/gtjkjvdppp.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.yj20258.top/gthiipieem.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.svipenyu.cn/gtfesxastj.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.xuetiantiany.cn/gtlxaqdmdx.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.sxryk.cn/gtmwvumvea.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.jianghu66.top/gtobnifcmd.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.cqqwz.cn/gtxzldptcp.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.hnxiangtu.top/gtlgnhfukc.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.52xcode.cn/gtpoydmjmq.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.fzhhl.top/gtlzqtvcie.html

Q SQL 专题                              90
来源：http://hz.jinqigfzy.top/gtqoajuypz.html

R Bash 专题                             80
来源：http://hz.wangdashe.top/gtmvjbhckv.html

S C / C++ 专题                          60
来源：http://hz.xuetiantiany.cn/gtgocfeici.html

T 其他语言补充                          60
来源：http://hz.xinyue.icu/gtecisctoh.html


<!-- 参考信息 -->