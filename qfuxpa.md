代发 wailian999

[U13] Py：固定长度队列
来源：http://hz.sxryk.cn/gtnjobowrg.html

deque(maxlen=10)
来源：http://hz.tanke756.top/gtkvezrxgf.html

[U14] Py：分组收集到列表
来源：http://hz.xziqi.cn/gtcdhmxwph.html

defaultdict(list)
来源：http://hz.ywan-chungtsiang.top/gtorecgewn.html

[U15] Py：高精度计时
来源：http://hz.jiagoushi.top/gtjhyznqij.html

t = time.perf_counter()
来源：http://hz.zhixingplan.top/gtzhnjudpo.html

[U16] Py：命令行参数解析
来源：http://hz.wangshuangyany.cn/gtmovgrdli.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.jinqigufen.top/gtzahsacxm.html

[U17] Py：初始化日志
来源：http://hz.yongpay.top/gtwkxtcavg.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.guannengcc.top/gtprkjxfxi.html

[U18] Py：预编译正则
来源：http://hz.wangshuangyany.cn/gtqngcaydp.html

pat = re.compile(r"\d+")
来源：http://hz.kuanghao11.cn/gtpfmkiumv.html

[U19] Py：正则替换带回调
来源：http://hz.gotoacloud.top/gtmisraggn.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.havefunace.top/gtqtrslzsh.html

[U20] Py：缓存函数结果
来源：http://hz.wangdashe.top/gtgyfvsirm.html

@functools.lru_cache(maxsize=None)
来源：http://hz.kuanghao11.cn/gtobtrhbyk.html

[U21] Py：自定义上下文管理器
来源：http://hz.birdmap.top/gturenthjk.html

@contextlib.contextmanager
来源：http://hz.xuetiantiany.cn/gtlbhjxawm.html

[U22] Py：矩阵转置
来源：http://hz.chenlongwang.top/gtszmbmmjw.html

list(zip(*m))
来源：http://hz.ybcxt.top/gtdzesaypi.html

[U23] Py：分块读取大文件
来源：http://hz.cashguo.top/gtokjevgvc.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.quarkkingdee.top/gtdhpzxsoc.html

[U24] Py：路径操作
来源：http://hz.redwolf501.top/gtwcfpyxzd.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.birdmap.top/gtgqkypqll.html

[U25] Py：CSV 按字典读
来源：http://hz.ivvv.top/gtcxuwuaxf.html

csv.DictReader(f)
来源：http://hz.hysaishi.cn/gtswjqtbol.html

[U26] Py：并发下载
来源：http://hz.jinyuanbaomall.cn/gtutmozawo.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.hongshengwenyu.top/gtbbivdwir.html

[U27] Py：异步 HTTP
来源：http://hz.xinyue.icu/gtqkyjnjxz.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.shanyushiyangtech.top/gttbmbkidu.html

[U28] Py：类型别名
来源：http://hz.iojbl.cn/gtqhrkqtsy.html

UserId = int
来源：http://hz.daria6918.cn/gtadwjixnf.html

[U29] Py：属性校验
来源：http://hz.chenzaomai.com/gtislvhbhu.html

@property 与 @x.setter 配合
来源：http://hz.zycfv.cn/gtjuuqhpiw.html

[U30] Py：数据类
来源：http://hz.shzxlz.cn/gtgipwgtqr.html

@dataclass(slots=True)
来源：http://hz.shanyushiyangkeji.top/gtkahfwgzg.html

[U31] Py：单测
来源：http://hz.iojbl.cn/gtlemnjjpi.html

python -m pytest -q
来源：http://hz.ybcxt.top/gtrzscukzg.html

[U32] Py：代码格式化
来源：http://hz.yongpay.top/gtwhanigad.html

ruff format . && ruff check --fix .
来源：http://hz.0kj1m.cn/gtnwmyjlpe.html

[U33] Py：打包发布
来源：http://hz.hongshengwenyu.top/gtyfrolobc.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.hnqzz.top/gtmcyxvamg.html

[U34] Py：判断编码
来源：http://hz.gotoacloud.top/gtmreiubru.html

chardet.detect(raw)
来源：http://hz.jlsjyb.cn/gttqlihibr.html

[U35] Py：发送邮件
来源：http://hz.zhijiandao.cn/gtqekbeffz.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.yanxiufei.cn/gtjvmwfkzr.html

