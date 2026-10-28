代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.shzxlz.cn/gtnrdkonup.html

[R52] 统计行数
来源：http://hz.daxiang520.top/gtpmzcmeoq.html

wc -l a.txt
来源：http://hz.yongpay.top/gtzsfhvrsj.html

[R53] 查看文件头与实时尾
来源：http://hz.aizwys.cn/gtaowyeaka.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.zycfv.cn/gtlxkxyobm.html

[R54] 比较两个文件
来源：http://hz.dashuyun.cn/gtjhsgxjol.html

diff a.txt b.txt
来源：http://hz.quarkkingdee.top/gtouqzeofv.html

[R55] 压缩与解压
来源：http://hz.ybcxt.top/gtaxmcwasl.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.mhx1999.top/gtjsiaempt.html

[R56] 远程拷贝
来源：http://hz.52xcode.cn/gtxoytjsgi.html

scp file user@host:/path/
来源：http://hz.cdnleiting.top/gtulbcsvbh.html

[R57] 远程执行命令
来源：http://hz.jinqigfzy.top/gtawxtdije.html

ssh user@host 'uptime'
来源：http://hz.shanyushiyangtech.top/gtdaobuhav.html

[R58] 下载文件
来源：http://hz.hnqzz.top/gtbmvxiomb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.nanxuanxn.top/gtfenpilmo.html

[R59] 发 POST JSON
来源：http://hz.nanxuanxn.top/gtffvtlgfj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.cucudq.cn/gtkniszqmk.html

[R60] 只看 HTTP 状态码
来源：http://hz.9152youxi.cn/gtajutfmky.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.ybcxt.top/gtsrpnaeks.html

[R61] 磁盘占用
来源：http://hz.shzxlz.cn/gteukzqtzq.html

df -h;  du -sh *
来源：http://hz.yangfankeji.com/gtyyeeykzb.html

[R62] 找最占空间的文件
来源：http://hz.xinyue.icu/gtcgsecdph.html

du -ah . | sort -rh | head -10
来源：http://hz.quarkkingdee.top/gthcjdrfru.html

[R63] 内存与进程
来源：http://hz.aizwys.cn/gtkfoyosit.html

free -h;  ps aux | grep nginx
来源：http://hz.wangdashe.top/gteooynvis.html

[R64] 结束进程
来源：http://hz.yongpay.top/gtcaddlrhe.html

kill -9 $(pgrep -f app.py)
来源：http://hz.tanke756.top/gtfbmisnwc.html

[R65] 查看端口占用
来源：http://hz.mhx1999.top/gtnbumvbkc.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.vqdsnc.cn/gthlmdaolr.html

[R66] 定时任务
来源：http://hz.hammf.cn/gtouhyqcpm.html

crontab -e;  crontab -l
来源：http://hz.zhoulong.xyz/gtzrkwxcpy.html

[R67] 生成随机十六进制串
来源：http://hz.yj20258888.top/gtkgxkgycw.html

openssl rand -hex 16
来源：http://hz.zhixingplan.top/gtqisejjnc.html

[R68] 计算文件校验值
来源：http://hz.yonumen.top/gtidljgltn.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.tian-w.cn/gturncbugy.html

[R69] 生成随机密码
来源：http://hz.dashuyun.cn/gtssqbgsag.html

head -c 16 /dev/urandom | base64
来源：http://hz.dashuyun.cn/gtlpgopvjf.html

[R70] 时间戳与互转
来源：http://hz.shanyushiyangtech.top/gthodfahvc.html

date +%s;  date -d @1700000000
来源：http://hz.aibaodan.cn/gtsvnlgsgx.html

[R71] 日期格式化
来源：http://hz.jqgfzy.top/gtotnwoftq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.chenzaomai.com/gtpzqbijzp.html

[R72] 等待端口就绪
来源：http://hz.cdnleiting.top/gtdhbvboth.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.chenjidiqi.icu/gtamhiqkql.html

[R73] 分割大日志
来源：http://hz.316326.xyz/gtgdmwjeda.html

split -l 1000 big.log part_
来源：http://hz.chenjidiqi.icu/gtmsjzmmnb.html

[R74] 批量重命名
来源：http://hz.tianlin.xyz/gtnsorczea.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.ehwqpu.com/gtiqdlrion.html

[R75] 导出环境变量
来源：http://hz.guannengcc.top/gtgcckmjts.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.gogol.net.cn/gtcdqsydin.html

