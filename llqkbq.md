代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://hz.vqdsnc.cn/gteulzreom.html

[T59] Scala：循环
来源：http://hz.feifeiyinyue.top/gtjpkvmyfg.html

for (i <- 1 to 10) println(i)
来源：http://hz.daxiang520.top/gtfyxtcpkq.html

[T60] Scala：折叠
来源：http://hz.smart0.xyz/gthnupzeei.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.yangfankeji.com/gtdykeiymk.html

================================================================================
来源：http://hz.vqdsnc.cn/gtcsogghqz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.yvedp.cn/gtiqnddpee.html

================================================================================
来源：http://hz.hnxiangtu.top/gtlxlyozgg.html

[U01] Py：创建虚拟环境
来源：http://hz.mhx1999.top/gtmtmtfzlq.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.jyoumei.cn/gttwiidoqj.html

[U02] Py：导出 / 安装依赖
来源：http://hz.yvedp.cn/gthqpqdtrz.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.ydjk.org.cn/gtbwhfqbez.html

[U03] Py：加载 .env 配置
来源：http://hz.meibo888.top/gtapshfpem.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.jqgfzy.top/gtftfdntej.html

[U04] Py：变量调试打印
来源：http://hz.shanyushiyangtech.top/gtuphgfeuz.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.pengpengdd.cyou/gtahezuxdq.html

[U05] Py：列表去重且保序
来源：http://hz.ppjwa.cn/gttvuudsdr.html

list(dict.fromkeys(arr))
来源：http://hz.guannengcc.top/gtiuzctxdn.html

[U06] Py：合并两个字典
来源：http://hz.guowangkeji.top/gtezawcapn.html

{**a, **b}
来源：http://hz.cdnleiting.top/gtjwpmonvl.html

[U07] Py：反转字典键值
来源：http://hz.yj20258888.top/gtefncmbxz.html

{v: k for k, v in d.items()}
来源：http://hz.nanxinkj.top/gtkwspweas.html

[U08] Py：展平二维列表
来源：http://hz.wangdashe.top/gtebpjlcpd.html

[y for x in nested for y in x]
来源：http://hz.jiagoushi.top/gtzodoablh.html

[U09] Py：字典取最大值的键
来源：http://hz.jinghuilouyu.cn/gtfuljbare.html

max(d, key=d.get)
来源：http://hz.yangfankeji.com/gtltvldxug.html

[U10] Py：按值排序字典
来源：http://hz.vqdsnc.cn/gtcvvyfuug.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.iojbl.cn/gteljzmqxk.html

[U11] Py：生成器表达式
来源：http://hz.zhengqikj.top/gtqenwrdku.html

(x * 2 for x in arr)
来源：http://hz.c1oappe.top/gtwnqxbqeq.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.andypj.xyz/gtjzdmjjzc.html

Counter(arr).most_common(3)
来源：http://hz.hfpthk.cn/gtzjaypnkv.html

[U13] Py：固定长度队列
来源：http://hz.jianghu66.top/gtqtcssvnq.html

deque(maxlen=10)
来源：http://hz.yueranfly.top/gtauswtcls.html

[U14] Py：分组收集到列表
来源：http://hz.aizwys.cn/gtlmelowxu.html

defaultdict(list)
来源：http://hz.fengsongda.top/gtzymlhgbm.html

[U15] Py：高精度计时
来源：http://hz.wangshuangyany.cn/gtszlodrbr.html

t = time.perf_counter()
来源：http://hz.cashguo.top/gtjfffrmhi.html

[U16] Py：命令行参数解析
来源：http://hz.nanxinkj.top/gtuxtkgsfu.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.xinyue.icu/gtnozjlqoj.html

[U17] Py：初始化日志
来源：http://hz.bjfxy.top/gtnfzrplwp.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.zhoulong.xyz/gthmioqyyn.html

