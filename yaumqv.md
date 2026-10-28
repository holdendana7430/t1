代发 wailian999

find . -name "*.log" -type f
来源：http://hz.sxryk.cn/gtmropmnhp.html

[R44] 按修改时间查找
来源：http://hz.pycfn.com/gttgcnbfxf.html

find . -mtime -7 -type f
来源：http://hz.dianchejie.cn/gtqmgoyuvz.html

[R45] 批量删除
来源：http://hz.xylfe.cn/gtfpuvgrpp.html

find . -name "*.tmp" -delete
来源：http://hz.hfpthk.cn/gthhnoemva.html

[R46] 递归替换文件内容
来源：http://hz.daria6918.cn/gtkxgnllua.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.hnxiangtu.top/gtrerwzrhq.html

[R47] sed 单行替换
来源：http://hz.wangdashe.top/gtmjbkzkqz.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.zhaomingkeji.xyz/gtxanvgrmt.html

[R48] awk 取指定列
来源：http://hz.xuetiantiany.cn/gtrqmdynso.html

awk '{print $1, $3}' a.txt
来源：http://hz.yanxiufei.cn/gtngslnwhl.html

[R49] awk 带条件
来源：http://hz.tanke756.top/gtgwndyawv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.yj20258888.top/gthnmkovpv.html

[R50] awk 求和
来源：http://hz.shzxlz.cn/gtrtqqfbys.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.shanyushiyangkeji.top/gthgtgibgy.html

[R51] 排序去重取前几
来源：http://hz.wangshuangyany.cn/gthildmvac.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.tian-w.cn/gtyrkaabyt.html

[R52] 统计行数
来源：http://hz.hongshengwenyu.top/gteqmmirpe.html

wc -l a.txt
来源：http://hz.iojbl.cn/gtovvbxnbs.html

[R53] 查看文件头与实时尾
来源：http://hz.jinghuilouyu.cn/gtspeemisu.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.zhengqikj.top/gtnqtmtada.html

[R54] 比较两个文件
来源：http://hz.jinqigufen.top/gteqhiazii.html

diff a.txt b.txt
来源：http://hz.meibo888.top/gtpvhenmsr.html

[R55] 压缩与解压
来源：http://hz.gotoacloud.top/gtoklvfypd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.ywan-chungtsiang.top/gtigbwtfnc.html

[R56] 远程拷贝
来源：http://hz.tanke756.top/gtghvqybyt.html

scp file user@host:/path/
来源：http://hz.jianghu66.top/gtzzbzsqvd.html

[R57] 远程执行命令
来源：http://hz.haohaochexian.top/gtuudsxhkv.html

ssh user@host 'uptime'
来源：http://hz.c1oappe.top/gtsoifcifk.html

[R58] 下载文件
来源：http://hz.9152youxi.cn/gtznxrsssn.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.shanyushiyangkeji.top/gtusmmkzmf.html

[R59] 发 POST JSON
来源：http://hz.hnxiangtu.top/gtsrymbify.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.hammf.cn/gtpokhmmxj.html

[R60] 只看 HTTP 状态码
来源：http://hz.ehwqpu.com/gtagznqsso.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jqgufenzy.top/gtvtibjcry.html

[R61] 磁盘占用
来源：http://hz.shanyushiyangkeji.top/gtfqlonowo.html

df -h;  du -sh *
来源：http://hz.gotoacloud.top/gtggncycoz.html

[R62] 找最占空间的文件
来源：http://hz.wangshuangyany.cn/gtsxwwvjoo.html

du -ah . | sort -rh | head -10
来源：http://hz.daxiang520.top/gtqqqwdjer.html

[R63] 内存与进程
来源：http://hz.xuanzx.com/gtebgdicsf.html

free -h;  ps aux | grep nginx
来源：http://hz.chenzaomai.com/gtbekjovax.html

