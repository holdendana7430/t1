代发 wailian999

[U23] Py：分块读取大文件
来源：http://hz.ppjwa.cn/gtjyyzulqj.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.c1oappe.top/gtoevasztx.html

[U24] Py：路径操作
来源：http://hz.cdnleiting.top/gtxvophxpy.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.iojbl.cn/gtchqzzyin.html

[U25] Py：CSV 按字典读
来源：http://hz.yj20258888.top/gtaabnnvsz.html

csv.DictReader(f)
来源：http://hz.svipenyu.cn/gtgumrckcv.html

[U26] Py：并发下载
来源：http://hz.jinqigufen.top/gtqolpjbhh.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.shzxlz.cn/gtvpkajlwv.html

[U27] Py：异步 HTTP
来源：http://hz.yongpay.top/gtcxsxynvz.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.ybcxt.top/gtdharxruu.html

[U28] Py：类型别名
来源：http://hz.shangyingyoupin.top/gtwfkyyrux.html

UserId = int
来源：http://hz.ivvv.top/gtscggnihh.html

[U29] Py：属性校验
来源：http://hz.svipenyu.cn/gtxopnsloj.html

@property 与 @x.setter 配合
来源：http://hz.gzhubu.top/gttwyctpfb.html

[U30] Py：数据类
来源：http://hz.cucudq.cn/gtcphjcpjd.html

@dataclass(slots=True)
来源：http://hz.shanyushiyangkeji.top/gtzhhezfuk.html

[U31] Py：单测
来源：http://hz.0kj1m.cn/gtcwdxgwmo.html

python -m pytest -q
来源：http://hz.yuxming.cn/gtwsyeqmqu.html

[U32] Py：代码格式化
来源：http://hz.sysykeji.top/gtvvovxwci.html

ruff format . && ruff check --fix .
来源：http://hz.svipenyu.cn/gtwqjkcfhf.html

[U33] Py：打包发布
来源：http://hz.daria6918.cn/gtgubtgobq.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.andypj.xyz/gtxhgrulih.html

[U34] Py：判断编码
来源：http://hz.hammf.cn/gtlywpebwi.html

chardet.detect(raw)
来源：http://hz.yuanzhike.top/gtgjixvbgp.html

[U35] Py：发送邮件
来源：http://hz.andypj.xyz/gtfqmkbivw.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.hammf.cn/gtgpywwvad.html

[U36] Py：定时任务
来源：http://hz.ydzc1.top/gtjribtxce.html

schedule.every(10).minutes.do(job)
来源：http://hz.cashguo.top/gtknikkcdy.html

[U37] Py：读写 Excel
来源：http://hz.jyoumei.cn/gtzdqqksdb.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.yj20258888.top/gttnucstlk.html

[U38] Py：获取脚本所在目录
来源：http://hz.cqqwz.cn/gtcrdxsslt.html

Path(__file__).resolve().parent
来源：http://hz.fzhhl.top/gtgpjjunfs.html

[U39] Py：判断是否在交互环境
来源：http://hz.gaohongyu789.top/gtxxverkdm.html

sys.stdout.isatty()
来源：http://hz.hongshengwenyu.top/gtcqymaluz.html

[U40] Py：打印到标准错误
来源：http://hz.redwolf501.top/gtgxalebvl.html

print("err", file=sys.stderr)
来源：http://hz.pengpengdd.cyou/gtgtdvacyv.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.yj20258.top/gtsgdljpfn.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.zhijiandao.cn/gtuapqcttr.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.hfpthk.cn/gtxhdhukzj.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.gogol.net.cn/gtnowmmlti.html

[U43] PHP：声明命名空间
来源：http://hz.xuetiantiany.cn/gtkfskmzto.html

namespace App\Http;
来源：http://hz.yj202588.top/gtljoaizyh.html

[U44] PHP：开启严格类型
来源：http://hz.shanyushiyangtech.top/gtnhkbdngm.html

declare(strict_types=1);
来源：http://hz.yanxiufei.cn/gtpvvxgpml.html

[U45] PHP：类型声明与返回类型
来源：http://hz.zdqjudy.top/gttluwrdai.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.nanxinkj.top/gtrojoktfu.html