[U18] Py：预编译正则
来源：http://hz.andypj.xyz/gtdwhmzafy.html

pat = re.compile(r"\d+")
来源：http://hz.jinqigufen.top/gtamsbvcwi.html

[U19] Py：正则替换带回调
来源：http://hz.iojbl.cn/gtvtjyzsol.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.bjfxy.top/gtmzuweoxz.html

[U20] Py：缓存函数结果
来源：http://hz.wangshuangyany.cn/gtzercmwvf.html

@functools.lru_cache(maxsize=None)
来源：http://hz.cdnleiting.top/gtqxbohser.html

[U21] Py：自定义上下文管理器
来源：http://hz.shuidangran.top/gtestvfuup.html

@contextlib.contextmanager
来源：http://hz.aizwys.cn/gtcrzmchat.html

[U22] Py：矩阵转置
来源：http://hz.birdmap.top/gtuqsxsthy.html

list(zip(*m))
来源：http://hz.aibaodan.cn/gtudtfyqgh.html

[U23] Py：分块读取大文件
来源：http://hz.fengsongda.top/gtnojgqpzz.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.redwolf501.top/gtsbctvplg.html

[U24] Py：路径操作
来源：http://hz.ybcxt.top/gtkzeoaykl.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.yongpay.top/gtofngocsf.html

[U25] Py：CSV 按字典读
来源：http://hz.zhijiandao.cn/gtrlfedluy.html

csv.DictReader(f)
来源：http://hz.zhoulong.xyz/gthbaowvnr.html

[U26] Py：并发下载
来源：http://hz.hongshengwenyu.top/gtqmyoqzzf.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.ywan-chungtsiang.top/gtgfydjpoj.html

[U27] Py：异步 HTTP
来源：http://hz.meibo888.top/gtyypqcmbn.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.ybcxt.top/gtbfwerkjy.html

[U28] Py：类型别名
来源：http://hz.gaohongyu789.top/gtuzckyqyr.html

UserId = int
来源：http://hz.zdqjudy.top/gtymxdmhfa.html

[U29] Py：属性校验
来源：http://hz.shuidangran.top/gtevzzdsdg.html

@property 与 @x.setter 配合
来源：http://hz.sufxvd.cn/gtzwkhnkst.html

[U30] Py：数据类
来源：http://hz.yj202588.top/gtgcknuzja.html

@dataclass(slots=True)
来源：http://hz.xuetiantiany.cn/gthrwksofi.html

[U31] Py：单测
来源：http://hz.shanyushiyangkeji.top/gtdmvmoijm.html

python -m pytest -q
来源：http://hz.zhiwuduotai.top/gtpwdppgwi.html

[U32] Py：代码格式化
来源：http://hz.wangshuangyany.cn/gtkwwdnclt.html

ruff format . && ruff check --fix .
来源：http://hz.nanxuanxn.top/gtswukvspg.html

[U33] Py：打包发布
来源：http://hz.xingfuxueyuan.xyz/gtsbqjtcsh.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.hfpthk.cn/gtimitdnwi.html

[U34] Py：判断编码
来源：http://hz.52xcode.cn/gtbusdlcxz.html

chardet.detect(raw)
来源：http://hz.hysaishi.cn/gttvyfwwsp.html

[U35] Py：发送邮件
来源：http://hz.zhongyouzk.top/gtmynmokfl.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.redwolf501.top/gticrsdhxz.html

[U36] Py：定时任务
来源：http://hz.sweek.top/gttoohrtkz.html

schedule.every(10).minutes.do(job)
来源：http://hz.chenlongwang.top/gtqnolgdhz.html

[U37] Py：读写 Excel
来源：http://hz.cashguo.top/gtpockmfvu.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.xuanzx.com/gttipmeqbu.html

[U38] Py：获取脚本所在目录
来源：http://hz.redwolf501.top/gtsrkennyh.html

Path(__file__).resolve().parent
来源：http://hz.nanxinkj.top/gtjkzvxlxm.html