[R64] 结束进程
来源：http://hz.wangdashe.top/gtuhvxuiki.html

kill -9 $(pgrep -f app.py)
来源：http://hz.c1oappe.top/gtfmwryoot.html

[R65] 查看端口占用
来源：http://hz.ppjwa.cn/gtbkrodzhe.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.ywan-chungtsiang.top/gtyoaarsyc.html

[R66] 定时任务
来源：http://hz.zhaomingkeji.xyz/gtalnkmaqr.html

crontab -e;  crontab -l
来源：http://hz.cheryme.top/gtylznaajd.html

[R67] 生成随机十六进制串
来源：http://hz.cashguo.top/gtkxkpjxgc.html

openssl rand -hex 16
来源：http://hz.birdmap.top/gtzqakboui.html

[R68] 计算文件校验值
来源：http://hz.xziqi.cn/gtmwmevwcu.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.jianghu66.top/gtncfweoud.html

[R69] 生成随机密码
来源：http://hz.hongshengwenyu.top/gtmfxbejws.html

head -c 16 /dev/urandom | base64
来源：http://hz.andypj.xyz/gtsdkkkahf.html

[R70] 时间戳与互转
来源：http://hz.fengsongda.top/gtxahxhezk.html

date +%s;  date -d @1700000000
来源：http://hz.hnqzz.top/gtnrgbvyni.html

[R71] 日期格式化
来源：http://hz.nwbrower.top/gthnstebju.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.9152youxi.cn/gtqbvqmpmu.html

[R72] 等待端口就绪
来源：http://hz.dashuyun.cn/gtgxjqlcat.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jqgufenzy.top/gtfqnmsyvl.html

[R73] 分割大日志
来源：http://hz.yj20258.top/gtxxeqztga.html

split -l 1000 big.log part_
来源：http://hz.yvedp.cn/gtnrglkpfq.html

[R74] 批量重命名
来源：http://hz.smart0.xyz/gtbejufgya.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.shanyushiyangkeji.top/gtubmuqzfb.html

[R75] 导出环境变量
来源：http://hz.yueranfly.top/gtbhycyyyw.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.hnqzz.top/gttmcjeffj.html

[R76] 使用临时文件
来源：http://hz.andypj.xyz/gtrzqopytg.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.sweek.top/gtaqgjekzz.html

[R77] 读取用户输入
来源：http://hz.shangyingyoupin.top/gtfggmntlz.html

read -rp "请输入: " ans
来源：http://hz.pengpengdd.cyou/gtkagosnut.html

[R78] 交互式菜单
来源：http://hz.wangdashe.top/gtqdakogtv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.hywenlv.cn/gtcxxfprnr.html

[R79] 解析命令行选项
来源：http://hz.ivvv.top/gtqqrvylpd.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yj20258.top/gtjskrghxh.html

[R80] 查看脚本执行耗时
来源：http://hz.xziqi.cn/gtetmiwzen.html

time ./run.sh
来源：http://hz.zhaomingkeji.xyz/gtufoyzkum.html

================================================================================
来源：http://hz.jyoumei.cn/gtbsepldso.html

S. C / C++ 专题
来源：http://hz.yonumen.top/gtmrdtdqkz.html

================================================================================
来源：http://hz.cqqwz.cn/gthlcfmsvd.html

[S01] C：Hello World
来源：http://hz.tianlin.xyz/gtgxxultne.html

#include <stdio.h>
来源：http://hz.shanyushiyangkeji.top/gtulajpvzx.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.cdnleiting.top/gtozslonbp.html

[S02] C：变量与格式化输出
来源：http://hz.ybcxt.top/gtrafjngla.html

int a = 10; printf("%d\n", a);
来源：http://hz.jianghu66.top/gtctwgqhyi.html

[S03] C：读入整数
来源：http://hz.zhaomingkeji.xyz/gtofkkipfy.html

int x; scanf("%d", &x);
来源：http://hz.hfpthk.cn/gthihyfcny.html