[U46] PHP：可空类型
来源：http://hz.kuanghao11.cn/gtnrzvnskr.html

?string $name = null
来源：http://hz.meibo888.top/gtuezpjlot.html

[U47] PHP：联合类型
来源：http://hz.gotoacloud.top/gtiispueax.html

int|string $id
来源：http://hz.yonumen.top/gtjworvmji.html

[U48] PHP：纯枚举
来源：http://hz.nanxinkj.top/gtkxtgrwxe.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.wangdashe.top/gtnhygwtvz.html

[U49] PHP：只读属性
来源：http://hz.tian-w.cn/gtthrfnmpr.html

public readonly string $name
来源：http://hz.sweek.top/gtizlythgf.html

[U50] PHP：构造器属性提升
来源：http://hz.yanxiufei.cn/gtqumtgllk.html

public function __construct(private int $id) {}
来源：http://hz.hongshengwenyu.top/gtaqcnshey.html

[U51] PHP：数组解构
来源：http://hz.aizwys.cn/gtnrqvaams.html

[$a, $b] = $arr;
来源：http://hz.zhoulong.xyz/gtnsffabtn.html

[U52] PHP：箭头函数
来源：http://hz.yonumen.top/gtffczuglp.html

$double = fn($x) => $x * 2;
来源：http://hz.yj20258.top/gtgiihmqvw.html

[U53] PHP：空合并运算符
来源：http://hz.cashguo.top/gtdjplawgw.html

$v = $a ?? $b ?? "default";
来源：http://hz.jiagoushi.top/gtatxaluom.html

[U54] PHP：空安全调用
来源：http://hz.xuetiantiany.cn/gthtypfyeb.html

$obj?->method()
来源：http://hz.ivvv.top/gtuftcuvpr.html

[U55] PHP：match 表达式
来源：http://hz.iojbl.cn/gtqwcxsovn.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.jqgufenzy.top/gtzndvfxjm.html

[U56] PHP：命名参数
来源：http://hz.feifeiyinyue.top/gtlmhpqghs.html

f(a: 1, b: 2)
来源：http://hz.cashguo.top/gtqkbpbnhw.html

[U57] PHP：字符串插值
来源：http://hz.shuidangran.top/gtcyxxnzzm.html

"值: {$a}"
来源：http://hz.cucudq.cn/gtcqktswom.html

[U58] PHP：数组三件套
来源：http://hz.jinqigfzy.top/gtdvkuummi.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.havefunace.top/gtckuylrsv.html

[U59] PHP：自定义排序
来源：http://hz.xuetiantiany.cn/gtuxbkaalo.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.aibaodan.cn/gtcepynvlo.html

[U60] PHP：JSON 编解码
来源：http://hz.havefunace.top/gtuljzwrjs.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.ybcxt.top/gtzpkksoum.html

[U61] PHP：正则
来源：http://hz.hongshengwenyu.top/gtilhftmsd.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.zycfv.cn/gtbzfmydzo.html

[U62] PHP：日期对象
来源：http://hz.zhengqikj.top/gtjlspehrb.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.feifeiyinyue.top/gtwukmldee.html

[U63] PHP：文件读写
来源：http://hz.chenlongwang.top/gtvpwwdltq.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.ydzc1.top/gtetbnblst.html

[U64] PHP：目录遍历
来源：http://hz.wangdashe.top/gtwizmbmku.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.meibo888.top/gtjtqwljta.html

[U65] PHP：会话
来源：http://hz.xingfuxueyuan.xyz/gtmhkmekrs.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.yj20258.top/gtcjhdtfle.html

[U66] PHP：设置 Cookie
来源：http://hz.vqdsnc.cn/gtrkirnwgq.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.shanyushiyangkeji.top/gtryestyyy.html

[U67] PHP：处理文件上传
来源：http://hz.daxiang520.top/gtyrmtxovk.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.dashuyun.cn/gthzqksvub.html

[U68] PHP：PDO 连接
来源：http://hz.xuanzx.com/gthroebxyf.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.pengpengdd.cyou/gtxodlpjln.html

[U69] PHP：PDO 预处理
来源：http://hz.dianchejie.cn/gtgvupujdo.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.jinyuanbaomall.cn/gttlogsvlb.html