[U39] Py：判断是否在交互环境
来源：http://hz.yueranfly.top/gtqxhjjdov.html

sys.stdout.isatty()
来源：http://hz.sysykeji.top/gtbluzzbbc.html

[U40] Py：打印到标准错误
来源：http://hz.xuetiantiany.cn/gteiiqcjae.html

print("err", file=sys.stderr)
来源：http://hz.hfpthk.cn/gtkdpimfla.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.daxiang520.top/gtjqvnxhvm.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.feifeiyinyue.top/gtjkitdvdx.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.bjfxy.top/gtflqmkvyh.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.zhengqikj.top/gtgzqwroaj.html

[U43] PHP：声明命名空间
来源：http://hz.bjfxy.top/gtyvmmlbzy.html

namespace App\Http;
来源：http://hz.svipenyu.cn/gtxoynphnu.html

[U44] PHP：开启严格类型
来源：http://hz.tian-w.cn/gtcawtigle.html

declare(strict_types=1);
来源：http://hz.yueranfly.top/gtjkxfpqtv.html

[U45] PHP：类型声明与返回类型
来源：http://hz.shzxlz.cn/gtpipdshsf.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.xinyue.icu/gtluhsmvgk.html

[U46] PHP：可空类型
来源：http://hz.zhixingplan.top/gtymworzmi.html

?string $name = null
来源：http://hz.ppjwa.cn/gtwjelinrd.html

[U47] PHP：联合类型
来源：http://hz.0kj1m.cn/gtkeaqzfty.html

int|string $id
来源：http://hz.wangdashe.top/gtwbnzyiqv.html

[U48] PHP：纯枚举
来源：http://hz.yj20258.top/gtdivwsnvw.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.mhx1999.top/gtnzetolwb.html

[U49] PHP：只读属性
来源：http://hz.jinqigfzy.top/gtlazkgkkm.html

public readonly string $name
来源：http://hz.dashuyun.cn/gtjpwjtxwi.html

[U50] PHP：构造器属性提升
来源：http://hz.hammf.cn/gtvloampic.html

public function __construct(private int $id) {}
来源：http://hz.cheryme.top/gthalyjsob.html

[U51] PHP：数组解构
来源：http://hz.xingfuxueyuan.xyz/gtpbngfnti.html

[$a, $b] = $arr;
来源：http://hz.sxryk.cn/gtwgcyrrxn.html

[U52] PHP：箭头函数
来源：http://hz.zhongyouzk.top/gtnuvvfzpt.html

$double = fn($x) => $x * 2;
来源：http://hz.sxryk.cn/gtgortgjac.html

[U53] PHP：空合并运算符
来源：http://hz.jqgfzy.top/gtyzwnkgvf.html

$v = $a ?? $b ?? "default";
来源：http://hz.redwolf501.top/gtkfimjiqb.html

[U54] PHP：空安全调用
来源：http://hz.cheryme.top/gtprxzvhmg.html

$obj?->method()
来源：http://hz.ywan-chungtsiang.top/gtrmaprczf.html

[U55] PHP：match 表达式
来源：http://hz.jiagoushi.top/gtdostcqwk.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.jqgfzy.top/gtlgftaiwa.html

[U56] PHP：命名参数
来源：http://hz.wangshuangyany.cn/gtmmlddjfo.html

f(a: 1, b: 2)
来源：http://hz.jqgfzy.top/gtczilbcvq.html

[U57] PHP：字符串插值
来源：http://hz.zhaomingkeji.xyz/gtejaeeuvo.html

"值: {$a}"
来源：http://hz.wangdashe.top/gtzgzojbdc.html

[U58] PHP：数组三件套
来源：http://hz.daxiang520.top/gtbuboyoga.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.sufxvd.cn/gtfmbkqgco.html