[S04] C：字符串复制
来源：http://hz.zhengqikj.top/gtjwyzuoue.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.jqgfzy.top/gtsdaxmbzq.html

[S05] C：字符串长度
来源：http://hz.jlsjyb.cn/gtuqgpusox.html

strlen(s)
来源：http://hz.sxryk.cn/gtgwwfsivq.html

[S06] C：字符串比较
来源：http://hz.316326.xyz/gtkphmbgtm.html

strcmp(a, b) == 0
来源：http://hz.dianchejie.cn/gtjjpbrwgt.html

[S07] C：数组遍历求和
来源：http://hz.hysaishi.cn/gtgqlmhygz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.jinghuilouyu.cn/gtcenrwqni.html

[S08] C：动态内存分配与释放
来源：http://hz.kuanghao11.cn/gtjfmalpaj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jinghuilouyu.cn/gtwonaydmg.html

[S09] C：结构体定义与初始化
来源：http://hz.mhx1999.top/gtwkyhtqrs.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.dianchejie.cn/gtuvjdsqqz.html

[S10] C：指针与解引用
来源：http://hz.guannengcc.top/gthcbegnhj.html

int *p = &a;  *p = 5;
来源：http://hz.zycfv.cn/gtncavnglq.html

[S11] C：逐行读文件
来源：http://hz.hywenlv.cn/gtwftssche.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.smart0.xyz/gthcinrfks.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.52xcode.cn/gtlahcxnno.html

fclose(f);
来源：http://hz.daria6918.cn/gtwuivcaxz.html

[S12] C：写文件
来源：http://hz.9152youxi.cn/gtvohctzyq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.wangdashe.top/gtcttbvluw.html

[S13] C：宏定义
来源：http://hz.jinyuanbaomall.cn/gtwaipmbue.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.cashguo.top/gtyqwycujc.html

[S14] C：枚举
来源：http://hz.sxryk.cn/gtwbzwtufr.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.yvedp.cn/gtuxjzgczm.html

[S15] C：类型转换
来源：http://hz.hammf.cn/gtoffyvslv.html

(double) a / b
来源：http://hz.yj20258.top/gtrcyiqkrb.html

[S16] C：位操作置位
来源：http://hz.yuxming.cn/gtcmlqkdea.html

x |= (1 << 3);
来源：http://hz.redwolf501.top/gtwxybrrmo.html

[S17] C：安全拼接字符串
来源：http://hz.yvedp.cn/gtbcwoazjc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.52xcode.cn/gtbknzigam.html

[S18] C：命令行参数
来源：http://hz.chenzaomai.com/gtdplydhlr.html

int main(int argc, char **argv)
来源：http://hz.tian-w.cn/gtkcqwodby.html

[S19] C：快速排序
来源：http://hz.jinqigfzy.top/gtjtjcdiaf.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.chenzaomai.com/gtxmyimran.html

[S20] C：二分查找
来源：http://hz.cheryme.top/gterdieesy.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.smart0.xyz/gtsgreyjsc.html

[S21] C：字符类别判断
来源：http://hz.xinyue.icu/gtfwwkrtiz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.9152youxi.cn/gtnakhauuj.html

[S22] C：字符串转数字
来源：http://hz.gogol.net.cn/gtioqephhu.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.nanxinkj.top/gteepdjway.html

[S23] C：随机数
来源：http://hz.daria6918.cn/gtjnqsnzbm.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.fengsongda.top/gtjgwpaxfx.html

[S24] C：获取本地时间
来源：http://hz.hfpthk.cn/gtrpkrdjlq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.smart0.xyz/gtzjeliyzs.html

[S25] C：内存拷贝
来源：http://hz.jinghuilouyu.cn/gtioegtwej.html

memcpy(dst, src, n);
来源：http://hz.cdnleiting.top/gtxmwjutxk.html