[U36] Py：定时任务
来源：http://hz.wangdashe.top/gtvdjwetje.html

schedule.every(10).minutes.do(job)
来源：http://hz.gogol.net.cn/gtnjvqlqbp.html

[U37] Py：读写 Excel
来源：http://hz.sufxvd.cn/gtsrucbqke.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.dianchejie.cn/gtlyepyklm.html

[U38] Py：获取脚本所在目录
来源：http://hz.zhaomingkeji.xyz/gtmcvdanfm.html

Path(__file__).resolve().parent
来源：http://hz.shzxlz.cn/gtjznxlsbt.html

[U39] Py：判断是否在交互环境
来源：http://hz.yueranfly.top/gtqmxzrhkq.html

sys.stdout.isatty()
来源：http://hz.ybcxt.top/gtuzqmnbqf.html

[U40] Py：打印到标准错误
来源：http://hz.yueranfly.top/gthalncdci.html

print("err", file=sys.stderr)
来源：http://hz.zycfv.cn/gtvdfwsimu.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.jinqigufen.top/gtkggbitxv.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.nanxinkj.top/gtprgyhicc.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.xinyue.icu/gtqhescyyh.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.xinyue.icu/gtehcomytm.html

[U43] PHP：声明命名空间
来源：http://hz.shzxlz.cn/gtrezuwamb.html

namespace App\Http;
来源：http://hz.xinyue.icu/gtwbsrxesd.html

[U44] PHP：开启严格类型
来源：http://hz.yonumen.top/gtanjbzxuf.html

declare(strict_types=1);
来源：http://hz.hammf.cn/gtpvfnrcpo.html

[U45] PHP：类型声明与返回类型
来源：http://hz.aibaodan.cn/gtlvdvzsug.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.cdnleiting.top/gtanhegwyx.html

[U46] PHP：可空类型
来源：http://hz.guannengcc.top/gtqtdtzznf.html

?string $name = null
来源：http://hz.wangshuangyany.cn/gtdtjsowzx.html

[U47] PHP：联合类型
来源：http://hz.daxiang520.top/gtyivlgnqp.html

int|string $id
来源：http://hz.chenlongwang.top/gthprrrcam.html

[U48] PHP：纯枚举
来源：http://hz.quarkkingdee.top/gtmjbllrsq.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.zycfv.cn/gtzefthbud.html

[U49] PHP：只读属性
来源：http://hz.svipenyu.cn/gtiaicojwb.html

public readonly string $name
来源：http://hz.dashuyun.cn/gtngtwwmlr.html

[U50] PHP：构造器属性提升
来源：http://hz.jyoumei.cn/gtdyqxdbxj.html

public function __construct(private int $id) {}
来源：http://hz.gotoacloud.top/gtkuvlrvlu.html

[U51] PHP：数组解构
来源：http://hz.daxiang520.top/gtclnlaxdl.html

[$a, $b] = $arr;
来源：http://hz.birdmap.top/gtaqkyffol.html

[U52] PHP：箭头函数
来源：http://hz.yanxiufei.cn/gtkkriqyvq.html

$double = fn($x) => $x * 2;
来源：http://hz.tanke756.top/gtteamtvqn.html

[U53] PHP：空合并运算符
来源：http://hz.yj202588.top/gtpmfkqbru.html

$v = $a ?? $b ?? "default";
来源：http://hz.zhoulong.xyz/gteuqbqclu.html

[U54] PHP：空安全调用
来源：http://hz.tanke756.top/gtzevmtfze.html

$obj?->method()
来源：http://hz.hywenlv.cn/gtirwohirs.html

[U55] PHP：match 表达式
来源：http://hz.xuetiantiany.cn/gtnqetjzpv.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.zhiwuduotai.top/gtjjgfckvf.html

[U56] PHP：命名参数
来源：http://hz.yvedp.cn/gtppwhdslf.html

f(a: 1, b: 2)
来源：http://hz.c1oappe.top/gtsqtfbheb.html

[U57] PHP：字符串插值
来源：http://hz.ywan-chungtsiang.top/gtmhvsggpq.html

"值: {$a}"
来源：http://hz.smart0.xyz/gtjgptzffj.html

[U58] PHP：数组三件套
来源：http://hz.xuetiantiany.cn/gtzzxomndc.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.tian-w.cn/gtkybpyjvs.html