[R76] 使用临时文件
来源：http://hz.tian-w.cn/gtozzmopzr.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhoulong.xyz/gtondvyukz.html

[R77] 读取用户输入
来源：http://hz.yanxiufei.cn/gtlvhdtizg.html

read -rp "请输入: " ans
来源：http://hz.tianlin.xyz/gtpjchuprx.html

[R78] 交互式菜单
来源：http://hz.jiagoushi.top/gtjlgvwpgk.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yj202588.top/gtfixflzik.html

[R79] 解析命令行选项
来源：http://hz.316326.xyz/gtnxsiykjv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.aibaodan.cn/gtvypywotl.html

[R80] 查看脚本执行耗时
来源：http://hz.smart0.xyz/gtmdlbwmui.html

time ./run.sh
来源：http://hz.ybcxt.top/gtmayjjrrm.html

================================================================================
来源：http://hz.snrcjt.cn/gtgbgayvit.html

S. C / C++ 专题
来源：http://hz.aizwys.cn/gtlxdknyrh.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtyahpuvam.html

[S01] C：Hello World
来源：http://hz.sweek.top/gtqejuwgdx.html

#include <stdio.h>
来源：http://hz.tanke756.top/gttouxgphm.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.wangdashe.top/gtpcyjucak.html

[S02] C：变量与格式化输出
来源：http://hz.tian-w.cn/gtivittwya.html

int a = 10; printf("%d\n", a);
来源：http://hz.aizwys.cn/gtjvyufryt.html

[S03] C：读入整数
来源：http://hz.havefunace.top/gtpjdfyqjy.html

int x; scanf("%d", &x);
来源：http://hz.birdmap.top/gtscybruhn.html

[S04] C：字符串复制
来源：http://hz.yvedp.cn/gtafioekgp.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.daria6918.cn/gtvybiufqo.html

[S05] C：字符串长度
来源：http://hz.guannengcc.top/gtjhpsdmiw.html

strlen(s)
来源：http://hz.gzhubu.top/gtjlsaatsp.html

[S06] C：字符串比较
来源：http://hz.yangfankeji.com/gtflzdtixz.html

strcmp(a, b) == 0
来源：http://hz.feifeiyinyue.top/gtfqyndfkc.html

[S07] C：数组遍历求和
来源：http://hz.gzhubu.top/gtrbtuccnp.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.meibo888.top/gtfiwbgdcc.html

[S08] C：动态内存分配与释放
来源：http://hz.yj202588.top/gtehmwwsea.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.sysykeji.top/gtrmexqqln.html

[S09] C：结构体定义与初始化
来源：http://hz.yuanzhike.top/gtfzvlobhr.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.hywenlv.cn/gtvqaomtcm.html

[S10] C：指针与解引用
来源：http://hz.cqqwz.cn/gtottffqew.html

int *p = &a;  *p = 5;
来源：http://hz.birdmap.top/gtrbhlmxka.html

[S11] C：逐行读文件
来源：http://hz.hysaishi.cn/gtvkyqkwah.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.aizwys.cn/gthdxunppo.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.dianchejie.cn/gtivgayzyz.html

fclose(f);
来源：http://hz.316326.xyz/gtgonbnlkq.html

[S12] C：写文件
来源：http://hz.sysykeji.top/gtaexrxtub.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.vqdsnc.cn/gtdgidfsju.html

[S13] C：宏定义
来源：http://hz.shzxlz.cn/gtsrtpjmpz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.cashguo.top/gtfpeofuzd.html

[S14] C：枚举
来源：http://hz.yuxming.cn/gtvmcqfzxw.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.jinqigfzy.top/gtamjutogk.html

[S15] C：类型转换
来源：http://hz.kuanghao11.cn/gtfpaxyfzh.html

(double) a / b
来源：http://hz.jinqigfzy.top/gtundykizr.html

[S16] C：位操作置位
来源：http://hz.yuxming.cn/gtisoaamhs.html

x |= (1 << 3);
来源：http://hz.cashguo.top/gtxdmuwgls.html

[S17] C：安全拼接字符串
来源：http://hz.nanxinkj.top/gtlyawcrfo.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.chenzaomai.com/gtrabjbzxe.html

[S18] C：命令行参数
来源：http://hz.svipenyu.cn/gtqyrwdveu.html

int main(int argc, char **argv)
来源：http://hz.52xcode.cn/gtqqyjnwfl.html

[S19] C：快速排序
来源：http://hz.yuanzhike.top/gtnucitonu.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.wangdashe.top/gtlamlzxtt.html