[S26] C：内存清零
来源：http://hz.yj202588.top/gtgoqetaio.html

memset(a, 0, sizeof a);
来源：http://hz.chenjidiqi.icu/gtnagxghye.html

[S27] C：定义常量
来源：http://hz.meibo888.top/gtjxbaiqof.html

const double PI = 3.14159;
来源：http://hz.jiagoushi.top/gtiqpbnbta.html

[S28] C：静态变量
来源：http://hz.bjfxy.top/gtrgnvqjax.html

static int counter = 0;
来源：http://hz.xinyue.icu/gtwvtudtpf.html

[S29] C：变参函数
来源：http://hz.yj202588.top/gtyixjetnj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.haohaochexian.top/gtqcnaafae.html

[S30] C：头文件保护
来源：http://hz.ydzc1.top/gtuvrnbepu.html

#ifndef X_H
来源：http://hz.hfpthk.cn/gtccatpfic.html

#define X_H
来源：http://hz.guannengcc.top/gtjfdicbal.html

#endif
来源：http://hz.ywan-chungtsiang.top/gtxgnxbvti.html

[S31] C++：Hello World
来源：http://hz.tian-w.cn/gtcpfocqte.html

#include <iostream>
来源：http://hz.cqqwz.cn/gtarljxbsd.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.ywan-chungtsiang.top/gtnfhkliyh.html

[S32] C++：字符串
来源：http://hz.quarkkingdee.top/gtwbumvbjg.html

std::string s = "hi";  s += "!";
来源：http://hz.gotoacloud.top/gtkqogzghb.html

[S33] C++：vector 增删
来源：http://hz.yvedp.cn/gtntdytqmn.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.gotoacloud.top/gtkekgsznc.html

[S34] C++：遍历 vector
来源：http://hz.shangyingyoupin.top/gtnnrsucge.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.jiagoushi.top/gtwsoffacd.html

[S35] C++：map
来源：http://hz.hysaishi.cn/gthcvqjfgb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jinqigufen.top/gtzuovyzxg.html

[S36] C++：unordered_map
来源：http://hz.shanyushiyangtech.top/gthwsxhsji.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.andypj.xyz/gtoypvwwdm.html

[S37] C++：set
来源：http://hz.aibaodan.cn/gtxzvncawl.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.xinyue.icu/gtpcrrekmq.html

[S38] C++：排序
来源：http://hz.ehwqpu.com/gtyvpliknk.html

std::sort(v.begin(), v.end());
来源：http://hz.yueranfly.top/gtosqsmwtc.html

[S39] C++：自定义比较器排序
来源：http://hz.52xcode.cn/gtyyhcqbyd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.dianchejie.cn/gtnxavvaox.html

[S40] C++：查找元素
来源：http://hz.andypj.xyz/gtwttyvlho.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.jqgufenzy.top/gtepwzjjdq.html

[S41] C++：类与构造函数
来源：http://hz.cqqwz.cn/gtvrseuntb.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yj20258.top/gtimuxdetn.html

[S42] C++：继承与虚函数
来源：http://hz.ehwqpu.com/gtzudnistz.html

class B : public Base { public: void f() override {} };
来源：http://hz.nanxinkj.top/gtpksvytls.html

[S43] C++：智能指针
来源：http://hz.chenzaomai.com/gtajwiaudt.html

auto p = std::make_unique<int>(5);
来源：http://hz.gaohongyu789.top/gtnwovsiec.html

[S44] C++：引用传参
来源：http://hz.ydjk.org.cn/gtozzgbitn.html

void inc(int &x) { ++x; }
来源：http://hz.zhixingplan.top/gtfotyptgd.html

[S45] C++：lambda
来源：http://hz.tian-w.cn/gttitpsfxg.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.cdnleiting.top/gtbihkaxxf.html

[S46] C++：函数模板
来源：http://hz.sxryk.cn/gtywupktrk.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.xylfe.cn/gtgzmhgljz.html