[U70] PHP：PDO 事务
来源：http://hz.tanke756.top/gttzlvfzhu.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.daria6918.cn/gtqfrnsast.html

[U71] PHP：抛出异常
来源：http://hz.smart0.xyz/gtpkmbuive.html

throw new RuntimeException("失败", 500);
来源：http://hz.jinqigfzy.top/gtlutmxbwr.html

[U72] PHP：写错误日志
来源：http://hz.feifeiyinyue.top/gtotifeqze.html

error_log("失败: " . $e->getMessage());
来源：http://hz.c1oappe.top/gtugrhdalz.html

[U73] PHP：读取 ini 配置
来源：http://hz.yonumen.top/gtmoxxdgku.html

parse_ini_file("config.ini", true)
来源：http://hz.nanxuanxn.top/gtiylrexne.html

[U74] PHP：读取环境变量
来源：http://hz.cqqwz.cn/gtqdftujmw.html

getenv("APP_ENV") ?: "production"
来源：http://hz.hnqzz.top/gtpvnbhmca.html

[U75] PHP：依赖注入
来源：http://hz.jianghu66.top/gtepconnfb.html

composer require psr/container
来源：http://hz.wangdashe.top/gtghhtdpyx.html

[U76] PHP：简单路由
来源：http://hz.chenzaomai.com/gtqdofmqjt.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.daria6918.cn/gtluytfivs.html

[U77] PHP：模板渲染
来源：http://hz.yuanzhike.top/gtlgypyeda.html

composer require twig/twig
来源：http://hz.bjfxy.top/gtarucabbr.html

[U78] PHP：单元测试
来源：http://hz.yvedp.cn/gtxazvnemq.html

composer require --dev phpunit/phpunit
来源：http://hz.kuanghao11.cn/gtutisuyak.html

[U79] PHP：静态分析
来源：http://hz.dashuyun.cn/gttckjaoqe.html

composer require --dev phpstan/phpstan
来源：http://hz.guannengcc.top/gtiqajbnat.html

[U80] PHP：代码规范修复
来源：http://hz.daria6918.cn/gtpqwbemmi.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.hongshengwenyu.top/gtvrnjoltd.html

[U81] JS：初始化项目
来源：http://hz.daxiang520.top/gtbzijmwiz.html

npm init -y;  npm i express
来源：http://hz.daxiang520.top/gtdarvptih.html

[U82] JS：package.json 脚本
来源：http://hz.svipenyu.cn/gtnfdscdbm.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.mhx1999.top/gtoabtdlmj.html

[U83] JS：ES Module 导入导出
来源：http://hz.jianghu66.top/gtthjnjwsh.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.nwbrower.top/gtvbggunzv.html

[U84] JS：CommonJS 写法
来源：http://hz.tanke756.top/gtbizvebio.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.snrcjt.cn/gtshszvveo.html

[U85] JS：可选链
来源：http://hz.yuxming.cn/gtrfqwshvz.html

a?.b?.c
来源：http://hz.shanyushiyangkeji.top/gtetutioma.html

[U86] JS：空值合并
来源：http://hz.feifeiyinyue.top/gtycmigjcj.html

a ?? b
来源：http://hz.redwolf501.top/gtvlmlkten.html

[U87] JS：解构默认值
来源：http://hz.vqdsnc.cn/gtbzwwkcpp.html

const { a = 1, b = 2 } = obj;
来源：http://hz.zhaomingkeji.xyz/gtempbjvvr.html

[U88] JS：对象展开合并
来源：http://hz.yj20258888.top/gtxrhrklum.html

{ ...a, ...b }
来源：http://hz.jqgufenzy.top/gtqrpcqdjx.html

[U89] JS：数组去重
来源：http://hz.shanyushiyangtech.top/gtjivlgvdp.html

[...new Set(arr)]
来源：http://hz.xziqi.cn/gtpgnvrpzv.html

[U90] JS：数字数组排序
来源：http://hz.jqgufenzy.top/gtlrwqopso.html

[...arr].sort((a, b) => a - b)
来源：http://hz.zycfv.cn/gtplnhmlui.html

[U91] JS：对象键值遍历
来源：http://hz.ywan-chungtsiang.top/gtzozhhgvc.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.zdqjudy.top/gtignnctro.html