[S20] C：二分查找
来源：http://hz.iojbl.cn/gtwfwnaohh.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.chenzaomai.com/gtlerajxzi.html

[S21] C：字符类别判断
来源：http://hz.tanke756.top/gtaggmtzep.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.ivvv.top/gtaskdtvfg.html

[S22] C：字符串转数字
来源：http://hz.snrcjt.cn/gtphlwknuj.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.dianchejie.cn/gtamnbmeej.html

[S23] C：随机数
来源：http://hz.316326.xyz/gtstybaidn.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.ehwqpu.com/gtfunmhnyn.html

[S24] C：获取本地时间
来源：http://hz.zhijiandao.cn/gtsbrqteph.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.dianchejie.cn/gtgcpbkytu.html

[S25] C：内存拷贝
来源：http://hz.dashuyun.cn/gtccelsfpi.html

memcpy(dst, src, n);
来源：http://hz.guowangkeji.top/gttnxcanqr.html

[S26] C：内存清零
来源：http://hz.sufxvd.cn/gtrovjprtv.html

memset(a, 0, sizeof a);
来源：http://hz.ehwqpu.com/gtmfbepnem.html

[S27] C：定义常量
来源：http://hz.jiagoushi.top/gthpguzmaj.html

const double PI = 3.14159;
来源：http://hz.gotoacloud.top/gtdouvejpo.html

[S28] C：静态变量
来源：http://hz.yongpay.top/gtfhvienpu.html

static int counter = 0;
来源：http://hz.zdqjudy.top/gtnfeaoqwr.html

[S29] C：变参函数
来源：http://hz.jlsjyb.cn/gtlyfixvwn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.zhengqikj.top/gtjpryjmpu.html

[S30] C：头文件保护
来源：http://hz.yj20258.top/gtzswdyeis.html

#ifndef X_H
来源：http://hz.tianlin.xyz/gttzhqhznk.html

#define X_H
来源：http://hz.zhixingplan.top/gtwptvlruz.html

#endif
来源：http://hz.yanxiufei.cn/gtmungotwm.html

[S31] C++：Hello World
来源：http://hz.yj202588.top/gtjkdnlilc.html

#include <iostream>
来源：http://hz.jqgfzy.top/gtsqhtgmtc.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.zhijiandao.cn/gtjwltrvld.html

[S32] C++：字符串
来源：http://hz.yj20258888.top/gtifazpmbj.html

std::string s = "hi";  s += "!";
来源：http://hz.daria6918.cn/gthmephudd.html

[S33] C++：vector 增删
来源：http://hz.wangdashe.top/gtewrsgxbh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.cdnleiting.top/gtoihovvjl.html

[S34] C++：遍历 vector
来源：http://hz.kuanghao11.cn/gtgtsnarqx.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.zhixingplan.top/gtctqslvsn.html

[S35] C++：map
来源：http://hz.aizwys.cn/gtvnmdkywx.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.guannengcc.top/gtolgppfod.html

[S36] C++：unordered_map
来源：http://hz.wangshuangyany.cn/gtejyfwigc.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hfpthk.cn/gtvzincpxz.html

[S37] C++：set
来源：http://hz.jqgfzy.top/gtdulrpghj.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.gzhubu.top/gtpjwrsoky.html

[S38] C++：排序
来源：http://hz.ydjk.org.cn/gtpgjzyqxy.html

std::sort(v.begin(), v.end());
来源：http://hz.aizwys.cn/gtnschrnof.html

[S39] C++：自定义比较器排序
来源：http://hz.cqqwz.cn/gtjrmsxaaj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.hnqzz.top/gtwuycfngp.html

[S40] C++：查找元素
来源：http://hz.redwolf501.top/gtdqhwxonf.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.quarkkingdee.top/gtvhfzrmme.html

[S41] C++：类与构造函数
来源：http://hz.hysaishi.cn/gteziupdlu.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.zhongyouzk.top/gtzhhfgtox.html

[S42] C++：继承与虚函数
来源：http://hz.smart0.xyz/gtsobedtvx.html

class B : public Base { public: void f() override {} };
来源：http://hz.chenzaomai.com/gtmsohxprt.html

[S43] C++：智能指针
来源：http://hz.pengpengdd.cyou/gtvxaxdjgq.html

auto p = std::make_unique<int>(5);
来源：http://hz.xziqi.cn/gtqipxmbpu.html

[S44] C++：引用传参
来源：http://hz.dashuyun.cn/gtuzcdgawl.html