[S47] C++：结构化绑定遍历
来源：http://hz.c1oappe.top/gtndhezfjr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.zhaomingkeji.xyz/gtthnnjkrm.html

[S48] C++：逐行读文件
来源：http://hz.xinyue.icu/gtrhrxdsrj.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.feifeiyinyue.top/gtcaxpnuxy.html

while (std::getline(in, line)) { }
来源：http://hz.nanxinkj.top/gtyfpgpube.html

[S49] C++：写文件
来源：http://hz.jinqigfzy.top/gteleghlie.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.sufxvd.cn/gtfvgnupjb.html

[S50] C++：格式化数字
来源：http://hz.yongpay.top/gtdylbeeez.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.jianghu66.top/gtxikgyssm.html

[S51] C++：显式类型转换
来源：http://hz.cashguo.top/gtfiqfmubz.html

static_cast<double>(a) / b
来源：http://hz.gogol.net.cn/gtqmkxbkyp.html

[S52] C++：const 与 noexcept
来源：http://hz.svipenyu.cn/gttimenlia.html

int size() const noexcept { return n_; }
来源：http://hz.316326.xyz/gtyesmgwpx.html

[S53] C++：移动语义
来源：http://hz.zhixingplan.top/gtufzvidtc.html

std::vector<int> w = std::move(v);
来源：http://hz.aibaodan.cn/gtqztxagek.html

[S54] C++：异常处理
来源：http://hz.c1oappe.top/gtkhxmyaey.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.pycfn.com/gtrsamocxu.html

[S55] C++：结构化绑定
来源：http://hz.yj20258888.top/gtrjmypnzk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.guowangkeji.top/gtnqzauxji.html

[S56] C++：optional
来源：http://hz.chenjidiqi.icu/gtbqycsenh.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.hongshengwenyu.top/gthcrjwcfg.html

[S57] C++：编译期常量
来源：http://hz.zycfv.cn/gtuymxnfam.html

constexpr int N = 10;
来源：http://hz.mhx1999.top/gtaktrbkhv.html

[S58] C++：命名空间
来源：http://hz.jqgufenzy.top/gtbrntdrko.html

namespace ns { int f() { return 1; } }
来源：http://hz.guowangkeji.top/gtsjvtvasi.html

[S59] C++：静态断言
来源：http://hz.dashuyun.cn/gtvtggikds.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.zhaomingkeji.xyz/gtfgdbiffl.html

[S60] C++：遍历并删除元素
来源：http://hz.hywenlv.cn/gtwduuegtx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.gotoacloud.top/gtwanzpfvs.html

================================================================================
来源：http://hz.jqgfzy.top/gtypfxyvsw.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.hnqzz.top/gtxwmglzyq.html

================================================================================
来源：http://hz.kuanghao11.cn/gtzoduzjpc.html

[T01] Kotlin：Hello World
来源：http://hz.tian-w.cn/gtcoetstof.html

println("Hello")
来源：http://hz.ydjk.org.cn/gtuxuxeroj.html

[T02] Kotlin：变量
来源：http://hz.zdqjudy.top/gtadttmwzg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.hongshengwenyu.top/gtyosqvvfd.html

[T03] Kotlin：字符串模板
来源：http://hz.fengsongda.top/gtgbgwxkeh.html

"值: $b"
来源：http://hz.yuxming.cn/gtsastikdu.html

[T04] Kotlin：空安全
来源：http://hz.hysaishi.cn/gtyolssaul.html

val n: String? = null;  n?.length
来源：http://hz.mhx1999.top/gtbjyauvbe.html

[T05] Kotlin：when 表达式
来源：http://hz.daxiang520.top/gtqfzlknds.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.gotoacloud.top/gtppluuita.html

[T06] Kotlin：集合映射
来源：http://hz.yonumen.top/gtqrlrgkmj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.tian-w.cn/gthxufknlq.html