[U92] JS：深拷贝
来源：http://hz.gaohongyu789.top/gtlzbhxrot.html

structuredClone(obj)
来源：http://hz.cashguo.top/gtsrrubflm.html

[U93] JS：模板字符串
来源：http://hz.c1oappe.top/gtqzzkcudt.html

`共 ${n} 条`
来源：http://hz.svipenyu.cn/gtbndudvqp.html

[U94] JS：箭头函数
来源：http://hz.dianchejie.cn/gtgqwpfqzv.html

const double = x => x * 2;
来源：http://hz.yuxming.cn/gtyuznpkmk.html

[U95] JS：Promise 包装
来源：http://hz.chenjidiqi.icu/gttijgeqrm.html

new Promise((resolve, reject) => {})
来源：http://hz.nanxuanxn.top/gtzcruhhgq.html

[U96] JS：async/await 与异常
来源：http://hz.pengpengdd.cyou/gtmboierml.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.ehwqpu.com/gtmryhfovl.html

[U97] JS：并发请求
来源：http://hz.nanxuanxn.top/gtrytntxxy.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.tanke756.top/gttrhcpfro.html

[U98] JS：fetch 带 JSON
来源：http://hz.zhongyouzk.top/gtpayjhotu.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.andypj.xyz/gteworzqqp.html

[U99] JS：事件监听
来源：http://hz.shanyushiyangtech.top/gtohqckcti.html

el.addEventListener("click", e => {})
来源：http://hz.shanyushiyangkeji.top/gtfefxltui.html

[U100] JS：DOM 查询
来源：http://hz.jlsjyb.cn/gtaafxfhad.html

document.querySelector(".item")
来源：http://hz.jiagoushi.top/gtamspgqkh.html

[U101] JS：classList 操作
来源：http://hz.gogol.net.cn/gtjewpsefv.html

el.classList.toggle("active")
来源：http://hz.yangfankeji.com/gtnxpksuab.html

[U102] JS：本地存储
来源：http://hz.snrcjt.cn/gtlhkssjvy.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.svipenyu.cn/gtybwffpmp.html

[U103] JS：定时器
来源：http://hz.ydzc1.top/gtxazstzgo.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.zhaomingkeji.xyz/gthaajqzqz.html

[U104] JS：防抖
来源：http://hz.guannengcc.top/gtqmcesepr.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xuetiantiany.cn/gtiqhdodzw.html

[U105] JS：节流
来源：http://hz.yangfankeji.com/gtfhbyorpk.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.yangfankeji.com/gtvwnylufd.html

[U106] JS：日期格式化
来源：http://hz.zhongyouzk.top/gtxwuwerxz.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.bjfxy.top/gtfgaaicgv.html

[U107] JS：数字千分位
来源：http://hz.cucudq.cn/gtfvanjnds.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.nanxinkj.top/gtxswttpsf.html

[U108] JS：随机整数
来源：http://hz.cdnleiting.top/gtodpcdlax.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.hysaishi.cn/gtlqgidkdk.html

[U109] JS：数组分组
来源：http://hz.tanke756.top/gtnbdjckuk.html

Object.groupBy(arr, x => x.type)
来源：http://hz.zhiwuduotai.top/gtnakkiisd.html

[U110] JS：数组分块
来源：http://hz.fengsongda.top/gtiogktxtj.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.smart0.xyz/gtsuvovhvd.html

[U111] JS：对象转 Map
来源：http://hz.ydjk.org.cn/gtotgkffda.html

new Map(Object.entries(obj))
来源：http://hz.316326.xyz/gtkqqdxnew.html

[U112] JS：字符串补位
来源：http://hz.wangdashe.top/gtaiovmkgj.html

"7".padStart(3, "0")
来源：http://hz.316326.xyz/gtnpotwkmq.html

[U113] JS：正则替换全部
来源：http://hz.hnxiangtu.top/gttefdlrmz.html

s.replaceAll("a", "b")
来源：http://hz.hysaishi.cn/gtidqflldx.html

[U114] JS：JSON 深比较
来源：http://hz.yangfankeji.com/gtxzlywgyr.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.c1oappe.top/gtwjaumkyr.html