void inc(int &x) { ++x; }
来源：http://hz.shzxlz.cn/gtrspiraat.html

[S45] C++：lambda
来源：http://hz.sufxvd.cn/gtelhrtayo.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.zhongyouzk.top/gtdjojiiev.html

[S46] C++：函数模板
来源：http://hz.jinqigfzy.top/gtvavhiysb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.bjfxy.top/gtxglhptbb.html

[S47] C++：结构化绑定遍历
来源：http://hz.ybcxt.top/gtttfoqbsf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.yj20258888.top/gtcgvafwzv.html

[S48] C++：逐行读文件
来源：http://hz.nwbrower.top/gtsgapslwm.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.fengsongda.top/gtglrpxrxd.html

while (std::getline(in, line)) { }
来源：http://hz.jinyuanbaomall.cn/gtytljvgef.html

[S49] C++：写文件
来源：http://hz.tianlin.xyz/gtnwuqrdtn.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.zhijiandao.cn/gtpqlvryfd.html

[S50] C++：格式化数字
来源：http://hz.316326.xyz/gtehzxjapr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.daxiang520.top/gtuflbojaq.html

[S51] C++：显式类型转换
来源：http://hz.jqgufenzy.top/gtlrjphryh.html

static_cast<double>(a) / b
来源：http://hz.c1oappe.top/gtotvftvrw.html

[S52] C++：const 与 noexcept
来源：http://hz.tian-w.cn/gtdnzbgzon.html

int size() const noexcept { return n_; }
来源：http://hz.shuidangran.top/gtllbzzsgv.html

[S53] C++：移动语义
来源：http://hz.nwbrower.top/gtncfyrrvg.html

std::vector<int> w = std::move(v);
来源：http://hz.ywan-chungtsiang.top/gtncqkqdln.html

[S54] C++：异常处理
来源：http://hz.smart0.xyz/gtoajbxewx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.chenzaomai.com/gtuzsauhfw.html

[S55] C++：结构化绑定
来源：http://hz.zhixingplan.top/gtbawakdwk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.yueranfly.top/gtoqtdbhel.html

[S56] C++：optional
来源：http://hz.ydjk.org.cn/gtxzhsmtpe.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.316326.xyz/gtqioseopf.html

[S57] C++：编译期常量
来源：http://hz.yongpay.top/gtzxiktyea.html

constexpr int N = 10;
来源：http://hz.ydzc1.top/gtmjozwqvb.html

[S58] C++：命名空间
来源：http://hz.ydjk.org.cn/gtgkbqwxzp.html

namespace ns { int f() { return 1; } }
来源：http://hz.jqgufenzy.top/gtispxgdhy.html

[S59] C++：静态断言
来源：http://hz.nwbrower.top/gtndcaprew.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.316326.xyz/gtlpmiqnnk.html

[S60] C++：遍历并删除元素
来源：http://hz.cashguo.top/gthpbkqywx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.tianlin.xyz/gtkugiybck.html

================================================================================
来源：http://hz.haohaochexian.top/gtbtzwikfr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.ywan-chungtsiang.top/gtitithzxj.html

================================================================================
来源：http://hz.yuxming.cn/gtwuodzzvm.html

[T01] Kotlin：Hello World
来源：http://hz.smart0.xyz/gtxtogzplj.html

println("Hello")
来源：http://hz.jinghuilouyu.cn/gtbarvuvdj.html

[T02] Kotlin：变量
来源：http://hz.ppjwa.cn/gtpwbqndlz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.zdqjudy.top/gtkbglihnc.html

[T03] Kotlin：字符串模板
来源：http://hz.0kj1m.cn/gtkzjmycwc.html

"值: $b"
来源：http://hz.yuxming.cn/gtiterjlkr.html

[T04] Kotlin：空安全
来源：http://hz.zhixingplan.top/gtqynqquag.html

val n: String? = null;  n?.length
来源：http://hz.chenlongwang.top/gtxuchuomo.html

[T05] Kotlin：when 表达式
来源：http://hz.zhaomingkeji.xyz/gtjhiwriur.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.iojbl.cn/gtucqwkrhx.html

[T06] Kotlin：集合映射
来源：http://hz.zhaomingkeji.xyz/gtnioeehru.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.tianlin.xyz/gtapxhytpx.html

[T07] Kotlin：集合过滤
来源：http://hz.gotoacloud.top/gtfingeeth.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yuxming.cn/gtjldlqrxf.html