[T07] Kotlin：集合过滤
来源：http://hz.hongshengwenyu.top/gtwfyyfigw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.gotoacloud.top/gtjzaqsdqo.html

[T08] Kotlin：数据类
来源：http://hz.birdmap.top/gtfbviuang.html

data class User(val name: String, val age: Int)
来源：http://hz.jinghuilouyu.cn/gtytghvjmk.html

[T09] Kotlin：扩展函数
来源：http://hz.smart0.xyz/gtehvtgrsa.html

fun String.exclaim() = this + "!"
来源：http://hz.ehwqpu.com/gtrobchcun.html

[T10] Kotlin：默认参数
来源：http://hz.iojbl.cn/gtlrbtlgcu.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.bjfxy.top/gtrdakphot.html

[T11] Kotlin：协程
来源：http://hz.jinyuanbaomall.cn/gtyvusaxrm.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.meibo888.top/gtrablfpad.html

[T12] Kotlin：解构声明
来源：http://hz.jyoumei.cn/gtfecggavq.html

val (a, b) = Pair(1, 2)
来源：http://hz.shanyushiyangtech.top/gtzpyhfetl.html

[T13] Kotlin：只读 Map
来源：http://hz.cucudq.cn/gtwooyqxxw.html

val m = mapOf("a" to 1)
来源：http://hz.ivvv.top/gtkjpjxqqw.html

[T14] Kotlin：循环
来源：http://hz.aizwys.cn/gtbjlfbnls.html

for (i in 1..10) println(i)
来源：http://hz.snrcjt.cn/gtdydktgsf.html

[T15] Kotlin：接口
来源：http://hz.zhongyouzk.top/gttlajuqtq.html

interface Shape { fun area(): Double }
来源：http://hz.aizwys.cn/gtugmqnuky.html

[T16] Swift：Hello World
来源：http://hz.ywan-chungtsiang.top/gtyxenwfkw.html

print("Hello")
来源：http://hz.dianchejie.cn/gtuwagejss.html

[T17] Swift：变量与常量
来源：http://hz.aizwys.cn/gtbofxlsif.html

var a = 1;  let b = 2
来源：http://hz.daxiang520.top/gtvylhitxg.html

[T18] Swift：字符串插值
来源：http://hz.gzhubu.top/gthvwejija.html

"值: \(b)"
来源：http://hz.sufxvd.cn/gtulxgyqbo.html

[T19] Swift：可选绑定
来源：http://hz.daria6918.cn/gtpljfxzug.html

if let n = opt { print(n) }
来源：http://hz.kuanghao11.cn/gtmyizxada.html

[T20] Swift：数组操作
来源：http://hz.cashguo.top/gtngkolwnc.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.yvedp.cn/gtnmsmgxzf.html

[T21] Swift：遍历
来源：http://hz.gaohongyu789.top/gtzlpraitu.html

for x in a { print(x) }
来源：http://hz.zhongyouzk.top/gtajzqkzko.html

[T22] Swift：字典
来源：http://hz.mhx1999.top/gtshvikmbg.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.haohaochexian.top/gtxrulcars.html

[T23] Swift：函数
来源：http://hz.xinyue.icu/gtptphbkyh.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.smart0.xyz/gtruopspjj.html

[T24] Swift：闭包
来源：http://hz.fengsongda.top/gtdwhcycdd.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.cdnleiting.top/gttheenvxa.html

[T25] Swift：结构体
来源：http://hz.chenzaomai.com/gtmrynsuvq.html

struct P { var x: Int }
来源：http://hz.jinqigfzy.top/gthjfzqjvx.html

[T26] Swift：类与重写
来源：http://hz.yj20258888.top/gtekenkjrk.html

class A: Base { override func f() {} }
来源：http://hz.yongpay.top/gtihqdpvtt.html

[T27] Swift：错误处理
来源：http://hz.cqqwz.cn/gtqqmfiyha.html