[U115] JS：生成 UUID
来源：http://hz.ppjwa.cn/gteskcdfzl.html

crypto.randomUUID()
来源：http://hz.nanxuanxn.top/gtllrdxxzg.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.jianghu66.top/gtouiwkyxd.html

/** @param {string} name */ function f(name) {}
来源：http://hz.jqgfzy.top/gtajmjqbwl.html

[U117] JS：单元测试
来源：http://hz.yueranfly.top/gtimetfgfj.html

npm i -D vitest;  npx vitest
来源：http://hz.shanyushiyangkeji.top/gtrupmejdi.html

[U118] JS：开发服务器
来源：http://hz.shanyushiyangtech.top/gtmzcqqwee.html

npm i -D vite;  npx vite
来源：http://hz.chenzaomai.com/gtbrphtkiv.html

[U119] JS：生产构建
来源：http://hz.jlsjyb.cn/gtvoecdrtm.html

npx vite build
来源：http://hz.sxryk.cn/gtjtyowzvo.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.zhaomingkeji.xyz/gtqailcigw.html

import.meta.env.VITE_API_URL
来源：http://hz.yueranfly.top/gtomghhgvg.html

================================================================================
来源：http://hz.jianghu66.top/gtldubuymt.html

统计汇总
来源：http://hz.zdqjudy.top/gtvybbbjnm.html

================================================================================
来源：http://hz.hammf.cn/gtjkyaieoq.html

按语言统计（条）：
来源：http://hz.jinqigfzy.top/gtsqhmpsoq.html

Python ......... 252
来源：http://hz.gaohongyu789.top/gtygvmngla.html

PHP ............ 252
来源：http://hz.xuetiantiany.cn/gttqgvtyfw.html

JavaScript ..... 252
来源：http://hz.guannengcc.top/gthvycnkzx.html

TypeScript ..... 212
来源：http://hz.xuanzx.com/gtiltvkqsu.html

Java ........... 212
来源：http://hz.cheryme.top/gttiuqmctk.html

Go ............. 212
来源：http://hz.sufxvd.cn/gtmumodzzr.html

Ruby ........... 212
来源：http://hz.52xcode.cn/gtchkyedgz.html

C# ............. 212
来源：http://hz.fzhhl.top/gtoulsgeiu.html

C .............. 30
来源：http://hz.tian-w.cn/gtkyvupbnv.html

C++ ............ 30
来源：http://hz.xinyue.icu/gtmmzxvvup.html

SQL ............ 90
来源：http://hz.jianghu66.top/gtvoggcfoq.html

Bash ........... 80
来源：http://hz.sweek.top/gtphymljfu.html

Kotlin ......... 15
来源：http://hz.ppjwa.cn/gttbqkryqx.html

Swift .......... 15
来源：http://hz.yanxiufei.cn/gtangbakdu.html

Lua ............ 10
来源：http://hz.ywan-chungtsiang.top/gtpwyryxuk.html

Perl ........... 10
来源：http://hz.ydzc1.top/gtyztlkkdu.html

Scala .......... 10
来源：http://hz.feifeiyinyue.top/gtjjvnuxhk.html

------------------------------------
来源：http://hz.hysaishi.cn/gtcwbuutdy.html

合计 ........... 2106 条
来源：http://hz.gogol.net.cn/gthdqlokkc.html

按章节统计：
来源：http://hz.yj20258888.top/gteadvbtup.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.ehwqpu.com/gtdngpuvyi.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.0kj1m.cn/gtqroultiy.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.hnqzz.top/gthuowrmpy.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.fzhhl.top/gttqmeambp.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.ehwqpu.com/gtvexgpjtg.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.aizwys.cn/gtmiuxbjxj.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.yvedp.cn/gtaufrpoxc.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.xingfuxueyuan.xyz/gttkbwuahf.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.cheryme.top/gttrgrwhsf.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.xziqi.cn/gtapvcecqm.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.yj202588.top/gtpijsxixh.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.ydzc1.top/gtmflwzmyf.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.daxiang520.top/gtopnydowi.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.cqqwz.cn/gtnkcyvqno.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.jqgfzy.top/gtmnszselb.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.cheryme.top/gtpterhpzf.html