[U59] PHP：自定义排序
来源：http://hz.hysaishi.cn/gtimzhwxgo.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yj202588.top/gtwxrpttig.html

[U60] PHP：JSON 编解码
来源：http://hz.nanxuanxn.top/gtttpegpkd.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.jinyuanbaomall.cn/gtcfehnsoj.html

[U61] PHP：正则
来源：http://hz.cdnleiting.top/gtraeiexxw.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.hnxiangtu.top/gtoehfffpk.html

[U62] PHP：日期对象
来源：http://hz.zhixingplan.top/gtoocnjwun.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.wangshuangyany.cn/gturcvcfcy.html

[U63] PHP：文件读写
来源：http://hz.xziqi.cn/gtqyqsurwh.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.jianghu66.top/gtfulrmxyg.html

[U64] PHP：目录遍历
来源：http://hz.jlsjyb.cn/gtcdpjpnzc.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.yanxiufei.cn/gtszpwyhfx.html

[U65] PHP：会话
来源：http://hz.zhongyouzk.top/gtsykrbjfm.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.hnqzz.top/gtntbfslvk.html

[U66] PHP：设置 Cookie
来源：http://hz.ybcxt.top/gthwyydpra.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.vqdsnc.cn/gtqewgtpes.html

[U67] PHP：处理文件上传
来源：http://hz.zdqjudy.top/gtaciwrkkj.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.birdmap.top/gterhewmbh.html

[U68] PHP：PDO 连接
来源：http://hz.jinqigufen.top/gttahsulxu.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.yj20258888.top/gttpypebjp.html

[U69] PHP：PDO 预处理
来源：http://hz.52xcode.cn/gtfhecnaoq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.xuetiantiany.cn/gtitxhyzgr.html

[U70] PHP：PDO 事务
来源：http://hz.jiagoushi.top/gtsdjuthdt.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.nwbrower.top/gtqrmeemiy.html

[U71] PHP：抛出异常
来源：http://hz.zhiwuduotai.top/gtxpbxnvhi.html

throw new RuntimeException("失败", 500);
来源：http://hz.bjfxy.top/gtqkgrvfmb.html

[U72] PHP：写错误日志
来源：http://hz.mhx1999.top/gtzwkwpoqj.html

error_log("失败: " . $e->getMessage());
来源：http://hz.shuidangran.top/gtjgikrltx.html

[U73] PHP：读取 ini 配置
来源：http://hz.daxiang520.top/gtzrgqgexn.html

parse_ini_file("config.ini", true)
来源：http://hz.zycfv.cn/gttjzwkbnj.html

[U74] PHP：读取环境变量
来源：http://hz.xinyue.icu/gticzgvwvi.html

getenv("APP_ENV") ?: "production"
来源：http://hz.shangyingyoupin.top/gtlwtizuwr.html

[U75] PHP：依赖注入
来源：http://hz.redwolf501.top/gtnpxywgym.html

composer require psr/container
来源：http://hz.pengpengdd.cyou/gtyiduvahe.html

[U76] PHP：简单路由
来源：http://hz.c1oappe.top/gtzzdlpgrh.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.svipenyu.cn/gtfraztpox.html

[U77] PHP：模板渲染
来源：http://hz.yvedp.cn/gthdlyumpw.html

composer require twig/twig
来源：http://hz.redwolf501.top/gtodxxfzam.html

[U78] PHP：单元测试
来源：http://hz.haohaochexian.top/gtzultdswb.html

composer require --dev phpunit/phpunit
来源：http://hz.quarkkingdee.top/gtahizkgoz.html

[U79] PHP：静态分析
来源：http://hz.hammf.cn/gtlsiyjmmx.html

composer require --dev phpstan/phpstan
来源：http://hz.feifeiyinyue.top/gttiepixrc.html

[U80] PHP：代码规范修复
来源：http://hz.yongpay.top/gtcnfuvnmd.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.guannengcc.top/gtbxwavebz.html

[U81] JS：初始化项目
来源：http://hz.jinqigufen.top/gtgenqsmyb.html

npm init -y;  npm i express
来源：http://hz.hnqzz.top/gtlvbjpifv.html

[U82] JS：package.json 脚本
来源：http://hz.gzhubu.top/gtocaqmufl.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.shzxlz.cn/gtrxeeparz.html

[U83] JS：ES Module 导入导出
来源：http://hz.cdnleiting.top/gtalwxdfks.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.yuanzhike.top/gtgqgedyzd.html