[U59] PHP：自定义排序
来源：http://hz.hongshengwenyu.top/gtaellfrhw.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yj20258888.top/gtyqdltnol.html

[U60] PHP：JSON 编解码
来源：http://hz.yj202588.top/gtrydtywim.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.bjfxy.top/gtcxbiypgv.html

[U61] PHP：正则
来源：http://hz.jinqigfzy.top/gtcqdbpiig.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhixingplan.top/gtlbfqpfuf.html

[U62] PHP：日期对象
来源：http://hz.jinqigfzy.top/gtukreslul.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.vqdsnc.cn/gtfpikgxud.html

[U63] PHP：文件读写
来源：http://hz.0kj1m.cn/gttckgyvdd.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.jiagoushi.top/gtefvppevs.html

[U64] PHP：目录遍历
来源：http://hz.jlsjyb.cn/gtrqfzoatv.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.zhijiandao.cn/gtwepdyqcr.html

[U65] PHP：会话
来源：http://hz.hammf.cn/gteveydzod.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.zhiwuduotai.top/gtxguerqwa.html

[U66] PHP：设置 Cookie
来源：http://hz.sweek.top/gtdohlasgl.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.zhengqikj.top/gtyqcengpx.html

[U67] PHP：处理文件上传
来源：http://hz.aizwys.cn/gtemdwwmkn.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.pycfn.com/gtxemwamzd.html

[U68] PHP：PDO 连接
来源：http://hz.wangshuangyany.cn/gtmwoujfun.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.hnxiangtu.top/gthxulbeak.html

[U69] PHP：PDO 预处理
来源：http://hz.svipenyu.cn/gtpwdzllll.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.yuxming.cn/gtpxcbpgvl.html

[U70] PHP：PDO 事务
来源：http://hz.tianlin.xyz/gtwccvtirl.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.hysaishi.cn/gtwxkehhlf.html

[U71] PHP：抛出异常
来源：http://hz.aibaodan.cn/gtropzwbrm.html

throw new RuntimeException("失败", 500);
来源：http://hz.andypj.xyz/gthhpcichm.html

[U72] PHP：写错误日志
来源：http://hz.sweek.top/gtcimhekdd.html

error_log("失败: " . $e->getMessage());
来源：http://hz.jinghuilouyu.cn/gtpmqiqpjd.html

[U73] PHP：读取 ini 配置
来源：http://hz.wangshuangyany.cn/gtbyhnbioh.html

parse_ini_file("config.ini", true)
来源：http://hz.aizwys.cn/gtmxkowuka.html

[U74] PHP：读取环境变量
来源：http://hz.gotoacloud.top/gtxphjzvow.html

getenv("APP_ENV") ?: "production"
来源：http://hz.ydjk.org.cn/gtvfoxhmot.html

[U75] PHP：依赖注入
来源：http://hz.tian-w.cn/gtpsybksek.html

composer require psr/container
来源：http://hz.xingfuxueyuan.xyz/gtqhwwuvwy.html

[U76] PHP：简单路由
来源：http://hz.nwbrower.top/gtnkfpdxbz.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.gaohongyu789.top/gtfmvzikdn.html

[U77] PHP：模板渲染
来源：http://hz.mhx1999.top/gtrmcvzfvx.html

composer require twig/twig
来源：http://hz.jinqigufen.top/gtkxmgcjif.html

[U78] PHP：单元测试
来源：http://hz.c1oappe.top/gtyzqctzze.html

composer require --dev phpunit/phpunit
来源：http://hz.sweek.top/gtfcstmohx.html

[U79] PHP：静态分析
来源：http://hz.sxryk.cn/gthfcugcvs.html

composer require --dev phpstan/phpstan
来源：http://hz.yj20258888.top/gtfdcucyax.html

[U80] PHP：代码规范修复
来源：http://hz.guannengcc.top/gtopjwkwsj.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.ywan-chungtsiang.top/gtduvzzwto.html