do { try f() } catch { print(error) }
来源：http://hz.sweek.top/gtdpklfquh.html

[T28] Swift：枚举
来源：http://hz.xziqi.cn/gtdnpsenaa.html

enum Color { case red, green }
来源：http://hz.hammf.cn/gtofvyumoz.html

[T29] Swift：guard 提前返回
来源：http://hz.hammf.cn/gtfbrytyxn.html

guard let x = opt else { return }
来源：http://hz.yvedp.cn/gtxbhawbwa.html

[T30] Swift：协议
来源：http://hz.zhixingplan.top/gtoyzvhdyw.html

protocol Shape { func area() -> Double }
来源：http://hz.zhiwuduotai.top/gtldhplicv.html

[T31] Lua：Hello World
来源：http://hz.hongshengwenyu.top/gthleuzbct.html

print("Hello")
来源：http://hz.feifeiyinyue.top/gteqxsczth.html

[T32] Lua：局部变量
来源：http://hz.hongshengwenyu.top/gtvbhhjahx.html

local a = 1
来源：http://hz.wangshuangyany.cn/gttgocwsma.html

[T33] Lua：表（数组）
来源：http://hz.birdmap.top/gtljazxjcr.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.daria6918.cn/gtkfihhvfg.html

[T34] Lua：遍历表
来源：http://hz.jiagoushi.top/gtiqxonmha.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.cucudq.cn/gtegnnarer.html

[T35] Lua：字典表
来源：http://hz.ivvv.top/gtsinldawv.html

local d = { a = 1 };  d.b = 2
来源：http://hz.vqdsnc.cn/gtuqfelqmh.html

[T36] Lua：函数
来源：http://hz.birdmap.top/gtadfufwvu.html

function add(a, b) return a + b end
来源：http://hz.9152youxi.cn/gtpzcwpwoa.html

[T37] Lua：字符串拼接
来源：http://hz.hammf.cn/gtsiovvxkl.html

"a" .. "b"
来源：http://hz.wangshuangyany.cn/gtdohoxbxs.html

[T38] Lua：条件
来源：http://hz.svipenyu.cn/gteokygrmz.html

if x > 0 then print("正") end
来源：http://hz.xylfe.cn/gtgjrwwmtu.html

[T39] Lua：模式匹配
来源：http://hz.tanke756.top/gtjauqaapd.html

string.find(s, "%d+")
来源：http://hz.mhx1999.top/gtynbpgnlv.html

[T40] Lua：元表
来源：http://hz.jlsjyb.cn/gtpfxbclin.html

setmetatable({}, { __index = base })
来源：http://hz.jlsjyb.cn/gtqcprpxnq.html

[T41] Perl：Hello World
来源：http://hz.cashguo.top/gtamlgrdyx.html

print "Hello\n";
来源：http://hz.jinghuilouyu.cn/gtjznrviqh.html

[T42] Perl：变量类型
来源：http://hz.hongshengwenyu.top/gtdabjlref.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.shanyushiyangkeji.top/gtayfyfxth.html

[T43] Perl：字符串插值
来源：http://hz.gotoacloud.top/gtdfrcqxcz.html

"值: $a"
来源：http://hz.cucudq.cn/gtnnizmqkf.html

[T44] Perl：条件
来源：http://hz.fzhhl.top/gtgbsraenh.html

if ($a > 0) { print "正"; }
来源：http://hz.dashuyun.cn/gtttvnqmrw.html

[T45] Perl：数组遍历
来源：http://hz.hongshengwenyu.top/gtuvlgsmah.html

for my $x (@arr) { print $x; }
来源：http://hz.yj20258.top/gtagrutsxk.html

[T46] Perl：哈希操作
来源：http://hz.pycfn.com/gtkvwclgsr.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.xuetiantiany.cn/gtohyfjnch.html


<!-- 参考信息 -->