[U84] JS：CommonJS 写法
来源：http://hz.wangdashe.top/gtdbmloqrd.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.zycfv.cn/gtgwvtrchn.html

[U85] JS：可选链
来源：http://hz.zhengqikj.top/gtqolrwhpn.html

a?.b?.c
来源：http://hz.yuanzhike.top/gtvdsaahyt.html

[U86] JS：空值合并
来源：http://hz.nanxinkj.top/gtjhhstzct.html

a ?? b
来源：http://hz.zhiwuduotai.top/gtgpatouov.html

[U87] JS：解构默认值
来源：http://hz.ydzc1.top/gtxkcfhksh.html

const { a = 1, b = 2 } = obj;
来源：http://hz.dashuyun.cn/gtdcsyvpzk.html

[U88] JS：对象展开合并
来源：http://hz.jiagoushi.top/gtjzqmhhyi.html

{ ...a, ...b }
来源：http://hz.hysaishi.cn/gttglocoxc.html

[U89] JS：数组去重
来源：http://hz.jqgufenzy.top/gtezogyjgx.html

[...new Set(arr)]
来源：http://hz.xziqi.cn/gtqazookud.html

[U90] JS：数字数组排序
来源：http://hz.shanyushiyangtech.top/gtockfmtab.html

[...arr].sort((a, b) => a - b)
来源：http://hz.haohaochexian.top/gtdrqmcpui.html

[U91] JS：对象键值遍历
来源：http://hz.wangdashe.top/gtdsrtiphu.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.yvedp.cn/gtmekxsyck.html

[U92] JS：深拷贝
来源：http://hz.52xcode.cn/gtmohbaeda.html

structuredClone(obj)
来源：http://hz.cheryme.top/gtpnogmcpe.html

[U93] JS：模板字符串
来源：http://hz.c1oappe.top/gtxojbuxid.html

`共 ${n} 条`
来源：http://hz.jinghuilouyu.cn/gtykyuqzty.html

[U94] JS：箭头函数
来源：http://hz.bjfxy.top/gtgsvedmdf.html

const double = x => x * 2;
来源：http://hz.yj202588.top/gtlquvzats.html

[U95] JS：Promise 包装
来源：http://hz.yanxiufei.cn/gtxrppccer.html

new Promise((resolve, reject) => {})
来源：http://hz.xuanzx.com/gtqgedumei.html

[U96] JS：async/await 与异常
来源：http://hz.andypj.xyz/gtrccmcuyt.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.yj202588.top/gtyrlkcmxf.html

[U97] JS：并发请求
来源：http://hz.tanke756.top/gtiqsbwrgc.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.bjfxy.top/gtwfkfcgbk.html

[U98] JS：fetch 带 JSON
来源：http://hz.tian-w.cn/gtjmbrzdxn.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.gotoacloud.top/gtflyxvzep.html

[U99] JS：事件监听
来源：http://hz.pengpengdd.cyou/gtirvtbmps.html

el.addEventListener("click", e => {})
来源：http://hz.smart0.xyz/gtutxnbqyu.html

[U100] JS：DOM 查询
来源：http://hz.ivvv.top/gtfeuclnoc.html

document.querySelector(".item")
来源：http://hz.ydzc1.top/gttopveaan.html

[U101] JS：classList 操作
来源：http://hz.zhixingplan.top/gthyaeqszo.html

el.classList.toggle("active")
来源：http://hz.zdqjudy.top/gtosyqlnoi.html

[U102] JS：本地存储
来源：http://hz.chenjidiqi.icu/gtofwxbldb.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.nwbrower.top/gtktwpeykk.html

[U103] JS：定时器
来源：http://hz.fengsongda.top/gtaqggyexn.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.chenjidiqi.icu/gtgqwqnayc.html

[U104] JS：防抖
来源：http://hz.gaohongyu789.top/gtckbojhey.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xinyue.icu/gtqtdeaxxe.html

[U105] JS：节流
来源：http://hz.yuxming.cn/gtwxnhtcmq.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.ehwqpu.com/gtzokuhcbr.html

[U106] JS：日期格式化
来源：http://hz.shanyushiyangtech.top/gtwsroaufw.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.shanyushiyangkeji.top/gtnanfdcxs.html

[U107] JS：数字千分位
来源：http://hz.gotoacloud.top/gtkvmsfymc.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.hfpthk.cn/gtxquyleeg.html