[U81] JS：初始化项目
来源：http://hz.xingfuxueyuan.xyz/gttespapor.html

npm init -y;  npm i express
来源：http://hz.aizwys.cn/gtblssfdnn.html

[U82] JS：package.json 脚本
来源：http://hz.jinqigfzy.top/gtndbmzkbm.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.zhiwuduotai.top/gtifplucxy.html

[U83] JS：ES Module 导入导出
来源：http://hz.sysykeji.top/gtxlqmfysr.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.yj20258.top/gtneyifykn.html

[U84] JS：CommonJS 写法
来源：http://hz.yanxiufei.cn/gtcpzezzns.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.dianchejie.cn/gtvqcrcijg.html

[U85] JS：可选链
来源：http://hz.gogol.net.cn/gtdnrzjvag.html

a?.b?.c
来源：http://hz.zhiwuduotai.top/gthrrpcoqy.html

[U86] JS：空值合并
来源：http://hz.zdqjudy.top/gtvyifmlaa.html

a ?? b
来源：http://hz.xylfe.cn/gtjtxyjczc.html

[U87] JS：解构默认值
来源：http://hz.fzhhl.top/gtlnmhftvt.html

const { a = 1, b = 2 } = obj;
来源：http://hz.52xcode.cn/gtecaadnvt.html

[U88] JS：对象展开合并
来源：http://hz.sweek.top/gtsajhcpbz.html

{ ...a, ...b }
来源：http://hz.xuetiantiany.cn/gtowxodgmc.html

[U89] JS：数组去重
来源：http://hz.shangyingyoupin.top/gtmuzyvdnx.html

[...new Set(arr)]
来源：http://hz.zhijiandao.cn/gtnydqhaiu.html

[U90] JS：数字数组排序
来源：http://hz.ydjk.org.cn/gtpkcgdkhf.html

[...arr].sort((a, b) => a - b)
来源：http://hz.daria6918.cn/gthgomwolk.html

[U91] JS：对象键值遍历
来源：http://hz.wangshuangyany.cn/gtkmnatoja.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.sufxvd.cn/gtuhpfxorj.html

[U92] JS：深拷贝
来源：http://hz.hongshengwenyu.top/gtlvxgakpy.html

structuredClone(obj)
来源：http://hz.tian-w.cn/gtpvbdxtgy.html

[U93] JS：模板字符串
来源：http://hz.hysaishi.cn/gtgpugtpun.html

`共 ${n} 条`
来源：http://hz.hfpthk.cn/gtyuzusxss.html

[U94] JS：箭头函数
来源：http://hz.pycfn.com/gtpleimbiu.html

const double = x => x * 2;
来源：http://hz.9152youxi.cn/gtnbadvtpa.html

[U95] JS：Promise 包装
来源：http://hz.chenlongwang.top/gttodrfkvd.html

new Promise((resolve, reject) => {})
来源：http://hz.316326.xyz/gthamuwtth.html

[U96] JS：async/await 与异常
来源：http://hz.shzxlz.cn/gtxwzslijy.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.hywenlv.cn/gtjaukmxyk.html

[U97] JS：并发请求
来源：http://hz.xuetiantiany.cn/gtvzbffyuq.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.nanxuanxn.top/gtfalwhilw.html

[U98] JS：fetch 带 JSON
来源：http://hz.mhx1999.top/gtkwnamfkk.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.feifeiyinyue.top/gthqhhuoum.html

[U99] JS：事件监听
来源：http://hz.sufxvd.cn/gtmffyrbtn.html

el.addEventListener("click", e => {})
来源：http://hz.hammf.cn/gtwswmakew.html

[U100] JS：DOM 查询
来源：http://hz.nanxuanxn.top/gtjnlfrlhu.html

document.querySelector(".item")
来源：http://hz.fengsongda.top/gtpnfjrrjd.html

[U101] JS：classList 操作
来源：http://hz.chenlongwang.top/gtfpcpdkcu.html