Q SQL 专题                              90
来源：http://hz.yj20258888.top/gtptlrlvmn.html

R Bash 专题                             80
来源：http://hz.yuxming.cn/gtwlydjtkz.html

S C / C++ 专题                          60
来源：http://hz.wangdashe.top/gtejoimrip.html

T 其他语言补充                          60
来源：http://hz.shanyushiyangkeji.top/gthqnowskw.html

U 高频实用片段                         120
来源：http://hz.yangfankeji.com/gtsgajdcml.html

------------------------------------
来源：http://hz.meibo888.top/gtpqgaxrbn.html

合计                                  2106 条
来源：http://hz.svipenyu.cn/gtisinsdtz.html

--------------------------------------------------------------------------------
来源：http://hz.cqqwz.cn/gtfknjupjw.html

使用提醒
来源：http://hz.birdmap.top/gtocpnbsik.html

--------------------------------------------------------------------------------
来源：http://hz.xziqi.cn/gtmusfttfb.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.shuidangran.top/gtcclitnsd.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.ywan-chungtsiang.top/gtrmdyaovv.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.yanxiufei.cn/gtwknyrfqz.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.316326.xyz/gtsxpfoboi.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.shuidangran.top/gtuxvxwtgd.html

—— 文件结束 ——
来源：http://hz.gzhubu.top/gtfxveshty.html

================================================================================
来源：http://hz.jiagoushi.top/gtbutgeotb.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.zdqjudy.top/gtazolxxbc.html

Common Programming Examples Cheat Book
来源：http://hz.gzhubu.top/gtvpowgugp.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtidnedfzm.html

【收录内容】
来源：http://hz.sxryk.cn/gtbwegtitx.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.ywan-chungtsiang.top/gtshsmclyu.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.cheryme.top/gttintpbxs.html

SQL · Bash · C · C++
来源：http://hz.chenjidiqi.icu/gtyvtdrrbo.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.meibo888.top/gtrsethcir.html

【使用说明】
来源：http://hz.meibo888.top/gthfqoaxkh.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.ivvv.top/gtczduuays.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.fengsongda.top/gtsbryvjdp.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.9152youxi.cn/gtqwzhmfsn.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.shanyushiyangkeji.top/gtvnqsiabe.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.nanxinkj.top/gtcefecfum.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.c1oappe.top/gtzdzcegcc.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.gzhubu.top/gtegezayeo.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.zhiwuduotai.top/gtewrtnkbb.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.yj20258.top/gtdydnlkkk.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.vqdsnc.cn/gtrxfgljlm.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.wangdashe.top/gtwcyruntx.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.wangshuangyany.cn/gtqvfcxhgx.html

【文件统计】
来源：http://hz.jianghu66.top/gtyvkgawtc.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.yangfankeji.com/gtrkcfjjbk.html

--------------------------------------------------------------------------------
来源：http://hz.ybcxt.top/gtdxtrrzxa.html

目  录
来源：http://hz.feifeiyinyue.top/gtmoyljloq.html

--------------------------------------------------------------------------------
来源：http://hz.shuidangran.top/gtgvyzqvbn.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.pengpengdd.cyou/gtmrcclkuk.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.iojbl.cn/gtbaiocrid.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.meibo888.top/gtdeeqlqlm.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.vqdsnc.cn/gtsyigwlbx.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.dashuyun.cn/gtkcjavror.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.shuidangran.top/gtzmnryhfp.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.smart0.xyz/gtdlsfipyn.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.0kj1m.cn/gtrigswure.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.xingfuxueyuan.xyz/gtteouuyds.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.gogol.net.cn/gtexzavngb.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.chenjidiqi.icu/gthlougaef.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.nanxinkj.top/gttkwaxyhj.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.yvedp.cn/gtuqjdmska.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.wangshuangyany.cn/gtwymdzegl.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.zhijiandao.cn/gtnfwarpni.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.316326.xyz/gtenyqhhzk.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.jqgufenzy.top/gtehjyptax.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.aizwys.cn/gtlggwmdtp.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.nwbrower.top/gtlhsenwki.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.shuidangran.top/gtqfdhzfwv.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.hongshengwenyu.top/gtmptweaak.html


<!-- 参考信息 -->