[U108] JS：随机整数
来源：http://hz.iojbl.cn/gtmednaopv.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.yvedp.cn/gtrsjuxksg.html

[U109] JS：数组分组
来源：http://hz.zhaomingkeji.xyz/gtjqinrqiy.html

Object.groupBy(arr, x => x.type)
来源：http://hz.guannengcc.top/gtjyfcyiyg.html

[U110] JS：数组分块
来源：http://hz.ydzc1.top/gtmncsvsjg.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.mhx1999.top/gtvkdkbuto.html

[U111] JS：对象转 Map
来源：http://hz.hnqzz.top/gtihdkocyl.html

new Map(Object.entries(obj))
来源：http://hz.yongpay.top/gtmersjkxo.html

[U112] JS：字符串补位
来源：http://hz.ywan-chungtsiang.top/gtntasrdgv.html

"7".padStart(3, "0")
来源：http://hz.yongpay.top/gtmtekesrn.html

[U113] JS：正则替换全部
来源：http://hz.zhijiandao.cn/gtwquzacdc.html

s.replaceAll("a", "b")
来源：http://hz.ivvv.top/gtzzlbdjqs.html

[U114] JS：JSON 深比较
来源：http://hz.iojbl.cn/gtujorhptd.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.cucudq.cn/gtpqzxikxf.html

[U115] JS：生成 UUID
来源：http://hz.haohaochexian.top/gtmlytpgen.html

crypto.randomUUID()
来源：http://hz.guannengcc.top/gtkeualxcj.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.ydzc1.top/gtfglwwsts.html

/** @param {string} name */ function f(name) {}
来源：http://hz.birdmap.top/gtynovscml.html

[U117] JS：单元测试
来源：http://hz.ywan-chungtsiang.top/gtucumwljp.html

npm i -D vitest;  npx vitest
来源：http://hz.smart0.xyz/gtirjywghc.html

[U118] JS：开发服务器
来源：http://hz.zhaomingkeji.xyz/gtrgdygydo.html

npm i -D vite;  npx vite
来源：http://hz.sysykeji.top/gtjfnwoliq.html

[U119] JS：生产构建
来源：http://hz.shanyushiyangtech.top/gtgieiyjrg.html

npx vite build
来源：http://hz.xziqi.cn/gtefxsfioo.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.xziqi.cn/gtxpmtinzc.html

import.meta.env.VITE_API_URL
来源：http://hz.cucudq.cn/gtehhuqhjf.html

================================================================================
来源：http://hz.cucudq.cn/gtgzfifjgk.html

统计汇总
来源：http://hz.shanyushiyangtech.top/gthfpjbsyc.html

================================================================================
来源：http://hz.jianghu66.top/gtdwtwfctc.html

按语言统计（条）：
来源：http://hz.jiagoushi.top/gttbnipdiv.html

Python ......... 252
来源：http://hz.zhoulong.xyz/gthmotzqnt.html

PHP ............ 252
来源：http://hz.smart0.xyz/gtjfdniijd.html

JavaScript ..... 252
来源：http://hz.yongpay.top/gtwvmnpbih.html

TypeScript ..... 212
来源：http://hz.zhengqikj.top/gtxzoeeynm.html

Java ........... 212
来源：http://hz.yuxming.cn/gtcrspswvw.html

Go ............. 212
来源：http://hz.sxryk.cn/gtndcquagl.html

Ruby ........... 212
来源：http://hz.52xcode.cn/gtjfnansnf.html

C# ............. 212
来源：http://hz.yvedp.cn/gtpwuqllyu.html

C .............. 30
来源：http://hz.sxryk.cn/gtjechhicy.html

C++ ............ 30
来源：http://hz.dianchejie.cn/gtmasmbdtd.html

SQL ............ 90
来源：http://hz.dianchejie.cn/gtrlaaaeqv.html

Bash ........... 80
来源：http://hz.jqgufenzy.top/gturnsgggk.html

Kotlin ......... 15
来源：http://hz.jinqigufen.top/gtsztwoztf.html

Swift .......... 15
来源：http://hz.havefunace.top/gtjrnfmers.html

Lua ............ 10
来源：http://hz.yj20258888.top/gtwqnudfdl.html

Perl ........... 10
来源：http://hz.yongpay.top/gtxkxyggne.html

Scala .......... 10
来源：http://hz.cdnleiting.top/gtzbydhdrg.html