[T08] Kotlin：数据类
来源：http://hz.xingfuxueyuan.xyz/gtigvicmwh.html

data class User(val name: String, val age: Int)
来源：http://hz.sxryk.cn/gtobjacuyl.html

[T09] Kotlin：扩展函数
来源：http://hz.aibaodan.cn/gtqkpwzyay.html

fun String.exclaim() = this + "!"
来源：http://hz.xylfe.cn/gtfopahuep.html

[T10] Kotlin：默认参数
来源：http://hz.mhx1999.top/gtwlqesjod.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.guannengcc.top/gtjmsediqf.html

[T11] Kotlin：协程
来源：http://hz.zdqjudy.top/gtwpksswrh.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.yuanzhike.top/gtusxcwylz.html

[T12] Kotlin：解构声明
来源：http://hz.birdmap.top/gtjapwkfxr.html

val (a, b) = Pair(1, 2)
来源：http://hz.ivvv.top/gthgcsphgs.html

[T13] Kotlin：只读 Map
来源：http://hz.zhixingplan.top/gtixfgtctj.html

val m = mapOf("a" to 1)
来源：http://hz.jiagoushi.top/gtmgvvackk.html

[T14] Kotlin：循环
来源：http://hz.0kj1m.cn/gtqfuoqqrg.html

for (i in 1..10) println(i)
来源：http://hz.hfpthk.cn/gtypisdklh.html

[T15] Kotlin：接口
来源：http://hz.xuanzx.com/gtzadqktsk.html

interface Shape { fun area(): Double }
来源：http://hz.xziqi.cn/gtmeytmsgi.html

[T16] Swift：Hello World
来源：http://hz.gotoacloud.top/gtncynquyf.html

print("Hello")
来源：http://hz.yongpay.top/gtniqhrjvm.html

[T17] Swift：变量与常量
来源：http://hz.daxiang520.top/gtoazhqjnh.html

var a = 1;  let b = 2
来源：http://hz.svipenyu.cn/gtnwurhdna.html

[T18] Swift：字符串插值
来源：http://hz.zdqjudy.top/gtvvmphcpc.html

"值: \(b)"
来源：http://hz.zhixingplan.top/gtozbazmfc.html

[T19] Swift：可选绑定
来源：http://hz.pengpengdd.cyou/gtwzaqvegs.html

if let n = opt { print(n) }
来源：http://hz.jinyuanbaomall.cn/gtfbcmurzt.html

[T20] Swift：数组操作
来源：http://hz.zhixingplan.top/gtkjisqtjm.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.wangshuangyany.cn/gtsdmzepdb.html

[T21] Swift：遍历
来源：http://hz.guannengcc.top/gtljqvkihw.html

for x in a { print(x) }
来源：http://hz.hysaishi.cn/gtbqbvlear.html

[T22] Swift：字典
来源：http://hz.feifeiyinyue.top/gtygiqjaoj.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.gzhubu.top/gtcamlnpdu.html

[T23] Swift：函数
来源：http://hz.daria6918.cn/gtkldbuzqz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.hywenlv.cn/gtxtamnggg.html

[T24] Swift：闭包
来源：http://hz.tian-w.cn/gttxssbekz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.smart0.xyz/gtahcrksdj.html

[T25] Swift：结构体
来源：http://hz.zycfv.cn/gtylwmfyza.html

struct P { var x: Int }
来源：http://hz.quarkkingdee.top/gtohlgvgew.html

[T26] Swift：类与重写
来源：http://hz.birdmap.top/gtntcnaaaj.html

class A: Base { override func f() {} }
来源：http://hz.andypj.xyz/gtcylhuwai.html

[T27] Swift：错误处理
来源：http://hz.sxryk.cn/gtascufajh.html

do { try f() } catch { print(error) }
来源：http://hz.fengsongda.top/gtdyppmmnf.html

[T28] Swift：枚举
来源：http://hz.daxiang520.top/gtinldfjtt.html

enum Color { case red, green }
来源：http://hz.ydzc1.top/gtktyqhsax.html

[T29] Swift：guard 提前返回
来源：http://hz.ywan-chungtsiang.top/gtdifcvceu.html

guard let x = opt else { return }
来源：http://hz.tian-w.cn/gtkqboxsgg.html

[T30] Swift：协议
来源：http://hz.cashguo.top/gtawjatzyy.html

protocol Shape { func area() -> Double }
来源：http://hz.redwolf501.top/gtklncsowa.html