el.classList.toggle("active")
来源：http://hz.cheryme.top/gtabztagwj.html

[U102] JS：本地存储
来源：http://hz.iojbl.cn/gttjzlvpfm.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.jlsjyb.cn/gtasthlilf.html

[U103] JS：定时器
来源：http://hz.0kj1m.cn/gtoxlpeduh.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.zdqjudy.top/gtmhtkyuwn.html

[U104] JS：防抖
来源：http://hz.hywenlv.cn/gtpziggqri.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shanyushiyangtech.top/gtxlqmiqia.html

[U105] JS：节流
来源：http://hz.zhoulong.xyz/gtqiynstjs.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.zhoulong.xyz/gtbnbzzwzl.html

[U106] JS：日期格式化
来源：http://hz.daria6918.cn/gtunivvwqz.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.hongshengwenyu.top/gtdtxaypny.html

[U107] JS：数字千分位
来源：http://hz.wangdashe.top/gtoltbsmzf.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.zhiwuduotai.top/gtdyugttpl.html

[U108] JS：随机整数
来源：http://hz.dianchejie.cn/gtilkfyuse.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.ywan-chungtsiang.top/gtqhjfvtqd.html

[U109] JS：数组分组
来源：http://hz.yueranfly.top/gtxufgemhv.html

Object.groupBy(arr, x => x.type)
来源：http://hz.jianghu66.top/gtwuwtwzsk.html

[U110] JS：数组分块
来源：http://hz.daxiang520.top/gtzjtvkzpn.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.zhongyouzk.top/gtzeriqfvh.html

[U111] JS：对象转 Map
来源：http://hz.yvedp.cn/gtscearxml.html

new Map(Object.entries(obj))
来源：http://hz.zhengqikj.top/gtnllggiii.html

[U112] JS：字符串补位
来源：http://hz.tian-w.cn/gtfmvebmgy.html

"7".padStart(3, "0")
来源：http://hz.dashuyun.cn/gttjmmtcrl.html

[U113] JS：正则替换全部
来源：http://hz.chenlongwang.top/gtzbsaignu.html

s.replaceAll("a", "b")
来源：http://hz.pengpengdd.cyou/gtyoeigxhm.html

[U114] JS：JSON 深比较
来源：http://hz.wangdashe.top/gtbilfjvja.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zhiwuduotai.top/gtthzsvxjl.html

[U115] JS：生成 UUID
来源：http://hz.c1oappe.top/gtavnxdlfn.html

crypto.randomUUID()
来源：http://hz.jinqigufen.top/gtsyayofnx.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.redwolf501.top/gtipekhgnl.html

/** @param {string} name */ function f(name) {}
来源：http://hz.ywan-chungtsiang.top/gthtjwtznw.html

[U117] JS：单元测试
来源：http://hz.chenlongwang.top/gtsrevowjx.html

npm i -D vitest;  npx vitest
来源：http://hz.redwolf501.top/gtftbxtnyo.html

[U118] JS：开发服务器
来源：http://hz.nanxinkj.top/gteayvczlm.html

npm i -D vite;  npx vite
来源：http://hz.shanyushiyangtech.top/gtrupwsyee.html

[U119] JS：生产构建
来源：http://hz.zhoulong.xyz/gtvaynykck.html

npx vite build
来源：http://hz.yuanzhike.top/gtiwuadldk.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.yuxming.cn/gtruikydlo.html

import.meta.env.VITE_API_URL
来源：http://hz.cheryme.top/gtolwstzcv.html

================================================================================
来源：http://hz.gaohongyu789.top/gteavvbcfx.html

统计汇总
来源：http://hz.yueranfly.top/gtlpvnsnsv.html

================================================================================
来源：http://hz.ybcxt.top/gtccxxzrhs.html

按语言统计（条）：
来源：http://hz.yangfankeji.com/gtxojzerkh.html