------------------------------------
来源：http://hz.pycfn.com/gtdgyiatkc.html

合计 ........... 2106 条
来源：http://hz.ivvv.top/gtzskqbbqy.html

按章节统计：
来源：http://hz.gaohongyu789.top/gtixvpaxfq.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.hnxiangtu.top/gtgteiljqj.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.ywan-chungtsiang.top/gtpcrpnzjk.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.zhengqikj.top/gtgedcmsnx.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.ivvv.top/gtovcgbkpp.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.chenjidiqi.icu/gtzbtjzulj.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.zhengqikj.top/gtlwsfzzty.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.yangfankeji.com/gtjdfqrmhs.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.redwolf501.top/gtrcedbizs.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.dianchejie.cn/gtscsypdui.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.redwolf501.top/gtmjabohoq.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.chenzaomai.com/gtsuynkrde.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.smart0.xyz/gtbojendhe.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.cheryme.top/gtbvnvxplz.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.dashuyun.cn/gtxezabmxn.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.gzhubu.top/gtbiifhcmn.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.zhengqikj.top/gtlhifznsw.html

Q SQL 专题                              90
来源：http://hz.tianlin.xyz/gthmkcemyj.html

R Bash 专题                             80
来源：http://hz.meibo888.top/gttepoqnqf.html

S C / C++ 专题                          60
来源：http://hz.tian-w.cn/gtetgkpzfw.html

T 其他语言补充                          60
来源：http://hz.cqqwz.cn/gtcmpgtzyj.html

U 高频实用片段                         120
来源：http://hz.ydzc1.top/gtzcetdvjf.html

------------------------------------
来源：http://hz.gotoacloud.top/gtyrorfpho.html

合计                                  2106 条
来源：http://hz.jlsjyb.cn/gtzwkqxzvc.html

--------------------------------------------------------------------------------
来源：http://hz.gzhubu.top/gtignwnhfj.html

使用提醒
来源：http://hz.quarkkingdee.top/gtpdslmsno.html

--------------------------------------------------------------------------------
来源：http://hz.jlsjyb.cn/gtqoltwpdi.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.jinghuilouyu.cn/gtmvzgvprm.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.hongshengwenyu.top/gtpuoyduho.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.guowangkeji.top/gtvfmokssd.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.svipenyu.cn/gttwnzygul.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.ydzc1.top/gtflolcsta.html

—— 文件结束 ——
来源：http://hz.chenjidiqi.icu/gttwngfzjf.html

================================================================================
来源：http://hz.xylfe.cn/gthyjcxgic.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.wangshuangyany.cn/gtmfkdzcxu.html

Common Programming Examples Cheat Book
来源：http://hz.sysykeji.top/gtcczcvqae.html

================================================================================
来源：http://hz.9152youxi.cn/gtczsyjanw.html

【收录内容】
来源：http://hz.0kj1m.cn/gtzitrjtan.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.tanke756.top/gtjmefcqzo.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.jinghuilouyu.cn/gtflzvaprt.html

SQL · Bash · C · C++
来源：http://hz.jqgufenzy.top/gtpysbrwjk.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.jqgfzy.top/gtuemwiamu.html

【使用说明】
来源：http://hz.iojbl.cn/gtcctfyfil.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.yonumen.top/gtipboeczd.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.hysaishi.cn/gtktpdhpiz.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.bjfxy.top/gtksumrqgt.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.aizwys.cn/gtoditkwbm.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.chenzaomai.com/gtqghvtajt.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.cashguo.top/gtmmrrbwov.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.guowangkeji.top/gtwahwaigd.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.zycfv.cn/gtvqoequde.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.cdnleiting.top/gtgyywnhqj.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.shuidangran.top/gtlswverwa.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.xinyue.icu/gtnlnxlern.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.xinyue.icu/gtgmsijvxn.html

【文件统计】
来源：http://hz.jiagoushi.top/gtoxpdzrce.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.yongpay.top/gtndhhlnmx.html

--------------------------------------------------------------------------------
来源：http://hz.cashguo.top/gtpayqazay.html

目  录
来源：http://hz.zycfv.cn/gtjlcsxgxj.html

--------------------------------------------------------------------------------
来源：http://hz.jiagoushi.top/gtzgzzpnrg.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.jyoumei.cn/gtoxnwvlbq.html


<!-- 参考信息 -->