[T31] Lua：Hello World
来源：http://hz.jqgufenzy.top/gtbmivkski.html

print("Hello")
来源：http://hz.nanxuanxn.top/gtqiatmkta.html

[T32] Lua：局部变量
来源：http://hz.hammf.cn/gtkgivnuxl.html

local a = 1
来源：http://hz.nwbrower.top/gttumhebvb.html

[T33] Lua：表（数组）
来源：http://hz.zhiwuduotai.top/gtjkjrpwyo.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.wangshuangyany.cn/gtelspjbtl.html

[T34] Lua：遍历表
来源：http://hz.quarkkingdee.top/gtfmbqkqct.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.jianghu66.top/gtwuwuksjm.html

[T35] Lua：字典表
来源：http://hz.nanxuanxn.top/gtixzzlleb.html

local d = { a = 1 };  d.b = 2
来源：http://hz.sysykeji.top/gtoggwrfcw.html

[T36] Lua：函数
来源：http://hz.havefunace.top/gthrazegzj.html

function add(a, b) return a + b end
来源：http://hz.hnxiangtu.top/gtkuaqatec.html

[T37] Lua：字符串拼接
来源：http://hz.daria6918.cn/gtxzwanjxq.html

"a" .. "b"
来源：http://hz.ivvv.top/gtjlcusbni.html

[T38] Lua：条件
来源：http://hz.xylfe.cn/gtnrraoofs.html

if x > 0 then print("正") end
来源：http://hz.shzxlz.cn/gtbkrbwjmh.html

[T39] Lua：模式匹配
来源：http://hz.yonumen.top/gtqtuzcwot.html

string.find(s, "%d+")
来源：http://hz.pycfn.com/gtiopkzoqa.html

[T40] Lua：元表
来源：http://hz.aizwys.cn/gtlmuwxlzh.html

setmetatable({}, { __index = base })
来源：http://hz.chenlongwang.top/gtnlyhkgkl.html

[T41] Perl：Hello World
来源：http://hz.dianchejie.cn/gthfyzmtjp.html

print "Hello\n";
来源：http://hz.jianghu66.top/gtbqdbcots.html

[T42] Perl：变量类型
来源：http://hz.quarkkingdee.top/gtkmslzhsa.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.jqgfzy.top/gtfwcveqyz.html

[T43] Perl：字符串插值
来源：http://hz.smart0.xyz/gtlpledbai.html

"值: $a"
来源：http://hz.cheryme.top/gtisyzimsi.html

[T44] Perl：条件
来源：http://hz.andypj.xyz/gtcrnymxwb.html

if ($a > 0) { print "正"; }
来源：http://hz.quarkkingdee.top/gtaclgyvcs.html

[T45] Perl：数组遍历
来源：http://hz.nanxuanxn.top/gtiaikdhtr.html

for my $x (@arr) { print $x; }
来源：http://hz.quarkkingdee.top/gtnewdozgy.html

[T46] Perl：哈希操作
来源：http://hz.yuxming.cn/gtedexqngi.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.shuidangran.top/gtapgglaub.html

[T47] Perl：正则捕获
来源：http://hz.ehwqpu.com/gtlylplsjp.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.zhaomingkeji.xyz/gtfsfuuimj.html

[T48] Perl：正则替换
来源：http://hz.0kj1m.cn/gthssrrnse.html

$s =~ s/old/new/g;
来源：http://hz.aizwys.cn/gtqrnwxidk.html

[T49] Perl：函数
来源：http://hz.wangshuangyany.cn/gtnpbylimr.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.9152youxi.cn/gtnzqmtsia.html

[T50] Perl：逐行读文件
来源：http://hz.cheryme.top/gtbnnrblyg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.hongshengwenyu.top/gtnjfsqyfp.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.xziqi.cn/gthothyxol.html

[T51] Scala：Hello World
来源：http://hz.pycfn.com/gtwkvdoowf.html

println("Hello")
来源：http://hz.andypj.xyz/gtbmborfok.html

[T52] Scala：变量
来源：http://hz.9152youxi.cn/gtdgxxxghd.html

val a = 1;  var b = 2
来源：http://hz.shanyushiyangtech.top/gtypjgsmdg.html

[T53] Scala：字符串插值
来源：http://hz.jiagoushi.top/gtqnqehqeq.html

s"值: $b"
来源：http://hz.shuidangran.top/gtbarfmbch.html

[T54] Scala：集合映射
来源：http://hz.shuidangran.top/gthvziaszp.html


<!-- 参考信息 -->