Python ......... 252
来源：http://hz.nanxuanxn.top/gtmuexlqsl.html

PHP ............ 252
来源：http://hz.xuanzx.com/gtmdusoxdn.html

JavaScript ..... 252
来源：http://hz.aibaodan.cn/gttwysatoz.html

TypeScript ..... 212
来源：http://hz.chenjidiqi.icu/gtakkrqohr.html

Java ........... 212
来源：http://hz.dianchejie.cn/gtmdkddtfl.html

Go ............. 212
来源：http://hz.zdqjudy.top/gtqqhlamnn.html

Ruby ........... 212
来源：http://hz.zhijiandao.cn/gtzajdevdz.html

C# ............. 212
来源：http://hz.9152youxi.cn/gtlyxmadwn.html

C .............. 30
来源：http://hz.fengsongda.top/gttvsclnui.html

C++ ............ 30
来源：http://hz.xuanzx.com/gtqfsamxdg.html

SQL ............ 90
来源：http://hz.yj202588.top/gtouefnhdp.html

Bash ........... 80
来源：http://hz.shzxlz.cn/gthkjtsooe.html

Kotlin ......... 15
来源：http://hz.fengsongda.top/gthszlgcub.html

Swift .......... 15
来源：http://hz.316326.xyz/gtzcfkaurw.html

Lua ............ 10
来源：http://hz.shanyushiyangtech.top/gtdgptrdda.html

Perl ........... 10
来源：http://hz.xuanzx.com/gtxfxorypd.html

Scala .......... 10
来源：http://hz.wangdashe.top/gtuwyowroh.html

------------------------------------
来源：http://hz.zdqjudy.top/gtfyyufkui.html

合计 ........... 2106 条
来源：http://hz.jianghu66.top/gtglwccuaf.html

按章节统计：
来源：http://hz.jqgufenzy.top/gtloqagzlz.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.hongshengwenyu.top/gtozcxlkyq.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.jqgufenzy.top/gtlrpqauvv.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.xuetiantiany.cn/gtaxwkyxyu.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.yongpay.top/gtiqbnwvhn.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.jinqigufen.top/gtisoyazxy.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.sufxvd.cn/gtgghklkte.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.ywan-chungtsiang.top/gtsxhvxrdt.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.iojbl.cn/gtqgqqevfs.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.hnxiangtu.top/gtaqjjkwfq.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.ydjk.org.cn/gtfxxiufej.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.yueranfly.top/gtjuiahpnj.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.chenlongwang.top/gtblzimwho.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.cucudq.cn/gtkiilzxet.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.wangdashe.top/gtrysedsku.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.wangdashe.top/gthnbgqatw.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.9152youxi.cn/gtdeoclpwf.html

Q SQL 专题                              90
来源：http://hz.shangyingyoupin.top/gtdiaphdnb.html

R Bash 专题                             80
来源：http://hz.pycfn.com/gtiakyppjw.html

S C / C++ 专题                          60
来源：http://hz.jinghuilouyu.cn/gtgkpgpszo.html

T 其他语言补充                          60
来源：http://hz.sxryk.cn/gtqfbrbrvb.html

U 高频实用片段                         120
来源：http://hz.zhengqikj.top/gtdlbkjggx.html

------------------------------------
来源：http://hz.cheryme.top/gtyrmgwaoa.html

合计                                  2106 条
来源：http://hz.zdqjudy.top/gtcloqqdep.html

--------------------------------------------------------------------------------
来源：http://hz.yj20258888.top/gtixyorzle.html

使用提醒
来源：http://hz.jinghuilouyu.cn/gtyfdiiyla.html

--------------------------------------------------------------------------------
来源：http://hz.hywenlv.cn/gtejgrfhcd.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.dashuyun.cn/gtkwfarxrh.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.jyoumei.cn/gtremyfpvd.html


<!-- 参考信息 -->